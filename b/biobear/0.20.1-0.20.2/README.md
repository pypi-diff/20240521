# Comparing `tmp/biobear-0.20.1.tar.gz` & `tmp/biobear-0.20.2.tar.gz`

## Comparing `biobear-0.20.1.tar` & `biobear-0.20.2.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0      411 1970-01-01 00:00:00.000000 biobear-0.20.1/Cargo.toml
--rw-r--r--   0     1001      127       18 2024-05-17 17:53:51.000000 biobear-0.20.1/.github/FUNDING.yml
--rw-r--r--   0     1001      127     3295 2024-05-17 17:53:51.000000 biobear-0.20.1/.github/biobear.svg
--rw-r--r--   0     1001      127      100 2024-05-17 17:53:51.000000 biobear-0.20.1/.github/dependabot.yml
--rw-r--r--   0     1001      127     4104 2024-05-17 17:53:51.000000 biobear-0.20.1/.github/workflows/release.yml
--rw-r--r--   0     1001      127     1517 2024-05-17 17:53:51.000000 biobear-0.20.1/.github/workflows/smoke-test.yml
--rw-r--r--   0     1001      127      143 2024-05-17 17:53:51.000000 biobear-0.20.1/.github/workflows/smoketest.py
--rw-r--r--   0     1001      127     1160 2024-05-17 17:53:51.000000 biobear-0.20.1/.github/workflows/test.yml
--rw-r--r--   0     1001      127     4135 2024-05-17 17:53:51.000000 biobear-0.20.1/.gitignore
--rw-r--r--   0     1001      127     4524 2024-05-17 17:53:51.000000 biobear-0.20.1/CHANGELOG.md
--rw-r--r--   0     1001      127     1055 2024-05-17 17:53:51.000000 biobear-0.20.1/LICENSE
--rw-r--r--   0     1001      127      207 2024-05-17 17:53:51.000000 biobear-0.20.1/Makefile
--rw-r--r--   0     1001      127     7956 2024-05-17 17:53:51.000000 biobear-0.20.1/README.md
--rw-r--r--   0     1001      127      393 2024-05-17 17:53:51.000000 biobear-0.20.1/benchmarks/biobear-scan.py
--rw-r--r--   0     1001      127      467 2024-05-17 17:53:51.000000 biobear-0.20.1/benchmarks/biopython-scan.py
--rw-r--r--   0     1001      127      979 2024-05-17 17:53:51.000000 biobear-0.20.1/benchmarks/results.json
--rw-r--r--   0     1001      127     1569 2024-05-17 17:53:51.000000 biobear-0.20.1/bin/test.sh
--rw-r--r--   0     1001      127      285 2024-05-17 17:53:51.000000 biobear-0.20.1/cz.json
--rw-r--r--   0     1001      127      252 2024-05-17 17:53:51.000000 biobear-0.20.1/docs.bash
--rw-r--r--   0     1001      127     2587 2024-05-17 17:53:51.000000 biobear-0.20.1/python/biobear/__init__.py
--rw-r--r--   0     1001      127     2304 2024-05-17 17:53:51.000000 biobear-0.20.1/python/biobear/bam_reader.py
--rw-r--r--   0     1001      127     2087 2024-05-17 17:53:51.000000 biobear-0.20.1/python/biobear/bcf_reader.py
--rw-r--r--   0     1001      127     7988 2024-05-17 17:53:51.000000 biobear-0.20.1/python/biobear/biobear.pyi
--rw-r--r--   0     1001      127     1309 2024-05-17 17:53:51.000000 biobear-0.20.1/python/biobear/compression.py
--rw-r--r--   0     1001      127     1762 2024-05-17 17:53:51.000000 biobear-0.20.1/python/biobear/fasta_reader.py
--rw-r--r--   0     1001      127     1756 2024-05-17 17:53:51.000000 biobear-0.20.1/python/biobear/fastq_reader.py
--rw-r--r--   0     1001      127      858 2024-05-17 17:53:51.000000 biobear-0.20.1/python/biobear/genbank_reader.py
--rw-r--r--   0     1001      127     1564 2024-05-17 17:53:51.000000 biobear-0.20.1/python/biobear/gff_reader.py
--rw-r--r--   0     1001      127     1566 2024-05-17 17:53:51.000000 biobear-0.20.1/python/biobear/gtf_reader.py
--rw-r--r--   0     1001      127     1050 2024-05-17 17:53:51.000000 biobear-0.20.1/python/biobear/mzml_reader.py
--rw-r--r--   0     1001      127        0 2024-05-17 17:53:51.000000 biobear-0.20.1/python/biobear/py.typed
--rw-r--r--   0     1001      127     2910 2024-05-17 17:53:51.000000 biobear-0.20.1/python/biobear/reader.py
--rw-r--r--   0     1001      127     2129 2024-05-17 17:53:51.000000 biobear-0.20.1/python/biobear/vcf_reader.py
--rw-r--r--   0     1001      127   124562 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/BGC0000404.gbk
--rw-r--r--   0     1001      127     6152 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/bedcov.bam
--rw-r--r--   0     1001      127     7608 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/bedcov.bam.bai
--rw-r--r--   0     1001      127      939 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/cram/0500_mapped.cram
--rw-r--r--   0     1001      127     7275 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/cram/1404_index_multislice.cram
--rw-r--r--   0     1001      127      156 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/cram/1404_index_multislice.cram.crai
--rw-r--r--   0     1001      127  1060702 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/cram/ce.fa
--rw-r--r--   0     1001      127      230 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/cram/ce.fa.fai
--rw-r--r--   0     1001      127     3178 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/cram/test_input_1_a.cram
--rw-r--r--   0     1001      127   339527 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/fake_fastq_file.fastq.gz
--rw-r--r--   0     1001      127     1749 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/file.vcf
--rw-r--r--   0     1001      127     9521 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/index.bcf
--rw-r--r--   0     1001      127      143 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/index.bcf.csi
--rw-r--r--   0     1001      127     8638 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/index.vcf.gz
--rw-r--r--   0     1001      127      213 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/index.vcf.gz.tbi
--rw-r--r--   0     1001      127       41 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/test.fa
--rw-r--r--   0     1001      127       55 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/test.fa.gz
--rw-r--r--   0     1001      127       41 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/test.fasta
--rw-r--r--   0     1001      127       22 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/test.fasta.fai
--rw-r--r--   0     1001      127       58 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/test.fasta.gz
--rw-r--r--   0     1001      127      286 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/test.fastq
--rw-r--r--   0     1001      127      134 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/test.fastq.gz
--rw-r--r--   0     1001      127      286 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/test.fq
--rw-r--r--   0     1001      127      156 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/test.fq.gz
--rw-r--r--   0     1001      127      112 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/test.gff
--rw-r--r--   0     1001      127       91 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/test.gff.gz
--rw-r--r--   0     1001      127    17994 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/test.gtf
--rw-r--r--   0     1001      127     1478 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/test.gtf.gz
--rw-r--r--   0     1001      127    17171 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/test.mzML
--rw-r--r--   0     1001      127     2845 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/test.mzML.gz
--rw-r--r--   0     1001      127     1025 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/two-cram/rand1k.fa
--rw-r--r--   0     1001      127       20 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/two-cram/rand1k.fa.fai
--rw-r--r--   0     1001      127     1029 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/two-cram/twolib.sorted.cram
--rw-r--r--   0     1001      127       42 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/two-cram/twolib.sorted.cram.crai
--rw-r--r--   0     1001      127     1669 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/vcf-partition/sample=1/vcf_file.vcf.gz
--rw-r--r--   0     1001      127      254 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/vcf-partition/sample=1/vcf_file.vcf.gz.tbi
--rw-r--r--   0     1001      127     4302 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/vcf_file.vcf
--rw-r--r--   0     1001      127     1669 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/vcf_file.vcf.gz
--rw-r--r--   0     1001      127      254 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/data/vcf_file.vcf.gz.tbi
--rw-r--r--   0     1001      127    14881 2024-05-17 17:53:51.000000 biobear-0.20.1/python/tests/test_session.py
--rw-r--r--   0     1001      127       47 2024-05-17 17:53:51.000000 biobear-0.20.1/requirements-dev.txt
--rw-r--r--   0     1001      127     3705 2024-05-17 17:53:51.000000 biobear-0.20.1/src/bam_reader.rs
--rw-r--r--   0     1001      127     3590 2024-05-17 17:53:51.000000 biobear-0.20.1/src/bcf_reader.rs
--rw-r--r--   0     1001      127     1397 2024-05-17 17:53:51.000000 biobear-0.20.1/src/datasources/bam.rs
--rw-r--r--   0     1001      127     1631 2024-05-17 17:53:51.000000 biobear-0.20.1/src/datasources/bcf.rs
--rw-r--r--   0     1001      127     1561 2024-05-17 17:53:51.000000 biobear-0.20.1/src/datasources/bed.rs
--rw-r--r--   0     1001      127     2572 2024-05-17 17:53:51.000000 biobear-0.20.1/src/datasources/bigwig.rs
--rw-r--r--   0     1001      127     1548 2024-05-17 17:53:51.000000 biobear-0.20.1/src/datasources/cram.rs
--rw-r--r--   0     1001      127     3265 2024-05-17 17:53:51.000000 biobear-0.20.1/src/datasources/fasta.rs
--rw-r--r--   0     1001      127     3322 2024-05-17 17:53:51.000000 biobear-0.20.1/src/datasources/fastq.rs
--rw-r--r--   0     1001      127     1353 2024-05-17 17:53:51.000000 biobear-0.20.1/src/datasources/fcs.rs
--rw-r--r--   0     1001      127     1380 2024-05-17 17:53:51.000000 biobear-0.20.1/src/datasources/genbank.rs
--rw-r--r--   0     1001      127     1913 2024-05-17 17:53:51.000000 biobear-0.20.1/src/datasources/gff.rs
--rw-r--r--   0     1001      127     1476 2024-05-17 17:53:51.000000 biobear-0.20.1/src/datasources/gtf.rs
--rw-r--r--   0     1001      127     1322 2024-05-17 17:53:51.000000 biobear-0.20.1/src/datasources/hmm_dom_tab.rs
--rw-r--r--   0     1001      127     1224 2024-05-17 17:53:51.000000 biobear-0.20.1/src/datasources/mod.rs
--rw-r--r--   0     1001      127     1517 2024-05-17 17:53:51.000000 biobear-0.20.1/src/datasources/mzml.rs
--rw-r--r--   0     1001      127     1071 2024-05-17 17:53:51.000000 biobear-0.20.1/src/datasources/sam.rs
--rw-r--r--   0     1001      127     2839 2024-05-17 17:53:51.000000 biobear-0.20.1/src/datasources/vcf.rs
--rw-r--r--   0     1001      127     2606 2024-05-17 17:53:51.000000 biobear-0.20.1/src/error.rs
--rw-r--r--   0     1001      127     4185 2024-05-17 17:53:51.000000 biobear-0.20.1/src/execution_result.rs
--rw-r--r--   0     1001      127     3784 2024-05-17 17:53:51.000000 biobear-0.20.1/src/exon_reader.rs
--rw-r--r--   0     1001      127     3225 2024-05-17 17:53:51.000000 biobear-0.20.1/src/file_compression_type.rs
--rw-r--r--   0     1001      127     2706 2024-05-17 17:53:51.000000 biobear-0.20.1/src/lib.rs
--rw-r--r--   0     1001      127     1247 2024-05-17 17:53:51.000000 biobear-0.20.1/src/runtime.rs
--rw-r--r--   0     1001      127     9978 2024-05-17 17:53:51.000000 biobear-0.20.1/src/session_context.rs
--rw-r--r--   0     1001      127     3752 2024-05-17 17:53:51.000000 biobear-0.20.1/src/vcf_reader.rs
--rw-r--r--   0     1001      127   111135 2024-05-17 17:53:58.000000 biobear-0.20.1/Cargo.lock
--rw-r--r--   0     1001      127      725 2024-05-17 17:53:51.000000 biobear-0.20.1/pyproject.toml
--rw-r--r--   0        0        0     8469 1970-01-01 00:00:00.000000 biobear-0.20.1/PKG-INFO
+-rw-r--r--   0        0        0      413 1970-01-01 00:00:00.000000 biobear-0.20.2/Cargo.toml
+-rw-r--r--   0     1001      127       18 2024-05-21 16:32:44.000000 biobear-0.20.2/.github/FUNDING.yml
+-rw-r--r--   0     1001      127     3295 2024-05-21 16:32:44.000000 biobear-0.20.2/.github/biobear.svg
+-rw-r--r--   0     1001      127      100 2024-05-21 16:32:44.000000 biobear-0.20.2/.github/dependabot.yml
+-rw-r--r--   0     1001      127     4104 2024-05-21 16:32:44.000000 biobear-0.20.2/.github/workflows/release.yml
+-rw-r--r--   0     1001      127     1517 2024-05-21 16:32:44.000000 biobear-0.20.2/.github/workflows/smoke-test.yml
+-rw-r--r--   0     1001      127      143 2024-05-21 16:32:44.000000 biobear-0.20.2/.github/workflows/smoketest.py
+-rw-r--r--   0     1001      127     1160 2024-05-21 16:32:44.000000 biobear-0.20.2/.github/workflows/test.yml
+-rw-r--r--   0     1001      127     4135 2024-05-21 16:32:44.000000 biobear-0.20.2/.gitignore
+-rw-r--r--   0     1001      127     4593 2024-05-21 16:32:44.000000 biobear-0.20.2/CHANGELOG.md
+-rw-r--r--   0     1001      127     1055 2024-05-21 16:32:44.000000 biobear-0.20.2/LICENSE
+-rw-r--r--   0     1001      127      273 2024-05-21 16:32:44.000000 biobear-0.20.2/Makefile
+-rw-r--r--   0     1001      127     7956 2024-05-21 16:32:44.000000 biobear-0.20.2/README.md
+-rw-r--r--   0     1001      127      393 2024-05-21 16:32:44.000000 biobear-0.20.2/benchmarks/biobear-scan.py
+-rw-r--r--   0     1001      127      467 2024-05-21 16:32:44.000000 biobear-0.20.2/benchmarks/biopython-scan.py
+-rw-r--r--   0     1001      127      979 2024-05-21 16:32:44.000000 biobear-0.20.2/benchmarks/results.json
+-rw-r--r--   0     1001      127     1569 2024-05-21 16:32:44.000000 biobear-0.20.2/bin/test.sh
+-rw-r--r--   0     1001      127      285 2024-05-21 16:32:44.000000 biobear-0.20.2/cz.json
+-rw-r--r--   0     1001      127      252 2024-05-21 16:32:44.000000 biobear-0.20.2/docs.bash
+-rw-r--r--   0     1001      127     2587 2024-05-21 16:32:44.000000 biobear-0.20.2/python/biobear/__init__.py
+-rw-r--r--   0     1001      127     2304 2024-05-21 16:32:44.000000 biobear-0.20.2/python/biobear/bam_reader.py
+-rw-r--r--   0     1001      127     2087 2024-05-21 16:32:44.000000 biobear-0.20.2/python/biobear/bcf_reader.py
+-rw-r--r--   0     1001      127     7988 2024-05-21 16:32:44.000000 biobear-0.20.2/python/biobear/biobear.pyi
+-rw-r--r--   0     1001      127     1309 2024-05-21 16:32:44.000000 biobear-0.20.2/python/biobear/compression.py
+-rw-r--r--   0     1001      127     1762 2024-05-21 16:32:44.000000 biobear-0.20.2/python/biobear/fasta_reader.py
+-rw-r--r--   0     1001      127     1756 2024-05-21 16:32:44.000000 biobear-0.20.2/python/biobear/fastq_reader.py
+-rw-r--r--   0     1001      127      858 2024-05-21 16:32:44.000000 biobear-0.20.2/python/biobear/genbank_reader.py
+-rw-r--r--   0     1001      127     1564 2024-05-21 16:32:44.000000 biobear-0.20.2/python/biobear/gff_reader.py
+-rw-r--r--   0     1001      127     1566 2024-05-21 16:32:44.000000 biobear-0.20.2/python/biobear/gtf_reader.py
+-rw-r--r--   0     1001      127     1050 2024-05-21 16:32:44.000000 biobear-0.20.2/python/biobear/mzml_reader.py
+-rw-r--r--   0     1001      127        0 2024-05-21 16:32:44.000000 biobear-0.20.2/python/biobear/py.typed
+-rw-r--r--   0     1001      127     2910 2024-05-21 16:32:44.000000 biobear-0.20.2/python/biobear/reader.py
+-rw-r--r--   0     1001      127     2129 2024-05-21 16:32:44.000000 biobear-0.20.2/python/biobear/vcf_reader.py
+-rw-r--r--   0     1001      127   124562 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/BGC0000404.gbk
+-rw-r--r--   0     1001      127     6152 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/bedcov.bam
+-rw-r--r--   0     1001      127     7608 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/bedcov.bam.bai
+-rw-r--r--   0     1001      127      939 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/cram/0500_mapped.cram
+-rw-r--r--   0     1001      127     7275 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/cram/1404_index_multislice.cram
+-rw-r--r--   0     1001      127      156 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/cram/1404_index_multislice.cram.crai
+-rw-r--r--   0     1001      127  1060702 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/cram/ce.fa
+-rw-r--r--   0     1001      127      230 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/cram/ce.fa.fai
+-rw-r--r--   0     1001      127     3178 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/cram/test_input_1_a.cram
+-rw-r--r--   0     1001      127   339527 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/fake_fastq_file.fastq.gz
+-rw-r--r--   0     1001      127     1749 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/file.vcf
+-rw-r--r--   0     1001      127     9521 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/index.bcf
+-rw-r--r--   0     1001      127      143 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/index.bcf.csi
+-rw-r--r--   0     1001      127     8638 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/index.vcf.gz
+-rw-r--r--   0     1001      127      213 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/index.vcf.gz.tbi
+-rw-r--r--   0     1001      127       41 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.fa
+-rw-r--r--   0     1001      127       55 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.fa.gz
+-rw-r--r--   0     1001      127       41 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.fasta
+-rw-r--r--   0     1001      127       22 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.fasta.fai
+-rw-r--r--   0     1001      127       58 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.fasta.gz
+-rw-r--r--   0     1001      127      286 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.fastq
+-rw-r--r--   0     1001      127      134 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.fastq.gz
+-rw-r--r--   0     1001      127      286 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.fq
+-rw-r--r--   0     1001      127      156 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.fq.gz
+-rw-r--r--   0     1001      127      112 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.gff
+-rw-r--r--   0     1001      127       91 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.gff.gz
+-rw-r--r--   0     1001      127    17994 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.gtf
+-rw-r--r--   0     1001      127     1478 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.gtf.gz
+-rw-r--r--   0     1001      127    17171 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.mzML
+-rw-r--r--   0     1001      127     2845 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/test.mzML.gz
+-rw-r--r--   0     1001      127     1025 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/two-cram/rand1k.fa
+-rw-r--r--   0     1001      127       20 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/two-cram/rand1k.fa.fai
+-rw-r--r--   0     1001      127     1029 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/two-cram/twolib.sorted.cram
+-rw-r--r--   0     1001      127       42 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/two-cram/twolib.sorted.cram.crai
+-rw-r--r--   0     1001      127     1669 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/vcf-partition/sample=1/vcf_file.vcf.gz
+-rw-r--r--   0     1001      127      254 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/vcf-partition/sample=1/vcf_file.vcf.gz.tbi
+-rw-r--r--   0     1001      127     4302 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/vcf_file.vcf
+-rw-r--r--   0     1001      127     1669 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/vcf_file.vcf.gz
+-rw-r--r--   0     1001      127      254 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/data/vcf_file.vcf.gz.tbi
+-rw-r--r--   0     1001      127    14881 2024-05-21 16:32:44.000000 biobear-0.20.2/python/tests/test_session.py
+-rw-r--r--   0     1001      127       47 2024-05-21 16:32:44.000000 biobear-0.20.2/requirements-dev.txt
+-rw-r--r--   0     1001      127     3705 2024-05-21 16:32:44.000000 biobear-0.20.2/src/bam_reader.rs
+-rw-r--r--   0     1001      127     3590 2024-05-21 16:32:44.000000 biobear-0.20.2/src/bcf_reader.rs
+-rw-r--r--   0     1001      127     1397 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/bam.rs
+-rw-r--r--   0     1001      127     1631 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/bcf.rs
+-rw-r--r--   0     1001      127     1561 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/bed.rs
+-rw-r--r--   0     1001      127     2572 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/bigwig.rs
+-rw-r--r--   0     1001      127     1548 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/cram.rs
+-rw-r--r--   0     1001      127     3265 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/fasta.rs
+-rw-r--r--   0     1001      127     3322 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/fastq.rs
+-rw-r--r--   0     1001      127     1353 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/fcs.rs
+-rw-r--r--   0     1001      127     1380 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/genbank.rs
+-rw-r--r--   0     1001      127     1913 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/gff.rs
+-rw-r--r--   0     1001      127     1476 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/gtf.rs
+-rw-r--r--   0     1001      127     1322 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/hmm_dom_tab.rs
+-rw-r--r--   0     1001      127     1224 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/mod.rs
+-rw-r--r--   0     1001      127     1517 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/mzml.rs
+-rw-r--r--   0     1001      127     1071 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/sam.rs
+-rw-r--r--   0     1001      127     2839 2024-05-21 16:32:44.000000 biobear-0.20.2/src/datasources/vcf.rs
+-rw-r--r--   0     1001      127     2606 2024-05-21 16:32:44.000000 biobear-0.20.2/src/error.rs
+-rw-r--r--   0     1001      127     4634 2024-05-21 16:32:44.000000 biobear-0.20.2/src/execution_result.rs
+-rw-r--r--   0     1001      127     3784 2024-05-21 16:32:44.000000 biobear-0.20.2/src/exon_reader.rs
+-rw-r--r--   0     1001      127     3225 2024-05-21 16:32:44.000000 biobear-0.20.2/src/file_compression_type.rs
+-rw-r--r--   0     1001      127     2706 2024-05-21 16:32:44.000000 biobear-0.20.2/src/lib.rs
+-rw-r--r--   0     1001      127     1247 2024-05-21 16:32:44.000000 biobear-0.20.2/src/runtime.rs
+-rw-r--r--   0     1001      127     9978 2024-05-21 16:32:44.000000 biobear-0.20.2/src/session_context.rs
+-rw-r--r--   0     1001      127     3752 2024-05-21 16:32:44.000000 biobear-0.20.2/src/vcf_reader.rs
+-rw-r--r--   0     1001      127   111359 2024-05-21 16:32:48.000000 biobear-0.20.2/Cargo.lock
+-rw-r--r--   0     1001      127      725 2024-05-21 16:32:44.000000 biobear-0.20.2/pyproject.toml
+-rw-r--r--   0        0        0     8469 1970-01-01 00:00:00.000000 biobear-0.20.2/PKG-INFO
```

### Comparing `biobear-0.20.1/.github/biobear.svg` & `biobear-0.20.2/.github/biobear.svg`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/.github/workflows/release.yml` & `biobear-0.20.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/.github/workflows/smoke-test.yml` & `biobear-0.20.2/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/.github/workflows/test.yml` & `biobear-0.20.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/.gitignore` & `biobear-0.20.2/.gitignore`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/CHANGELOG.md` & `biobear-0.20.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## v0.20.2 (2024-05-21)
+
+### Fix
+
+- new exon to fix overflow (#135)
+
 ## v0.20.1 (2024-05-16)
 
 ### Refactor
 
 - simplify bounds
 
 ## v0.20.0 (2024-04-24)
```

### Comparing `biobear-0.20.1/LICENSE` & `biobear-0.20.2/LICENSE`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/README.md` & `biobear-0.20.2/README.md`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/benchmarks/results.json` & `biobear-0.20.2/benchmarks/results.json`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/bin/test.sh` & `biobear-0.20.2/bin/test.sh`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/biobear/__init__.py` & `biobear-0.20.2/python/biobear/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 from .biobear import FCSReadOptions
 from .biobear import CRAMReadOptions
 from .biobear import connect
 from .biobear import new_session
 from .biobear import __runtime
 
 
-__version__ = "0.20.1"
+__version__ = "0.20.2"
 
 __all__ = [
     "FastaReader",
     "FastqReader",
     "VCFReader",
     "VCFIndexedReader",
     "BamReader",
```

### Comparing `biobear-0.20.1/python/biobear/bam_reader.py` & `biobear-0.20.2/python/biobear/bam_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/biobear/bcf_reader.py` & `biobear-0.20.2/python/biobear/bcf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/biobear/biobear.pyi` & `biobear-0.20.2/python/biobear/biobear.pyi`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/biobear/compression.py` & `biobear-0.20.2/python/biobear/compression.py`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/biobear/fasta_reader.py` & `biobear-0.20.2/python/biobear/fasta_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/biobear/fastq_reader.py` & `biobear-0.20.2/python/biobear/fastq_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/biobear/genbank_reader.py` & `biobear-0.20.2/python/biobear/genbank_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/biobear/gff_reader.py` & `biobear-0.20.2/python/biobear/gff_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/biobear/gtf_reader.py` & `biobear-0.20.2/python/biobear/gtf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/biobear/mzml_reader.py` & `biobear-0.20.2/python/biobear/mzml_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/biobear/reader.py` & `biobear-0.20.2/python/biobear/reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/biobear/vcf_reader.py` & `biobear-0.20.2/python/biobear/vcf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/tests/data/BGC0000404.gbk` & `biobear-0.20.2/python/tests/data/BGC0000404.gbk`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/tests/data/bedcov.bam` & `biobear-0.20.2/python/tests/data/bedcov.bam`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/tests/data/bedcov.bam.bai` & `biobear-0.20.2/python/tests/data/bedcov.bam.bai`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/tests/data/cram/0500_mapped.cram` & `biobear-0.20.2/python/tests/data/cram/0500_mapped.cram`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/tests/data/cram/1404_index_multislice.cram` & `biobear-0.20.2/python/tests/data/cram/1404_index_multislice.cram`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/tests/data/cram/ce.fa` & `biobear-0.20.2/python/tests/data/cram/ce.fa`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/tests/data/cram/test_input_1_a.cram` & `biobear-0.20.2/python/tests/data/cram/test_input_1_a.cram`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/tests/data/fake_fastq_file.fastq.gz` & `biobear-0.20.2/python/tests/data/fake_fastq_file.fastq.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/tests/data/file.vcf` & `biobear-0.20.2/python/tests/data/file.vcf`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/tests/data/index.bcf` & `biobear-0.20.2/python/tests/data/index.bcf`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/tests/data/index.vcf.gz` & `biobear-0.20.2/python/tests/data/index.vcf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/tests/data/test.gtf` & `biobear-0.20.2/python/tests/data/test.gtf`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/tests/data/test.gtf.gz` & `biobear-0.20.2/python/tests/data/test.gtf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/tests/data/test.mzML` & `biobear-0.20.2/python/tests/data/test.mzML`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/tests/data/test.mzML.gz` & `biobear-0.20.2/python/tests/data/test.mzML.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/tests/data/two-cram/rand1k.fa` & `biobear-0.20.2/python/tests/data/two-cram/rand1k.fa`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/tests/data/two-cram/twolib.sorted.cram` & `biobear-0.20.2/python/tests/data/two-cram/twolib.sorted.cram`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/tests/data/vcf-partition/sample=1/vcf_file.vcf.gz` & `biobear-0.20.2/python/tests/data/vcf-partition/sample=1/vcf_file.vcf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/tests/data/vcf_file.vcf` & `biobear-0.20.2/python/tests/data/vcf_file.vcf`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/tests/data/vcf_file.vcf.gz` & `biobear-0.20.2/python/tests/data/vcf_file.vcf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/python/tests/test_session.py` & `biobear-0.20.2/python/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/src/bam_reader.rs` & `biobear-0.20.2/src/bam_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/src/bcf_reader.rs` & `biobear-0.20.2/src/bcf_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/src/datasources/bam.rs` & `biobear-0.20.2/src/datasources/bam.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/src/datasources/bcf.rs` & `biobear-0.20.2/src/datasources/bcf.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/src/datasources/bed.rs` & `biobear-0.20.2/src/datasources/bed.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/src/datasources/bigwig.rs` & `biobear-0.20.2/src/datasources/bigwig.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/src/datasources/cram.rs` & `biobear-0.20.2/src/datasources/cram.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/src/datasources/fasta.rs` & `biobear-0.20.2/src/datasources/fasta.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/src/datasources/fastq.rs` & `biobear-0.20.2/src/datasources/fastq.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/src/datasources/fcs.rs` & `biobear-0.20.2/src/datasources/fcs.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/src/datasources/genbank.rs` & `biobear-0.20.2/src/datasources/genbank.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/src/datasources/gff.rs` & `biobear-0.20.2/src/datasources/gff.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/src/datasources/gtf.rs` & `biobear-0.20.2/src/datasources/gtf.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/src/datasources/hmm_dom_tab.rs` & `biobear-0.20.2/src/datasources/hmm_dom_tab.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/src/datasources/mod.rs` & `biobear-0.20.2/src/datasources/mod.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/src/datasources/mzml.rs` & `biobear-0.20.2/src/datasources/mzml.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/src/datasources/sam.rs` & `biobear-0.20.2/src/datasources/sam.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/src/datasources/vcf.rs` & `biobear-0.20.2/src/datasources/vcf.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/src/error.rs` & `biobear-0.20.2/src/error.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/src/execution_result.rs` & `biobear-0.20.2/src/execution_result.rs`

 * *Files 10% similar despite different names*

```diff
@@ -98,18 +98,29 @@
         let args = PyTuple::new(py, &[batches, schema]);
         let table: PyObject = table_class.call_method1("from_batches", args)?.into();
         Ok(table)
     }
 
     /// Convert to a Polars DataFrame
     fn to_polars(&self, py: Python) -> PyResult<PyObject> {
-        let batches = self.collect(py)?.to_object(py);
-        let schema = self.schema().into_py(py);
+        let stream = wait_for_future(py, self.df.as_ref().clone().execute_stream())
+            .map_err(error::BioBearError::from)?;
+
+        let runtime = Arc::new(Runtime::new()?);
+
+        let dataframe_record_batch_stream = DataFrameRecordBatchStream::new(stream, runtime);
+
+        let mut stream = FFI_ArrowArrayStream::new(Box::new(dataframe_record_batch_stream));
 
-        let schema = schema.into_py(py);
+        let batches =
+            unsafe { ArrowArrayStreamReader::from_raw(&mut stream).map_err(BioBearError::from) }?;
+
+        let batches = batches.into_pyarrow(py)?;
+
+        let schema = self.schema().into_py(py);
 
         let table_class = py.import("pyarrow")?.getattr("Table")?;
         let args = (batches, schema);
         let table: PyObject = table_class.call_method1("from_batches", args)?.into();
 
         let module = py.import("polars")?;
         let args = (table,);
```

### Comparing `biobear-0.20.1/src/exon_reader.rs` & `biobear-0.20.2/src/exon_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/src/file_compression_type.rs` & `biobear-0.20.2/src/file_compression_type.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/src/lib.rs` & `biobear-0.20.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/src/runtime.rs` & `biobear-0.20.2/src/runtime.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/src/session_context.rs` & `biobear-0.20.2/src/session_context.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/src/vcf_reader.rs` & `biobear-0.20.2/src/vcf_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.20.1/Cargo.lock` & `biobear-0.20.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -381,15 +381,15 @@
 name = "async-trait"
 version = "0.1.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6fa2087f2753a7da8cc1c0dbfcf89579dd57458e36769de5ac750b4671737ca"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "atoi"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f28d99ec8bfea296261ca1af174f24225171fea9664ba9003cbebee704810528"
@@ -748,17 +748,17 @@
 dependencies = [
  "outref",
  "vsimd",
 ]
 
 [[package]]
 name = "bigtools"
-version = "0.4.2"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2e7e3e2801e665559947318628677a989ee986fd6f18ac572e332127e72e27aa"
+checksum = "3991a416f05e8b4b5dc3c21bf86840217cd2fe2f995673d82698803d8e229c61"
 dependencies = [
  "attohttpc",
  "bincode",
  "byteorder",
  "byteordered",
  "bytes",
  "clap",
@@ -783,15 +783,15 @@
 checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "biobear"
-version = "0.20.1"
+version = "0.20.2"
 dependencies = [
  "arrow",
  "datafusion",
  "exon",
  "noodles",
  "pyo3",
  "tokio",
@@ -933,17 +933,17 @@
  "cc",
  "libc",
  "pkg-config",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.97"
+version = "1.0.98"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "099a5357d84c4c61eb35fc8eafa9a79a902c2f76911e5747ced4e032edd8d9b4"
+checksum = "41c270e7540d725e65ac7f1b212ac8ce349719624d7bcff99f8e2e488e8cf03f"
 dependencies = [
  "jobserver",
  "libc",
  "once_cell",
 ]
 
 [[package]]
@@ -1020,15 +1020,15 @@
 version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "528131438037fd55894f62d6e9f068b8f45ac57ffa77517819645d10aed04f64"
 dependencies = [
  "heck 0.5.0",
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
@@ -1105,35 +1105,35 @@
 checksum = "53fe5e26ff1b7aef8bca9c6080520cfb8d9333c7568e1829cef191a9723e5504"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32fast"
-version = "1.4.0"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b3855a8a784b474f333699ef2bbca9db2c4a1f6d9088a90a2d25b1eb53111eaa"
+checksum = "a97769d94ddab943e4510d138150169a2758b5ef3eb191a9ee688de3e23ef7b3"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.12"
+version = "0.5.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab3db02a9c5b5121e1e42fbdb1aeb65f5e02624cc58c43f2884c6ccac0b82f95"
+checksum = "33480d6946193aa8033910124896ca395333cae7e2d1113d1fef6c3272217df2"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.19"
+version = "0.8.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
+checksum = "22ec99545bb0ed0ea7bb9b8e1e9122ea386ff8a48c0922e43f36d45ab09e0e80"
 
 [[package]]
 name = "crunchy"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
 
@@ -1545,17 +1545,17 @@
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "exon"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94174e47e0e6244dcf1d610337887e36caee7c843a8d34ad02b19a1d914dab77"
+checksum = "b4db976195ae0c60902a35065692958c67abb20eb229687bd657d066b87009be"
 dependencies = [
  "arrow",
  "async-trait",
  "bytes",
  "coitrees",
  "datafusion",
  "exon-bam",
@@ -1572,15 +1572,15 @@
  "exon-gtf",
  "exon-io",
  "exon-mzml",
  "exon-sam",
  "exon-vcf",
  "futures",
  "fxhash",
- "itertools 0.12.1",
+ "itertools 0.13.0",
  "lazy_static",
  "noodles",
  "num_cpus",
  "object_store",
  "pin-project",
  "regex",
  "serde",
@@ -1589,212 +1589,212 @@
  "tracing",
  "tracing-subscriber",
  "url",
 ]
 
 [[package]]
 name = "exon-bam"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b47a06a8bbbeb0759b71126c2c85d345faebd926b9a418c0db39e467874caee"
+checksum = "bd9b95b31b8d8a6bbe37aa64303a03136d1035ec7185b1a44914f22e5f1be7a0"
 dependencies = [
  "arrow",
  "exon-common",
  "exon-sam",
  "futures",
- "itertools 0.12.1",
+ "itertools 0.13.0",
  "noodles",
  "object_store",
  "tokio",
 ]
 
 [[package]]
 name = "exon-bcf"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d8d9b74eee0bf4817ef38233d5556d81d183849937e955b037a5180a1f53758f"
+checksum = "da121f3b2c602eeece0b1d44f3a9cf838f71618a7e754151196e6c32c4ab129f"
 dependencies = [
  "arrow",
  "exon-common",
  "exon-vcf",
  "futures",
  "noodles",
  "object_store",
  "tokio",
 ]
 
 [[package]]
 name = "exon-bed"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2004cba15c0b43ca7ef8d0c52eee09369f638fe6835ee2061922ca57fd2658d"
+checksum = "c4799af616d89b424450e286914043469d8eaeafd9fb23287cba9aaa877a4124"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "noodles",
  "object_store",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
 name = "exon-bigwig"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60d06a876a344530cf97e9e273b1fa255f3d17a8d1bc3c5bcda9079a1d7d7de4"
+checksum = "06399ae57ddff134f0db19dfd3f96e385993cc15768942c62736ea29d9b1f409"
 dependencies = [
  "arrow",
  "bigtools",
  "exon-common",
  "futures",
  "noodles",
  "object_store",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
 name = "exon-common"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f8c8e491601267aa9a940967d1d7c612aa1f9a728670f4e1990f2236daafcb4d"
+checksum = "ae04f53aef64634ffbc45dc0dafd2e5fb5f30eaece28b8f206bc1e5c756058a8"
 dependencies = [
  "arrow",
  "datafusion",
  "futures",
  "glob",
  "object_store",
  "url",
 ]
 
 [[package]]
 name = "exon-cram"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3b5815611cea4a073464ad021a681ba97f27fc0b32b706feb17d4aa76d1726a9"
+checksum = "abb3e4efc7df09ce07d638c1eeed3c2ac34faf33e48f5e52911d26eee78137ad"
 dependencies = [
  "arrow",
  "coitrees",
  "exon-common",
  "exon-sam",
  "futures",
  "noodles",
  "object_store",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "exon-fasta"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "174903417f3d7032520bb48c7d42a40bd479afa3ba51b98a15a5972efe8af4ce"
+checksum = "1930a9127842fc218e959c70a48f2235f38e532207abaa607bbf509563320348"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "noodles",
  "object_store",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
 name = "exon-fastq"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e700b842882e3e7a2c35f75b53c4606bf309fe21b5a54e693247eee4ce112225"
+checksum = "44e0d93b39464c0a7985912ee5746bd54e6b543daed969ae1a6e278c2bc8d860"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "noodles",
  "object_store",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
 name = "exon-fcs"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5300c21a773ad4d9dc9c232e1d45081456ee7f7608bc13c971ab02b76cb8da6a"
+checksum = "d62b7c4b6fecfcb32981e7a9b2156dee12efa7fefbcfb89a6cc5802919248c5b"
 dependencies = [
  "arrow",
  "byteorder",
  "exon-common",
  "futures",
  "object_store",
  "tokio",
 ]
 
 [[package]]
 name = "exon-genbank"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e78032f646af4e01af3b564d587f53289a8eb533f0465a8ac10b2398be9c7f8f"
+checksum = "9d9c74945da538f254aa5c2f35680ae9dfcb25d9fd90df8ed011bf339d34fdb7"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "gb-io",
  "object_store",
  "tokio",
 ]
 
 [[package]]
 name = "exon-gff"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6dcee91a897ab9a127cde2beb09c4ff8c18612d6a8ec6b631e0b3c6fd2b5f571"
+checksum = "4ff0a1b56a57230a09344cf9f4c0eb390a70631d973decb1797d9f77c8a05fc3"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "noodles",
  "noodles-gff",
  "object_store",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
 name = "exon-gtf"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5202aa16bc7745d645497eb92bd680e7d05ff74d97b0403aae92a53633aa13de"
+checksum = "cace0693f2a5df616b290eb22315ace0f8b85cb98eb48290bc05412d73ebacc9"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "noodles",
  "object_store",
  "tokio",
 ]
 
 [[package]]
 name = "exon-io"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f0cff77568a301486fc87e038c87cf6fe417c942cb16e69fdf0a7f99016d661"
+checksum = "93751b18742c4562f6a7b297db4a0af448b9781b66e7002b6fcefe3c26658ad6"
 dependencies = [
  "async-trait",
  "aws-config",
  "aws-credential-types",
  "object_store",
  "tokio",
  "url",
 ]
 
 [[package]]
 name = "exon-mzml"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ce1e9340d2a849af54b871a07497683a7a0087fff107e0bd64f92ffb2e6a4f02"
+checksum = "4877eaba359662d2934dffce0342e0cfd85a973e4f39b9810e5c2f3bd26b806c"
 dependencies = [
  "arrow",
  "base64 0.22.1",
  "byteorder",
  "exon-common",
  "flate2",
  "futures",
@@ -1802,32 +1802,32 @@
  "quick-xml",
  "serde",
  "tokio",
 ]
 
 [[package]]
 name = "exon-sam"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "08327c443c3a0e5e191a222efa3f57766092f460aba905fbab4d7eb1afd3d9be"
+checksum = "afc3ce5645b3a32ea71eea35a9ca8db98baebfde644505cdb926214b44929897"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
- "itertools 0.12.1",
+ "itertools 0.13.0",
  "noodles",
  "object_store",
  "tokio",
 ]
 
 [[package]]
 name = "exon-vcf"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "29e016a4baa30c6647344ee9324725ebbce2ba2919e6fb6b9a265b56653b422e"
+checksum = "f7a856ac28fe0d4d119a61b03acae4a5458c66e52cfa0d5b44a911f59cca9bf3"
 dependencies = [
  "arrow",
  "exon-common",
  "futures",
  "noodles",
  "object_store",
  "tokio",
@@ -1933,15 +1933,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -2004,17 +2004,17 @@
 dependencies = [
  "typenum",
  "version_check 0.9.4",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.14"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
+checksum = "c4567c8db10ae91089c99af84c68c38da3ec2f087c3f82960bcdbf3656b6f4d7"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -2263,17 +2263,17 @@
 name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "instant"
-version = "0.1.12"
+version = "0.1.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
+checksum = "e0242819d153cba4b4b05a5a8f2a7e9bbf97b6055b2a002b395c96b5ff3c0222"
 dependencies = [
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
@@ -2310,14 +2310,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
 dependencies = [
  "either",
 ]
 
 [[package]]
+name = "itertools"
+version = "0.13.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "413ee7dfc52ee1a4949ceeb7dbc8a33f2d6c088194d9f922fb8318faf1f01186"
+dependencies = [
+ "either",
+]
+
+[[package]]
 name = "itoa"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "jobserver"
@@ -2405,17 +2414,17 @@
 dependencies = [
  "lexical-util",
  "static_assertions",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
 name = "libdeflate-sys"
 version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c301042beb41d94bc0f8dc667712f8fa8c42d3ea058dd7a71bed3fee8370c75e"
 dependencies = [
@@ -2508,17 +2517,17 @@
 name = "mime"
 version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.2"
+version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
+checksum = "87dfd01fe195c66b572b37921ad8803d010623c0aca821bea2302239d155cdae"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
 version = "0.8.11"
@@ -3106,15 +3115,15 @@
 name = "pin-project-internal"
 version = "1.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2f38a4412a78282e09a2cf38d195ea5420d15ba0602cb375210efbc877243965"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
@@ -3177,17 +3186,17 @@
  "proc-macro2",
  "quote",
  "version_check 0.9.4",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.82"
+version = "1.0.83"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ad3d49ab951a01fbaafe34f2ec74122942fe18a3f9814c3268f1bb72042131b"
+checksum = "0b33eb56c327dec362a9e55b3ad14f9d2f0904fb5a5b03b513ab5465399e9f43"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.20.3"
@@ -3231,28 +3240,28 @@
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
  "heck 0.4.1",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "quick-xml"
 version = "0.31.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1004a344b30a54e2ee58d66a71b32d2db2feb0a31f9a2d302bf0536f15de2a33"
@@ -3577,15 +3586,15 @@
 name = "serde_derive"
 version = "1.0.202"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6048858004bcff69094cd972ed40a32500f153bd3be9f716b2eed2e8217c4838"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
@@ -3715,15 +3724,15 @@
 name = "sqlparser_derive"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "01b2e185515564f15375f593fb966b5718bc624ba77fe49fa4616ad619690554"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
@@ -3775,15 +3784,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6cf59daf282c0a494ba14fd21610a0325f9f90ec9d1231dea26bcb1d696c946"
 dependencies = [
  "heck 0.4.1",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn 2.0.64",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "subtle"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
@@ -3797,17 +3806,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.64"
+version = "2.0.65"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ad3dee41f36859875573074334c200d1add8e4a87bb37113ebd31d926b7b11f"
+checksum = "d2863d96a84c6439701d7a38f9de935ec562c8832cc55d1dde0f513b52fad106"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -3880,15 +3889,15 @@
 name = "thiserror-impl"
 version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "46c3384250002a6d5af4d114f2845d37b57521033f30d5c3f46c4d70e1197533"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b9ef9bad013ada3808854ceac7b46812a6465ba368859a37e2100283d2d719c"
@@ -3984,15 +3993,15 @@
 name = "tokio-macros"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "tokio-rustls"
 version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c28327cf380ac148141087fbfb9de9d7bd4e84ab5d2c28fbc911d753de8a7081"
@@ -4036,15 +4045,15 @@
 name = "tracing-attributes"
 version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
@@ -4276,15 +4285,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.65",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -4310,15 +4319,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.65",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -4575,15 +4584,15 @@
 name = "zerocopy-derive"
 version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "15e934569e47891f7d9411f1a451d947a60e000ab3bd24fbb970f000387d1b3b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.64",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "zeroize"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
```

### Comparing `biobear-0.20.1/pyproject.toml` & `biobear-0.20.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 dependencies = ["pyarrow>=15"]
 license = { file = "LICENSE" }
 name = "biobear"
 readme = "README.md"
 requires-python = ">=3.8"
 description = "A package for working with Bioinformatics data with SQL and Arrow"
 summary = "A package for working with Bioinformatics data with SQL and Arrow"
-version = "0.20.1"
+version = "0.20.2"
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 python-source = "python"
```

### Comparing `biobear-0.20.1/PKG-INFO` & `biobear-0.20.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: biobear
-Version: 0.20.1
+Version: 0.20.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pyarrow >=15
 License-File: LICENSE
 Summary: A package for working with Bioinformatics data with SQL and Arrow
 Author-email: WHERE TRUE devs <thauck+biobear@wheretrue.com>
```

