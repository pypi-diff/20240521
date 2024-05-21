# Comparing `tmp/ip2asn-1.3.1.tar.gz` & `tmp/ip2asn-1.4.tar.gz`

## Comparing `ip2asn-1.3.1.tar` & `ip2asn-1.4.tar`

### file list

```diff
@@ -1,9 +1,13 @@
--rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 ip2asn-1.3.1/ip2asn/__init__.py
--rw-r--r--   0        0        0     6309 2020-02-02 00:00:00.000000 ip2asn-1.3.1/ip2asn/main.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 ip2asn-1.3.1/ip2asn/test.py
--rw-r--r--   0        0        0     8645 2020-02-02 00:00:00.000000 ip2asn-1.3.1/ip2asn/tests/test_ip2asn.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 ip2asn-1.3.1/.gitignore
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 ip2asn-1.3.1/LICENSE.txt
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 ip2asn-1.3.1/README.md
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 ip2asn-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 ip2asn-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    10349 2020-02-02 00:00:00.000000 ip2asn-1.4/ip2asn/__init__.py
+-rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 ip2asn-1.4/ip2asn/main.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ip2asn-1.4/ip2asn/main.py.~1~
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 ip2asn-1.4/ip2asn/main.py.~2~
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 ip2asn-1.4/ip2asn/tests/test_big_numbers_converter.py
+-rw-r--r--   0        0        0     8645 2020-02-02 00:00:00.000000 ip2asn-1.4/ip2asn/tests/test_ip2asn.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 ip2asn-1.4/ip2asn/tests/test_ip2asn.py.~1~
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 ip2asn-1.4/.gitignore
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 ip2asn-1.4/LICENSE.txt
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 ip2asn-1.4/LICENSE.~1~
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 ip2asn-1.4/README.md
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 ip2asn-1.4/pyproject.toml
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 ip2asn-1.4/PKG-INFO
```

### Comparing `ip2asn-1.3.1/ip2asn/main.py` & `ip2asn-1.4/ip2asn/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import logging
 from logging import info, error
 from pathlib import Path
 
 COLUMN_NAMES = ['address', 'ip_numeric', 'ASN', 'owner', 'country', 'ip_range']
 ASN_COLUMN_NAMES = ['ASN', 'owner', 'country', 'ip_range']
 
+
 def parse_args():
     """Handles argument parsing for the ip2asn script."""
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter,
                                      description="Describes one or more IP addresses from an ip2asn database",
                                      epilog="""Example Usage: ip2asn -f ip2asn-v4-43.tsv 1.1.1.1""")
 
     parser.add_argument("-f", "--ip2asn-database", type=str,
@@ -39,14 +40,18 @@
 
     parser.add_argument("-I", "--input-fsdb", type=argparse.FileType("r"),
                         help="Read an input FSDB and add columns to it; implies -F as well")
     
     parser.add_argument("-k", "--key", default="key", type=str,
                         help="The input key of the FSDB input file that contains the ip address to analyze")
 
+    parser.add_argument("-C", "--cache-database", action="store_true",
+                        help="After loading the ip2asn file, cache it in a msgpack file for faster loading next time.")
+
+
     parser.add_argument(
         "--log-level",
         "--ll",
         default="info",
         help="Define the logging verbosity level (debug, info, warning, error, fotal, critical).",
     )
     
@@ -59,25 +64,27 @@
         args.search_by_asn = True
         
     log_level = args.log_level.upper()
     logging.basicConfig(level=log_level, format="%(levelname)-10s:\t%(message)s")
         
     return args
 
+
 def print_result(to, address, result):
     """Displays the results to the output terminal/stdout"""
     if 'ip_numeric' in result:
         to.write("Address: {}\n".format(address))
         to.write("  Numeric ip: {}\n".format(result['ip_numeric']))
     to.write("         ASN: {}\n".format(result['ASN']))
     to.write("       Owner: {}\n".format(result['owner']))
     to.write("     Country: {}\n".format(result['country']))
     to.write("    ip_range: {}\n".format(result['ip_range']))
     to.write("\n")
 
+
 def output_fsdb_row(outf, address, result):
     if 'ip_numeric' in result:
         outf.append([address, 
                      result['ip_numeric'],
                      result['ASN'],
                      result['owner'],
                      result['country'],
@@ -115,31 +122,32 @@
                             result['ASN'],
                             result['owner'],
                             result['country'],
                             result['ip_range']])
             else:
                 row.extend(['-', '-', '-', '-', '-'])
         outf.append(row)
-        
-                
+
+
 def main():
     "The meat of the ip2asn script"
     args = parse_args()
 
     if Path(args.ip2asn_database).exists():
         database = args.ip2asn_database
     elif Path("ip2asn-combined.tsv").exists():
         info("using ./ip2asn-combined.tsv")
         database = "ip2asn-combined.tsv"
     else:
         error("Cannot find the ip2asn-combined.tsv or other similar database file")
         error("Please specify a location with -f or download from ip2asn.com")
         sys.exit(1)
 
-    i2a = ip2asn.IP2ASN(database, ipversion=None)
+    i2a = ip2asn.IP2ASN(database, ipversion=None,
+                        cache_contents=args.cache_database)
 
     if args.input_fsdb:
         process_fsdb(i2a, args.input_fsdb, args.output_file,
                      args.key, by_asn=args.search_by_asn)
         exit()
 
     if args.output_fsdb:
```

### Comparing `ip2asn-1.3.1/ip2asn/tests/test_ip2asn.py` & `ip2asn-1.4/ip2asn/tests/test_ip2asn.py`

 * *Files identical despite different names*

### Comparing `ip2asn-1.3.1/LICENSE.txt` & `ip2asn-1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ip2asn-1.3.1/README.md` & `ip2asn-1.4/README.md`

 * *Files identical despite different names*

### Comparing `ip2asn-1.3.1/pyproject.toml` & `ip2asn-1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ip2asn-1.3.1/PKG-INFO` & `ip2asn-1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: ip2asn
-Version: 1.3.1
+Version: 1.4
 Summary: A tool for doing differential analysis of pcap files
 Project-URL: Homepage, https://github.com/hardaker/ip2asn
 Author-email: Wes Hardaker <opensource@hardakers.net>
 License-Expression: MIT
 License-File: LICENSE.txt
+License-File: LICENSE.~1~
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: pyfsdb
 Description-Content-Type: text/markdown
 
 # Objective
```

