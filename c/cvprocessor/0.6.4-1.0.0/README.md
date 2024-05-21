# Comparing `tmp/cvprocessor-0.6.4.tar.gz` & `tmp/cvprocessor-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvprocessor-0.6.4.tar", last modified: Wed May 15 07:16:53 2024, max compression
+gzip compressed data, was "cvprocessor-1.0.0.tar", last modified: Tue May 21 01:39:52 2024, max compression
```

## Comparing `cvprocessor-0.6.4.tar` & `cvprocessor-1.0.0.tar`

### file list

```diff
@@ -1,34 +1,50 @@
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-15 07:16:53.431023 cvprocessor-0.6.4/
--rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.6.4/LICENSE
--rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-15 07:16:53.430442 cvprocessor-0.6.4/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-0.6.4/README.md
--rw-r--r--   0 fernando   (501) staff       (20)      769 2024-05-15 07:16:43.000000 cvprocessor-0.6.4/pyproject.toml
--rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-15 07:16:53.431131 cvprocessor-0.6.4/setup.cfg
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-15 07:16:53.409819 cvprocessor-0.6.4/src/
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-15 07:16:53.426519 cvprocessor-0.6.4/src/cvprocessor/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.6.4/src/cvprocessor/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)    10464 2024-05-15 03:47:26.000000 cvprocessor-0.6.4/src/cvprocessor/authors.py
--rw-r--r--   0 fernando   (501) staff       (20)      363 2024-05-15 02:16:23.000000 cvprocessor-0.6.4/src/cvprocessor/common.py
--rw-r--r--   0 fernando   (501) staff       (20)     7750 2024-05-15 05:44:19.000000 cvprocessor-0.6.4/src/cvprocessor/cv.py
--rw-r--r--   0 fernando   (501) staff       (20)     4882 2024-05-15 03:56:47.000000 cvprocessor-0.6.4/src/cvprocessor/education.py
--rw-r--r--   0 fernando   (501) staff       (20)     3758 2024-05-15 04:08:11.000000 cvprocessor-0.6.4/src/cvprocessor/experience.py
--rw-r--r--   0 fernando   (501) staff       (20)     4051 2024-05-15 03:58:18.000000 cvprocessor-0.6.4/src/cvprocessor/grants_awards.py
--rw-r--r--   0 fernando   (501) staff       (20)     7113 2024-05-15 04:39:45.000000 cvprocessor-0.6.4/src/cvprocessor/institutes.py
--rw-r--r--   0 fernando   (501) staff       (20)     1943 2024-05-15 04:09:24.000000 cvprocessor-0.6.4/src/cvprocessor/intro.py
--rw-r--r--   0 fernando   (501) staff       (20)     1921 2024-05-15 04:10:03.000000 cvprocessor-0.6.4/src/cvprocessor/memberships.py
--rw-r--r--   0 fernando   (501) staff       (20)     4435 2024-05-15 04:11:19.000000 cvprocessor-0.6.4/src/cvprocessor/news.py
--rw-r--r--   0 fernando   (501) staff       (20)    16444 2024-05-15 07:16:36.000000 cvprocessor-0.6.4/src/cvprocessor/publications.py
--rw-r--r--   0 fernando   (501) staff       (20)     2697 2024-05-15 04:26:24.000000 cvprocessor-0.6.4/src/cvprocessor/references.py
--rw-r--r--   0 fernando   (501) staff       (20)     1656 2024-05-15 04:26:39.000000 cvprocessor-0.6.4/src/cvprocessor/research_interests.py
--rw-r--r--   0 fernando   (501) staff       (20)     2540 2024-05-15 04:27:18.000000 cvprocessor-0.6.4/src/cvprocessor/service.py
--rw-r--r--   0 fernando   (501) staff       (20)     3316 2024-05-15 04:27:50.000000 cvprocessor-0.6.4/src/cvprocessor/skills.py
--rw-r--r--   0 fernando   (501) staff       (20)     4916 2024-05-15 04:39:59.000000 cvprocessor-0.6.4/src/cvprocessor/software.py
--rw-r--r--   0 fernando   (501) staff       (20)     5247 2024-05-15 04:39:23.000000 cvprocessor-0.6.4/src/cvprocessor/supervision.py
--rw-r--r--   0 fernando   (501) staff       (20)     5270 2024-05-15 02:19:52.000000 cvprocessor-0.6.4/src/cvprocessor/teaching.py
--rw-r--r--   0 fernando   (501) staff       (20)     3482 2024-05-15 02:26:14.000000 cvprocessor-0.6.4/src/cvprocessor/year_data.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-15 07:16:53.429864 cvprocessor-0.6.4/src/cvprocessor.egg-info/
--rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-15 07:16:53.000000 cvprocessor-0.6.4/src/cvprocessor.egg-info/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      800 2024-05-15 07:16:53.000000 cvprocessor-0.6.4/src/cvprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-15 07:16:53.000000 cvprocessor-0.6.4/src/cvprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-15 07:16:53.000000 cvprocessor-0.6.4/src/cvprocessor.egg-info/requires.txt
--rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-15 07:16:53.000000 cvprocessor-0.6.4/src/cvprocessor.egg-info/top_level.txt
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-21 01:39:52.979585 cvprocessor-1.0.0/
+-rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-1.0.0/LICENSE
+-rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-21 01:39:52.978988 cvprocessor-1.0.0/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-1.0.0/README.md
+-rw-r--r--   0 fernando   (501) staff       (20)      769 2024-05-21 01:38:05.000000 cvprocessor-1.0.0/pyproject.toml
+-rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-21 01:39:52.979703 cvprocessor-1.0.0/setup.cfg
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-21 01:39:52.946666 cvprocessor-1.0.0/src/
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-21 01:39:52.966790 cvprocessor-1.0.0/src/cvprocessor/
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-21 01:39:52.971866 cvprocessor-1.0.0/src/cvprocessor/Personal/
+-rw-r--r--   0 fernando   (501) staff       (20)     1532 2024-05-19 08:40:56.000000 cvprocessor-1.0.0/src/cvprocessor/Personal/Personal.py
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-17 22:49:39.000000 cvprocessor-1.0.0/src/cvprocessor/Personal/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-1.0.0/src/cvprocessor/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4365 2024-05-19 02:09:16.000000 cvprocessor-1.0.0/src/cvprocessor/authors.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-21 01:39:52.972666 cvprocessor-1.0.0/src/cvprocessor/contact/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-17 23:11:09.000000 cvprocessor-1.0.0/src/cvprocessor/contact/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2459 2024-05-19 10:34:03.000000 cvprocessor-1.0.0/src/cvprocessor/contact/contact.py
+-rw-r--r--   0 fernando   (501) staff       (20)     7749 2024-05-20 00:37:00.000000 cvprocessor-1.0.0/src/cvprocessor/cv.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-21 01:39:52.973658 cvprocessor-1.0.0/src/cvprocessor/date/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-18 23:14:35.000000 cvprocessor-1.0.0/src/cvprocessor/date/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3445 2024-05-19 09:59:29.000000 cvprocessor-1.0.0/src/cvprocessor/date/date.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3179 2024-05-19 22:43:58.000000 cvprocessor-1.0.0/src/cvprocessor/education.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2945 2024-05-20 02:00:23.000000 cvprocessor-1.0.0/src/cvprocessor/experience.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3232 2024-05-19 23:43:56.000000 cvprocessor-1.0.0/src/cvprocessor/grants_awards.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3301 2024-05-19 02:18:35.000000 cvprocessor-1.0.0/src/cvprocessor/institutes.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1943 2024-05-15 04:09:24.000000 cvprocessor-1.0.0/src/cvprocessor/intro.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-21 01:39:52.974518 cvprocessor-1.0.0/src/cvprocessor/links/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-17 22:55:50.000000 cvprocessor-1.0.0/src/cvprocessor/links/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2957 2024-05-21 01:29:26.000000 cvprocessor-1.0.0/src/cvprocessor/links/links.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1534 2024-05-19 10:04:27.000000 cvprocessor-1.0.0/src/cvprocessor/memberships.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-21 01:39:52.975411 cvprocessor-1.0.0/src/cvprocessor/name/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-19 02:13:29.000000 cvprocessor-1.0.0/src/cvprocessor/name/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)      937 2024-05-19 02:16:28.000000 cvprocessor-1.0.0/src/cvprocessor/name/name.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2568 2024-05-19 02:27:08.000000 cvprocessor-1.0.0/src/cvprocessor/news.py
+-rw-r--r--   0 fernando   (501) staff       (20)    13634 2024-05-19 23:51:45.000000 cvprocessor-1.0.0/src/cvprocessor/publications.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1623 2024-05-20 03:02:34.000000 cvprocessor-1.0.0/src/cvprocessor/references.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1491 2024-05-19 08:07:27.000000 cvprocessor-1.0.0/src/cvprocessor/research_interests.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-21 01:39:52.976791 cvprocessor-1.0.0/src/cvprocessor/security/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-17 23:18:52.000000 cvprocessor-1.0.0/src/cvprocessor/security/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1021 2024-05-17 23:21:12.000000 cvprocessor-1.0.0/src/cvprocessor/security/security.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2110 2024-05-20 02:54:45.000000 cvprocessor-1.0.0/src/cvprocessor/service.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2982 2024-05-20 02:08:33.000000 cvprocessor-1.0.0/src/cvprocessor/skills.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3484 2024-05-19 22:06:55.000000 cvprocessor-1.0.0/src/cvprocessor/software.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3048 2024-05-20 01:46:13.000000 cvprocessor-1.0.0/src/cvprocessor/supervision.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2577 2024-05-20 01:38:33.000000 cvprocessor-1.0.0/src/cvprocessor/teaching.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-21 01:39:52.978061 cvprocessor-1.0.0/src/cvprocessor.egg-info/
+-rw-r--r--   0 fernando   (501) staff       (20)     1700 2024-05-21 01:39:52.000000 cvprocessor-1.0.0/src/cvprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)     1153 2024-05-21 01:39:52.000000 cvprocessor-1.0.0/src/cvprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-21 01:39:52.000000 cvprocessor-1.0.0/src/cvprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-21 01:39:52.000000 cvprocessor-1.0.0/src/cvprocessor.egg-info/requires.txt
+-rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-21 01:39:52.000000 cvprocessor-1.0.0/src/cvprocessor.egg-info/top_level.txt
```

### Comparing `cvprocessor-0.6.4/LICENSE` & `cvprocessor-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.4/PKG-INFO` & `cvprocessor-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.6.4
+Version: 1.0.0
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.6.4/README.md` & `cvprocessor-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.4/pyproject.toml` & `cvprocessor-1.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cvprocessor"
-version = "0.6.4"
+version = "1.0.0"
 authors = [
     { name = "F. Fernando Jurado-Lasso", email = "fdo.jurado@gmail.com" },
 ]
 description = "CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cvprocessor-0.6.4/src/cvprocessor/cv.py` & `cvprocessor-1.0.0/src/cvprocessor/cv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 This module contains the CV class that is used to create a CV object.
 The CV object is used to store all the information
 """
 import sys
 
 from cvprocessor.intro import Intro
-from cvprocessor.education import Education
+from cvprocessor.education import Educations
 from cvprocessor.publications import Publications
 from cvprocessor.authors import Authors
 from cvprocessor.software import Software
 from cvprocessor.institutes import Institutes
 from cvprocessor.news import News
 from cvprocessor.research_interests import ResearchInterests
 from cvprocessor.grants_awards import GrantsAwards
@@ -30,27 +30,27 @@
     :type filename: str
 
     :param cv_class: The CV class object.
     :type cv_class: CV
     """
 
     def __init__(self):
-        self.education = Education()
+        self.education = Educations()
         self.institutes = Institutes()
         self.research_interests = ResearchInterests()
         self.grants_awards = GrantsAwards()
         self.teaching = Teaching()
         self.supervision = Supervision()
         self.publications = Publications()
 
     def __str__(self):
         string = f"Education: {self.education}\n"
         string += f"Institutes: {self.institutes}\n"
         string += f"Research Interests: {self.research_interests}\n"
-        string += f"Grants and Awards: {self.grants_awards}\n"
+        string += f"Grants & Awards: {self.grants_awards}\n"
         string += f"Teaching: {self.teaching}\n"
         string += f"Supervision: {self.supervision}\n"
         string += f"Publications: {self.publications}\n"
         return string
 
     def __repr__(self):
         string = (
@@ -162,19 +162,19 @@
         authors_ids = []
         for author_id in authors_ids_affiliations_ids:
             authors_ids.append(author_id.get_author_id())
         authors_alias_short = []
         for author_id in authors_ids:
             author = self.personal.authors.get_author(author_id)
             if author is not None:
-                authors_alias_short.append(author.personal.get_alias_short())
+                authors_alias_short.append(author.personal.get_alias())
         if len(authors_alias_short) > 1:
             authors_alias_short[-1] = "& " + authors_alias_short[-1]
         authors_alias_short = ", ".join(authors_alias_short)
-        apa = authors_alias_short + apa
+        apa = authors_alias_short + " " + apa
         return apa
 
     def _load_cv(self, filename):
         """
         The _load_cv method is used to load the CV file.
 
         :param filename: The filename of the CV file.
@@ -214,14 +214,14 @@
             f"software={repr(self.software)}, "
             f"news={repr(self.news)})\n")
         return string
 
 
 if __name__ == "__main__":
     cv = CV("cv.xlsx")
-    print(str(cv.personal.references))
+    print(str(cv.academic.education))
     # Get the first publication
     # pub = cv.academic.publications.get_publications_by_index(0)
     # print(f"Publication title: {pub.details.get_title()}")
     # apa = cv.get_publications_apa_citation(pub.details.get_title())
     # print(f"APA Citation: {apa}")
     sys.exit(0)
```

### Comparing `cvprocessor-0.6.4/src/cvprocessor/education.py` & `cvprocessor-1.0.0/src/cvprocessor/authors.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,189 +1,149 @@
 """
-This module contains the classes to represent the education data of an author.
+    Authors module.
+
+    This module contains the classes to represent the authors of the CV.
+
+    Classes:
+    AuthorsData: A class to represent an author.
+    Authors: A class to represent a list of authors.
 """
 import pandas as pd
-from cvprocessor import year_data as yd
+from cvprocessor.security.security import Security
+from cvprocessor.Personal.Personal import Personal
+from cvprocessor.contact.contact import Contact
+from cvprocessor.links.links import Links
 
 
-class ThesisInfo:
+class AuthorsData:
     """
-    A class to represent the thesis information of an author.
+    A class to represent an author.
 
     Attributes:
-    thesis: The thesis.
-    thesis_link: The thesis link.
-    advisor: The advisor.
+    id (int): The ID of the author.
+    affiliations (list): The affiliations of the author.
+    personal_info (Personal): The personal information of the author.
+    contact_info (Contact): The contact information of the author.
+    research_info (Social): The research information of the author.
 
     Methods:
-    __str__: Returns the string representation of the thesis information.
-    __repr__: Returns the string representation of the thesis information.
+    load(filename): Loads the author data from the file.
+    __str__(): Returns a string representation of the author.
+    __repr__(): Returns a string representation of the author.
     """
 
     def __init__(self):
-        self.thesis = None
-        self.thesis_link = None
-        self.advisor = None
+        self.id = int()
+        self.job_title = str()
+        self.affiliation_ids = []
+        self.personal = Personal()
+        self.contact = Contact()
+        self.links = Links()
+        self.security = Security()
 
-    def get_thesis(self):
+    def get_id(self):
         """
-        Get the thesis.
+        Returns the ID of the author.
         """
-        return self.thesis
+        return self.id
 
-    def get_thesis_link(self):
+    def get_job_title(self):
         """
-        Get the thesis link.
+        Returns the job title of the author.
         """
-        return self.thesis_link
+        return self.job_title
 
-    def get_advisor(self):
+    def get_affiliation_ids(self):
         """
-        Get the advisor.
+        Returns the affiliations of the author.
         """
-        return self.advisor
+        return self.affiliation_ids
 
-    def load(self, filename):
+    def load(self, df):
         """
-        Load the thesis information.
+        Loads the author data from the file.
         """
-        self.thesis = filename["Thesis"]
-        self.thesis_link = filename["Thesis link"]
-        self.advisor = filename["Advisor"]
-
-    def __str__(self):
-        string = f"Thesis: {self.thesis}\n"
-        string += f"Thesis link: {self.thesis_link}\n"
-        string += f"Advisor: {self.advisor}\n"
-        return string
+        self.id = df["id"]
+        self.job_title = df["Job Title"]
+        if isinstance(df["Affiliations"], str) and\
+                ("," in df["Affiliations"] or ";" in df["Affiliations"]):
+            affiliations = df["Affiliations"].split(",")
+            for affiliation in affiliations:
+                self.affiliation_ids.append(int(affiliation))
+        else:
+            self.affiliation_ids.append(int(df["Affiliations"]))
+        self.personal.load(df)
+        self.contact.load(df)
+        self.links.load(df)
+        self.security.load(df)
 
     def __repr__(self):
         string = (
-            f"ThesisInfo("
-            f"thesis={self.thesis}, "
-            f"thesis_link={self.thesis_link}, "
-            f"advisor={self.advisor})"
+            f"AuthorsData("
+            f"id={self.id}, "
+            f"job_title={self.job_title}, "
+            f"affiliation_ids={self.affiliation_ids}, "
+            f"personal={repr(self.personal)}, "
+            f"contact={repr(self.contact)}, "
+            f"links={repr(self.links)}, "
+            f"security={repr(self.security)})"
         )
         return string
 
 
-class EducationData:
+class Authors:
     """
-    A class to represent the education data of an author.
-    """
-
-    def __init__(self):
-        self.degree = str()
-        self.award = str()
-        self.institution = str()
-        self.education_period = []
-        self.thesis_info = ThesisInfo()
-
-    def get_degree(self):
-        """
-        Get the degree.
-        """
-        return self.degree
-
-    def get_institution(self):
-        """
-        Get the institution.
-        """
-        return self.institution
-
-    def get_award(self):
-        """
-        Get the award.
-        """
-        return self.award
-
-    def get_start_year(self):
-        """
-        Get the start year of this experience.
-        """
-        return yd.get_start_year(self.education_period)
-
-    def get_end_year(self):
-        """
-        Get the end year of this experience.
-        """
-        return yd.get_end_year(self.education_period)
-
-    def process_year_data(self, filename):
-        """
-        Process the year data.
-        """
-        self.education_period = yd.process_year_data(
-            filename, self.education_period)
-
-    def load(self, filename):
-        """
-        Load the education data from the filename.
-        """
-        self.degree = filename["Degree"]
-        self.award = filename["Award"]
-        self.institution = filename["Institution"]
-        self.process_year_data(filename)
-        self.thesis_info.load(filename)
-
-    def __str__(self):
-        string = f"Degree: {self.degree}\n"
-        string += f"Award: {self.award}\n"
-        string += f"Institution: {self.institution}\n"
-        string += str(self.education_period)
-        string += str(self.thesis_info)
-        return string
-
-    def __repr__(self) -> str:
-        string = (
-            f"EducationData("
-            f"degree={repr(self.degree)}, "
-            f"award={repr(self.award)}, "
-            f"institution={repr(self.institution)}, "
-            f"education_period={repr(self.education_period)}, "
-            f"thesis_info={repr(self.thesis_info)})"
-        )
-        return string
-
-
-class Education:
-    """
-    A class to represent the education data of an author.
+    A class to represent a list of authors.
 
     Attributes:
-    educations (list): The list of education data.
+    authors (list): The list of authors.
+
+    Methods:
+    get_author(author_id, affiliation_id): Gets the author.
+    load(filename): Loads the authors from the file.
+    __str__(): Returns a string representation of the authors.
+    __repr__(): Returns a string representation of the authors.
     """
 
     def __init__(self):
-        self.educations = []
+        self.authors = []
 
-    # Get the oldest end year
-    def get_oldest_end_year(self):
+    def get_author(self, author_id, affiliation_id=None):
         """
-        Gets the oldest end year of the education data.
+        Gets the author by ID and affiliation ID.
         """
-        return self.educations[-1].education_period.end_year
+        if isinstance(author_id, str):
+            author_id = int(author_id)
+        if affiliation_id is None:
+            for author in self.authors:
+                if author.get_id() == author_id:
+                    return author
+            return None
+        for author in self.authors:
+            if author.get_id() == author_id and affiliation_id in author.get_affiliation_ids():
+                return author
+        return None
 
     def load(self, filename):
         """
-        Load the education data.
+        Loads the authors from the file.
         """
-        education_df = pd.read_excel(filename, sheet_name="Education")
-        for _, row in education_df.iterrows():
-            self.educations.append(EducationData())
-            self.educations[-1].load(row)
-        # sort the education data by end year
-        self.educations = sorted(
-            self.educations, key=lambda x: x.get_end_year(), reverse=True)
+        authors_df = pd.read_excel(filename, sheet_name="Authors")
+        for _, row in authors_df.iterrows():
+            self.authors.append(AuthorsData())
+            self.authors[-1].load(row)
 
-    def __str__(self) -> str:
+    def __str__(self):
         string = ""
-        for education in self.educations:
-            string += str(education) + "\n"
+        for author in self.authors:
+            string += str(author) + "\n"
         return string
 
-    def __repr__(self) -> str:
-        string = f"Education(educations={repr(self.educations)})"
+    def __repr__(self):
+        string = (
+            f"Authors("
+            f"authors={repr(self.authors)})"
+        )
         return string
 
     def __iter__(self):
-        return iter(self.educations)
+        return iter(self.authors)
```

### Comparing `cvprocessor-0.6.4/src/cvprocessor/experience.py` & `cvprocessor-1.0.0/src/cvprocessor/grants_awards.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,132 +1,109 @@
 """
-This module contains the ExperienceData and Experience classes.
+This module contains the GrantsAwards class and GrantsAwardsData class.
 """
 import pandas as pd
-from cvprocessor import year_data as yd
 
+from cvprocessor.date.date import Dates
 
-class ExperienceData:
+
+class GrantsAwardsData:
     """
-    The ExperienceData class is used to store the experience data.
+    A class to represent the grants and awards data.
 
     Attributes:
-    year (YearData): The year of the experience.
-    position (str): The position of the experience.
-    institution (str): The institution of the experience.
-    description (str): The description of the experience.
-    responsibilities (str): The responsibilities of the experience.
+    date: The date of the grant or award.
+    description: The description of the grant or award.
+    institution: The institution that awarded the grant or award.
+    country: The country where the grant or award was awarded.
+    value: The value of the grant or award.
+
+    Methods:
+    __str__: Returns the string representation of the grants and awards data.
+    __repr__: Returns the string representation of the grants and awards data.
     """
 
     def __init__(self):
-        self.years = []
-        self.position = str()
-        self.institution = str()
+        self.dates: Dates = Dates()
         self.description = str()
-        self.responsibilities = str()
-
-    def get_start_year(self):
-        """
-        Get the start year of this experience.
-        """
-        return yd.get_start_year(self.years)
-
-    def get_end_year(self):
-        """
-        Get the end year of this experience.
-        """
-        return yd.get_end_year(self.years)
-
-    def get_position(self):
-        """
-        Get the position of this experience.
-        """
-        return self.position
-
-    def get_institution(self):
-        """
-        Get the institution of this experience.
-        """
-        return self.institution
+        self.institution_id = str()
+        self.value = str()
 
     def get_description(self):
         """
-        Get the description of this experience.
+        Get the description of the grant or award.
         """
         return self.description
 
-    def get_responsibilities(self):
+    def get_institution_id(self):
         """
-        Get the responsibilities of this experience.
+        Get the institution id of the grant or award.
         """
-        return self.responsibilities
+        return self.institution_id
 
-    def process_year_data(self, filename):
+    def get_value(self):
         """
-        Process the year data.
+        Get the value of the grant or award.
         """
-        self.years = yd.process_year_data(filename, self.years)
+        return self.value
 
     def load(self, filename):
         """
-        Load the experience data.
+        Load the grants and awards data from the given file.
         """
-        self.process_year_data(filename)
-        self.position = filename["Position"]
-        self.institution = filename["Institution"]
+        self.dates.load(filename)
         self.description = filename["Description"]
-        self.responsibilities = filename["Responsibilities"]
-
-    def __str__(self) -> str:
-        string = f"Years: {list(map(str, self.years))}\n"
-        string += f"Position: {self.position}\n"
-        string += f"Institution: {self.institution}\n"
-        string += f"Description: {self.description}\n"
-        string += f"Responsibilities: {self.responsibilities}\n"
-        return string
+        self.institution_id = filename["Institution id"]
+        self.value = filename["Value"]
 
     def __repr__(self) -> str:
         string = (
-            f"ExperienceData("
-            f"years={[repr(year) for year in self.years]}, "
-            f"position={self.position}, "
-            f"institution={self.institution}, "
+            f"GrantsAwardsData("
+            f"dates={repr(self.dates)}, "
             f"description={self.description}, "
-            f"responsibilities={self.responsibilities})"
+            f"institution id={self.institution_id}, "
+            f"value={self.value})"
         )
         return string
 
 
-class Experience:
+class GrantsAwards:
     """
-    The Experience class is used to store the experience data.
+    A class to represent the grants and awards data.
 
     Attributes:
-    experience (list): The list of experience data.
+    grants_awards: The grants and awards data.
+
+    Methods:
+    get_oldest_date: Returns the oldest date in the grants and awards data.
+    load: Loads the grants and awards data from the given file.
+    __str__: Returns the string representation of the grants and awards data.
+    __repr__: Returns the string representation of the grants and awards data.
     """
 
     def __init__(self):
-        self.experiences = []
+        self.grants_awards = []
+
+    def get_oldest_date(self):
+        """
+        Returns the oldest date in the grants and awards data.
+        """
+        return self.grants_awards[-1].dates.get_start()
 
     def load(self, filename):
         """
-        Load the experience data.
+        Load the grants and awards data from the given file.
         """
-        experience_df = pd.read_excel(filename, sheet_name="Experience")
-        for _, row in experience_df.iterrows():
-            self.experiences.append(ExperienceData())
-            self.experiences[-1].load(row)
-        self.experiences = sorted(
-            self.experiences, key=lambda x: x.get_start_year(), reverse=True)
-
-    def __str__(self) -> str:
-        string = ""
-        for experience in self.experiences:
-            string += str(experience) + "\n"
-        return string
+        grants_rewards_df = pd.read_excel(
+            filename, sheet_name="Grants_awards")
+        for _, row in grants_rewards_df.iterrows():
+            self.grants_awards.append(GrantsAwardsData())
+            self.grants_awards[-1].load(row)
+        self.grants_awards = sorted(
+            self.grants_awards, key=lambda x: x.dates.get_start(), reverse=True)
 
     def __repr__(self) -> str:
-        string = f"Experience(experience={repr(self.experiences)})"
+        string = f"GrantsAwards(grants_awards={repr(list(self.grants_awards))})"
         return string
 
     def __iter__(self):
-        return iter(self.experiences)
+        return iter(self.grants_awards)
```

### Comparing `cvprocessor-0.6.4/src/cvprocessor/intro.py` & `cvprocessor-1.0.0/src/cvprocessor/intro.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.6.4/src/cvprocessor/memberships.py` & `cvprocessor-1.0.0/src/cvprocessor/memberships.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,52 +1,43 @@
 """
 This module contains the Memberships class and the MembershipData class.
 """
 import pandas as pd
 
+from cvprocessor.date.date import Dates
+
 
 class MembershipData:
     """
     The MembershipData class is used to store the membership data.
 
     Attributes:
-    year (pd.Timestamp): The year of the membership.
+    date (pd.Timestamp): The date of the membership.
     membership (str): The membership.
     """
 
     def __init__(self):
-        self.year: pd.Timestamp = pd.Timestamp("NaT")
+        self.dates: Dates = Dates()
         self.membership = str()
 
-    def get_year(self):
-        """
-        Get the year of the membership.
-        """
-        return self.year
-
     def get_membership(self):
         """
         Get the membership.
         """
         return self.membership
 
     def load(self, filename):
         """
         Load the membership data.
         """
-        self.year = filename["Year"]
+        self.dates.load(filename)
         self.membership = filename["Membership"]
 
-    def __str__(self):
-        string = f"Year: {self.year}\n"
-        string += f"Membership: {self.membership}\n"
-        return string
-
     def __repr__(self):
-        return f"MembershipData({repr(self.year)}, {repr(self.membership)})\n"
+        return f"MembershipData({repr(self.dates)}, {repr(self.membership)})\n"
 
 
 class Memberships:
     """
     The Memberships class is used to store the memberships data.
     """
 
@@ -60,18 +51,12 @@
         membership_df = pd.read_excel(
             filename, sheet_name="Professional_memberships")
         for _, row in membership_df.iterrows():
             membership = MembershipData()
             membership.load(row)
             self.memberships.append(membership)
 
-    def __str__(self):
-        string = ""
-        for membership in self.memberships:
-            string += str(membership) + "\n"
-        return string
-
     def __repr__(self):
         return f"Memberships(memberships={repr(list(map(repr, self.memberships)))})\n"
 
     def __iter__(self):
         return iter(self.memberships)
```

### Comparing `cvprocessor-0.6.4/src/cvprocessor/news.py` & `cvprocessor-1.0.0/src/cvprocessor/news.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,79 +1,12 @@
 """
 This module contains the classes to handle news data.
 """
 import pandas as pd
-
-
-class NewsResources:
-    """
-    The NewsResources class is used to store the resources for a news item.
-
-    Attributes:
-    pdf (str): The PDF link for the news item.
-    preprint (str): The preprint link for the news item.
-    code (str): The code link for the news item.
-    doi (str): The DOI link for the news item.
-    """
-
-    def __init__(self):
-        self.pdf = str()
-        self.preprint = str()
-        self.code = str()
-        self.doi = str()
-
-    def get_pdf(self):
-        """
-        Get the PDF link for the news item.
-        """
-        return self.pdf
-
-    def get_preprint(self):
-        """
-        Get the preprint link for the news item.
-        """
-        return self.preprint
-
-    def get_code(self):
-        """
-        Get the code link for the news item.
-        """
-        return self.code
-
-    def get_doi(self):
-        """
-        Get the DOI link for the news item.
-        """
-        return self.doi
-
-    def load(self, filename):
-        """
-        Load the resources for the news item.
-        """
-        self.pdf = filename["PDF"]
-        self.preprint = filename["Preprint"]
-        self.code = filename["Code"]
-        self.doi = filename["DOI"]
-
-    def __str__(self):
-        string = f"PDF: {self.pdf}\n"
-        string += f"Preprint: {self.preprint}\n"
-        string += f"Code: {self.code}\n"
-        string += f"DOI: {self.doi}\n"
-        return string
-
-    def __repr__(self):
-        string = (
-            f"NewsResources("
-            f"pdf={self.pdf}, "
-            f"preprint={self.preprint}, "
-            f"code={self.code}, "
-            f"doi={self.doi})"
-        )
-        return string
+from cvprocessor.links.links import Links
 
 
 class NewsData:
     """
     The NewsData class is used to store the data for a news item.
 
     Attributes:
@@ -83,15 +16,15 @@
     resources (NewsResources): The resources for the news item.
     """
 
     def __init__(self):
         self.title = str()
         self.date = str()
         self.description = str()
-        self.resources = NewsResources()
+        self.links = Links()
 
     def get_title(self):
         """
         Get the title of the news item.
         """
         return self.title
 
@@ -111,30 +44,23 @@
         """
         Load the news data from a Pandas DataFrame.
         """
         self.title = pd_dataframe["Title"]
         self.date = pd_dataframe["Date"]
         self.date = self.date.strftime("%b %d, %Y")
         self.description = pd_dataframe["Description"]
-        self.resources.load(pd_dataframe)
-
-    def __str__(self) -> str:
-        string = f"Title: {self.title}\n"
-        string += f"Date: {self.date}\n"
-        string += f"Description: {self.description}\n"
-        string += str(self.resources)
-        return string
+        self.links.load(pd_dataframe)
 
     def __repr__(self) -> str:
         string = (
             f"NewsData("
             f"title={self.title}, "
             f"date={self.date}, "
             f"description={self.description}, "
-            f"resources={repr(self.resources)})"
+            f"links={repr(self.links)})"
         )
         return string
 
 
 class News:
     """
     The News class is used to store the news data.
```

### Comparing `cvprocessor-0.6.4/src/cvprocessor/publications.py` & `cvprocessor-1.0.0/src/cvprocessor/publications.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 This module contains the classes and methods to process the publications data from the CV file.
 """
 import pandas as pd
 
-
-from cvprocessor import common
+from cvprocessor.links.links import Links
+from cvprocessor.date.date import Dates
 
 
 class Source:
     """
     A class to represent the source of a publication.
 
     Attributes:
@@ -17,15 +17,15 @@
     artno (str): The article number of the publication.
     """
 
     def __init__(self):
         self.volume = str()
         self.issue = str()
         self.artno = str()
-        self.source = str()
+        self.venue = str()
 
     def get_volume(self):
         """
         Get the volume of the publication.
         """
         return self.volume
 
@@ -37,36 +37,36 @@
 
     def get_artno(self):
         """
         Get the article number of the publication.
         """
         return self.artno
 
-    def get_source(self):
+    def get_venue(self):
         """
-        Get the source of the publication.
+        Get the venue of the publication.
         """
-        return self.source
+        return self.venue
 
     def load(self, filename):
         """
         Load the publication journal information from the file.
         """
         self.volume = filename["Volume"]
         self.issue = filename["Issue"]
         self.artno = filename["Art. No."]
-        self.source = filename["Source"]
+        self.venue = filename["Source"]
 
     def __repr__(self):
         string = (
             f"Source("
             f"volume={self.volume}, "
             f"issue={self.issue}, "
             f"artno={self.artno}, "
-            f"source={self.source})"
+            f"venue={self.venue})"
         )
         return string
 
 
 class Pages:
     """
     A class to represent the page information of a publication.
@@ -117,43 +117,37 @@
     """
     A class to represent the details of a publication.
 
     Attributes:
     basic_info (PublicationBasicInfo): The basic information of the publication.
     journal_info (Source): The journal information of the publication.
     page_info (Pages): The page information of the publication.
-    document_type (str): The document type of the publication.
+    type (str): The document type of the publication.
     """
 
     def __init__(self):
         self.title = str()
-        self.date = pd.Timestamp("NaT")
-        self.source = Source()
+        self.dates = Dates()
+        self.venue = Source()
         self.pages = Pages()
-        self.document_type = str()
+        self.type = str()
         self.abstract = str()
         self.keywords = str()
 
     def get_title(self):
         """
         Get the title of the publication.
         """
         return self.title
 
-    def get_date(self):
-        """
-        Get the date of the publication.
-        """
-        return self.date
-
-    def get_document_type(self):
+    def get_type(self):
         """
         Get the document type of the publication.
         """
-        return self.document_type
+        return self.type
 
     def get_abstract(self):
         """
         Get the abstract of the publication.
         """
         return self.abstract
 
@@ -164,107 +158,35 @@
         return self.keywords
 
     def load(self, filename):
         """
         Load the publication details from the file.
         """
         self.title = filename["Title"]
-        self.date = filename["Year"]
-        if len(self.date.split()) == 1:
-            self.date = "Jan "+self.date
-        # To datetime month year format
-        self.date = pd.to_datetime(self.date, format="%b %Y").date()
-        self.source.load(filename)
+        self.dates.load(filename)
+        self.venue.load(filename)
         self.pages.load(filename)
-        self.document_type = filename["Document Type"]
+        self.type = filename["Document Type"]
         self.abstract = filename["Abstract"]
         self.keywords = filename["Keywords"]
 
     def __repr__(self):
         string = (
             f"Details("
             f"title={self.title}, "
-            f"date={self.date}, "
-            f"source={repr(self.source)}, "
+            f"dates={repr(self.dates)}, "
+            f"source={repr(self.venue)}, "
             f"pages={repr(self.pages)}, "
-            f"document_type={self.document_type}, "
+            f"type={self.type}, "
             f"abstract={self.abstract}, "
             f"keywords={self.keywords})"
         )
         return string
 
 
-class Social:
-    """
-    A class to represent the resources of a publication.
-
-    Attributes:
-    code (str): The code of the publication.
-    slides (str): The slides of the publication.
-    doi (str): The DOI of the publication.
-    preprint_doi (str): The preprint DOI of the publication.
-    """
-
-    def __init__(self):
-        self.code = str()
-        self.slides = str()
-        self.doi = str()
-        self.preprint_doi = str()
-
-    def get_code(self):
-        """
-        Get the code of the publication.
-        """
-        return self.code
-
-    def get_slides(self):
-        """
-        Get the slides of the publication.
-        """
-        return self.slides
-
-    def get_doi(self):
-        """
-        Get the DOI of the publication.
-        """
-        return self.doi
-
-    def get_preprint_doi(self):
-        """
-        Get the preprint DOI of the publication.
-        """
-        return self.preprint_doi
-
-    def load(self, filename):
-        """
-        Load the publication resources from the file.
-        """
-        self.code = filename["Code"]
-        self.slides = filename["Slides"]
-        self.doi = filename["DOI"]
-        self.preprint_doi = filename["Preprint DOI"]
-
-    def __repr__(self):
-        string = (
-            f"Social("
-            f"code={self.code}, "
-            f"slides={self.slides}, "
-            f"doi={self.doi}, "
-            f"preprint_doi={self.preprint_doi})"
-        )
-        return string
-
-    def __str__(self):
-        string = f"Code: {self.code}\n"
-        string += f"Slides: {self.slides}\n"
-        string += f"DOI: {self.doi}\n"
-        string += f"Preprint DOI: {self.preprint_doi}\n"
-        return string
-
-
 class Rights:
     """
     A class to represent the rights of a publication.
 
     Attributes:
     license (str): The license of the publication.
     copyright (str): The copyright of the publication.
@@ -297,19 +219,14 @@
         string = (
             f"Rights("
             f"license={self.license}, "
             f"copyright={self.copyright})"
         )
         return string
 
-    def __str__(self):
-        string = f"License: {self.license}\n"
-        string += f"Copyright: {self.copyright}"
-        return string
-
 
 class AuthorIDAffiliationIDs:
     """
     A class to represent the author ID and affiliation IDs.
 
     Attributes:
     author_id (int): The author ID.
@@ -366,15 +283,15 @@
     load: Load the publication data from the file.
     build_apa_citation: Build the APA citation.
     """
 
     def __init__(self):
         self.auth_id_aff_id = []
         self.details = Details()
-        self.social = Social()
+        self.links = Links()
         self.rights = Rights()
 
     def get_auth_id_aff_id(self):
         """
         Get the author IDs and affiliation IDs.
         """
         return self.auth_id_aff_id
@@ -397,56 +314,51 @@
             authors.append(AuthorIDAffiliationIDs())
             authors[-1].author_id = int(author_id)
             if author_affiliation is not None:
                 for affiliation in author_affiliation:
                     authors[-1].add_affiliation_id(int(affiliation))
         self.auth_id_aff_id = authors
         self.details.load(filename)
-        self.social.load(filename)
+        self.links.load(filename)
         self.rights.load(filename)
 
     def get_apa_citation(self) -> str:
         """
         Build the APA citation.
         """
         citation = ""
-        if not common.check_nan(self.details.get_date()):
-            citation += f"({self.details.get_date().year}). "
-        if not common.check_nan(self.details.get_title()):
+        start_date = self.details.dates.get_start()
+        if pd.notna(start_date):
+            citation += f"({int(start_date.year)}). "
+        if pd.notna(self.details.get_title()):
             citation += f"{self.details.get_title()}. "
-        if not common.check_nan(self.details.source.get_source()):
-            citation += f"{self.details.source.get_source()}"
-        if not common.check_nan(self.details.source.get_volume()):
-            citation += f", {int(self.details.source.get_volume())}"
-        if not common.check_nan(self.details.source.get_issue()):
-            citation += f"({int(self.details.source.get_issue())})"
-        if not common.check_nan(self.details.source.get_artno()):
-            citation += f"{self.details.source.get_artno()}"
-        if not common.check_nan(self.details.pages.get_page_start()):
+        if pd.notna(self.details.venue.get_venue()):
+            citation += f"{self.details.venue.get_venue()}"
+        if pd.notna(self.details.venue.get_volume()):
+            citation += f", {int(self.details.venue.get_volume())}"
+        if pd.notna(self.details.venue.get_issue()):
+            citation += f"({int(self.details.venue.get_issue())})"
+        if pd.notna(self.details.venue.get_artno()):
+            citation += f"{self.details.venue.get_artno()}"
+        if pd.notna(self.details.pages.get_page_start()):
             citation += f", pp. {int(self.details.pages.get_page_start())}"
-        if not common.check_nan(self.details.pages.get_page_end()):
+        if pd.notna(self.details.pages.get_page_end()):
             citation += f"-{int(self.details.pages.get_page_end())}"
-        if not common.check_nan(self.social.get_doi()):
-            citation += f", doi: {self.social.get_doi()}"
+        doi = self.links.get_link("DOI")
+        if doi is not None:
+            citation += f", doi: {doi.get_url()}"
         citation += "."
         return citation
 
-    def __str__(self) -> str:
-        string = f"Authors' IDs and Affiliation IDs: {list(map(str, self.auth_id_aff_id))}\n"
-        string += str(self.details)
-        string += str(self.social)
-        string += str(self.rights)
-        return string
-
     def __repr__(self) -> str:
         string = (
             f"PublicationsData("
             f"authors={repr(self.auth_id_aff_id)}, "
             f"details={repr(self.details)}, "
-            f"social={repr(self.social)}, "
+            f"links={repr(self.links)}, "
             f"rights={repr(self.rights)})"
         )
         return string
 
 
 class Publications():
     """
@@ -454,19 +366,19 @@
 
     Attributes:
     publications (list): The list of publications.
 
     Methods:
     get_publications_count: Gets the number of publications.
     get_unique_sources: Gets the number of unique sources.
-    get_document_types: Gets the document types.
-    get_document_types_ordered: Gets the document types ordered.
-    get_num_publications_by_document_type: Gets the number of publications by document type.
+    get_types: Gets the document types.
+    get_types_ordered: Gets the document types ordered.
+    get_num_publications_by_type: Gets the number of publications by document type.
     get_num_publications_by_author: Gets the number of publications by author.
-    get_publications_year_range: Gets the year range of the publications.
+    get_publications_date_range: Gets the date range of the publications.
     """
 
     def __init__(self):
         self.publications = []
 
     def get_publications_count(self):
         """
@@ -482,95 +394,89 @@
 
     def get_unique_sources(self):
         """
         Gets the number of unique sources.
         """
         sources = set()
         for publication in self.publications:
-            sources.add(publication.details.source.get_source())
+            sources.add(publication.details.venue.get_venue())
         return len(sources)
 
-    def get_document_types(self):
+    def get_types(self):
         """
         Gets the document types.
         """
-        document_types = set()
+        types = set()
         for publication in self:
-            document_types.add(publication.details.document_type)
-        return document_types
+            types.add(publication.details.type)
+        return types
 
     def get_publication_by_title(self, title):
         """
         Get the publication by the title.
         """
         for publication in self:
             if publication.details.get_title() == title:
                 return publication
         return None
 
-    def get_document_types_ordered(self):
+    def get_types_ordered(self):
         """
         Gets the document types ordered.
         """
-        document_types = []
+        types = []
         for publication in self.publications:
-            if publication.details.document_type not in document_types:
-                document_types.append(publication.details.document_type)
-        return document_types
+            if publication.details.type not in types:
+                types.append(publication.details.type)
+        return types
 
-    def get_num_publications_by_document_type(self, document_type):
+    def get_num_publications_by_type(self, type):
         """
         Gets the number of publications by document type.
         """
         count = 0
         for publication in self.publications:
-            if publication.details.document_type == document_type:
+            if publication.details.type == type:
                 count += 1
         return count
 
     def get_num_publications_by_author(self, author_id):
         """
         Gets the number of publications by author.
         """
         count = 0
         for publication in self:
             for auth_id_aff_id in publication.get_auth_id_aff_id():
                 if auth_id_aff_id.get_author_id() == author_id:
                     count += 1
         return count
 
-    def get_publications_year_range(self):
+    def get_publications_date_range(self):
         """
-        Gets the year range of the publications.
+        Gets the date range of the publications.
         """
-        years = []
+        dates = []
         for publication in self.publications:
-            years.append(publication.details.get_date().year)
-        return min(years), max(years)
+            dates.append(publication.details.dates.get_start())
+        return min(dates), max(dates)
 
     def load(self, filename):
         """
         Load the publications data from the file.
         """
         publications_df = pd.read_excel(
             filename, sheet_name="Publications")
         for _, row in publications_df.iterrows():
             self.publications.append(PublicationsData())
             self.publications[-1].load(row)
         self.publications = sorted(
             self.publications, key=lambda x: (
-                x.details.get_date(), x.details.get_title()), reverse=True
+                x.details.dates.get_start(), x.details.get_title()), reverse=True
         )
 
-    def __str__(self):
-        string = ""
-        for publication in self.publications:
-            string += str(publication) + "\n\n"
-        return string
-
     def __repr__(self):
         string = (
             f"Publications("
             f"publications={list(map(repr, self.publications))}"
         )
         return string
```

### Comparing `cvprocessor-0.6.4/src/cvprocessor/research_interests.py` & `cvprocessor-1.0.0/src/cvprocessor/research_interests.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,19 +37,14 @@
         research_interests_pd = pd.read_excel(
             filename, sheet_name="Research_Interests")
         self.research_interests = research_interests_pd["Interests"].values[0]
         keywords = research_interests_pd["Keywords"]
         for keyword in keywords:
             self.keywords.append(keyword)
 
-    def __str__(self):
-        string = f"Research Interests: {self.research_interests}\n"
-        string += f"Keywords: {self.keywords}\n\n"
-        return string
-
     def __repr__(self):
         string = (
             f"ResearchInterests("
             f"research_interests={self.research_interests}, "
             f"keywords={self.keywords})"
         )
         return string
```

### Comparing `cvprocessor-0.6.4/src/cvprocessor/service.py` & `cvprocessor-1.0.0/src/cvprocessor/service.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,66 +1,48 @@
 """
 This module contains the ServiceData and Services classes.
 """
 import pandas as pd
 
+from cvprocessor.links.links import Link
+
 
 class ServiceData:
     """
     The ServiceData class is used to store the service data.
 
     Attributes:
     type (str): The type of the service.
     venue (str): The venue of the service.
-    link (str): The link to the service.
+    links (Link): The links of the service.
     """
 
     def __init__(self):
-        self.type = str()
         self.venue = str()
-        self.link = str()
-
-    def get_type(self) -> str:
-        """
-        Get the type of the service.
-        """
-        return self.type
+        self.link = Link()
 
     def get_venue(self) -> str:
         """
         Get the venue of the service.
         """
         return self.venue
 
-    def get_link(self) -> str:
-        """
-        Get the link to the service.
-        """
-        return self.link
-
-    def load(self, filename) -> None:
+    def load(self, df) -> None:
         """
         Load the service data.
         """
-        self.type = filename["Type"]
-        self.venue = filename["Venue"]
-        self.link = filename["Link"]
-
-    def __str__(self) -> str:
-        string = f"Type: {self.type}\n"
-        string += f"Venue: {self.venue}\n"
-        string += f"Link: {self.link}\n"
-        return string
+        self.venue = df["Venue"]
+        self.link.type = df["Type"]
+        self.link.url = df["Link"]
 
     def __repr__(self) -> str:
         string = (
             f"ServiceData("
-            f"type={self.type}, "
             f"venue={self.venue}, "
-            f"link={self.link})"
+            f"link={repr(self.link)})"
         )
         return string
 
 
 class Services:
     """
     The Services class is used to store the service data.
@@ -68,40 +50,36 @@
     Attributes:
     services (list): The list of services.
     """
 
     def __init__(self):
         self.services = []
 
-    def get_service_types_ordered(self):
+    def get_services_ordered(self):
         """
-        Get the service types in order.
+        Get the services ordered by link type.
         """
-        service_type = []
-        for service in self.services:
-            if service.type not in service_type:
-                service_type.append(service.type)
-        return service_type
+        services_ordered = []
+        for service in self:
+            if service.link.get_type() not in services_ordered:
+                services_ordered.append(service.link.get_type())
+        return services_ordered
 
     def load(self, filename):
         """
         Load the service data.
         """
         service_df = pd.read_excel(
             filename, sheet_name="Professional_services")
         for _, row in service_df.iterrows():
             service = ServiceData()
             service.load(row)
             self.services.append(service)
-
-    def __str__(self):
-        string = ""
-        for service in self.services:
-            string += str(service) + "\n"
-        return string
+        # Sort the services by venue alphabetically
+        self.services = sorted(self.services, key=lambda x: x.venue)
 
     def __repr__(self):
         string = f"Services(services={repr(list(self.services))})"
         return string
 
     def __iter__(self):
         return iter(self.services)
```

### Comparing `cvprocessor-0.6.4/src/cvprocessor/skills.py` & `cvprocessor-1.0.0/src/cvprocessor/skills.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,60 +6,54 @@
 
 class SkillData:
     """
     The SkillData class is used to store the skill data.
 
     Attributes:
     type (str): The type of the skill.
-    skill (str): The skill.
+    name (str): The name of the skill.
     level (str): The level of the skill.
     """
 
     def __init__(self):
         self.type = None
-        self.skill = None
+        self.name = None
         self.level = None
 
     def get_type(self):
         """
         Get the type of the skill.
         """
         return self.type
 
-    def get_skill(self):
+    def get_name(self):
         """
-        Get the skill.
+        Get the name of the skill.
         """
-        return self.skill
+        return self.name
 
     def get_level(self):
         """
         Get the level of the skill.
         """
         return self.level
 
     def load(self, filename):
         """
         Load the skill data.
         """
         self.type = filename["Type"]
-        self.skill = filename["Skill"]
+        self.name = filename["Skill"]
         self.level = filename["Level"]
 
-    def __str__(self) -> str:
-        string = f"Type: {self.type}\n"
-        string += f"Skill: {self.skill}\n"
-        string += f"Level: {self.level}\n"
-        return string
-
     def __repr__(self) -> str:
         string = (
             f"SkillData("
             f"type={self.type}, "
-            f"skill={self.skill}, "
+            f"name={self.name}, "
             f"level={self.level})"
         )
         return string
 
 
 class Skills:
     """
@@ -75,37 +69,37 @@
     get_skill_type(): Get the skills by the given type.
     load(): Load the skills data.
     """
 
     def __init__(self):
         self.skills = []
 
-    def get_skill_types_ordered(self):
+    def get_types_ordered(self):
         """
         Get the skill types in order.
         """
         skill_type = []
         for skill in self.skills:
             if skill.type not in skill_type:
                 skill_type.append(skill.type)
         return skill_type
 
-    def get_num_skills_except_type(self, skill_type):
+    def get_num_except_type(self, skill_type):
         """
         Get the number of skills except for the given type.
         """
         return len([skill for skill in self.skills if skill.type != skill_type])
 
-    def get_num_skills_by_type(self, skill_type):
+    def get_num_by_type(self, skill_type):
         """
         Get the number of skills by the given type.
         """
-        return len(self.get_skill_type(skill_type))
+        return len(self.get_type(skill_type))
 
-    def get_skill_type(self, skill_type: str):
+    def get_type(self, skill_type: str):
         """
         Get the skills by the given type.
         """
         return [skill for skill in self.skills if skill.type == skill_type]
 
     def load(self, filename):
         """
@@ -113,19 +107,13 @@
         """
         skills_pd = pd.read_excel(filename, sheet_name="Skills")
         for _, row in skills_pd.iterrows():
             skill_data = SkillData()
             skill_data.load(row)
             self.skills.append(skill_data)
 
-    def __str__(self):
-        string = ""
-        for skill in self.skills:
-            string += str(skill) + "\n"
-        return string
-
     def __repr__(self):
         string = f"Skills(skills={repr(list(self.skills))})"
         return string
 
     def __iter__(self):
         return iter(self.skills)
```

### Comparing `cvprocessor-0.6.4/src/cvprocessor.egg-info/PKG-INFO` & `cvprocessor-1.0.0/src/cvprocessor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.6.4
+Version: 1.0.0
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.6.4/src/cvprocessor.egg-info/SOURCES.txt` & `cvprocessor-1.0.0/src/cvprocessor.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 src/cvprocessor/__init__.py
 src/cvprocessor/authors.py
-src/cvprocessor/common.py
 src/cvprocessor/cv.py
 src/cvprocessor/education.py
 src/cvprocessor/experience.py
 src/cvprocessor/grants_awards.py
 src/cvprocessor/institutes.py
 src/cvprocessor/intro.py
 src/cvprocessor/memberships.py
@@ -16,13 +15,24 @@
 src/cvprocessor/references.py
 src/cvprocessor/research_interests.py
 src/cvprocessor/service.py
 src/cvprocessor/skills.py
 src/cvprocessor/software.py
 src/cvprocessor/supervision.py
 src/cvprocessor/teaching.py
-src/cvprocessor/year_data.py
 src/cvprocessor.egg-info/PKG-INFO
 src/cvprocessor.egg-info/SOURCES.txt
 src/cvprocessor.egg-info/dependency_links.txt
 src/cvprocessor.egg-info/requires.txt
-src/cvprocessor.egg-info/top_level.txt
+src/cvprocessor.egg-info/top_level.txt
+src/cvprocessor/Personal/Personal.py
+src/cvprocessor/Personal/__init__.py
+src/cvprocessor/contact/__init__.py
+src/cvprocessor/contact/contact.py
+src/cvprocessor/date/__init__.py
+src/cvprocessor/date/date.py
+src/cvprocessor/links/__init__.py
+src/cvprocessor/links/links.py
+src/cvprocessor/name/__init__.py
+src/cvprocessor/name/name.py
+src/cvprocessor/security/__init__.py
+src/cvprocessor/security/security.py
```

