# Comparing `tmp/waymore-4.3.tar.gz` & `tmp/waymore-4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waymore-4.3.tar", last modified: Wed May  8 23:17:25 2024, max compression
+gzip compressed data, was "waymore-4.4.tar", last modified: Tue May 21 20:27:41 2024, max compression
```

## Comparing `waymore-4.3.tar` & `waymore-4.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-05-08 23:17:25.817201 waymore-4.3/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)     1068 2024-05-08 20:42:52.000000 waymore-4.3/LICENSE
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    47245 2024-05-08 23:17:25.805375 waymore-4.3/PKG-INFO
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    46794 2024-05-08 21:49:16.000000 waymore-4.3/README.md
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       38 2024-05-08 23:17:25.820218 waymore-4.3/setup.cfg
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)     2142 2024-05-08 20:42:52.000000 waymore-4.3/setup.py
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-05-08 23:17:25.446064 waymore-4.3/waymore/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       17 2024-05-08 21:49:24.000000 waymore-4.3/waymore/__init__.py
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)   168145 2024-05-08 23:08:08.000000 waymore-4.3/waymore/waymore.py
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-05-08 23:17:25.779233 waymore-4.3/waymore.egg-info/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    47245 2024-05-08 23:17:25.000000 waymore-4.3/waymore.egg-info/PKG-INFO
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)      253 2024-05-08 23:17:25.000000 waymore-4.3/waymore.egg-info/SOURCES.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-05-08 23:17:25.000000 waymore-4.3/waymore.egg-info/dependency_links.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       49 2024-05-08 23:17:25.000000 waymore-4.3/waymore.egg-info/entry_points.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       63 2024-05-08 23:17:25.000000 waymore-4.3/waymore.egg-info/requires.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)        8 2024-05-08 23:17:25.000000 waymore-4.3/waymore.egg-info/top_level.txt
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-05-21 20:27:41.586592 waymore-4.4/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)     1068 2024-05-16 21:56:52.000000 waymore-4.4/LICENSE
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    47221 2024-05-21 20:27:41.571040 waymore-4.4/PKG-INFO
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    46794 2024-05-16 22:04:24.000000 waymore-4.4/README.md
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       38 2024-05-21 20:27:41.588115 waymore-4.4/setup.cfg
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)     2131 2024-05-16 22:04:34.000000 waymore-4.4/setup.py
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-05-21 20:27:41.267712 waymore-4.4/waymore/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       17 2024-05-16 22:05:08.000000 waymore-4.4/waymore/__init__.py
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)   169799 2024-05-16 23:58:20.000000 waymore-4.4/waymore/waymore.py
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-05-21 20:27:41.544288 waymore-4.4/waymore.egg-info/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    47221 2024-05-21 20:27:40.000000 waymore-4.4/waymore.egg-info/PKG-INFO
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)      253 2024-05-21 20:27:41.000000 waymore-4.4/waymore.egg-info/SOURCES.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-05-21 20:27:40.000000 waymore-4.4/waymore.egg-info/dependency_links.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       49 2024-05-21 20:27:40.000000 waymore-4.4/waymore.egg-info/entry_points.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       54 2024-05-21 20:27:40.000000 waymore-4.4/waymore.egg-info/requires.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)        8 2024-05-21 20:27:40.000000 waymore-4.4/waymore.egg-info/top_level.txt
```

### Comparing `waymore-4.3/LICENSE` & `waymore-4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `waymore-4.3/PKG-INFO` & `waymore-4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: waymore
-Version: 4.3
+Version: 4.4
 Summary: Find way more from the Wayback Machine, Common Crawl, Alien Vault OTX, URLScan & VirusTotal!
 Home-page: https://github.com/xnl-h4ck3r/waymore
 Author: @xnl-h4ck3r
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: argparse
 Requires-Dist: requests
 Requires-Dist: pyyaml
 Requires-Dist: termcolor
 Requires-Dist: psutil
 Requires-Dist: urlparse3
 Requires-Dist: tldextract
 
 <center><img src="https://github.com/xnl-h4ck3r/waymore/blob/main/waymore/images/title.png"></center>
 
-## About - v4.3
+## About - v4.4
 
 The idea behind **waymore** is to find even more links from the Wayback Machine than other existing tools.
 
 👉 The biggest difference between **waymore** and other tools is that it can also **download the archived responses** for URLs on wayback machine so that you can then search these for even more links, developer comments, extra parameters, etc. etc.
 👉 Also, other tools do not currenrtly deal with the rate limiting now in place by the sources, and will often just stop with incomplete results and not let you know they are incomplete.
 
 Anyone who does bug bounty will have likely used the amazing [waybackurls](https://github.com/tomnomnom/waybackurls) by @TomNomNoms. This tool gets URLs from [web.archive.org](https://web.archive.org) and additional links (if any) from one of the index collections on [index.commoncrawl.org](http://index.commoncrawl.org/).
```

### Comparing `waymore-4.3/README.md` & `waymore-4.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <center><img src="https://github.com/xnl-h4ck3r/waymore/blob/main/waymore/images/title.png"></center>
 
-## About - v4.3
+## About - v4.4
 
 The idea behind **waymore** is to find even more links from the Wayback Machine than other existing tools.
 
 👉 The biggest difference between **waymore** and other tools is that it can also **download the archived responses** for URLs on wayback machine so that you can then search these for even more links, developer comments, extra parameters, etc. etc.
 👉 Also, other tools do not currenrtly deal with the rate limiting now in place by the sources, and will often just stop with incomplete results and not let you know they are incomplete.
 
 Anyone who does bug bounty will have likely used the amazing [waybackurls](https://github.com/tomnomnom/waybackurls) by @TomNomNoms. This tool gets URLs from [web.archive.org](https://web.archive.org) and additional links (if any) from one of the index collections on [index.commoncrawl.org](http://index.commoncrawl.org/).
```

### Comparing `waymore-4.3/setup.py` & `waymore-4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     version=__import__('waymore').__version__,
     description="Find way more from the Wayback Machine, Common Crawl, Alien Vault OTX, URLScan & VirusTotal!",
     long_description=open("README.md").read(),
     long_description_content_type='text/markdown',
     author="@xnl-h4ck3r",
     url="https://github.com/xnl-h4ck3r/waymore",
     py_modules=["waymore"],
-    install_requires=["argparse","requests","pyyaml","termcolor","psutil","urlparse3","tldextract"],
+    install_requires=["requests","pyyaml","termcolor","psutil","urlparse3","tldextract"],
     entry_points={
         'console_scripts': [
             'waymore = waymore.waymore:main',
         ],
     },
 )
```

### Comparing `waymore-4.3/waymore/waymore.py` & `waymore-4.4/waymore/waymore.py`

 * *Files 1% similar despite different names*

```diff
@@ -702,31 +702,63 @@
         url = url[0:newline]
     else:
         newline = url.find('%0a')
         if newline > 0:
             url = url[0:newline]
     return url
 
+# Add a link to the linksFound collection for archived responses (included timestamp preifx)
+def linksFoundResponseAdd(link):
+    global linksFound, argsInput, argsInputHostname
+     
+    try:
+        if inputIsDomainANDPath:
+            checkInput = argsInput
+        else:
+            checkInput = argsInputHostname
+        
+        # Remove the timestamp
+        linkWithoutTimestamp = link.split('/', 1)[-1]
+        
+        # If the link specifies port 80 or 443, e.g. http://example.com:80, then remove the port
+        parsed = urlparse(linkWithoutTimestamp.strip())
+        if parsed.port in (80, 443):
+            new_netloc = parsed.hostname
+            parsed_url = parsed._replace(netloc=new_netloc).geturl()
+        else:
+            parsed_url = linkWithoutTimestamp
+
+        # Don't write it if the link does not contain the requested domain (this can sometimes happen)
+        if parsed_url.find(checkInput) >= 0:
+            linksFound.add(link)
+    except Exception as e:
+        linksFound.add(link)
+        
 # Add a link to the linksFound collection
 def linksFoundAdd(link):
     global linksFound, argsInput, argsInputHostname
-    # If the link specifies port 80 or 443, e.g. http://example.com:80, then remove the port 
+    
     try:
         if inputIsDomainANDPath:
             checkInput = argsInput
         else:
             checkInput = argsInputHostname
+        
+        # If the link specifies port 80 or 443, e.g. http://example.com:80, then remove the port
+        parsed = urlparse(link.strip())
+        if parsed.port in (80, 443):
+            new_netloc = parsed.hostname
+            parsed_url = parsed._replace(netloc=new_netloc).geturl()
+        else:
+            parsed_url = link
+        
         # Don't write it if the link does not contain the requested domain (this can sometimes happen)
-        if link.find(checkInput) >= 0:
-            parsed = urlparse(link.strip())
-            if parsed.netloc.find(':80') >= 0 or parsed.netloc.fnd(':443') >= 0:
-                newNetloc = parsed.netloc.split(':')[0]
-                parsed = parsed._replace(netloc=newNetloc).geturl()
-            linksFound.add(parsed)
-    except:
+        if parsed_url.find(checkInput) >= 0:
+            linksFound.add(link)
+    except Exception as e:
         linksFound.add(link)
     
 def processArchiveUrl(url):
     """
     Get the passed web archive response
     """
     global stopProgram, successCount, failureCount, fileCount, DEFAULT_OUTPUT_DIR, totalResponses, indexFile, argsInput, continueRespFile, REGEX_404
@@ -2343,15 +2375,15 @@
             if args.xwm and args.xcc and args.xav and args.xus:
                 write(getSPACER(colored('Links found on virustotal.com: ', 'cyan')+colored(str(linkCount),'white'))+'\n')
             else:
                 write(getSPACER(colored('Extra links found on virustotal.com: ', 'cyan')+colored(str(linkCount),'white'))+'\n')
         
     except Exception as e:
         writerr(colored('ERROR getVirusTotalUrls 1: ' + str(e), 'red'))
-        
+
 def processResponses():
     """
     Get archived responses from Wayback Machine (archive.org)
     """
     global linksFound, subs, path, indexFile, totalResponses, stopProgram, argsInput, continueRespFile, successCount, fileCount, DEFAULT_OUTPUT_DIR, responseOutputDirectory
     try:
         if not args.check_only:
@@ -2509,21 +2541,22 @@
                                 writerr(colored(getSPACER('Failed to get links from Wayback Machine (archive.org) - Blocked Site Error (they block the target site)'), 'red'))
                             else:
                                 writerr(colored(getSPACER('Failed to get links from Wayback Machine (archive.org) - check input domain and try again.'), 'red'))
                         return
                 except:
                     pass
             
-            # Go through the response to save the links found        
+            # Go through the response to save the links found    
             for line in resp.iter_lines():
                 try:
                     results = line.decode("utf-8") 
-                    timestamp = results.split(' ')[0]
-                    originalUrl = results.split(' ')[1]
-                    linksFoundAdd(timestamp+'/'+originalUrl)
+                    parts = results.split(' ', 2)
+                    timestamp = parts[0]
+                    originalUrl = parts[1]
+                    linksFoundResponseAdd(timestamp+'/'+originalUrl)
                 except Exception as e:
                     writerr(colored(getSPACER('ERROR processResponses 3: Cannot to get link from line: '+str(line)), 'red'))
             
             # Remove any links that have URL exclusions
             linkRequests = []
             exclusionRegex = re.compile(r'('+re.escape(FILTER_URL).replace(',','|')+')',flags=re.IGNORECASE)
             for link in linksFound:
@@ -2536,14 +2569,24 @@
             # Write the links to a temp file
             if not args.check_only:
                 with open(responsesPath,'wb') as f:
                     pickle.dump(linkRequests, f)
                 
         # Get the total number of responses we will try to get and set the current file count to the success count
         totalResponses = len(linkRequests)
+        
+        # If there are no reponses to download, diaplay an error and exit
+        if totalResponses == 0:
+            try:
+                if originalUrl:
+                    writerr(colored(getSPACER('Failed to get links from Wayback Machine (archive.org) - there were results (e.g. "'+originalUrl+'") but they didn\'t match the input you gave. Check input and try again.'), 'red'))
+            except:
+                writerr(colored(getSPACER('Failed to get links from Wayback Machine (archive.org) - check input and try again.'), 'red'))
+            return
+        
         fileCount = successCount
         
         if args.check_only:
             if args.limit == 5000 and totalResponses+1 == 5000:
                 writerr(colored('Downloading archived responses: ','cyan')+colored(str(totalResponses+1)+' requests (the --limit argument defaults to '+str(DEFAULT_LIMIT)+')','cyan'))
             else:
                 writerr(colored('Downloading archived responses: ','cyan')+colored(str(totalResponses+1)+' requests','white'))
```

### Comparing `waymore-4.3/waymore.egg-info/PKG-INFO` & `waymore-4.4/waymore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: waymore
-Version: 4.3
+Version: 4.4
 Summary: Find way more from the Wayback Machine, Common Crawl, Alien Vault OTX, URLScan & VirusTotal!
 Home-page: https://github.com/xnl-h4ck3r/waymore
 Author: @xnl-h4ck3r
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: argparse
 Requires-Dist: requests
 Requires-Dist: pyyaml
 Requires-Dist: termcolor
 Requires-Dist: psutil
 Requires-Dist: urlparse3
 Requires-Dist: tldextract
 
 <center><img src="https://github.com/xnl-h4ck3r/waymore/blob/main/waymore/images/title.png"></center>
 
-## About - v4.3
+## About - v4.4
 
 The idea behind **waymore** is to find even more links from the Wayback Machine than other existing tools.
 
 👉 The biggest difference between **waymore** and other tools is that it can also **download the archived responses** for URLs on wayback machine so that you can then search these for even more links, developer comments, extra parameters, etc. etc.
 👉 Also, other tools do not currenrtly deal with the rate limiting now in place by the sources, and will often just stop with incomplete results and not let you know they are incomplete.
 
 Anyone who does bug bounty will have likely used the amazing [waybackurls](https://github.com/tomnomnom/waybackurls) by @TomNomNoms. This tool gets URLs from [web.archive.org](https://web.archive.org) and additional links (if any) from one of the index collections on [index.commoncrawl.org](http://index.commoncrawl.org/).
```

