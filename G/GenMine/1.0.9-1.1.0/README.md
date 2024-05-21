# Comparing `tmp/GenMine-1.0.9.tar.gz` & `tmp/genmine-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GenMine-1.0.9.tar", last modified: Tue Apr 11 01:37:57 2023, max compression
+gzip compressed data, was "genmine-1.1.0.tar", last modified: Tue May 21 11:51:43 2024, max compression
```

## Comparing `GenMine-1.0.9.tar` & `genmine-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 01:37:57.790885 GenMine-1.0.9/
-drwxrwxrwx   0        0        0        0 2023-04-11 01:37:57.764882 GenMine-1.0.9/GenMine/
--rw-rw-rw-   0        0        0    43616 2023-04-11 01:28:45.000000 GenMine-1.0.9/GenMine/GenMine.py
--rw-rw-rw-   0        0        0        0 2022-10-27 01:45:14.000000 GenMine-1.0.9/GenMine/__init__.py
--rw-rw-rw-   0        0        0     1726 2022-11-01 23:36:51.000000 GenMine-1.0.9/GenMine/command.py
--rw-rw-rw-   0        0        0     5293 2022-11-04 00:39:34.000000 GenMine-1.0.9/GenMine/main.py
-drwxrwxrwx   0        0        0        0 2023-04-11 01:37:57.786883 GenMine-1.0.9/GenMine.egg-info/
--rw-rw-rw-   0        0        0      277 2023-04-11 01:37:57.000000 GenMine-1.0.9/GenMine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-04-11 01:37:57.000000 GenMine-1.0.9/GenMine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 01:37:57.000000 GenMine-1.0.9/GenMine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-11 01:37:57.000000 GenMine-1.0.9/GenMine.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-10-25 05:12:45.000000 GenMine-1.0.9/GenMine.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       68 2023-04-11 01:37:57.000000 GenMine-1.0.9/GenMine.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-11 01:37:57.000000 GenMine-1.0.9/GenMine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2022-02-07 04:16:54.000000 GenMine-1.0.9/LICENSE
--rw-rw-rw-   0        0        0      277 2023-04-11 01:37:57.788885 GenMine-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     3278 2023-02-01 06:40:14.000000 GenMine-1.0.9/README.md
--rw-rw-rw-   0        0        0       42 2023-04-11 01:37:57.790885 GenMine-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      741 2023-04-11 01:35:31.000000 GenMine-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 11:51:43.827531 genmine-1.1.0/
+drwxrwxrwx   0        0        0        0 2024-05-21 11:51:43.825530 genmine-1.1.0/GenMine.egg-info/
+-rw-rw-rw-   0        0        0      473 2024-05-21 11:51:43.000000 genmine-1.1.0/GenMine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2024-05-21 11:51:43.000000 genmine-1.1.0/GenMine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 11:51:43.000000 genmine-1.1.0/GenMine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-21 11:51:43.000000 genmine-1.1.0/GenMine.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-21 11:14:13.000000 genmine-1.1.0/GenMine.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       68 2024-05-21 11:51:43.000000 genmine-1.1.0/GenMine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-21 11:51:43.000000 genmine-1.1.0/GenMine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2022-02-07 04:16:54.000000 genmine-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      473 2024-05-21 11:51:43.826531 genmine-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3278 2024-05-21 10:14:31.000000 genmine-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 11:51:43.817435 genmine-1.1.0/genmine/
+-rw-rw-rw-   0        0        0        0 2024-05-15 23:54:07.000000 genmine-1.1.0/genmine/__init__.py
+-rw-rw-rw-   0        0        0     5832 2024-05-21 11:43:04.000000 genmine-1.1.0/genmine/main.py
+drwxrwxrwx   0        0        0        0 2024-05-21 11:51:43.823530 genmine-1.1.0/genmine/src/
+-rw-rw-rw-   0        0        0        0 2024-05-21 08:56:09.000000 genmine-1.1.0/genmine/src/__init__.py
+-rw-rw-rw-   0        0        0     1726 2024-05-21 08:50:16.000000 genmine-1.1.0/genmine/src/command.py
+-rw-rw-rw-   0        0        0    44280 2024-05-21 11:46:41.000000 genmine-1.1.0/genmine/src/genmine_module.py
+-rw-rw-rw-   0        0        0     1820 2024-05-21 11:30:10.000000 genmine-1.1.0/genmine/src/logger.py
+-rw-rw-rw-   0        0        0       42 2024-05-21 11:51:43.827531 genmine-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      707 2024-05-21 11:51:19.000000 genmine-1.1.0/setup.py
```

### Comparing `GenMine-1.0.9/GenMine/GenMine.py` & `genmine-1.1.0/genmine/src/genmine_module.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from Bio import Entrez
 from Bio import SeqIO
-from Bio import pairwise2
-from Bio.pairwise2 import format_alignment
 
-from Bio.Blast.Applications import NcbiblastnCommandline
-from Bio.Blast import NCBIXML
+# from Bio import pairwise2
+# from Bio.pairwise2 import format_alignment
+
+# from Bio.Blast.Applications import NcbiblastnCommandline
+# from Bio.Blast import NCBIXML
 from Bio.Seq import Seq
 import time
 from time import sleep
 import pickle
 import json
 import re
 from datetime import datetime
@@ -16,16 +17,17 @@
 import xmltodict
 import os, sys, subprocess
 import random
 import re
 import pickle
 import pandas as pd
 import shutil
+import logging
 
-log_file = open("log.txt", "w")
+# log_file = open("log.txt", "w")
 
 
 # Logging Functions
 def Time_now():
     now = datetime.now()
     Date_time = "%s-%s-%s %s:%s:%s " % (
         now.year,
@@ -35,19 +37,21 @@
         now.minute,
         now.second,
     )
     return Date_time
 
 
 # To both print to stdout and logfile
+"""
 def Mes(text):
     text = str(text)
     text = Time_now() + text
     log_file.write(text + "\n")
     print(text + "\n")
+"""
 
 
 def listtostring(list_in):
     if type(list_in) == type(["list"]):
         return ", ".join(list_in)
     else:
         return list_in
@@ -79,46 +83,46 @@
     cnt_all = len(list_acc)  # total number of records
 
     start_time = time.time()
 
     record_list = []
 
     if cnt_all == 0:
-        Mes("No accessions available in GenBank. Please check your input")
+        logging.error("No accessions available in GenBank. Please check your input")
         return -1
 
     # Iterating with 50 items
     for i in range(int((len(list_acc) - 1) / cut) + 1):
         # Try to parse saved files
         if str(i) in [file for file in os.listdir(f"{path_tmp}")]:
-            Mes("Found saved")
+            logging.info("Found saved")
             cnt += cut
             with open(f"{path_tmp}/{i}", "rb") as fp:
                 data = pickle.load(fp)
                 for record in data:
                     record_list.append(record)
 
         # for last last chunk
         elif i * cut + cut > len(list_acc):
             acc_string = ",".join(list_acc[i * cut :])
             sleep(0.3)
             cnt += len(list_acc[i * cut :])
-            Mes(
+            logging.info(
                 f"{cnt}/{cnt_all} {round(100*cnt/cnt_all,2)}% {round(time.time()-start_time,2)}s"
             )
 
             # Parse xml
             # First trial
             try:
                 handle = Entrez.efetch(
                     db="nucleotide", id=acc_string, rettype="gb", retmode="xml"
                 )
 
             except:
-                Mes("Requesting again...")
+                logging.warning("Server not responding, Requesting again...")
 
                 # Second trial
                 try:
                     sleep(10)
                     handle = Entrez.efetch(
                         db="nucleotide", id=acc_string, rettype="gb", retmode="xml"
                     )
@@ -128,15 +132,15 @@
                     try:
                         sleep(100)
                         handle = Entrez.efetch(
                             db="nucleotide", id=acc_string, rettype="gb", retmode="xml"
                         )
                     # Final trial
                     except:
-                        Mes(
+                        logging.warning(
                             "Last requesting due to connection error, will be take long (15 min)..."
                         )
                         sleep(900)
                         handle = Entrez.efetch(
                             db="nucleotide", id=acc_string, rettype="gb", retmode="xml"
                         )
 
@@ -154,49 +158,49 @@
                 tmp_record_list.append(record)
 
             # Intermediate save for current data
             try:
                 with open(f"{path_tmp}/{i}", "wb") as f:
                     pickle.dump(tmp_record_list, f)
             except:
-                Mes("Saving Error")
+                logging.error("[DEVELOPMENTAL ERROR] Data saving failed")
                 raise Exception
 
         # non last chunk
         else:
             acc_string = ",".join(list_acc[i * cut : i * cut + cut])
             sleep(0.3)
             cnt += cut
-            Mes(
+            logging.info(
                 f"{cnt}/{cnt_all} {round(100*cnt/cnt_all,2)}% {round(time.time()-start_time,2)}s"
             )
 
             # First trial
             try:
                 handle = Entrez.efetch(
                     db="nucleotide", id=acc_string, rettype="gb", retmode="xml"
                 )
             except:
                 # Second trial
-                Mes("Requesting again...")
+                logging.warning("Server not responding, Requesting again...")
                 try:
                     sleep(10)
                     handle = Entrez.efetch(
                         db="nucleotide", id=acc_string, rettype="gb", retmode="xml"
                     )
                 except:
                     # Third trial
                     try:
                         sleep(100)
                         handle = Entrez.efetch(
                             db="nucleotide", id=acc_string, rettype="gb", retmode="xml"
                         )
                     # Last trial
                     except:
-                        Mes(
+                        logging.warning(
                             "Last requesting due to connection error, will be take long (15 min)..."
                         )
                         sleep(900)
                         handle = Entrez.efetch(
                             db="nucleotide", id=acc_string, rettype="gb", retmode="xml"
                         )
 
@@ -213,15 +217,15 @@
                 record_list.append(record)
                 tmp_record_list.append(record)
 
             try:
                 with open(f"{path_tmp}/{i}", "wb") as f:
                     pickle.dump(tmp_record_list, f)
             except:
-                Mes("Saving Error")
+                logging.error("[DEVELOPMENTAL ERROR] Data saving failed")
                 raise Exception
 
     with open(out, "w") as fp:
         json_term = json.dump(record_list, fp, indent=4)
 
     # If success, remove tmp files
     tmp_file_list = [file for file in os.listdir(f"{path_tmp}")]
@@ -243,15 +247,15 @@
     handle = Entrez.esearch(
         db="Nucleotide", term=term, retmax=record["Count"], idtype="acc"
     )
     record = Entrez.read(handle)
 
     list_acc = record["IdList"]
 
-    Mes(f"Number of IDs: {len(list_acc)}")
+    logging.info(f"Number of IDs: {len(list_acc)}")
 
     return list_acc
 
 
 # To manage shotgun contig accessions
 def entrez_query_generator(acc_list):
     acc_tmp_list = []
@@ -265,16 +269,16 @@
         # For shotgun sequences
         elif re.fullmatch(
             r"(([A-Z]{4}[0-9]{8})(\.[0-9]{1}){0,1})|(([A-Z]{6}[0-9]{9,})(\.[0-9]{1}){0,1})",
             acc.strip(),
         ):
             acc_tmp_list.append(acc.strip().split(".")[0])
         else:
-            Mes(
-                f"[Error] Developmental error, bad accession {acc} entered entrez_query_generator please ask to developer"
+            logging.error(
+                f"[DEVELOPMENTAL ERROR] Bad accession {acc} entered entrez_query_generator. Please report your failed input to wan101010@snu.ac.kr"
             )
             raise Exception
 
     acc_string = " ".join(acc_tmp_list)
 
     return acc_string
 
@@ -297,43 +301,43 @@
         # For shotgun sequences
         elif re.fullmatch(
             r"(([A-Z]{4}[0-9]{8})(\.[0-9]{1}){0,1})|(([A-Z]{6}[0-9]{9,})(\.[0-9]{1}){0,1})",
             acc.strip(),
         ):
             return_acc_list.append(acc.strip().split(".")[0])
         else:
-            Mes(
-                f"[Warning] Accession {acc} does not seems to be valid accession. Passing"
+            logging.warning(
+                f"Accession {acc} does not seems to be valid accession. Passing"
             )
 
     # Check if acc are valid by asking to GenBank
     # to get number of result
     # get accession_list term
     Entrez.email = email
-    print(entrez_query_generator(return_acc_list))
+    # print(entrez_query_generator(return_acc_list))
     if len(return_acc_list) > 0:
         handle = Entrez.esearch(
             db="Nucleotide",
             term=entrez_query_generator(return_acc_list),
             retmax=2 * len(return_acc_list),
             idtype="acc",
         )
         record = Entrez.read(handle)
-        print(record["IdList"])
+        # print(record["IdList"])
         valid_acc_list = [acc.split(".")[0] for acc in record["IdList"]]
 
         for acc in return_acc_list:
             if not (acc in valid_acc_list):
-                Mes(
+                logging.warning(
                     f"GenBank accession {acc} cannot be found in GenBank. Please check misspelling or if the accessions are not opened yet."
                 )
     else:
         valid_acc_list = []
 
-    print(valid_acc_list)
+    # print(valid_acc_list)
 
     return valid_acc_list
 
 
 # GenBank record parser
 # get wanted object from iterating dictionary
 # if wanted object is in value of label
@@ -416,15 +420,15 @@
             if (
                 int(record["GBSeq_length"]) < max_len
             ):  # in order to get rid of genome data
                 for key in record.keys():
                     if not (key in dict_all):
                         dict_all[key] = []
         except:
-            print_json(json_data)
+            # print_json(json_data)
             raise Exception
 
     for record in json_data:
         if int(record["GBSeq_length"]) < max_len:  # in order to get rid of genome data
             for key in dict_all.keys():
                 try:
                     dict_all[key].append(str(record[key]))
@@ -565,30 +569,30 @@
                                 state = 2
                                 # print(title)
                                 if "Direct Submission" in title:
                                     title.remove("Direct Submission")
                                 title.append(reference["GBReference_title"])
 
                             else:  # unexpected input
-                                print(record["GBSeq_references"]["GBReference"])
-                                print(reference["GBReference_title"])
+                                logging.error(record["GBSeq_references"]["GBReference"])
+                                logging.error(reference["GBReference_title"])
                                 raise Exception
                         else:
                             if reference["GBReference_journal"] == "Unpublished":
                                 state = 1  # only unpublished file exists
                                 title.append("Direct Submission")
                             else:
                                 # only journal record exists and no title exists
                                 state = 2
                                 title.append("Unknown")
-                                print(record)
+                                # print(record)
                                 # raise Exception
 
                     except:
-                        print(record)
+                        logging.error(record)
                         raise Exception
         else:
             title = []
 
         return title
 
     # Get voucher from given record json
@@ -724,16 +728,16 @@
                             author_list.append(
                                 record["GBSeq_references"]["GBReference"][
                                     "GBReference_consortium"
                                 ]
                             )
 
                     else:
-                        print(record["GBSeq_references"]["GBReference"])
-                        print("Failed to find authors")
+                        # print(record["GBSeq_references"]["GBReference"])
+                        logging.warning("Failed to find authors")
                         return (
                             []
                         )  # in some of the records, no author exists. See NG_071242
                         # raise Exception
 
                 elif isinstance(record["GBSeq_references"]["GBReference"], list):
                     # print("Multiple GBReference")
@@ -770,26 +774,26 @@
                                             author_list.append(
                                                 reference["GBReference_authors"][
                                                     "GBAuthor"
                                                 ]
                                             )
 
                 else:
-                    print(record)
+                    logging.error(record)
                     raise Exception
             else:
                 if "GBReferene_authors" in record.keys():
-                    print(record)
+                    logging.error(record)
                     raise Exception
                 else:
-                    print(record)
+                    logging.error(record)
                     raise Exception
 
         else:
-            print("No author information")
+            logging.warning("No author information")
 
         author_list = list(set(author_list))
 
         return author_list
 
     with open(json_in) as json_file:
         json_data = json.load(json_file)
@@ -843,15 +847,17 @@
 
             if "GBSeq_sequence" in record:  # normal sequence data
                 dict_temp["seq"] = record["GBSeq_sequence"]
             elif "GBSeq_feature-table" in record:  # genomic data
                 dict_temp["seq"] = "Genomic"
 
         else:
-            Mes("Could not found GBSeq-sequence or GBSeq_feature-table from record")
+            logging.error(
+                "[DEVELOPMETAL ERROR] Could not found GBSeq-sequence or GBSeq_feature-table from record. Please send your input to wan101010@snu.ac.kr"
+            )
             print_json(record)
             raise Exception
 
     with open(out, "w") as fp:
         json_term = json.dump(json_temp, fp, indent=4)
 
 
@@ -884,15 +890,16 @@
                     outfasta.write(record["GBSeq_definition"])
                     outfasta.write("\n")
                     outfasta.write(record["GBSeq_sequence"])
                     outfasta.write("\n")
                 temp_list.append(record)
 
         else:
-            print(record)
+            pass
+            # print(record)
 
     outjson = out + ".json"
 
     with open(outjson, "w") as fp:
         json_term = json.dump(temp_list, fp, indent=4)
 
 
@@ -921,15 +928,16 @@
                         for term in additional_terms
                     ):
                         # print(record[key])
                         list_temp.append("1")
                     else:
                         list_temp.append("0")
             else:
-                print(record)
+                pass
+                # print(record)
         if "1" in list_temp:
             if "GBSeq_definition" in record and "GBSeq_sequence" in record:
                 outfasta.write(">")
                 outfasta.write(record["GBSeq_definition"])
                 outfasta.write("\n")
                 outfasta.write(record["GBSeq_sequence"])
                 outfasta.write("\n")
@@ -974,15 +982,15 @@
     return dict_record
 
 
 def date_remover(string):
     try:
         return string.split(")")[1]
     except:
-        print(string)
+        # print(string)
         raise exception
 
 
 def date_renamer(string):
     dict_mon = {
         "JAN": "01",
         "FEB": "02",
@@ -1019,15 +1027,15 @@
         print("ITS")
     elif any(x in description for x in ["beta-tubulin", "beta tubulin", "beta-tublin"]):
         return "TUB"
         print("TUB")
     elif "calmodulin" in description:
         return "CMD"
         print("CMD")
-    elif "RPB2" in description.upper():
+    elif any(x in description.upper() for x in ["RPB2", "RNA POLYMERASE II", "RBP2"]):
         return "RPB2"
         print("RPB2")
     elif "actin" in description.lower() or "ACT" in description:
         return "ACT"
         print("ACT")
     elif "cox1" in description:
         return "cox1"
@@ -1076,22 +1084,22 @@
     elif "PJ3" in description:
         return "PJ3"
         print("PJ3")
     elif "mitochond" in description:
         return "mt_others"
         print("mt_others")
     else:
-        print(description)
+        # print(description)
         return "others"
 
 
 def BLAST_downloader(fasta_in, blast_out):
     records = SeqIO.parse(fasta_in, "fasta")
     for i, record in enumerate(list(records)):
-        print(i)
+        # print(i)
         query = SeqIO.write(record, "temp.fasta", "fasta")
         os.system(
             f"blastn -out {blast_out}_{i}.xml -outfmt 5 -query temp.fasta -db /data/cwseo/BLAST_DB/public/nt -evalue 0.1 -num_threads 2"
         )
         # blastn_cline = ncbiblastnCommandline(query="temp.fasta",db="nr",evalue=0.1,outfmt=7,out=f"{blast_out}_{i}.xml")
         # print(blastn_cline)
         # blastn_cline()
@@ -1102,15 +1110,15 @@
     os.system(cmd)
 
 
 def BLASTn(query, db, evalue, out):
     blastn_cline = ncbiblastnCommandline(
         query=query, db=db, evalue=evalue, outfmt=7, out=out
     )
-    Mes("BLAST: " + str(blastn_cline))
+    logging.info("BLAST: " + str(blastn_cline))
     blastn_cline()
 
 
 def classifier(json_in, out):
     with open(json_in) as json_file:
         json_data = json.load(json_file)
 
@@ -1155,20 +1163,22 @@
 def json_pick(json_file, acc_list, out):
     file = open(json_file, encoding="UTF-8")
     json_list = json.loads(file.read())
 
     list_json = []
 
     for read in json_list:
-        print(read["acc"])
+        # print(read["acc"])
         if read["acc"] in acc_list:
             list_json.append(read)
 
     if len(list_json) == 0:
-        Mes(f"All accessions in {json_file} has already found in genbank search")
+        logging.warning(
+            f"All accessions in {json_file} has already found in genbank search"
+        )
         return False
 
     else:
         with open(out, "w") as fp:
             json.dump(list_json, fp, indent=4)
 
         return True
@@ -1215,15 +1225,15 @@
         f"{path_work}/{name_out}_transformed.json",
         f"{path_work}/{name_out}_transformed.xlsx",
     )
 
     # Parse finalized data
     term_acc = get_acc(f"{path_work}/{name_out}_transformed.json")
 
-    Mes(f"Total {len(term_acc)} found")
+    logging.info(f"Total {len(term_acc)} found")
     classified_genes = classifier(
         f"{path_work}/{name_out}_transformed.json",
         f"{path_work}/{name_out}",
     )
 
 
 # GenBank, download all by given term
@@ -1245,15 +1255,15 @@
     # Get all GenBank records
     handle = Entrez.esearch(db="Nucleotide", term=genus_term, retmax=record["Count"])
     record = Entrez.read(handle)
 
     # Parse number of records
     list_acc = record["IdList"]
 
-    Mes(f"Number of IDs: {len(list_acc)}")
+    logging.info(f"Number of IDs: {len(list_acc)}")
 
     # Download GenBank records
     status = downloader(
         list_acc=list_acc, path_tmp=path_tmp, out=f"{path_work}/{name_out}.json"
     )
 
     if not (status == -1):
@@ -1266,15 +1276,15 @@
         )
 
 
 # Download by given list of accession
 def ncbi_downloadbyacclist(email, list_acc, name_out, path_work, path_tmp, max_len):
     Entrez.email = email
 
-    Mes(f"Number of IDs: {len(list_acc)}")
+    logging.info(f"Number of IDs: {len(list_acc)}")
     # Download GenBank records
     status = downloader(
         list_acc=list_acc, path_tmp=path_tmp, out=f"{path_work}/{name_out}.json"
     )
 
     if not (status == -1):
         # save files
```

### Comparing `GenMine-1.0.9/GenMine/command.py` & `genmine-1.1.0/genmine/src/command.py`

 * *Files identical despite different names*

### Comparing `GenMine-1.0.9/LICENSE` & `genmine-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `GenMine-1.0.9/README.md` & `genmine-1.1.0/README.md`

 * *Files identical despite different names*

