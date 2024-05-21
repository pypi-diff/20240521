# Comparing `tmp/zeval-0.1.0.tar.gz` & `tmp/zeval-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeval-0.1.0.tar", last modified: Fri May 10 11:03:47 2024, max compression
+gzip compressed data, was "zeval-0.1.1.tar", last modified: Tue May 21 08:54:33 2024, max compression
```

## Comparing `zeval-0.1.0.tar` & `zeval-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-10 11:03:47.596884 zeval-0.1.0/
--rw-r--r--   0 everfly    (501) wheel        (0)      651 2024-05-10 11:03:47.596694 zeval-0.1.0/PKG-INFO
--rw-r--r--   0 everfly    (501) wheel        (0)       38 2024-05-10 11:03:47.596918 zeval-0.1.0/setup.cfg
--rw-r--r--   0 everfly    (501) wheel        (0)      887 2024-05-10 10:53:56.000000 zeval-0.1.0/setup.py
-drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-10 11:03:47.593958 zeval-0.1.0/zeval/
--rw-r--r--   0 everfly    (501) wheel        (0)        0 2024-05-01 07:04:24.000000 zeval-0.1.0/zeval/__init__.py
-drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-10 11:03:47.594859 zeval-0.1.0/zeval/config/
--rw-r--r--   0 everfly    (501) wheel        (0)        0 2024-05-01 07:08:33.000000 zeval-0.1.0/zeval/config/__init__.py
--rw-r--r--   0 everfly    (501) wheel        (0)      180 2024-05-10 10:53:55.000000 zeval-0.1.0/zeval/config/model_config.py
--rw-r--r--   0 everfly    (501) wheel        (0)      474 2024-05-10 10:59:01.000000 zeval-0.1.0/zeval/evaluation.py
-drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-10 11:03:47.596037 zeval-0.1.0/zeval/evaluators/
--rw-r--r--   0 everfly    (501) wheel        (0)      211 2024-05-10 10:53:55.000000 zeval-0.1.0/zeval/evaluators/__init__.py
--rw-r--r--   0 everfly    (501) wheel        (0)     7177 2024-05-10 10:53:55.000000 zeval-0.1.0/zeval/evaluators/answer_relevancy.py
--rw-r--r--   0 everfly    (501) wheel        (0)     4185 2024-05-10 10:53:55.000000 zeval-0.1.0/zeval/evaluators/context_precision.py
--rw-r--r--   0 everfly    (501) wheel        (0)     5730 2024-05-10 10:53:55.000000 zeval-0.1.0/zeval/evaluators/context_recall.py
--rw-r--r--   0 everfly    (501) wheel        (0)     7174 2024-05-10 10:53:55.000000 zeval-0.1.0/zeval/evaluators/faithfulness.py
-drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-10 11:03:47.596377 zeval-0.1.0/zeval/utils/
--rw-r--r--   0 everfly    (501) wheel        (0)        0 2024-05-01 07:08:26.000000 zeval-0.1.0/zeval/utils/__init__.py
--rw-r--r--   0 everfly    (501) wheel        (0)      757 2024-05-10 10:53:55.000000 zeval-0.1.0/zeval/utils/model_caller.py
-drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-10 11:03:47.594664 zeval-0.1.0/zeval.egg-info/
--rw-r--r--   0 everfly    (501) wheel        (0)      651 2024-05-10 11:03:47.000000 zeval-0.1.0/zeval.egg-info/PKG-INFO
--rw-r--r--   0 everfly    (501) wheel        (0)      468 2024-05-10 11:03:47.000000 zeval-0.1.0/zeval.egg-info/SOURCES.txt
--rw-r--r--   0 everfly    (501) wheel        (0)        1 2024-05-10 11:03:47.000000 zeval-0.1.0/zeval.egg-info/dependency_links.txt
--rw-r--r--   0 everfly    (501) wheel        (0)       25 2024-05-10 11:03:47.000000 zeval-0.1.0/zeval.egg-info/requires.txt
--rw-r--r--   0 everfly    (501) wheel        (0)        6 2024-05-10 11:03:47.000000 zeval-0.1.0/zeval.egg-info/top_level.txt
+drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-21 08:54:33.409367 zeval-0.1.1/
+-rw-r--r--   0 everfly    (501) wheel        (0)      651 2024-05-21 08:54:33.409211 zeval-0.1.1/PKG-INFO
+-rw-r--r--   0 everfly    (501) wheel        (0)       38 2024-05-21 08:54:33.409400 zeval-0.1.1/setup.cfg
+-rw-r--r--   0 everfly    (501) wheel        (0)      887 2024-05-21 08:53:46.000000 zeval-0.1.1/setup.py
+drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-21 08:54:33.407220 zeval-0.1.1/zeval/
+-rw-r--r--   0 everfly    (501) wheel        (0)        0 2024-05-01 07:04:24.000000 zeval-0.1.1/zeval/__init__.py
+drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-21 08:54:33.407843 zeval-0.1.1/zeval/config/
+-rw-r--r--   0 everfly    (501) wheel        (0)        0 2024-05-01 07:08:33.000000 zeval-0.1.1/zeval/config/__init__.py
+-rw-r--r--   0 everfly    (501) wheel        (0)      180 2024-05-10 10:53:55.000000 zeval-0.1.1/zeval/config/model_config.py
+-rw-r--r--   0 everfly    (501) wheel        (0)      492 2024-05-20 12:59:22.000000 zeval-0.1.1/zeval/evaluation.py
+drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-21 08:54:33.408495 zeval-0.1.1/zeval/evaluators/
+-rw-r--r--   0 everfly    (501) wheel        (0)      211 2024-05-10 10:53:55.000000 zeval-0.1.1/zeval/evaluators/__init__.py
+-rw-r--r--   0 everfly    (501) wheel        (0)     6929 2024-05-19 09:09:39.000000 zeval-0.1.1/zeval/evaluators/answer_relevancy.py
+-rw-r--r--   0 everfly    (501) wheel        (0)     4327 2024-05-19 09:09:28.000000 zeval-0.1.1/zeval/evaluators/context_precision.py
+-rw-r--r--   0 everfly    (501) wheel        (0)     8276 2024-05-19 09:09:17.000000 zeval-0.1.1/zeval/evaluators/context_recall.py
+-rw-r--r--   0 everfly    (501) wheel        (0)     9640 2024-05-20 12:57:21.000000 zeval-0.1.1/zeval/evaluators/faithfulness.py
+drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-21 08:54:33.408687 zeval-0.1.1/zeval/utils/
+-rw-r--r--   0 everfly    (501) wheel        (0)        0 2024-05-01 07:08:26.000000 zeval-0.1.1/zeval/utils/__init__.py
+-rw-r--r--   0 everfly    (501) wheel        (0)     1245 2024-05-19 07:31:36.000000 zeval-0.1.1/zeval/utils/model.py
+drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-21 08:54:33.408983 zeval-0.1.1/zeval.egg-info/
+-rw-r--r--   0 everfly    (501) wheel        (0)      651 2024-05-21 08:54:33.000000 zeval-0.1.1/zeval.egg-info/PKG-INFO
+-rw-r--r--   0 everfly    (501) wheel        (0)      461 2024-05-21 08:54:33.000000 zeval-0.1.1/zeval.egg-info/SOURCES.txt
+-rw-r--r--   0 everfly    (501) wheel        (0)        1 2024-05-21 08:54:33.000000 zeval-0.1.1/zeval.egg-info/dependency_links.txt
+-rw-r--r--   0 everfly    (501) wheel        (0)       25 2024-05-21 08:54:33.000000 zeval-0.1.1/zeval.egg-info/requires.txt
+-rw-r--r--   0 everfly    (501) wheel        (0)        6 2024-05-21 08:54:33.000000 zeval-0.1.1/zeval.egg-info/top_level.txt
```

### Comparing `zeval-0.1.0/PKG-INFO` & `zeval-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeval
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library for evaluating RAG outputs of Chinese large language models.
 Home-page: https://github.com/yourgithub/zeval
 Author: everfly
 Author-email: tagriver@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zeval-0.1.0/setup.py` & `zeval-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='zeval',
-    version='0.1.0',
+    version='0.1.1',
     author='everfly',
     author_email='tagriver@gmail.com',
     description='A Python library for evaluating RAG outputs of Chinese large language models.',
     # long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/yourgithub/zeval',
     packages=find_packages(),
```

### Comparing `zeval-0.1.0/zeval/evaluators/answer_relevancy.py` & `zeval-0.1.1/zeval/evaluators/answer_relevancy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,146 +1,148 @@
-# zeval/zeval/evaluators/faithfulness.py
-from zeval.utils.model_caller import ModelCaller
+from zeval.utils.model import ModelCaller
 from typing import Any, Callable, Dict
 from datasets import Dataset
 import logging
 import time, json, os 
 import numpy as np
 import re, json, logging
 from openai import OpenAI
 logging.basicConfig(level=logging.INFO)
 
 class AnswerRelevancy:
     name = 'answer_relevancy'
 
-    #################
-    # question template
-    #################
-    QUESTION_TEMPLDATE = """
-    为给定的答案生成问题。
-    答案：
-    PSLV-C56任务预定于2023年7月30日星期日IST上午6:30 / UTC凌晨1:00发射。它将从位于印度安得拉邦斯里赫里戈塔的萨蒂什·达瓦恩航天中心发射。
-    问题：
-    PSLV-C56任务的预定发射日期和时间是什么时候？它将从哪里发射？
-
-    答案：{answer}
-    问题：
-    """
-    
-    CORRELATION_PROMPT_TEMPLATE = """任务：估计两个给定字符串之间的相关度。在你的评估中，不仅要考虑直接的联系，还要考虑间接和微妙的关联。
-    例如，如果第一个字符串中出现了‘桥’，第二个中出现了‘水’，你可以考虑组合词‘水上桥梁’。同样地，对于‘书’和‘智慧’，考虑像‘书籍是智慧的钥匙’这样的短语。
-    你应该使用以下从0.00到1.00的评分标准来评估相关性，其中：
-    0.00表示完全没有相关性。
-    0.50表示中等程度的相关性。这意味着两个字符串中的术语有几个显著的联系，但这些联系不是压倒性的。
-    1.00仅保留给完全相同的两个字符串。
-
-    要比较相关度的字符串：
-    string_one: {statement_one}
-    string_two: {statement_two}
-
-    你的最终输出应该按照以下格式（注意：包括方括号）：
-    理由：<your reasoning>
-    最终答案：[<float, rounded to the 100th place>]"""
-
-    REASONING_MESSAGE = """
-    我的推理过程如下：
-    首先，我根据给定的答案生成了一个最可能的问题，然后我将生成的问题和原始问题分别通过embedding转化成向量，然后再计算向量之间的余弦相似度。
-    
-    大模型生成的答案是：
-    {answer}
-    
-    我由此生成的问题是：
-    {gen_question}
-    
-    用户原来的问题是：
-    {question}
-        
-    通过计算余弦相似度，由此得出的回答相似度得分是：{result}
-    """
+    PROMPTS = {
+        'en': {
+            'QUESTION_TEMPLATE': """
+Generate a question for the given answer.
+Answer:
+The PSLV-C56 mission is scheduled to launch on Sunday, July 30, 2023, at 6:30 AM IST / 1:00 AM UTC. It will be launched from the Satish Dhawan Space Centre in Sriharikota, Andhra Pradesh, India.
+Question:
+What is the scheduled launch date and time for the PSLV-C56 mission? Where will it be launched from?
+
+Answer: {answer}
+Question:
+""",
+            'CORRELATION_PROMPT_TEMPLATE': """
+Task: Estimate the correlation between the two given strings. In your evaluation, consider not only direct connections but also indirect and subtle associations.
+For example, if 'bridge' appears in the first string and 'water' in the second, consider the compound term 'water bridge.' Similarly, for 'book' and 'wisdom,' consider phrases like 'books are keys to wisdom.'
+You should use the following scoring scale from 0.00 to 1.00 to assess correlation, where:
+0.00 means no correlation at all.
+0.50 means moderate correlation. This implies several significant links between the terms in the two strings, but not overwhelmingly so.
+1.00 is reserved for two identical strings.
+
+Strings to compare:
+string_one: {statement_one}
+string_two: {statement_two}
+
+Your final output should follow this format (note: include the brackets):
+Reasoning: <your reasoning>
+Final answer: [<float, rounded to the 100th place>]""",
+            'REASONING_MESSAGE': """
+My reasoning process is as follows:
+First, I generated the most likely question for the given answer, then I converted the generated question and the original question into vectors using embeddings, and finally calculated the cosine similarity between the vectors.
+
+The generated answer by the large model is:
+{answer}
+
+The question I generated is:
+{gen_question}
+
+The original question provided by the user is:
+{question}
+
+By calculating the cosine similarity, the derived answer relevance score is: {result}
+"""
+        },
+        'zh': {
+            'QUESTION_TEMPLATE': """
+为给定的答案生成问题。
+答案：
+PSLV-C56任务预定于2023年7月30日星期日IST上午6:30 / UTC凌晨1:00发射。它将从位于印度安得拉邦斯里赫里戈塔的萨蒂什·达瓦恩航天中心发射。
+问题：
+PSLV-C56任务的预定发射日期和时间是什么时候？它将从哪里发射？
+
+答案：{answer}
+问题：
+""",
+            'CORRELATION_PROMPT_TEMPLATE': """
+任务：估计两个给定字符串之间的相关度。在你的评估中，不仅要考虑直接的联系，还要考虑间接和微妙的关联。
+例如，如果第一个字符串中出现了‘桥’，第二个中出现了‘水’，你可以考虑组合词‘水上桥梁’。同样地，对于‘书’和‘智慧’，考虑像‘书籍是智慧的钥匙’这样的短语。
+你应该使用以下从0.00到1.00的评分标准来评估相关性，其中：
+0.00表示完全没有相关性。
+0.50表示中等程度的相关性。这意味着两个字符串中的术语有几个显著的联系，但这些联系不是压倒性的。
+1.00仅保留给完全相同的两个字符串。
+
+要比较相关度的字符串：
+string_one: {statement_one}
+string_two: {statement_two}
+
+你的最终输出应该按照以下格式（注意：包括方括号）：
+理由：<your reasoning>
+最终答案：[<float, rounded to the 100th place>]""",
+            'REASONING_MESSAGE': """
+我的推理过程如下：
+首先，我根据给定的答案生成了一个最可能的问题，然后我将生成的问题和原始问题分别通过embedding转化成向量，然后再计算向量之间的余弦相似度。
+
+大模型生成的答案是：
+{answer}
+
+我由此生成的问题是：
+{gen_question}
+
+用户原来的问题是：
+{question}
+
+通过计算余弦相似度，由此得出的回答相似度得分是：{result}
+"""
+        }
+    }
 
-    def __init__(self):
-        pass
+    def __init__(self, lang='zh'):
+        self.language = lang
 
-    def score(self, dataset: Dataset, sample_kwargs: Dict[str, Any] = None):
+    def get_prompt(self, key):
+        return self.PROMPTS[self.language][key]
 
+    def score(self, dataset: Dataset, sample_kwargs: Dict[str, Any] = None):
         if dataset is None:
             params = {}
         if sample_kwargs is None:
             sample_kwargs = {}
 
         question = dataset["question"]
         answer = dataset["answer"]
         context = dataset["context"]
-        
-        question_prompt = self.QUESTION_TEMPLDATE.format(answer=answer)
+
+        question_prompt = self.get_prompt('QUESTION_TEMPLATE').format(answer=answer)
         if isinstance(question_prompt, str):
             messages = [{"role": "user", "content": question_prompt}]
-            
-        start_time = time.time() # 开始计时
-        gen_question_response = ModelCaller.call(self, messages=messages, **sample_kwargs)
-        end_time = time.time() # 结束计时
-        elapsed_time = end_time - start_time # 计算经过的时间
-        
-        gen_question = self.parse_response(gen_question_response)
-        
-        print("gen_question: ", gen_question)
 
+        gen_question_response, elapsed_time = ModelCaller.call(self, messages=messages, **sample_kwargs)
+        gen_question = ModelCaller.parse_response(gen_question_response)
         gen_question_response.elapsed_time = elapsed_time
         gen_question_response.prompt = json.dumps(question_prompt)
         gen_question_response.completion = gen_question
 
-        end_time = time.time() # 结束计时
-        elapsed_time = end_time - start_time # 计算经过的时间
-        
-        # # 计算余弦相似度
-        # params = {}        
-        # # 指定OpenAI的api_key
-        # _evn_api_key = os.environ.get("OPENAI_API_KEY")
-        # if 'api_key' in sample_kwargs and sample_kwargs["provider"] == "openai":
-        #     params["api_key"] = sample_kwargs["api_key"]
-        # else:
-        #     params["api_key"] = _evn_api_key
-
-        # client = OpenAI(**params)
-        # question_vec_response = client.embeddings.create(model="text-embedding-ada-002", input=question, encoding_format="float")
-        # embedding_score = question_vec_response.data[0].embedding
-        # question_vec = np.asarray(embedding_score).reshape(1, -1)
-
-        # gen_question_vec_response = client.embeddings.create(model="text-embedding-ada-002", input=gq_output, encoding_format="float")
-        # gen_embedding_score = gen_question_vec_response.data[0].embedding    
-        # gen_question_vec = np.asarray(gen_embedding_score).reshape(1, -1)
-
-        # norm = np.linalg.norm(gen_question_vec, axis=1) * np.linalg.norm(question_vec, axis=1)
-        # cosine_sim = np.dot(gen_question_vec, question_vec.T).reshape(-1,) / norm
-
-        # result = cosine_sim.mean()
-        
-        correlation_prompt = self.CORRELATION_PROMPT_TEMPLATE.format(statement_one=question, statement_two=gen_question)
+        correlation_prompt = self.get_prompt('CORRELATION_PROMPT_TEMPLATE').format(statement_one=question, statement_two=gen_question)
         if isinstance(correlation_prompt, str):
             messages = [{"role": "user", "content": correlation_prompt}]
-            
-        start_time = time.time() # 开始计时
-        correlation_response = ModelCaller.call(self, messages=messages, **sample_kwargs)
-        end_time = time.time() # 结束计时
-        elapsed_time = end_time - start_time # 计算经过的时间
-        
+
+        correlation_response, elapsed_time = ModelCaller.call(self, messages=messages, **sample_kwargs)
         correlation_result = self.parse_response(correlation_response)
-        print("correlation_result: ", correlation_result)
-        
         correlation_response.elapsed_time = elapsed_time
         correlation_response.prompt = json.dumps(correlation_prompt)
         correlation_response.completion = correlation_result
-        
+
         result_score = self.extract_score(correlation_result)
-        
-        reasoning = self.REASONING_MESSAGE.format(answer=answer, gen_question=gen_question, question=question, result=result_score)
-        
+
+        reasoning = self.get_prompt('REASONING_MESSAGE').format(answer=answer, gen_question=gen_question, question=question, result=result_score)
+
         responses = [gen_question_response, correlation_response]
-        print("reasoning: ", reasoning)
-        print("responses: ", responses)
         return result_score, reasoning, responses
 
     @staticmethod
     def extract_score(response_content: str) -> float:
         """
         Extracts the similarity score from the content of a GPT model's response.
 
@@ -154,16 +156,7 @@
             match = re.search(r"最终答案[:：]\s*\[(.+?)]", response_content).group(1)
             score = float(match)
             logging.debug(f"response_content: {response_content}, score: {score}")
         except AttributeError:
             score = 0.0
             logging.warning("Answer not found in response, score set to 0, will autofail validation scoring.")
         return score
-    
-    def parse_response(self, response):
-        try:
-            # 从模型响应中获得最终陈述
-            choices = response.choices
-            final_statement = choices[0].message.content 
-            return final_statement
-        except Exception as e:
-            return False
```

### Comparing `zeval-0.1.0/zeval/evaluators/context_precision.py` & `zeval-0.1.1/zeval/evaluators/context_precision.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,107 +1,114 @@
-# zeval/zeval/evaluators/faithfulness.py
-from zeval.utils.model_caller import ModelCaller
+from zeval.utils.model import ModelCaller
 from typing import Any, Callable, Dict
 from datasets import Dataset
 import logging
 import time, json
 logging.basicConfig(level=logging.INFO)
 
 class ContextPrecision:
     name = 'context_precision'
 
-    ##############################
-    # CONTEXT PRECISION TEMPLATE #
-    ##############################
-    CONTEXT_PRECISION_TEMPLATE = """\
-    给定一个问题和一个上下文，验证给定的上下文中的信息是否有助于回答这个问题。返回一个“Yes”或“No”的答案。
-    问题：
-    {question}
-    上下文：
-    {context}
-    答案：
-    """ 
-    
-    REASONING_MESSAGE = """
-    我的推理过程如下：
-    我会遍历每个上下文信息，验证给定的上下文中的信息是否有助于回答这个问题。返回一个“Yes”或“No”的答案，并将其转化为True或False的相应。
-    
-    以下依次是我对每个上下文的判断：
-    {judges}
-    
-    然后，通过计算排在前面的所有正确响应（True）的累计精度的平均值，得出的平均精度得分是：{result}  
-    """
+    PROMPTS = {
+        'en': {
+            'CONTEXT_PRECISION_TEMPLATE': """\
+Given a question and a context, verify whether the information in the given context helps answer the question. Return a "Yes" or "No" answer.
+Question:
+{question}
+Context:
+{context}
+Answer:
+""",
+            'REASONING_MESSAGE': """
+My reasoning process is as follows:
+I will go through each context, verify whether the information in the given context helps answer the question, and return a "Yes" or "No" answer, which I will convert to True or False accordingly.
+
+Here are my judgments for each context:
+{judges}
+
+Then, by calculating the cumulative precision of all the correct responses (True) up to that point, the average precision score is: {result}
+"""
+        },
+        'zh': {
+            'CONTEXT_PRECISION_TEMPLATE': """\
+给定一个问题和一个上下文，验证给定的上下文中的信息是否有助于回答这个问题。返回一个“Yes”或“No”的答案。
+问题：
+{question}
+上下文：
+{context}
+答案：
+""",
+            'REASONING_MESSAGE': """
+我的推理过程如下：
+我会遍历每个上下文信息，验证给定的上下文中的信息是否有助于回答这个问题。返回一个“Yes”或“No”的答案，并将其转化为True或False的相应。
+
+以下依次是我对每个上下文的判断：
+{judges}
+
+然后，通过计算排在前面的所有正确响应（True）的累计精度的平均值，得出的平均精度得分是：{result}
+"""
+        }
+    }
 
-    def __init__(self):
-        pass
+    def __init__(self, lang='zh'):
+        self.language = lang
+
+    def get_prompt(self, key):
+        return self.PROMPTS[self.language][key]
 
     def score(self, dataset: Dataset, sample_kwargs: Dict[str, Any] = None):
         if dataset is None:
             params = {}
         if sample_kwargs is None:
             sample_kwargs = {}
-        
+
         question = dataset["question"]
-        answer = dataset["answer"]
         context = dataset["context"][0]
-                
+
         """
         根据问题和上下文计算上下文精确度。
         """
         determine_results, determine_responses = self.determine_usefulness(question, context, sample_kwargs)
-        
-        print("determine_results: ", determine_results)
 
         result_score = self.calculate_average_precision(determine_results)
-        
+
         string_results = [str(result) for result in determine_results]
         judges = ",".join(string_results)
-    
-        reasoning = self.REASONING_MESSAGE.format(judges=judges, result=result_score)
+
+        reasoning = self.get_prompt('REASONING_MESSAGE').format(judges=judges, result=result_score)
         print("reasoning: ", reasoning)
         return result_score, reasoning, determine_responses
 
     def determine_usefulness(self, question: str, contexts: list[str], sample_kwargs: dict = None) -> list[bool]:
         determine_responses = []
         determine_results = []
         for context in contexts:
-            start_time = time.time() # 开始计时
-            determine_prompt = self.CONTEXT_PRECISION_TEMPLATE.format(question=question, context=context)
+            start_time = time.time()  # 开始计时
+            determine_prompt = self.get_prompt('CONTEXT_PRECISION_TEMPLATE').format(question=question, context=context)
             if isinstance(determine_prompt, str):
                 messages = [{"role": "user", "content": determine_prompt}]
-                
-            start_time = time.time() # 开始计时
+
             determine_response = ModelCaller.call(self, messages=messages, **sample_kwargs)
-            end_time = time.time() # 结束计时
-            elapsed_time = end_time - start_time # 计算经过的时间
-            
-            determine_result = self.parse_response(determine_response)
-            
+            elapsed_time = time.time() - start_time  # 计算经过的时间
+
+            determine_result = ModelCaller.parse_response(determine_response)
+
             print("determine_result: ", determine_result)
 
             determine_response.elapsed_time = elapsed_time
             determine_response.prompt = json.dumps(determine_prompt)
             determine_response.completion = determine_result
-            
+
             determine_results.append("Yes" in determine_result)
             determine_responses.append(determine_response)
 
         return determine_results, determine_responses
 
     def calculate_average_precision(self, responses: list[bool]) -> float:
         if not responses:
             return 0.0
         numerator, denominator = 0, 0
         for i, resp in enumerate(responses, start=1):
             if resp:
                 numerator += sum(responses[:i]) / i
                 denominator += 1
         return numerator / denominator if denominator > 0 else 0.0
-    
-    def parse_response(self, response):
-        try:
-            # 从模型响应中获得最终陈述
-            choices = response.choices
-            final_statement = choices[0].message.content 
-            return final_statement
-        except Exception as e:
-            return False
```

### Comparing `zeval-0.1.0/zeval.egg-info/PKG-INFO` & `zeval-0.1.1/zeval.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeval
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library for evaluating RAG outputs of Chinese large language models.
 Home-page: https://github.com/yourgithub/zeval
 Author: everfly
 Author-email: tagriver@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

