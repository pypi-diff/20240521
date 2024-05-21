# Comparing `tmp/novowrap-1.20-py3-none-any.whl.zip` & `tmp/novowrap-1.32-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 52392 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat        0 b- defN 20-Jul-28 07:30 novowrap/__init__.py
+Zip file size: 53071 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat      910 b- defN 21-Mar-31 10:23 novowrap/__init__.py
 -rw-rw-rw-  2.0 fat      910 b- defN 21-Mar-31 10:23 novowrap/__main__.py
 -rw-rw-rw-  2.0 fat    25394 b- defN 21-Aug-10 04:13 novowrap/assembly.py
 -rw-rw-rw-  2.0 fat    17236 b- defN 20-Oct-29 02:31 novowrap/merge.py
 -rw-rw-rw-  2.0 fat    24474 b- defN 21-Aug-10 04:26 novowrap/ui.py
--rw-rw-rw-  2.0 fat    31829 b- defN 21-Aug-10 04:15 novowrap/utils.py
+-rw-rw-rw-  2.0 fat    31802 b- defN 24-Apr-16 08:53 novowrap/utils.py
 -rw-rw-rw-  2.0 fat    25631 b- defN 21-Aug-10 02:31 novowrap/validate.py
--rw-rw-rw-  2.0 fat    35184 b- defN 21-Aug-10 04:49 novowrap-1.20.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    17001 b- defN 21-Aug-10 04:49 novowrap-1.20.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 21-Aug-10 04:49 novowrap-1.20.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 21-Aug-10 04:49 novowrap-1.20.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      915 b- defN 21-Aug-10 04:49 novowrap-1.20.dist-info/RECORD
-12 files, 178675 bytes uncompressed, 50884 bytes compressed:  71.5%
+-rw-rw-rw-  2.0 fat    35184 b- defN 24-May-21 16:12 novowrap-1.32.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    17428 b- defN 24-May-21 16:12 novowrap-1.32.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-21 16:12 novowrap-1.32.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       43 b- defN 24-May-21 16:12 novowrap-1.32.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 24-May-21 16:12 novowrap-1.32.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1012 b- defN 24-May-21 16:12 novowrap-1.32.dist-info/RECORD
+13 files, 180125 bytes uncompressed, 51407 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -15,23 +15,26 @@
 
 Filename: novowrap/utils.py
 Comment: 
 
 Filename: novowrap/validate.py
 Comment: 
 
-Filename: novowrap-1.20.dist-info/LICENSE
+Filename: novowrap-1.32.dist-info/LICENSE
 Comment: 
 
-Filename: novowrap-1.20.dist-info/METADATA
+Filename: novowrap-1.32.dist-info/METADATA
 Comment: 
 
-Filename: novowrap-1.20.dist-info/WHEEL
+Filename: novowrap-1.32.dist-info/WHEEL
 Comment: 
 
-Filename: novowrap-1.20.dist-info/top_level.txt
+Filename: novowrap-1.32.dist-info/entry_points.txt
 Comment: 
 
-Filename: novowrap-1.20.dist-info/RECORD
+Filename: novowrap-1.32.dist-info/top_level.txt
+Comment: 
+
+Filename: novowrap-1.32.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## novowrap/__init__.py

```diff
@@ -0,0 +1,57 @@
+00000000: 2321 2f75 7372 2f62 696e 2f70 7974 686f  #!/usr/bin/pytho
+00000010: 6e33 0d0a 0d0a 6672 6f6d 2073 7973 2069  n3....from sys i
+00000020: 6d70 6f72 7420 6172 6776 0d0a 6672 6f6d  mport argv..from
+00000030: 206e 6f76 6f77 7261 702e 6173 7365 6d62   novowrap.assemb
+00000040: 6c79 2069 6d70 6f72 7420 6173 7365 6d62  ly import assemb
+00000050: 6c79 5f6d 6169 6e0d 0a66 726f 6d20 6e6f  ly_main..from no
+00000060: 766f 7772 6170 2e75 7469 6c73 2069 6d70  vowrap.utils imp
+00000070: 6f72 7420 6765 745f 616c 6c5f 7468 6972  ort get_all_thir
+00000080: 645f 7061 7274 790d 0a69 6d70 6f72 7420  d_party..import 
+00000090: 6c6f 6767 696e 670d 0a0d 0a0d 0a23 2064  logging......# d
+000000a0: 6566 696e 6520 6c6f 6767 6572 0d0a 464d  efine logger..FM
+000000b0: 5420 3d20 2725 2861 7363 7469 6d65 2973  T = '%(asctime)s
+000000c0: 2025 286c 6576 656c 6e61 6d65 292d 3873   %(levelname)-8s
+000000d0: 2025 286d 6573 7361 6765 2973 270d 0a44   %(message)s'..D
+000000e0: 4154 4546 4d54 203d 2027 2548 3a25 4d3a  ATEFMT = '%H:%M:
+000000f0: 2553 270d 0a6c 6f67 6769 6e67 2e62 6173  %S'..logging.bas
+00000100: 6963 436f 6e66 6967 2866 6f72 6d61 743d  icConfig(format=
+00000110: 464d 542c 2064 6174 6566 6d74 3d44 4154  FMT, datefmt=DAT
+00000120: 4546 4d54 2c20 6c65 7665 6c3d 6c6f 6767  EFMT, level=logg
+00000130: 696e 672e 494e 464f 290d 0a6c 6f67 203d  ing.INFO)..log =
+00000140: 206c 6f67 6769 6e67 2e67 6574 4c6f 6767   logging.getLogg
+00000150: 6572 2827 6e6f 766f 7772 6170 2729 0d0a  er('novowrap')..
+00000160: 7472 793a 0d0a 2020 2020 696d 706f 7274  try:..    import
+00000170: 2063 6f6c 6f72 6564 6c6f 6773 0d0a 2020   coloredlogs..  
+00000180: 2020 636f 6c6f 7265 646c 6f67 732e 696e    coloredlogs.in
+00000190: 7374 616c 6c28 6c65 7665 6c3d 6c6f 6767  stall(level=logg
+000001a0: 696e 672e 494e 464f 2c20 666d 743d 464d  ing.INFO, fmt=FM
+000001b0: 542c 2064 6174 6566 6d74 3d44 4154 4546  T, datefmt=DATEF
+000001c0: 4d54 290d 0a65 7863 6570 7420 496d 706f  MT)..except Impo
+000001d0: 7274 4572 726f 723a 0d0a 2020 2020 7061  rtError:..    pa
+000001e0: 7373 0d0a 6c6f 6720 3d20 6c6f 6767 696e  ss..log = loggin
+000001f0: 672e 6765 744c 6f67 6765 7228 276e 6f76  g.getLogger('nov
+00000200: 6f77 7261 7027 290d 0a0d 0a0d 0a64 6566  owrap')......def
+00000210: 206d 6169 6e28 293a 0d0a 2020 2020 6966   main():..    if
+00000220: 2061 7267 765b 2d31 5d20 3d3d 2027 696e   argv[-1] == 'in
+00000230: 6974 273a 0d0a 2020 2020 2020 2020 6765  it':..        ge
+00000240: 745f 616c 6c5f 7468 6972 645f 7061 7274  t_all_third_part
+00000250: 7928 290d 0a20 2020 2020 2020 2072 6574  y()..        ret
+00000260: 7572 6e0d 0a20 2020 2065 6c69 6620 6172  urn..    elif ar
+00000270: 6776 5b2d 315d 203d 3d20 272d 6827 3a0d  gv[-1] == '-h':.
+00000280: 0a20 2020 2020 2020 2061 7373 656d 626c  .        assembl
+00000290: 795f 6d61 696e 2829 0d0a 2020 2020 2020  y_main()..      
+000002a0: 2020 7265 7475 726e 0d0a 2020 2020 656c    return..    el
+000002b0: 6966 206c 656e 2861 7267 7629 203e 2031  if len(argv) > 1
+000002c0: 3a0d 0a20 2020 2020 2020 2061 7373 656d  :..        assem
+000002d0: 626c 795f 6d61 696e 2829 0d0a 2020 2020  bly_main()..    
+000002e0: 2020 2020 7265 7475 726e 0d0a 2020 2020      return..    
+000002f0: 7472 793a 0d0a 2020 2020 2020 2020 6672  try:..        fr
+00000300: 6f6d 206e 6f76 6f77 7261 702e 7569 2069  om novowrap.ui i
+00000310: 6d70 6f72 7420 7569 5f6d 6169 6e0d 0a20  mport ui_main.. 
+00000320: 2020 2020 2020 2075 695f 6d61 696e 2829         ui_main()
+00000330: 0d0a 2020 2020 6578 6365 7074 2045 7863  ..    except Exc
+00000340: 6570 7469 6f6e 3a0d 0a20 2020 2020 2020  eption:..       
+00000350: 2061 7373 656d 626c 795f 6d61 696e 2829   assembly_main()
+00000360: 0d0a 0d0a 0d0a 6966 205f 5f6e 616d 655f  ......if __name_
+00000370: 5f20 3d3d 2027 5f5f 6d61 696e 5f5f 273a  _ == '__main__':
+00000380: 0d0a 2020 2020 6d61 696e 2829 0d0a       ..    main()..
```

## novowrap/utils.py

```diff
@@ -558,16 +558,15 @@
                               'small single copy (SSC)',
                               'inverted repeat B (IRb)'),
                              (region_LSC, region_IRa, region_SSC, region_IRb)):
             length = f.stop - f.start
             features.append(SeqFeature(
                 FeatureLocation(offset+1, length+offset+1),
                 type='misc_feature',
-                qualifiers={'note': f_name, 'software': 'rotate_seq'},
-                strand=1))
+                qualifiers={'note': f_name, 'software': 'rotate_seq'}))
             offset += length
         new_seq.features.extend(features)
         # print feature
         log.info(f'\tRegions of rotated record:')
         for f in features:
             log.info(f'\t{f.qualifiers["note"][-4:-1]}: {f.location.start} to '
                      f'{f.location.end} ({len(f)} bp)')
```

## Comparing `novowrap-1.20.dist-info/LICENSE` & `novowrap-1.32.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `novowrap-1.20.dist-info/METADATA` & `novowrap-1.32.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,454 +1,450 @@
-Metadata-Version: 2.1
-Name: novowrap
-Version: 1.20
-Summary: Assembly Plastid Genome
-Home-page: https://github.com/wpwupingwp/novowrap
-Author: Ping Wu
-Author-email: wpwupingwp@outlook.com
-License: GNU AGPL v3
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Requires-Dist: wheel (>=0.32.3)
-Requires-Dist: biopython (>=1.77)
-Requires-Dist: coloredlogs (>=10.0)
-Requires-Dist: matplotlib (>=3.2.0)
-Requires-Dist: numpy (>=1.19.1)
-Requires-Dist: pip (>=18.0)
-Requires-Dist: graphviz (>=0.13)
-
-[![Build Status](https://travis-ci.org/wpwupingwp/novowrap.svg?branch=master)](https://travis-ci.org/wpwupingwp/novowrap)
-[![PyPI version](https://badge.fury.io/py/novowrap.svg)](https://badge.fury.io/py/novowrap)
-[![Anaconda version](https://anaconda.org/wpwupingwp/novowrap/badges/version.svg)](https://anaconda.org/wpwupingwp/novowrap)
-# Quick start
-Download [the package](https://github.com/wpwupingwp/novowrap/releases),
-unzip, and then double-click `novowrap.exe` or `novowrap`.
-
-__OR__
-
-Make sure you have [Python](https://www.python.org/) (3.7 or higher) or 
-[conda](https://docs.conda.io/en/latest/miniconda.html) installed.
-
-Open terminal, run
-   ```shell
-   # Install, using pip (recommended)
-   pip install novowrap --user
-   # Or, use conda
-   conda install -c wpwupingwp novowrap
-
-   # Initiliaze with Internet
-   # Windows
-   python -m novowrap init
-   # Linux and MacOS
-   python3 -m novowrap init
-
-   # Run
-   # Windows
-   python -m novowrap
-   # Linux and MacOS
-   python3 -m novowrap
-   ```
-
-# Table of Contents
-   * [Quick start](#quickstart)
-   * [Feature](#feature)
-   * [Prerequisite](#prerequisite)
-      * [Hardware](#hardware)
-      * [Software](#software)
-   * [Installation](#installation)
-      * [Portable](#portable)
-      * [Install with pip](#Installwithpip)
-      * [Install with conda](#Installwithconda)
-      * [Initialization](#Initialization)
-   * [Usage](#usage)
-      * [Command line](#commandline)
-      * [Graphical user interface](#graphicaluserintetface)
-   * [Input](#input)
-   * [Output](#output)
-   * [Options](#options)
-      * [Assembly](#assembly)
-      * [Validate](#validate)
-      * [Merge](#merge)
-   * [Performance](#performance)
-# Feature
-:heavy_check_mark: Assembly chloroplast genomes from given NGS data, with minimal
-parameters to set. Also, it supports batch mode.  
-
-Automatic generate uniform structure with reference (typically, start from 
-_trnH-psbA_, and, SSC/LSC region have the same direction with reference).
-
-:heavy_check_mark: Merge contigs according to overlapping region. May handle
-Invert-Repeat fragments.
-
-:heavy_check_mark: Validate assembly results by comparing the synteny and sequence
-homology with given reference (or taxonomy name).
-# Prerequisite
-## Hardware
-The assembly function will call NOVOPlasty, which requires 2 GB memory for 1
-GB uncompressed data.
-
-The other functions could run in normal computers and have no extra
-requirements for memory, CPU, et al.
-
-The software requires Internet for the first run to install the missing
-dependencies. Then, it could work if offline, but better with the internet.
-## Software
-For the portable version, nothing needs to be installed manually.
-
-For installing from pip, [Python](https://www.python.org/downloads/) is
-required. Notice that the python version should be **3.7** or higher.
-
-:white_check_mark: All third-party dependencies will be automatically
-installed with the Internet, including `biopython`, `matplotlib`, `coloredlogs`,
-`graphviz` (python packages), and
-[perl(for Windows only)](http://strawberryperl.com/download/5.30.1.1/strawberry-perl-5.30.1.1-64bit-portable.zip), 
-[NOVOPlasty](https://github.com/ndierckx/NOVOPlasty),
-[BLAST](https://blast.ncbi.nlm.nih.gov/Blast.cgi?CMD=Web&PAGE_TYPE=BlastDocs&DOC_TYPE=Download).
-
-# Installation
-## Portable
-Download from the [link](https://github.com/wpwupingwp/novowrap/releases),
-unpack and run with Internet for the first time.
-## Install with pip
-1. Install [Python](https://www.python.org/downloads/). *3.7 or newer* is
-   required.
-
-2. Open the command line, run
-```shell
-pip install novowrap --user
-```
-## Install with conda
-After installed [conda](https://docs.conda.io/en/latest/miniconda.html), run
-```
-conda install -c wpwupingwp novowrap
-```
-## Initialization
-During the first running, `novowrap` will check and initialize the running environment. 
-Missing dependencies will be automatically installed.
-This step requires the Internet connection.
-```shell
-# Windows
-python -m novowrap init
-# Linux and MacOS
-python3 -m novowrap init
-```
-# Usage
-## Command line
-:exclamation: In Linux and macOS, Python2 is `python2` and Python3 is `python3`.  However,
-in Windows, Python3 is called `python`, too. Please notice the difference.
-
- * Show help information of each module
- ```shell
- # Windows
- python -m novowrap.assembly -h
- python -m novowrap.validate -h
- python -m novowrap.merge -h
- # Linux and MacOS
- python3 -m novowrap.assembly -h
- python3 -m novowrap.validate -h
- python3 -m novowrap.merge -h
- ```
- * Assembly and validate
- ```shell
- # Windows, single sample
- python -m novowrap -input [input1] [input2] -taxon [taxonomy]
- # Windows, batch mode for numerous samples
- python -m novowrap -list [list file]
- # Linux and MacOS, single sample
- python3 -m novowrap -input [input1] [input2] -taxon [taxonomy]
- # Linux and MacOS, batch mode for numerous samples
- python3 -m novowrap -list [list file]
- ```
- * Only validate
- ```shell
- # Windows
- python -m novowrap.validate -input [input file] -taxon [taxonomy]
- # Linux and MacOS
- python3 -m novowrap.validate -input [input file] -taxon [taxonomy]
- ```
- * Only merge
- ```shell
- # Windows
- python -m novowrap.merge -input [input file]
- # Linux and MacOS
- python3 -m novowrap.merge -input [input file]
- ```
-## Graphical user interface
- If installed with pip,
-```shell
-# Windows
-python -m novowrap
-# Linux and MacOS
-python3 -m novowrap
-```
-
-If use the portable version, just double-click the `novowrap.exe` or `novowrap` in
-the folder.
-
-Then click the button to choose which module to use. Notice that if one of the
-option was set to the wrong value, the program will refuse to run and hint the
-user to correct the invalid option.
-# Input
-The `assembly` module accepts `gz` or `fastq` format as input. If use `input
-list`, the list file should be `csv` format. If use `reference` file instead
-of automatically get from NCBI, the file format should be `genbank`.
-
-The `merge` module accepts `fasta` format as input.
-
-The `validate` module accepts `fasta` format as input. If use `reference` file
-instead of automatically get from NCBI, the file format should be `genbank`
-**or** `fasta` as long as it is a complete chloroplast genome.
-
-# Output
-`.gb` files: **genbank** format sequence, with annotation of the boundary of
-LSC/SSC/IR regions.
-
-`.rotate` files: rotated sequence as **fasta** format; start from `trnH-psbA`, same direction with
-reference
-
-`.pdf` files: figure of validation of assembly
-
-`_RC_` files: if filenames contain `_RC_`, it means one of the regions of the
-sequence was adjusted according to the reference. The unadjusted sequence
-could be found in `Temp` folder.
-
-# Options
-## Assembly
-### General
-These options are for general usage.
-
-`-h` or `-help`: print help message
-
-`-input [filenames]`: input filenames, could be single or pair-end, support gz
-and fastq format
-
-`-list [filenames]`: input list for batch mode. The list should be a csv file
-with three columns,
-```csv
-Input 1,Input 2,Taxonomy
-```
-If only has one input file, just leave the `Input 2` column empty.
-
-Please use *full path* of file names, for instance, `d:\data\sample-1\forward.fastq`
-instead of `forward.fastq` or `sample-1\forward.fastq`.
-
-`-ref [filename]`: reference file for assembly and validation, should be
-`genbank` format contains *only one* chloroplast genome sequence. Extra
-sequences will be *ignored*. For automatic running, `-taxon` is recommended
-
-`-taxon [taxonomy name]`: taxonomy name of the sample, space is allowed.  For
-instance, `-taxon Oryza sativa`, will find reference chloroplast genome of
-`_Oryza sativa_` from NCBI RefSeq database. If not found, will find most related
-species' reference, `Oryza`, `Poaceae`, `Poales` et al.
-
-If `-ref` and `-taxon` were both not set, will use `_Nicotiana tabacum_`
-to get the reference (which is one of the earliest sequenced chloroplast
-genomes)
-
-`-out [folder name]`: output folder, if not set, the program will auto
-create it according to the input file's name
-
-### Advanced
-These options are for advanced users. If not sure, just keep the default
-value.
-
-`-platform [illumina/ion]`: sequencing platform, the default is `illumina`. If
-use ion-torrent, set `-platform ion`
-
-`-insert_size [number]`: the insert size of the sequencing library, should be
-integer
-
-`-seed [names]`: gene names as seeds for assembly, separated by commas, the
-default seeds are `rbcL,psaB,psaC,rrn23`
-
-`-seed_file [filename]`: seed file, will overwrite `-seed` option
-
-`-split [number]`: split input file, only use `[number]` of them, useful for
-large data while computer memory is limited.  For instance, `-split 10000000`
-will only use 10 million reads
-
-`-kmer [number]`: kmer size for assembly, should be an odd number. Most time
-it's unnecessary to change it
-
-`-min [number]`: minimum genome size, default is 100 kB
-
-`-max [number]`: maximum genome size, default is 200 kB. Only change `-min`
-and `-max` if the target genome size is out of the default range. The program
-needn't know the precise size of the genome
-
-`-mem [number]`: memory limit, the unit is GB. For instance, `-mem 8` will
-limit the memory usage to 8 GB. Should be integer
-
-`-perc_identity [number]`: the threshold of minimum percent of identity, used
-for validation with BLAST. The default value is `0.7`. Should be a float number
-between 0 and 1.
-
-`-len_diff [number]`: the threshold of maximum percent of length different of
-query and reference. Used for eliminating invalid assembly results. If the
-sequence length's difference of assembly and reference genome is larger than
-the value, the assembly result will be discarded. The default value is `0.2`.
-Should be a float number between 0 and 1.
-
-`-debug`: print debug information if set
-
-`-mt`: for mitochondria genomes (experimental function)
-
-`-simple_validate`: for chloroplast genomes without quadripartite structure
-
-## Validate
-### General
-`-h` or `-help`: print help message
-
-`-input [filename]`: input filename. Only support `fasta` format
-
-`-ref [filename]`, reference file for assembly and validation, should be
-`genbank` or `fasta` format that contains *only one* chloroplast genome
-sequence. Extra sequences will be *ignored*.
-
-`-taxon [taxonomy name]`: taxonomy name of the reference's species, space
-is allowed. Recommend to use same genus or family, or higher rank if it's well
-known that the target taxonomy's chloroplast genome is conserved.
-
-`-out [folder name]`: output folder, if not set, the program will automatically 
-create it according to input file's name
-### Advanced
-`-perc_identity [number]`: the threshold of minimum percent of identity, used
-for validation with BLAST. The default value is `0.7`. Should be a float number
-between 0 and 1.
-
-`-len_diff [number]`: the threshold of maximum percent of length different of
-query and reference. Used for eliminating invalid assembly results. If the
-sequence length's difference of assembly and reference genome is larger than
-the value, the assembly result will be discarded. The default value is `0.2`.
-Should be a float number between 0 and 1.
-
-`-debug`: print debug information if set
-
-`-mt`: for mitochondria genomes (experimental function)
-
-`-simple_validate`: for chloroplast genomes without quadripartite structure
-
-## Merge
-`-h` or `-help`: print help message
-
-`-input [filename]`: input filename. Only support `fasta` format
-
-`-out [folder name]`: output folder, if not set, the program will auto create
-it according to the input file's name
-
-# Performance
-The most time-consuming step is assembly. If the chloroplast genome's reads in
-sequencing data is plentiful enough, and the computer's memory is big enough
-for the data size, the assembly will be finished in minutes.
-
-The validation step usually could finish in less than one minute. If slower,
-please check the Internet connection since the program may query the NCBI
-database.
-
-The merge module could cost seconds or minutes. It depends on input data.
-The complex relationship of contigs requires much more time.
-
-# Citation
-Wu, P., Xu, C., Chen, H., Yang, J., Zhang, X. and Zhou, S. (2021), NOVOWrap: An automated solution for plastid genome assembly and structure standardization. Molecular Ecology Resources. https://doi.org/10.1111/1755-0998.13410
-# License
-The software itself is licensed under
-[AGPL-3.0](https://github.com/wpwupingwp/novowrap/blob/master/LICENSE) (**not include third-party
-software**).
-
-# Q&A
-Please submit your questions in the
-[Issue](https://github.com/wpwupingwp/novowrap/issues) page :smiley:
-
-* Q: I can't see the full UI, some part was missing.
-
-  A: Please try to drag the corner of the window to enlarge it. We got reports
-  that some users in macOS have this issue.
-
-* Q: I got the error message that the program failed to install
-  perl/BLAST/NOVOPlasty.
-
-  A: Uncommonly, users in a specific area will have connection issue for those
-  websites. Users have to manually download packages and install (see
-  [Software](#software) for the download links).
-
-  For Windows users, please download and unpack files into
-  `%HOMEDRIVE%%HOMEPATH%/.novowrap`.
-
-  For Linux  and MacOS users, please download and unpack files into
-  `~/.novowrap`.
-
-* Q: I got the error message that I don't have `tkinter `module installed.
-
-  A: If you want to run GUI on Linux or macOS, this error may happen because the
-  Python you used did not include tkinter as default package (kind of weird). Run
-  ```
-  # Debian and Ubuntu
-  sudo apt install python3-tk
-  # CentOS
-  sudo yum install python3-tk
-  ```
-  may help.
-
-  For macOS users or linux users without root privilege, please try to install the 
-  newest version of Python or to use conda, see [conda](https://docs.conda.io/en/latest/miniconda.html) 
-  and [Python](https://www.python.org/download/mac/tcltk/) for details.
-
-* Q: It says my input is invalid, but I'm sure it's OK!
-
-  A: Please check your files' path. The `space` character in the folder name
-  or filename may cause this error.
-* Q: It says `ImportError: Bio.Alphabet has been removed from Biopython` and 
-  the program failed to start.
-
-  A: In *2020.9*, Biopython removed Bio.Alphabet module in 
-  [v1.78](https://biopython.org/wiki/Alphabet), which may cause this trouble 
-  in the old version of novowrap. Please upgrade your `novowrap` to `v0.97` 
-  or higher. If you find difficult to upgrade novowrap, please try to use the 
-  portable packages.
-* Q: I want to assemble mitochondria genomes.
-
-  A: add `-mt` option or click the related checkbutton on the GUI.
-  Since mitochondria genomes do not have a stable 
-  and uniform structure like chloroplast, wet-lab experiments may be necessary 
-  for verification.
-* Q: I want to assemble chloroplast genomes without quadripartite structure.
-
-  A: add `-simple_validate` option in command-line or click the related checkbutton 
-  on the GUI. Note that without quadripartite structure, the Validate module 
-  will skip the adjustment of the structure of the sequences. We have test this function on
-  _Cytinus hypocistis_, a parasitic plant having a 19kb plastid genome.
-* Q: I am a `conda` user...
-
-  A: Install `novowrap` with `conda install -c wpwupingwp novowrap` and the usage is the same.
-  In order to avoid potential conflicts with other packages, it is highly recommended 
-  to create a new running environment with `conda` before installation. For example,
-  ```
-  conda create -n test
-  conda activate test
-  conda install -c wpwupingwp novowrap
-  ```
-
-  If fail, try to download conda packages from [this link](https://github.com/wpwupingwp/novowrap/releases),
-  and run
-  ```shell
-  conda install [filename]
-
-  ```
-* Q: I want to use novowrap in parallel.
-
-  A: Ideally, each novowrap instance is independent. However, the initialization process 
-  could affect other running instances. To avoid this, please running "python3 -m novowrap init"
-  one time before running in parallel.
-* Q: The assembly failed.
-
-  A: Make sure your sequencing data is okay. Otherwise, try to set the "-min" and "-max" options to 
-  restrict the size of the target genome. Sometimes it may fail due to inappropriate size values. The 
-  default size is 100-200 kb, which is okay for the common situation.
-
-
+Metadata-Version: 2.1
+Name: novowrap
+Version: 1.32
+Summary: Assembly Plastid Genome
+Author-email: Ping Wu <wpwupingwp@outlook.com>
+License: GNU AGPL v3
+Project-URL: Homepage, https://github.com/wpwupingwp/novowrap
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: biopython >=1.77
+Requires-Dist: coloredlogs >=10.0
+Requires-Dist: matplotlib >=3.2.0
+Requires-Dist: numpy >=1.19.1
+Requires-Dist: pip >=18.0
+Requires-Dist: graphviz >=0.13
+
+[![Build Status](https://travis-ci.org/wpwupingwp/novowrap.svg?branch=master)](https://travis-ci.org/wpwupingwp/novowrap)
+[![PyPI version](https://badge.fury.io/py/novowrap.svg)](https://badge.fury.io/py/novowrap)
+[![Anaconda version](https://anaconda.org/wpwupingwp/novowrap/badges/version.svg)](https://anaconda.org/wpwupingwp/novowrap)
+# Quick start
+Download [the package](https://github.com/wpwupingwp/novowrap/releases),
+unzip, and then double-click `novowrap.exe` or `novowrap`.
+
+__OR__
+
+Make sure you have [Python](https://www.python.org/) (3.7 or higher) or 
+[conda](https://docs.conda.io/en/latest/miniconda.html) installed.
+
+Open terminal, run
+   ```shell
+   # Install, using pip (recommended)
+   pip install novowrap --user
+   # Or, use conda
+   conda install -c wpwupingwp novowrap
+
+   # Initiliaze with Internet
+   # Windows
+   python -m novowrap init
+   # Linux and MacOS
+   python3 -m novowrap init
+
+   # Run
+   # Windows
+   python -m novowrap
+   # Linux and MacOS
+   python3 -m novowrap
+   ```
+
+# Table of Contents
+   * [Quick start](#quickstart)
+   * [Feature](#feature)
+   * [Prerequisite](#prerequisite)
+      * [Hardware](#hardware)
+      * [Software](#software)
+   * [Installation](#installation)
+      * [Portable](#portable)
+      * [Install with pip](#Installwithpip)
+      * [Install with conda](#Installwithconda)
+      * [Initialization](#Initialization)
+   * [Usage](#usage)
+      * [Command line](#commandline)
+      * [Graphical user interface](#graphicaluserintetface)
+   * [Input](#input)
+   * [Output](#output)
+   * [Options](#options)
+      * [Assembly](#assembly)
+      * [Validate](#validate)
+      * [Merge](#merge)
+   * [Performance](#performance)
+# Feature
+:heavy_check_mark: Assembly chloroplast genomes from given NGS data, with minimal
+parameters to set. Also, it supports batch mode.  
+
+Automatic generate uniform structure with reference (typically, start from 
+_trnH-psbA_, and, SSC/LSC region have the same direction with reference).
+
+:heavy_check_mark: Merge contigs according to overlapping region. May handle
+Invert-Repeat fragments.
+
+:heavy_check_mark: Validate assembly results by comparing the synteny and sequence
+homology with given reference (or taxonomy name).
+# Prerequisite
+## Hardware
+The assembly function will call NOVOPlasty, which requires 2 GB memory for 1
+GB uncompressed data.
+
+The other functions could run in normal computers and have no extra
+requirements for memory, CPU, et al.
+
+The software requires Internet for the first run to install the missing
+dependencies. Then, it could work if offline, but better with the internet.
+## Software
+For the portable version, nothing needs to be installed manually.
+
+For installing from pip, [Python](https://www.python.org/downloads/) is
+required. Notice that the python version should be **3.7** or higher.
+
+:white_check_mark: All third-party dependencies will be automatically
+installed with the Internet, including `biopython`, `matplotlib`, `coloredlogs`,
+`graphviz` (python packages), and
+[perl(for Windows only)](http://strawberryperl.com/download/5.30.1.1/strawberry-perl-5.30.1.1-64bit-portable.zip), 
+[NOVOPlasty](https://github.com/ndierckx/NOVOPlasty),
+[BLAST](https://blast.ncbi.nlm.nih.gov/Blast.cgi?CMD=Web&PAGE_TYPE=BlastDocs&DOC_TYPE=Download).
+
+# Installation
+## Portable
+Download from the [link](https://github.com/wpwupingwp/novowrap/releases),
+unpack and run with Internet for the first time.
+## Install with pip
+1. Install [Python](https://www.python.org/downloads/). *3.7 or newer* is
+   required.
+     
+2. Open the command line, run
+```shell
+pip install novowrap --user
+```
+## Install with conda
+After installed [conda](https://docs.conda.io/en/latest/miniconda.html), run
+```
+conda install -c wpwupingwp novowrap
+```
+## Initialization
+During the first running, `novowrap` will check and initialize the running environment. 
+Missing dependencies will be automatically installed.
+This step requires the Internet connection.
+```shell
+# Windows
+python -m novowrap init
+# Linux and MacOS
+python3 -m novowrap init
+```
+# Usage
+## Command line
+:exclamation: In Linux and macOS, Python2 is `python2` and Python3 is `python3`.  However,
+in Windows, Python3 is called `python`, too. Please notice the difference.
+
+ * Show help information of each module
+ ```shell
+ # Windows
+ python -m novowrap.assembly -h
+ python -m novowrap.validate -h
+ python -m novowrap.merge -h
+ # Linux and MacOS
+ python3 -m novowrap.assembly -h
+ python3 -m novowrap.validate -h
+ python3 -m novowrap.merge -h
+ ```
+ * Assembly and validate
+ ```shell
+ # Windows, single sample
+ python -m novowrap -input [input1] [input2] -taxon [taxonomy]
+ # Windows, batch mode for numerous samples
+ python -m novowrap -list [list file]
+ # Linux and MacOS, single sample
+ python3 -m novowrap -input [input1] [input2] -taxon [taxonomy]
+ # Linux and MacOS, batch mode for numerous samples
+ python3 -m novowrap -list [list file]
+ ```
+ * Only validate
+ ```shell
+ # Windows
+ python -m novowrap.validate -input [input file] -taxon [taxonomy]
+ # Linux and MacOS
+ python3 -m novowrap.validate -input [input file] -taxon [taxonomy]
+ ```
+ * Only merge
+ ```shell
+ # Windows
+ python -m novowrap.merge -input [input file]
+ # Linux and MacOS
+ python3 -m novowrap.merge -input [input file]
+ ```
+## Graphical user interface
+ If installed with pip,
+```shell
+# Windows
+python -m novowrap
+# Linux and MacOS
+python3 -m novowrap
+```
+
+If use the portable version, just double-click the `novowrap.exe` or `novowrap` in
+the folder.
+
+Then click the button to choose which module to use. Notice that if one of the
+option was set to the wrong value, the program will refuse to run and hint the
+user to correct the invalid option.
+# Input
+The `assembly` module accepts `gz` or `fastq` format as input. If use `input
+list`, the list file should be `csv` format. If use `reference` file instead
+of automatically get from NCBI, the file format should be `genbank`.
+
+The `merge` module accepts `fasta` format as input.
+
+The `validate` module accepts `fasta` format as input. If use `reference` file
+instead of automatically get from NCBI, the file format should be `genbank`
+**or** `fasta` as long as it is a complete chloroplast genome.
+
+# Output
+`.gb` files: **genbank** format sequence, with annotation of the boundary of
+LSC/SSC/IR regions.
+
+`.rotate` files: rotated sequence as **fasta** format; start from `trnH-psbA`, same direction with
+reference
+
+`.pdf` files: figure of validation of assembly
+
+`_RC_` files: if filenames contain `_RC_`, it means one of the regions of the
+sequence was adjusted according to the reference. The unadjusted sequence
+could be found in `Temp` folder.
+
+# Options
+## Assembly
+### General
+These options are for general usage.
+
+`-h` or `-help`: print help message
+
+`-input [filenames]`: input filenames, could be single or pair-end, support gz
+and fastq format
+
+`-list [filenames]`: input list for batch mode. The list should be a csv file
+with three columns,
+```csv
+Input 1,Input 2,Taxonomy
+```
+If only has one input file, just leave the `Input 2` column empty.
+
+Please use *full path* of file names, for instance, `d:\data\sample-1\forward.fastq`
+instead of `forward.fastq` or `sample-1\forward.fastq`.
+
+`-ref [filename]`: reference file for assembly and validation, should be
+`genbank` format contains *only one* chloroplast genome sequence. Extra
+sequences will be *ignored*. For automatic running, `-taxon` is recommended
+
+`-taxon [taxonomy name]`: taxonomy name of the sample, space is allowed.  For
+instance, `-taxon Oryza sativa`, will find reference chloroplast genome of
+`_Oryza sativa_` from NCBI RefSeq database. If not found, will find most related
+species' reference, `Oryza`, `Poaceae`, `Poales` et al.
+
+If `-ref` and `-taxon` were both not set, will use `_Nicotiana tabacum_`
+to get the reference (which is one of the earliest sequenced chloroplast
+genomes)
+
+`-out [folder name]`: output folder, if not set, the program will auto
+create it according to the input file's name
+
+### Advanced
+These options are for advanced users. If not sure, just keep the default
+value.
+
+`-platform [illumina/ion]`: sequencing platform, the default is `illumina`. If
+use ion-torrent, set `-platform ion`
+
+`-insert_size [number]`: the insert size of the sequencing library, should be
+integer
+
+`-seed [names]`: gene names as seeds for assembly, separated by commas, the
+default seeds are `rbcL,psaB,psaC,rrn23`
+
+`-seed_file [filename]`: seed file, will overwrite `-seed` option
+
+`-split [number]`: split input file, only use `[number]` of them, useful for
+large data while computer memory is limited.  For instance, `-split 10000000`
+will only use 10 million reads
+
+`-kmer [number]`: kmer size for assembly, should be an odd number. Most time
+it's unnecessary to change it
+
+`-min [number]`: minimum genome size, default is 100 kB
+
+`-max [number]`: maximum genome size, default is 200 kB. Only change `-min`
+and `-max` if the target genome size is out of the default range. The program
+needn't know the precise size of the genome
+
+`-mem [number]`: memory limit, the unit is GB. For instance, `-mem 8` will
+limit the memory usage to 8 GB. Should be integer
+
+`-perc_identity [number]`: the threshold of minimum percent of identity, used
+for validation with BLAST. The default value is `0.7`. Should be a float number
+between 0 and 1.
+
+`-len_diff [number]`: the threshold of maximum percent of length different of
+query and reference. Used for eliminating invalid assembly results. If the
+sequence length's difference of assembly and reference genome is larger than
+the value, the assembly result will be discarded. The default value is `0.2`.
+Should be a float number between 0 and 1.
+
+`-debug`: print debug information if set
+
+`-mt`: for mitochondria genomes (experimental function)
+
+`-simple_validate`: for chloroplast genomes without quadripartite structure
+
+## Validate
+### General
+`-h` or `-help`: print help message
+
+`-input [filename]`: input filename. Only support `fasta` format
+
+`-ref [filename]`, reference file for assembly and validation, should be
+`genbank` or `fasta` format that contains *only one* chloroplast genome
+sequence. Extra sequences will be *ignored*.
+
+`-taxon [taxonomy name]`: taxonomy name of the reference's species, space
+is allowed. Recommend to use same genus or family, or higher rank if it's well
+known that the target taxonomy's chloroplast genome is conserved.
+
+`-out [folder name]`: output folder, if not set, the program will automatically 
+create it according to input file's name
+### Advanced
+`-perc_identity [number]`: the threshold of minimum percent of identity, used
+for validation with BLAST. The default value is `0.7`. Should be a float number
+between 0 and 1.
+
+`-len_diff [number]`: the threshold of maximum percent of length different of
+query and reference. Used for eliminating invalid assembly results. If the
+sequence length's difference of assembly and reference genome is larger than
+the value, the assembly result will be discarded. The default value is `0.2`.
+Should be a float number between 0 and 1.
+
+`-debug`: print debug information if set
+
+`-mt`: for mitochondria genomes (experimental function)
+
+`-simple_validate`: for chloroplast genomes without quadripartite structure
+
+## Merge
+`-h` or `-help`: print help message
+
+`-input [filename]`: input filename. Only support `fasta` format
+
+`-out [folder name]`: output folder, if not set, the program will auto create
+it according to the input file's name
+
+# Performance
+The most time-consuming step is assembly. If the chloroplast genome's reads in
+sequencing data is plentiful enough, and the computer's memory is big enough
+for the data size, the assembly will be finished in minutes.
+
+The validation step usually could finish in less than one minute. If slower,
+please check the Internet connection since the program may query the NCBI
+database.
+
+The merge module could cost seconds or minutes. It depends on input data.
+The complex relationship of contigs requires much more time.
+
+# Citation
+Wu, P., Xu, C., Chen, H., Yang, J., Zhang, X. and Zhou, S. (2021), NOVOWrap: An automated solution for plastid genome assembly and structure standardization. Molecular Ecology Resources. https://doi.org/10.1111/1755-0998.13410
+# License
+The software itself is licensed under
+[AGPL-3.0](https://github.com/wpwupingwp/novowrap/blob/master/LICENSE) (**not include third-party
+software**).
+
+# Q&A
+Please submit your questions in the
+[Issue](https://github.com/wpwupingwp/novowrap/issues) page :smiley:
+
+* Q: I can't see the full UI, some part was missing.
+
+  A: Please try to drag the corner of the window to enlarge it. We got reports
+  that some users in macOS have this issue.
+
+* Q: I got the error message that the program failed to install
+  perl/BLAST/NOVOPlasty.
+
+  A: Uncommonly, users in a specific area will have connection issue for those
+  websites. Users have to manually download packages and install (see
+  [Software](#software) for the download links).
+
+  For Windows users, please download and unpack files into
+  `%HOMEDRIVE%%HOMEPATH%/.novowrap`.
+
+  For Linux  and MacOS users, please download and unpack files into
+  `~/.novowrap`.
+
+* Q: I got the error message that I don't have `tkinter `module installed.
+
+  A: If you want to run GUI on Linux or macOS, this error may happen because the
+  Python you used did not include tkinter as default package (kind of weird). Run
+  ```
+  # Debian and Ubuntu
+  sudo apt install python3-tk
+  # CentOS
+  sudo yum install python3-tk
+  ```
+  may help.
+  
+  For macOS users or linux users without root privilege, please try to install the 
+  newest version of Python or to use conda, see [conda](https://docs.conda.io/en/latest/miniconda.html) 
+  and [Python](https://www.python.org/download/mac/tcltk/) for details.
+  
+* Q: It says my input is invalid, but I'm sure it's OK!
+
+  A: Please check your files' path. The `space` character in the folder name
+  or filename may cause this error.
+* Q: It says `ImportError: Bio.Alphabet has been removed from Biopython` and 
+  the program failed to start.
+  
+  A: In *2020.9*, Biopython removed Bio.Alphabet module in 
+  [v1.78](https://biopython.org/wiki/Alphabet), which may cause this trouble 
+  in the old version of novowrap. Please upgrade your `novowrap` to `v0.97` 
+  or higher. If you find difficult to upgrade novowrap, please try to use the 
+  portable packages.
+* Q: I want to assemble mitochondria genomes.
+
+  A: add `-mt` option or click the related checkbutton on the GUI.
+  Since mitochondria genomes do not have a stable 
+  and uniform structure like chloroplast, wet-lab experiments may be necessary 
+  for verification.
+* Q: I want to assemble chloroplast genomes without quadripartite structure.
+
+  A: add `-simple_validate` option in command-line or click the related checkbutton 
+  on the GUI. Note that without quadripartite structure, the Validate module 
+  will skip the adjustment of the structure of the sequences. We have test this function on
+  _Cytinus hypocistis_, a parasitic plant having a 19kb plastid genome.
+* Q: I am a `conda` user...
+
+  A: Install `novowrap` with `conda install -c wpwupingwp novowrap` and the usage is the same.
+  In order to avoid potential conflicts with other packages, it is highly recommended 
+  to create a new running environment with `conda` before installation. For example,
+  ```
+  conda create -n test
+  conda activate test
+  conda install -c wpwupingwp novowrap
+  ```
+  
+  If fail, try to download conda packages from [this link](https://github.com/wpwupingwp/novowrap/releases),
+  and run
+  ```shell
+  conda install [filename]
+
+  ```
+* Q: I want to use novowrap in parallel.
+
+  A: Ideally, each novowrap instance is independent. However, the initialization process 
+  could affect other running instances. To avoid this, please running "python3 -m novowrap init"
+  one time before running in parallel.
+* Q: The assembly failed.
+
+  A: Make sure your sequencing data is okay. Otherwise, try to set the "-min" and "-max" options to 
+  restrict the size of the target genome. Sometimes it may fail due to inappropriate size values. The 
+  default size is 100-200 kb, which is okay for the common situation.
```

