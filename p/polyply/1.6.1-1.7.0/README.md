# Comparing `tmp/polyply-1.6.1.tar.gz` & `tmp/polyply-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/polyply_1.0/polyply_1.0/dist/.tmp-p6jrbqpp/polyply-1.6.1.tar", last modified: Fri Oct 20 12:03:24 2023, max compression
+gzip compressed data, was "/home/runner/work/polyply_1.0/polyply_1.0/dist/.tmp-csqu5jd7/polyply-1.7.0.tar", last modified: Sat Apr 27 10:36:14 2024, max compression
```

## Comparing `polyply-1.6.1.tar` & `polyply-1.7.0.tar`

### file list

```diff
@@ -1,398 +1,397 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-10-20 12:03:14.000000 polyply-1.6.1/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-10-20 12:03:14.000000 polyply-1.6.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2023-10-20 12:03:14.000000 polyply-1.6.1/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2023-10-20 12:03:14.000000 polyply-1.6.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      734 2023-10-20 12:03:14.000000 polyply-1.6.1/.github/ISSUE_TEMPLATE/parameter-submission.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2023-10-20 12:03:14.000000 polyply-1.6.1/.github/workflows/pypi_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2023-10-20 12:03:14.000000 polyply-1.6.1/.github/workflows/python-app.yml
--rw-r--r--   0 runner    (1001) docker     (127)    16445 2023-10-20 12:03:14.000000 polyply-1.6.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2023-10-20 12:03:14.000000 polyply-1.6.1/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-10-20 12:03:24.000000 polyply-1.6.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-10-20 12:03:24.000000 polyply-1.6.1/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)     5424 2023-10-20 12:03:14.000000 polyply-1.6.1/LIBRARY.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-10-20 12:03:14.000000 polyply-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8225 2023-10-20 12:03:24.000000 polyply-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7240 2023-10-20 12:03:14.000000 polyply-1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:14.000000 polyply-1.6.1/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15634 2023-10-20 12:03:14.000000 polyply-1.6.1/bin/polyply
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/data/2016H66/
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/2016H66/chiral_links.ff
--rw-r--r--   0 runner    (1001) docker     (127)      819 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/2016H66/citation.bib
--rw-r--r--   0 runner    (1001) docker     (127)      718 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/2016H66/polyether_blocks.ff
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/2016H66/polyether_links.ff
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/2016H66/polyether_polyvinyl_links.ff
--rw-r--r--   0 runner    (1001) docker     (127)    10410 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/2016H66/polyvinyl_blocks.ff
--rw-r--r--   0 runner    (1001) docker     (127)     5461 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/2016H66/polyvinyl_links.ff
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/2016H66/terminal_blocks.ff
--rw-r--r--   0 runner    (1001) docker     (127)      586 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/data/gromos53A6/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/gromos53A6/Hter.ff
--rwxr-xr-x   0 runner    (1001) docker     (127)     6644 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/gromos53A6/P3HT.gromos.53A6.ff
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/gromos53A6/citations.bib
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/gromos53A6/links.ff
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/data/ibi_cgm3/
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/ibi_cgm3/PTMA.cgm3.ibi.ff
--rw-r--r--   0 runner    (1001) docker     (127)      718 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/ibi_cgm3/citations.bib
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/data/ibi_gbcg/
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/ibi_gbcg/PTMA.gbno2.ibi.ff
--rw-r--r--   0 runner    (1001) docker     (127)      718 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/ibi_gbcg/citations.bib
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/data/martini2/
--rw-r--r--   0 runner    (1001) docker     (127)    11860 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/martini2/DNA_M2.ff
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/martini2/P3HT.martini.2.itp
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/martini2/PDADMA.martini.2.itp
--rw-r--r--   0 runner    (1001) docker     (127)      392 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/martini2/PE.martini.2.itp
--rw-r--r--   0 runner    (1001) docker     (127)      424 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/martini2/PEO.martini.2.itp
--rw-r--r--   0 runner    (1001) docker     (127)      379 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/martini2/PP.martini.2.itp
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/martini2/PS.martini.2.itp
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/martini2/PSS.martini.2.itp
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/martini2/citations.bib
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/martini2/links.ff
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/data/martini3/
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/martini3/P3HT.martini3.ff
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/martini3/PDMS.martini3.ff
--rw-r--r--   0 runner    (1001) docker     (127)      725 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/martini3/PE.martini3.ff
--rw-r--r--   0 runner    (1001) docker     (127)      391 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/martini3/PEL_link.ff
--rw-r--r--   0 runner    (1001) docker     (127)      896 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/martini3/PEO.martini3.ff
--rw-r--r--   0 runner    (1001) docker     (127)      566 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/martini3/PMA.martini3.ff
--rw-r--r--   0 runner    (1001) docker     (127)      571 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/martini3/PMMA.martini3.ff
--rw-r--r--   0 runner    (1001) docker     (127)     7283 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/martini3/PPE.martini3.ff
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/martini3/PS.martini3.ff
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/martini3/PSS.martini3.ff
--rw-r--r--   0 runner    (1001) docker     (127)      236 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/martini3/PS_PEO_link.ff
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/martini3/PTMA.martini3.ff
--rw-r--r--   0 runner    (1001) docker     (127)      331 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/martini3/PVA.martini3.ff
--rw-r--r--   0 runner    (1001) docker     (127)    16963 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/martini3/aminoacids.ff
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/martini3/cellulose.martini3.ff
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/martini3/citations.bib
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/martini3/dextran.martini3.ff
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/data/martini3_beta/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/martini3_beta/PEO.martini.3.itp
--rw-r--r--   0 runner    (1001) docker     (127)      757 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/martini3_beta/citations.bib
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/data/oplsaaLigParGen/
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/oplsaaLigParGen/CH3.ff
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/oplsaaLigParGen/OHter.ff
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/oplsaaLigParGen/PEO.oplsaa.LigParGen.ff
--rw-r--r--   0 runner    (1001) docker     (127)    18584 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/oplsaaLigParGen/PTMA.oplsaa.LigParGen.ff
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/oplsaaLigParGen/citations.bib
--rw-r--r--   0 runner    (1001) docker     (127)     8031 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/oplsaaLigParGen/links.ff
--rw-r--r--   0 runner    (1001) docker     (127)    12047 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/oplsaaLigParGen/links_PTMA.ff
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/data/parmbsc1/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/parmbsc1/citations.bib
--rw-r--r--   0 runner    (1001) docker     (127)    63766 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/data/parmbsc1/dna_final.ff
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/src/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7949 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/annotate_ligands.py
--rw-r--r--   0 runner    (1001) docker     (127)    20781 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/apply_links.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/apply_modifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     7838 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/backmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    11588 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/build_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8862 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/build_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/check_residue_equivalence.py
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/ff_parser_sub.py
--rw-r--r--   0 runner    (1001) docker     (127)    11338 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/gen_coords.py
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/gen_dna.py
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/gen_itp.py
--rw-r--r--   0 runner    (1001) docker     (127)    12701 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/gen_seq.py
--rw-r--r--   0 runner    (1001) docker     (127)    12692 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/generate_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     7239 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7011 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/linalg_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4893 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/load_library.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    14798 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/map_to_molecule.py
--rw-r--r--   0 runner    (1001) docker     (127)    12749 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/meta_molecule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/minimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14532 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/nonbond_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     7763 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)     7025 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/polyply_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    13080 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/random_walk.py
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/restraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    10528 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/simple_seq_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    19728 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/top_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    19814 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/topology.py
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/src/virtual_site_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/example_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)    10424 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_annotate_lingads.py
--rw-r--r--   0 runner    (1001) docker     (127)    29508 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_apply_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_backmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    13629 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_build_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6909 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_build_system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/ff/
--rw-r--r--   0 runner    (1001) docker     (127)    21928 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/ff/aminoacids.ff
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/ff/unknown_file.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/gen_params/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/gen_params/input/
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_params/input/P3HT.martini.2.itp
--rw-r--r--   0 runner    (1001) docker     (127)      982 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_params/input/PEO.martini.3.itp
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_params/input/PPI.ff
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_params/input/PPI.json
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_params/input/PS.json
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_params/input/PS.martini.2.itp
--rw-r--r--   0 runner    (1001) docker     (127)      919 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_params/input/removal.ff
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_params/input/test.ff
--rw-r--r--   0 runner    (1001) docker     (127)      884 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_params/input/test_edge_attr.ff
--rw-r--r--   0 runner    (1001) docker     (127)      774 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_params/input/test_edge_attr.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/gen_params/logging/
--rw-r--r--   0 runner    (1001) docker     (127)      852 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_params/logging/ERROR_block.ff
--rw-r--r--   0 runner    (1001) docker     (127)      853 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_params/logging/ERROR_link.ff
--rw-r--r--   0 runner    (1001) docker     (127)      850 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_params/logging/INFO_block.ff
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_params/logging/INFO_link.ff
--rw-r--r--   0 runner    (1001) docker     (127)      856 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_params/logging/WARNING_block.ff
--rw-r--r--   0 runner    (1001) docker     (127)      857 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_params/logging/WARNING_link.ff
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/gen_params/ref/
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_params/ref/G3.itp
--rw-r--r--   0 runner    (1001) docker     (127)     8673 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_params/ref/P3HT_10.itp
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_params/ref/PEO_10.itp
--rw-r--r--   0 runner    (1001) docker     (127)     7647 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_params/ref/PS_10.itp
--rw-r--r--   0 runner    (1001) docker     (127)        2 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_params/ref/end.itp
--rw-r--r--   0 runner    (1001) docker     (127)      414 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_params/ref/removal.itp
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_params/ref/test_edge_attr_ref.itp
--rw-r--r--   0 runner    (1001) docker     (127)      860 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_params/ref/test_rev.itp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/gen_seq/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/gen_seq/input/
--rw-r--r--   0 runner    (1001) docker     (127)    47345 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_seq/input/molecule_0.itp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/gen_seq/output/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_seq/output/PEO_PS.json
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_seq/output/PPI.json
--rw-r--r--   0 runner    (1001) docker     (127)   104933 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_seq/output/lysoPEG.json
--rw-r--r--   0 runner    (1001) docker     (127)   104933 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_seq/output/lyso_PEG.json
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_seq/output/rand_PEG_PPO.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/gen_seq/ref/
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_seq/ref/PEO_PS_ref.json
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_seq/ref/PPI_ref.json
--rw-r--r--   0 runner    (1001) docker     (127)    43061 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/gen_seq/ref/lyso_PEG.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/itp/
--rw-r--r--   0 runner    (1001) docker     (127)      808 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/itp/PEO.itp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/json/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/json/double_branch.json
--rw-r--r--   0 runner    (1001) docker     (127)      278 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/json/fail.json
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/json/hyperbranched.json
--rw-r--r--   0 runner    (1001) docker     (127)      264 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/json/linear.json
--rw-r--r--   0 runner    (1001) docker     (127)      264 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/json/linear_rev.json
--rw-r--r--   0 runner    (1001) docker     (127)      421 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/json/single_branch.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/C12E4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/C12E4/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)     7503 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/C12E4/polyply/C12E4.itp
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/C12E4/polyply/command
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PE/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PE/PE.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PE/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PE/polyply/PE.itp
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PE/polyply/command
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PMA/
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PMA/PMA.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PMA/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)     5494 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PMA/polyply/PMA.itp
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PMA/polyply/command
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PP/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PP/PP.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PP/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PP/polyply/PP.itp
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PP/polyply/command
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PS/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PS/PS.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PS/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)    11274 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PS/polyply/PS.itp
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PS/polyply/command
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PVA/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PVA/PVA.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PVA/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PVA/polyply/PVA.itp
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PVA/polyply/command
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/gromos53A6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/gromos53A6/P3HT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/gromos53A6/P3HT/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)    24651 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/gromos53A6/P3HT/polyply/P3HT.itp
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/gromos53A6/P3HT/polyply/command
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/ibi_cgm3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/ibi_cgm3/PTMA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/ibi_cgm3/PTMA/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)     9489 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/ibi_cgm3/PTMA/polyply/PTMA.itp
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/ibi_cgm3/PTMA/polyply/command
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/ibi_gbcg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/ibi_gbcg/PTMA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/ibi_gbcg/PTMA/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)     7618 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/ibi_gbcg/PTMA/polyply/PTMA.itp
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/ibi_gbcg/PTMA/polyply/command
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/PEL/
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/PEL/DPPC.itp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/PEL/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)    18178 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/PEL/polyply/PEL.itp
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/PEL/polyply/command
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/PEO/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/PEO/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)    10694 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/PEO/polyply/PEO.itp
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/PEO/polyply/command
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/PEO_PE/
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/PEO_PE/PEO_PE.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/PEO_PE/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/PEO_PE/polyply/PEO_PE.itp
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/PEO_PE/polyply/command
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/PS/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/PS/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/PS/polyply/PS.itp
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/PS/polyply/command
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/ssDNA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/ssDNA/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/ssDNA/polyply/command
--rw-r--r--   0 runner    (1001) docker     (127)   345908 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/ssDNA/polyply/ssDNA.itp
--rw-r--r--   0 runner    (1001) docker     (127)   203888 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/ssDNA/ssDNA.itp
--rw-r--r--   0 runner    (1001) docker     (127)    13518 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/ssDNA/ssDNA.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/CEL/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/CEL/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)    38643 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/CEL/polyply/CEL.itp
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/CEL/polyply/command
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/DEX/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/DEX/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/DEX/polyply/DEX.itp
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/DEX/polyply/command
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/P3HT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/P3HT/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/P3HT/polyply/P3HT.itp
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/P3HT/polyply/command
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PDMS/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PDMS/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PDMS/polyply/PDMS.itp
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PDMS/polyply/command
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PE/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PE/polyply/PE.itp
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PE/polyply/command
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PEO/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PEO/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PEO/polyply/PEO.itp
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PEO/polyply/command
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PPE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PPE/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)    12458 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PPE/polyply/PPE.itp
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PPE/polyply/command
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PROT/
--rw-r--r--   0 runner    (1001) docker     (127)    24391 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PROT/init.itp
--rw-r--r--   0 runner    (1001) docker     (127)    15988 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PROT/lysozyme_seq.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PROT/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)    28043 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PROT/polyply/PROT.itp
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PROT/polyply/command
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PS/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PS/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PS/polyply/PS.itp
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PS/polyply/command
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PTMA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PTMA/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)     9294 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PTMA/polyply/PTMA.itp
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PTMA/polyply/command
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/oplsaaLigParGen/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/oplsaaLigParGen/PEO/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/oplsaaLigParGen/PEO/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)    20712 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/oplsaaLigParGen/PEO/polyply/PEO.itp
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/oplsaaLigParGen/PEO/polyply/command
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/oplsaaLigParGen/PTMA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/oplsaaLigParGen/PTMA/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)   136964 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/oplsaaLigParGen/PTMA/polyply/PTMA.itp
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/oplsaaLigParGen/PTMA/polyply/command
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/parmbsc1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/parmbsc1/DNA/
--rw-r--r--   0 runner    (1001) docker     (127)   113048 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/parmbsc1/DNA/DNA.itp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/parmbsc1/DNA/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)   205587 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/parmbsc1/DNA/polyply/DNA.itp
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/parmbsc1/DNA/polyply/command
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/parmbsc1/DNA/ref.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/parmbsc1/dsDNA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/parmbsc1/dsDNA/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)   163132 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/parmbsc1/dsDNA/polyply/DNA.itp
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/parmbsc1/dsDNA/polyply/command
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/library_tests/parmbsc1/dsDNA/ref.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/polyply/
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/polyply/P3HT.martini.2.itp
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/polyply/PDADMA.martini.2.itp
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/polyply/PE.martini.2.itp
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/polyply/PEL_lipid.martini.2.itp
--rw-r--r--   0 runner    (1001) docker     (127)      991 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/polyply/PEO.martini.2.itp
--rw-r--r--   0 runner    (1001) docker     (127)      982 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/polyply/PEO.martini.3.itp
--rw-r--r--   0 runner    (1001) docker     (127)      927 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/polyply/PP.martini.2.itp
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/polyply/PS.martini.2.itp
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/polyply/PSS.martini.2.itp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/simple_seq_files/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/simple_seq_files/test.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      115 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/simple_seq_files/test.ig
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/simple_seq_files/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/simple_seq_files/test_RNA.fasta
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/simple_seq_files/test_RNA.ig
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/simple_seq_files/test_circle.ig
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/simple_seq_files/test_fail.ig
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/simple_seq_files/test_ig_warning.ig
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/simple_seq_files/test_protein.fasta
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/struc_build/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/struc_build/PEO.bld
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/struc_build/PEO.itp
--rwxr-xr-x   0 runner    (1001) docker     (127)    65123 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/struc_build/martini_PEO_PS_CNP.itp
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/struc_build/system.top
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply/tests/test_data/topology_test/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/topology_test/W.itp
--rw-r--r--   0 runner    (1001) docker     (127)      317 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/topology_test/cog.gro
--rw-r--r--   0 runner    (1001) docker     (127)      272 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/topology_test/cog_missing.gro
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/topology_test/complete.gro
--rw-r--r--   0 runner    (1001) docker     (127)      636 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/topology_test/fail.gro
--rwxr-xr-x   0 runner    (1001) docker     (127)   405803 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/topology_test/ffnonbonded.itp
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/topology_test/meta.gro
--rw-r--r--   0 runner    (1001) docker     (127)   121974 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/topology_test/molecule_0.itp
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/topology_test/pdb.top
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/topology_test/system.top
--rw-r--r--   0 runner    (1001) docker     (127)      188 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/topology_test/test.bld
--rw-r--r--   0 runner    (1001) docker     (127)      682 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/topology_test/test.gro
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/topology_test/test.itp
--rw-r--r--   0 runner    (1001) docker     (127)    82270 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_data/topology_test/test.pdb
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_ff_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_gen_coords.py
--rw-r--r--   0 runner    (1001) docker     (127)     6461 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_gen_coords_logic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_gen_dna.py
--rw-r--r--   0 runner    (1001) docker     (127)     5447 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_gen_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     8000 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_gen_seq.py
--rw-r--r--   0 runner    (1001) docker     (127)     8203 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_generate_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15757 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_itp_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     8525 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_lib_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_load_library.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    16131 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_map_to_molecule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9387 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_meta_molecule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9560 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_nb_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    11479 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_optimize_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    11766 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)     6618 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_polyply_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    12362 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_random_walk.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_residue_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_restraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     5539 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_simple_seq_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14543 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_top_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    26364 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_topology.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2023-10-20 12:03:14.000000 polyply-1.6.1/polyply/tests/test_vs_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8225 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13394 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)       75 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-20 12:03:24.000000 polyply-1.6.1/polyply.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-10-20 12:03:14.000000 polyply-1.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-10-20 12:03:14.000000 polyply-1.6.1/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-10-20 12:03:14.000000 polyply-1.6.1/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2023-10-20 12:03:14.000000 polyply-1.6.1/run_pylint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2023-10-20 12:03:24.000000 polyply-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2023-10-20 12:03:14.000000 polyply-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-27 10:36:09.000000 polyply-1.7.0/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-27 10:36:09.000000 polyply-1.7.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-27 10:36:09.000000 polyply-1.7.0/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-27 10:36:09.000000 polyply-1.7.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-27 10:36:09.000000 polyply-1.7.0/.github/ISSUE_TEMPLATE/parameter-submission.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-27 10:36:09.000000 polyply-1.7.0/.github/workflows/pypi_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-27 10:36:09.000000 polyply-1.7.0/.github/workflows/python-app.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    16445 2024-04-27 10:36:09.000000 polyply-1.7.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-27 10:36:09.000000 polyply-1.7.0/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-27 10:36:13.000000 polyply-1.7.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-27 10:36:13.000000 polyply-1.7.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-04-27 10:36:09.000000 polyply-1.7.0/LIBRARY.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-27 10:36:09.000000 polyply-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8225 2024-04-27 10:36:14.000000 polyply-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-04-27 10:36:09.000000 polyply-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:09.000000 polyply-1.7.0/bin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15634 2024-04-27 10:36:09.000000 polyply-1.7.0/bin/polyply
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/data/2016H66/
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/2016H66/chiral_links.ff
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/2016H66/citation.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/2016H66/polyether_blocks.ff
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/2016H66/polyether_links.ff
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/2016H66/polyether_polyvinyl_links.ff
+-rw-r--r--   0 runner    (1001) docker     (127)    10410 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/2016H66/polyvinyl_blocks.ff
+-rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/2016H66/polyvinyl_links.ff
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/2016H66/terminal_blocks.ff
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/data/gromos53A6/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/gromos53A6/Hter.ff
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6644 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/gromos53A6/P3HT.gromos.53A6.ff
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/gromos53A6/citations.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/gromos53A6/links.ff
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/data/ibi_cgm3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/ibi_cgm3/PTMA.cgm3.ibi.ff
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/ibi_cgm3/citations.bib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/data/ibi_gbcg/
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/ibi_gbcg/PTMA.gbno2.ibi.ff
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/ibi_gbcg/citations.bib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/data/martini2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11860 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/martini2/DNA_M2.ff
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/martini2/P3HT.martini.2.itp
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/martini2/PDADMA.martini.2.itp
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/martini2/PE.martini.2.itp
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/martini2/PEO.martini.2.itp
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/martini2/PP.martini.2.itp
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/martini2/PS.martini.2.itp
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/martini2/PSS.martini.2.itp
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/martini2/citations.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/martini2/links.ff
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/data/martini3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/martini3/P3HT.martini3.ff
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/martini3/PDMS.martini3.ff
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/martini3/PE.martini3.ff
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/martini3/PEL_link.ff
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/martini3/PEO.martini3.ff
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/martini3/PMA.martini3.ff
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/martini3/PMMA.martini3.ff
+-rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/martini3/PPE.martini3.ff
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/martini3/PS.martini3.ff
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/martini3/PSS.martini3.ff
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/martini3/PS_PEO_link.ff
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/martini3/PTMA.martini3.ff
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/martini3/PVA.martini3.ff
+-rw-r--r--   0 runner    (1001) docker     (127)    21481 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/martini3/aminoacids.ff
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/martini3/cellulose.martini3.ff
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/martini3/citations.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/martini3/dextran.martini3.ff
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/data/martini3_beta/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/martini3_beta/PEO.martini.3.itp
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/martini3_beta/citations.bib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/data/oplsaaLigParGen/
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/oplsaaLigParGen/CH3.ff
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/oplsaaLigParGen/OHter.ff
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/oplsaaLigParGen/PEO.oplsaa.LigParGen.ff
+-rw-r--r--   0 runner    (1001) docker     (127)    18584 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/oplsaaLigParGen/PTMA.oplsaa.LigParGen.ff
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/oplsaaLigParGen/citations.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     8031 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/oplsaaLigParGen/links.ff
+-rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/oplsaaLigParGen/links_PTMA.ff
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/data/parmbsc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/parmbsc1/citations.bib
+-rw-r--r--   0 runner    (1001) docker     (127)    63766 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/data/parmbsc1/dna_final.ff
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/annotate_ligands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20781 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/apply_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/apply_modifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/backmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11907 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/build_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/build_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/check_residue_equivalence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/ff_parser_sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/gen_coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/gen_dna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/gen_itp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12701 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/gen_seq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12880 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/generate_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/linalg_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/load_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14798 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/map_to_molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12749 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/meta_molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7073 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/minimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16481 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/nonbond_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7763 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/polyply_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14862 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/random_walk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/restraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10528 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/simple_seq_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19728 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/top_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19977 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/src/virtual_site_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/example_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_annotate_lingads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29508 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_apply_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_backmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13629 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_build_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6909 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_build_system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/ff/
+-rw-r--r--   0 runner    (1001) docker     (127)    21928 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/ff/aminoacids.ff
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/ff/unknown_file.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply/tests/test_data/gen_params/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/gen_params/input/
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_params/input/P3HT.martini.2.itp
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_params/input/PEO.martini.3.itp
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_params/input/PPI.ff
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_params/input/PPI.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_params/input/PS.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_params/input/PS.martini.2.itp
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_params/input/removal.ff
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_params/input/test.ff
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_params/input/test_edge_attr.ff
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_params/input/test_edge_attr.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/gen_params/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_params/logging/ERROR_block.ff
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_params/logging/ERROR_link.ff
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_params/logging/INFO_block.ff
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_params/logging/INFO_link.ff
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_params/logging/WARNING_block.ff
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_params/logging/WARNING_link.ff
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/gen_params/ref/
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_params/ref/G3.itp
+-rw-r--r--   0 runner    (1001) docker     (127)     8673 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_params/ref/P3HT_10.itp
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_params/ref/PEO_10.itp
+-rw-r--r--   0 runner    (1001) docker     (127)     7647 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_params/ref/PS_10.itp
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_params/ref/end.itp
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_params/ref/removal.itp
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_params/ref/test_edge_attr_ref.itp
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_params/ref/test_rev.itp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply/tests/test_data/gen_seq/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/gen_seq/input/
+-rw-r--r--   0 runner    (1001) docker     (127)    47345 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_seq/input/molecule_0.itp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/gen_seq/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_seq/output/PEO_PS.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_seq/output/PPI.json
+-rw-r--r--   0 runner    (1001) docker     (127)   104933 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_seq/output/lysoPEG.json
+-rw-r--r--   0 runner    (1001) docker     (127)   104933 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_seq/output/lyso_PEG.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_seq/output/rand_PEG_PPO.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/gen_seq/ref/
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_seq/ref/PEO_PS_ref.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_seq/ref/PPI_ref.json
+-rw-r--r--   0 runner    (1001) docker     (127)    43061 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/gen_seq/ref/lyso_PEG.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/itp/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/itp/PEO.itp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/json/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/json/double_branch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/json/fail.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/json/hyperbranched.json
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/json/linear.json
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/json/linear_rev.json
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/json/single_branch.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/C12E4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/C12E4/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/C12E4/polyply/C12E4.itp
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/C12E4/polyply/command
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PE/PE.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PE/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PE/polyply/PE.itp
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PE/polyply/command
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PMA/
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PMA/PMA.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PMA/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PMA/polyply/PMA.itp
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PMA/polyply/command
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PP/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PP/PP.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PP/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PP/polyply/PP.itp
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PP/polyply/command
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PS/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PS/PS.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PS/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)    11274 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PS/polyply/PS.itp
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PS/polyply/command
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PVA/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PVA/PVA.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PVA/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PVA/polyply/PVA.itp
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PVA/polyply/command
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/gromos53A6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/gromos53A6/P3HT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/gromos53A6/P3HT/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)    24651 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/gromos53A6/P3HT/polyply/P3HT.itp
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/gromos53A6/P3HT/polyply/command
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/ibi_cgm3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/ibi_cgm3/PTMA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/ibi_cgm3/PTMA/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/ibi_cgm3/PTMA/polyply/PTMA.itp
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/ibi_cgm3/PTMA/polyply/command
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/ibi_gbcg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/ibi_gbcg/PTMA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/ibi_gbcg/PTMA/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/ibi_gbcg/PTMA/polyply/PTMA.itp
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/ibi_gbcg/PTMA/polyply/command
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/PEL/
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/PEL/DPPC.itp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/PEL/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)    18178 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/PEL/polyply/PEL.itp
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/PEL/polyply/command
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/PEO/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/PEO/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)    10694 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/PEO/polyply/PEO.itp
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/PEO/polyply/command
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/PEO_PE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/PEO_PE/PEO_PE.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/PEO_PE/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/PEO_PE/polyply/PEO_PE.itp
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/PEO_PE/polyply/command
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/PS/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/PS/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/PS/polyply/PS.itp
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/PS/polyply/command
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/ssDNA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/ssDNA/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/ssDNA/polyply/command
+-rw-r--r--   0 runner    (1001) docker     (127)   345908 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/ssDNA/polyply/ssDNA.itp
+-rw-r--r--   0 runner    (1001) docker     (127)   203888 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/ssDNA/ssDNA.itp
+-rw-r--r--   0 runner    (1001) docker     (127)    13518 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/ssDNA/ssDNA.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/CEL/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/CEL/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)    38643 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/CEL/polyply/CEL.itp
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/CEL/polyply/command
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/DEX/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/DEX/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/DEX/polyply/DEX.itp
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/DEX/polyply/command
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/P3HT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/P3HT/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/P3HT/polyply/P3HT.itp
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/P3HT/polyply/command
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PDMS/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PDMS/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PDMS/polyply/PDMS.itp
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PDMS/polyply/command
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PE/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PE/polyply/PE.itp
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PE/polyply/command
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PEO/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PEO/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PEO/polyply/PEO.itp
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PEO/polyply/command
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PPE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PPE/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)    12458 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PPE/polyply/PPE.itp
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PPE/polyply/command
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PROT/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PROT/PNt.fasta
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PROT/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)   169940 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PROT/polyply/PROT.itp
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PROT/polyply/command
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PS/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PS/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PS/polyply/PS.itp
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PS/polyply/command
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PTMA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PTMA/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PTMA/polyply/PTMA.itp
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PTMA/polyply/command
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/oplsaaLigParGen/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/oplsaaLigParGen/PEO/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/oplsaaLigParGen/PEO/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)    20712 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/oplsaaLigParGen/PEO/polyply/PEO.itp
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/oplsaaLigParGen/PEO/polyply/command
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/oplsaaLigParGen/PTMA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/oplsaaLigParGen/PTMA/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)   136964 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/oplsaaLigParGen/PTMA/polyply/PTMA.itp
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/oplsaaLigParGen/PTMA/polyply/command
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/parmbsc1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/parmbsc1/DNA/
+-rw-r--r--   0 runner    (1001) docker     (127)   113048 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/parmbsc1/DNA/DNA.itp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/parmbsc1/DNA/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)   205587 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/parmbsc1/DNA/polyply/DNA.itp
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/parmbsc1/DNA/polyply/command
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/parmbsc1/DNA/ref.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/parmbsc1/dsDNA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/parmbsc1/dsDNA/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)   163132 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/parmbsc1/dsDNA/polyply/DNA.itp
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/parmbsc1/dsDNA/polyply/command
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/library_tests/parmbsc1/dsDNA/ref.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/polyply/
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/polyply/P3HT.martini.2.itp
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/polyply/PDADMA.martini.2.itp
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/polyply/PE.martini.2.itp
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/polyply/PEL_lipid.martini.2.itp
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/polyply/PEO.martini.2.itp
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/polyply/PEO.martini.3.itp
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/polyply/PP.martini.2.itp
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/polyply/PS.martini.2.itp
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/polyply/PSS.martini.2.itp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/simple_seq_files/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/simple_seq_files/test.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/simple_seq_files/test.ig
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/simple_seq_files/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/simple_seq_files/test_RNA.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/simple_seq_files/test_RNA.ig
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/simple_seq_files/test_circle.ig
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/simple_seq_files/test_fail.ig
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/simple_seq_files/test_ig_warning.ig
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/simple_seq_files/test_protein.fasta
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/struc_build/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/struc_build/PEO.bld
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/struc_build/PEO.itp
+-rwxr-xr-x   0 runner    (1001) docker     (127)    65123 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/struc_build/martini_PEO_PS_CNP.itp
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/struc_build/system.top
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply/tests/test_data/topology_test/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/topology_test/W.itp
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/topology_test/cog.gro
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/topology_test/cog_missing.gro
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/topology_test/complete.gro
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/topology_test/fail.gro
+-rwxr-xr-x   0 runner    (1001) docker     (127)   405803 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/topology_test/ffnonbonded.itp
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/topology_test/meta.gro
+-rw-r--r--   0 runner    (1001) docker     (127)   121974 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/topology_test/molecule_0.itp
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/topology_test/pdb.top
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/topology_test/system.top
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/topology_test/test.bld
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/topology_test/test.gro
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/topology_test/test.itp
+-rw-r--r--   0 runner    (1001) docker     (127)    82270 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_data/topology_test/test.pdb
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_ff_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_gen_coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_gen_coords_logic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_gen_dna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_gen_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8000 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_gen_seq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9520 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_generate_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15757 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_itp_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8525 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_lib_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_load_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16131 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_map_to_molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_meta_molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10998 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_nb_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11479 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_optimize_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11766 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_polyply_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13572 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_random_walk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_residue_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_restraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_simple_seq_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14543 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_top_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26364 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-27 10:36:09.000000 polyply-1.7.0/polyply/tests/test_vs_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:36:14.000000 polyply-1.7.0/polyply.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8225 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13325 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-27 10:36:13.000000 polyply-1.7.0/polyply.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-27 10:36:09.000000 polyply-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-27 10:36:09.000000 polyply-1.7.0/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-27 10:36:09.000000 polyply-1.7.0/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-27 10:36:09.000000 polyply-1.7.0/run_pylint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-27 10:36:14.000000 polyply-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-27 10:36:09.000000 polyply-1.7.0/setup.py
```

### Comparing `polyply-1.6.1/.github/CONTRIBUTING.md` & `polyply-1.7.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/.github/ISSUE_TEMPLATE/bug_report.md` & `polyply-1.7.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/.github/ISSUE_TEMPLATE/parameter-submission.md` & `polyply-1.7.0/.github/ISSUE_TEMPLATE/parameter-submission.md`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/.github/workflows/pypi_deploy.yml` & `polyply-1.7.0/.github/workflows/pypi_deploy.yml`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/.github/workflows/python-app.yml` & `polyply-1.7.0/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/.pylintrc` & `polyply-1.7.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/.travis.yml` & `polyply-1.7.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/LIBRARY.md` & `polyply-1.7.0/LIBRARY.md`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/LICENSE` & `polyply-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/PKG-INFO` & `polyply-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyply
-Version: 1.6.1
+Version: 1.7.0
 Home-page: https://github.com/marrink-lab/polyply_1.0
 Author: Fabian Grunewald
 Author-email: f.grunewald@rug.nl
 License: Apache 2.0
 Keywords: molecular dynamics charmm gromos martini polymers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `polyply-1.6.1/README.md` & `polyply-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/bin/polyply` & `polyply-1.7.0/bin/polyply`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/__init__.py` & `polyply-1.7.0/polyply/__init__.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/2016H66/chiral_links.ff` & `polyply-1.7.0/polyply/data/2016H66/chiral_links.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/2016H66/citation.bib` & `polyply-1.7.0/polyply/data/2016H66/citation.bib`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/2016H66/polyether_blocks.ff` & `polyply-1.7.0/polyply/data/2016H66/polyether_blocks.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/2016H66/polyether_links.ff` & `polyply-1.7.0/polyply/data/2016H66/polyether_links.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/2016H66/polyether_polyvinyl_links.ff` & `polyply-1.7.0/polyply/data/2016H66/polyether_polyvinyl_links.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/2016H66/polyvinyl_blocks.ff` & `polyply-1.7.0/polyply/data/2016H66/polyvinyl_blocks.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/2016H66/polyvinyl_links.ff` & `polyply-1.7.0/polyply/data/2016H66/polyvinyl_links.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/__init__.py` & `polyply-1.7.0/polyply/data/__init__.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/gromos53A6/P3HT.gromos.53A6.ff` & `polyply-1.7.0/polyply/data/gromos53A6/P3HT.gromos.53A6.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/gromos53A6/citations.bib` & `polyply-1.7.0/polyply/data/gromos53A6/citations.bib`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/gromos53A6/links.ff` & `polyply-1.7.0/polyply/data/gromos53A6/links.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/ibi_cgm3/PTMA.cgm3.ibi.ff` & `polyply-1.7.0/polyply/data/ibi_cgm3/PTMA.cgm3.ibi.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/ibi_cgm3/citations.bib` & `polyply-1.7.0/polyply/data/ibi_cgm3/citations.bib`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/ibi_gbcg/PTMA.gbno2.ibi.ff` & `polyply-1.7.0/polyply/data/ibi_gbcg/PTMA.gbno2.ibi.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/ibi_gbcg/citations.bib` & `polyply-1.7.0/polyply/data/ibi_gbcg/citations.bib`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/martini2/DNA_M2.ff` & `polyply-1.7.0/polyply/data/martini2/DNA_M2.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/martini2/P3HT.martini.2.itp` & `polyply-1.7.0/polyply/data/martini2/P3HT.martini.2.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/martini2/PDADMA.martini.2.itp` & `polyply-1.7.0/polyply/data/martini2/PDADMA.martini.2.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/martini2/PS.martini.2.itp` & `polyply-1.7.0/polyply/data/martini2/PS.martini.2.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/martini2/PSS.martini.2.itp` & `polyply-1.7.0/polyply/data/martini2/PSS.martini.2.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/martini2/citations.bib` & `polyply-1.7.0/polyply/data/martini2/citations.bib`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/martini2/links.ff` & `polyply-1.7.0/polyply/data/martini2/links.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/martini3/P3HT.martini3.ff` & `polyply-1.7.0/polyply/data/martini3/P3HT.martini3.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/martini3/PDMS.martini3.ff` & `polyply-1.7.0/polyply/data/martini3/PDMS.martini3.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/martini3/PE.martini3.ff` & `polyply-1.7.0/polyply/data/martini3/PE.martini3.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/martini3/PEO.martini3.ff` & `polyply-1.7.0/polyply/data/martini3/PEO.martini3.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/martini3/PMA.martini3.ff` & `polyply-1.7.0/polyply/data/martini3/PMA.martini3.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/martini3/PMMA.martini3.ff` & `polyply-1.7.0/polyply/data/martini3/PMMA.martini3.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/martini3/PPE.martini3.ff` & `polyply-1.7.0/polyply/data/martini3/PPE.martini3.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/martini3/PS.martini3.ff` & `polyply-1.7.0/polyply/data/martini3/PS.martini3.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/martini3/PSS.martini3.ff` & `polyply-1.7.0/polyply/data/martini3/PSS.martini3.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/martini3/PTMA.martini3.ff` & `polyply-1.7.0/polyply/data/martini3/PTMA.martini3.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/martini3/aminoacids.ff` & `polyply-1.7.0/polyply/data/martini3/aminoacids.ff`

 * *Files 24% similar despite different names*

```diff
@@ -21,325 +21,430 @@
 [ variables ]
 elastic_network_bond_type 1
 res_min_dist 3
 
 [ citations ]
 Martini3
 polyply
+M3_GO
 
 ;;; GLYCINE
 
 [ moleculetype ]
 ; molname       nrexcl
 GLY                1			
 
 [ atoms ]
-;id  type resnr residu atom cgnr   charge
+;id  type resnr residu atom cgnr   charge mass
  1   SP1   1     GLY    BB     1      0      
+ 2    VS   1     GLY    CA     1      0   0
+[ position_restraints ]
+1  1  1 1000 1000 1000 {"ifdef": "POSRES"}
+[ virtual_sitesn ]
+2 1 -- 1
 
 ;;; ALANINE
 
 [ moleculetype ]
 ; molname       nrexcl
 ALA                1
 
 [ atoms ]
 ;id type resnr residu atom cgnr   charge
  1   SP2    1   ALA    BB     1      0
- 2   TC3    1   ALA    SC1    2      0 
+ 2   TC3    1   ALA    SC1    1      0 
+ 3    VS    1   ALA    CA     1      0   0
+[ virtual_sitesn ]
+3 1 -- 1
 
 [ constraints ]
 #meta {"group": "Side chain bonds", "ifndef": "FLEXIBLE"}
 ;  i     j   funct   length  
   BB   SC1    1       0.270
 
 [ bonds ]
 #meta {"group": "Side chain bonds", "ifdef": "FLEXIBLE"}   
 ;  i     j   funct   length  
 BB   SC1    1       0.270  $stiff_fc
+[ position_restraints ]
+1  1  1 1000 1000 1000 {"ifdef": "POSRES"}
 
 ;;; CYSTEINE
 
 [ moleculetype ]
 ; molname       nrexcl
 CYS                1
 
 [ atoms ]
 ;id type resnr residu atom cgnr   charge
  1   $prot_default_bb_type     1   CYS    BB     1      0
- 2   TC6    1   CYS    SC1    2      0     
+ 2   TC6    1   CYS    SC1     1      0     
+ 3    VS    1   CYS    CA      1      0   0
+[ virtual_sitesn ]
+3 1 -- 1
 
 [bonds]
 #meta {"group": "Side chain bonds"}
 ;  i     j   funct   length  force.c.
   BB   SC1    1       0.341     7500        
+[ position_restraints ]
+1  1  1 1000 1000 1000 {"ifdef": "POSRES"}
 
 ;;; VALINE
 
 [ moleculetype ]
 ; molname       nrexcl
 VAL                1
 
 [ atoms ]
 ;id type resnr residu atom cgnr   charge
  1   SP2  1     VAL     BB     1      0    
- 2   SC3  1     VAL     SC1    2      0    
+ 2   SC3  1     VAL     SC1    1      0    
+ 3    VS  1     VAL     CA     1      0   0
+[ virtual_sitesn ]
+3 1 -- 1
 
 [ constraints ]
 #meta {"group": "Side chain bonds", "ifndef": "FLEXIBLE"}
 ;  i     j   funct   length  
   BB   SC1    1       0.292
 
 [ bonds ]
 #meta {"group": "Side chain bonds", "ifdef": "FLEXIBLE"}
 ;  i     j   funct   length  
   BB   SC1    1       0.292  $stiff_fc
 
+[ position_restraints ]
+1  1  1 1000 1000 1000 {"ifdef": "POSRES"}
+
 ;;; LEUCINE
 
 [ moleculetype ]
 ; molname       nrexcl
 LEU                1
 
 [ atoms ]
 ;id type resnr residu atom cgnr   charge
  1   $prot_default_bb_type   1     LEU     BB     1      0    
- 2   SC2  1     LEU     SC1    2      0    
+ 2   SC2  1     LEU     SC1    1      0    
+ 3    VS  1     LEU     CA     1      0   0
+[ virtual_sitesn ]
+3 1 -- 1
 
 [bonds]
 #meta {"group": "Side chain bonds"}
 ;  i     j   funct   length  force.c.
   BB   SC1    1       0.363     7500    
 
+[ position_restraints ]
+1  1  1 1000 1000 1000 {"ifdef": "POSRES"}
+
 ;;; ISOLEUCINE
 
 [ moleculetype ]
 ; molname       nrexcl
 ILE                1
 
 [ atoms ]
 ;id type resnr residu atom cgnr   charge
  1   $prot_default_bb_type   1     ILE     BB     1      0    
- 2   SC2  1     ILE     SC1    2      0    
+ 2   SC2  1     ILE     SC1    1      0    
+ 3    VS  1     ILE     CA     1      0   0
+[ virtual_sitesn ]
+3 1 -- 1
 
 [ constraints ]
 #meta {"group": "Side chain bonds", "ifndef": "FLEXIBLE"}
 ;  i     j   funct   length  
   BB   SC1    1       0.341
 
 [ bonds ]
 #meta {"group": "Side chain bonds", "ifdef": "FLEXIBLE"}
 ;  i     j   funct   length  
   BB   SC1    1       0.341  $stiff_fc
 
+[ position_restraints ]
+1  1  1 1000 1000 1000 {"ifdef": "POSRES"}
+
 ;;; METHIONINE
 
 [ moleculetype ]
 ; molname       nrexcl
 MET                1
 
 [ atoms ]
 ;id type resnr residu atom cgnr   charge
  1   $prot_default_bb_type   1     MET     BB     1      0    
- 2   C6   1     MET     SC1    2      0     
+ 2   C6   1     MET     SC1    1      0     
+ 3    VS  1     MET     CA     1      0   0
+[ virtual_sitesn ]
+3 1 -- 1
 
 [bonds]
 #meta {"group": "Side chain bonds"}
 ;  i     j   funct   length  force.c.
   BB   SC1    1       0.40     2500
 
+[ position_restraints ]
+1  1  1 1000 1000 1000 {"ifdef": "POSRES"}
+
 ;;; PROLINE
 
 [ moleculetype ]
 ; molname       nrexcl
 PRO                1
 
 [ atoms ]
 ;id type resnr residu atom cgnr   charge
  1   SP2a   1     PRO     BB     1      0    
- 2   SC3    1     PRO     SC1    2      0    
+ 2   SC3    1     PRO     SC1    1      0    
+ 3    VS    1     PRO     CA     1      0   0
+[ virtual_sitesn ]
+3 1 -- 1
+
 
 [bonds]
 #meta {"group": "Side chain bonds"}
 ;  i     j   funct   length  force.c.
   BB   SC1   1       0.330     7500
 
+[ position_restraints ]
+1  1  1 1000 1000 1000 {"ifdef": "POSRES"}
+
 [ moleculetype ]
 ; molname       nrexcl
 HYP                1
 
 [ atoms ]
 ;id type resnr residu atom cgnr   charge
  1    P1   1     HYP     BB     1      0    
- 2    P1   1     HYP     SC1    2      0    
+ 2    P1   1     HYP     SC1    1      0    
+ 3    VS   1     HYP     CA     1      0   0
+[ virtual_sitesn ]
+3 1 -- 1
+
 
 [bonds]
 #meta {"group": "Side chain bonds"}
 ;  i     j   funct   length  force.c.
   BB   SC1   1       0.300     7500
 
+[ position_restraints ]
+1  1  1 1000 1000 1000 {"ifdef": "POSRES"}
+
 ;;; ASPARAGINE
 
 [ moleculetype ]
 ; molname       nrexcl
 ASN                1
 
 [ atoms ]
 ;id type resnr residu atom cgnr   charge
  1   $prot_default_bb_type    1     ASN     BB     1      0    
- 2   SP5    1     ASN     SC1    2      0    
+ 2   SP5    1     ASN     SC1    1      0    
+ 3    VS    1     ASN     CA     1      0   0
+[ virtual_sitesn ]
+3 1 -- 1
 
 [bonds]
 #meta {"group": "Side chain bonds"}
 ;  i     j   funct   length  force.c.
   BB   SC1    1       0.352     5000
 
+[ position_restraints ]
+1  1  1 1000 1000 1000 {"ifdef": "POSRES"}
+
 ;;; GLUTAMINE
 
 [ moleculetype ]
 ; molname       nrexcl
 GLN                1
 
 [ atoms ]
 ;id type resnr residu atom cgnr   charge
  1   $prot_default_bb_type    1     GLN     BB     1      0    
- 2   P5    1     GLN     SC1    2      0    
+ 2   P5     1     GLN     SC1    1      0    
+ 3   VS     1     GLN     CA     1      0   0
+[ virtual_sitesn ]
+3 1 -- 1
 
 [bonds]
 #meta {"group": "Side chain bonds"}
 ;  i     j   funct   length  force.c.
   BB   SC1    1       0.400    5000     
 
+[ position_restraints ]
+1  1  1 1000 1000 1000 {"ifdef": "POSRES"}
+
 ;;; ASPARTATE
 
 [ moleculetype ]
 ; molname       nrexcl
 ASP                1
 
 [ atoms ]
 ;id type resnr residu atom cgnr   charge
  1   $prot_default_bb_type     1     ASP     BB     1      0    
- 2   SQ5n    1     ASP     SC1    2   -1.0    
+ 2   SQ5n    1     ASP     SC1    1   -1.0    
+ 3   VS      1     ASP     CA     1      0   0
+[ virtual_sitesn ]
+3 1 -- 1
 
 [bonds]
 #meta {"group": "Side chain bonds"}
 ;  i     j   funct   length  force.c.
   BB   SC1    1       0.352     7500
 
+[ position_restraints ]
+1  1  1 1000 1000 1000 {"ifdef": "POSRES"}
+
 ;;; GLUTAMATE
 
 [ moleculetype ]
 ; molname       nrexcl
 GLU                1
 
 [ atoms ]
 ;id type resnr residu atom cgnr   charge
  1   $prot_default_bb_type     1     GLU     BB     1      0    
- 2   Q5n    1     GLU     SC1    2   -1.0    
+ 2   Q5n    1     GLU     SC1    1   -1.0    
+ 3   VS     1     GLU     CA     1      0   0
+[ virtual_sitesn ]
+3 1 -- 1
 
 [bonds]
 #meta {"group": "Side chain bonds"}
 ;  i     j   funct   length  force.c.
   BB   SC1    1       0.400    5000     
 
+[ position_restraints ]
+1  1  1 1000 1000 1000 {"ifdef": "POSRES"}
+
 ;;; THREONINE
 
 [ moleculetype ]
 ; molname       nrexcl
 THR                1
 
 [ atoms ]
 ;id type resnr residu atom cgnr   charge
 1   $prot_default_bb_type     1     THR     BB     1      0    
-2   SP1     1     THR     SC1    2      0    
+2   SP1     1     THR     SC1    1      0    
+3   VS      1     THR     CA     1      0   0
+[ virtual_sitesn ]
+3 1 -- 1
 
 [ constraints ]
 #meta {"group": "Side chain bonds", "ifndef": "FLEXIBLE"}
 ;  i     j   funct   length (Modified by Paulo)
   BB   SC1    1       0.305
 
 [ bonds ]
 #meta {"group": "Side chain bonds", "ifdef": "FLEXIBLE"}
 ;  i     j   funct   length 
   BB   SC1    1       0.305  $stiff_fc
 
+[ position_restraints ]
+1  1  1 1000 1000 1000 {"ifdef": "POSRES"}
+
 ;;; SERINE
 
 [ moleculetype ]
 ; molname       nrexcl
 SER                1
 
 [ atoms ]
 ;id type resnr residu atom cgnr   charge
 1   $prot_default_bb_type     1    SER     BB     1      0    
-2   TP1     1    SER     SC1    2      0    
+2   TP1     1    SER     SC1    1      0    
+3   VS      1    SER     CA     1      0   0
+[ virtual_sitesn ]
+3 1 -- 1
 
 [bonds]
 #meta {"group": "Side chain bonds"}
 ;  i     j   funct   length  force.c.
   BB   SC1    1       0.287     7500
 
+[ position_restraints ]
+1  1  1 1000 1000 1000 {"ifdef": "POSRES"}
+
 ;;; LYSINE 
 
 [ moleculetype ]
 ; molname       nrexcl
 LYS                1
 
 [ atoms ]
 ;id type resnr residu atom cgnr   charge
  1   $prot_default_bb_type    1     LYS     BB     1      0    
- 2   SC3    1     LYS     SC1    2      0    
- 3   SQ4p   1     LYS     SC2    3    1.0    
+ 2   SC3    1     LYS     SC1    1      0    
+ 3   SQ4p   1     LYS     SC2    1    1.0    
+ 4   VS     1     LYS     CA     1      0   0
+[ virtual_sitesn ]
+4 1 -- 1
 
 [bonds]
 #meta {"group": "Side chain bonds"}
 ;  i     j   funct   length  force.c.
   BB   SC1    1       0.330     5000      
  SC1   SC2    1       0.360     5000  
 
 [angles]
 #meta {"group": "Side chain angles"}
 ;  i     j    k     funct   angle  force.c.
   BB   SC1  SC2       2   180.000    25.0      
 
+[ position_restraints ]
+1  1  1 1000 1000 1000 {"ifdef": "POSRES"}
+
 ;;; ARGININE 
 
 [ moleculetype ]
 ; molname       nrexcl
 ARG                1
 
 [ atoms ]
 ;id type resnr residu atom cgnr   charge
 1   $prot_default_bb_type     1     ARG     BB     1      0    
-2   SC3      1     ARG     SC1    2      0    
-3   SQ3p     1     ARG     SC2    3    1.0    
+2   SC3      1     ARG     SC1    1      0    
+3   SQ3p     1     ARG     SC2    1    1.0    
+4   VS       1     ARG     CA     1      0   0
+[ virtual_sitesn ]
+4 1 -- 1
 
 [bonds]
 #meta {"group": "Side chain bonds"}
 ;  i     j   funct   length  force.c.
   BB   SC1    1       0.330     5000   
  SC1   SC2    1       0.380     5000  
 
 [angles]
 #meta {"group": "Side chain angles"}
 ;  i     j    k     funct   angle  force.c.
   BB   SC1  SC2       2   180.000    25.0      
 
+[ position_restraints ]
+1  1  1 1000 1000 1000 {"ifdef": "POSRES"}
+
 ;;; HISTIDINE 
 
 [ moleculetype ]
 ;molname       nrexcl
 HIS                1
 
 [ atoms ]
 ;id type resnr residu atom cgnr   charge
 1   $prot_default_bb_type     1     HIS     BB     1      0    
-2   TC4     1     HIS     SC1    2    0    ; three side chains in triangle
-3   TN6d    1     HIS     SC2    3    0    ; configuration, mimicking
-4   TN5a    1     HIS     SC3    4    0    ; ring structure
+2   TC4     1     HIS     SC1    1    0    ; three side chains in triangle
+3   TN6d    1     HIS     SC2    1    0    ; configuration, mimicking
+4   TN5a    1     HIS     SC3    1    0    ; ring structure
+5   VS      1     HIS     CA     1      0   0
+[ virtual_sitesn ]
+5 1 -- 1
 
 [ bonds ]
 #meta {"group": "Side chain bonds"}
 ;  i     j   funct   length  force.c.
   BB   SC1    1       0.336     7500 
 #meta {"group": "Side chain bonds", "ifdef": "FLEXIBLE"}
 ;  i     j   funct   length  
@@ -366,27 +471,34 @@
 
 [exclusions]
 ; We do not want non-bounded interactions within the residue.
 BB SC1 SC2 SC3
 SC1 SC2 SC3
 SC2 SC3
 
+[ position_restraints ]
+1  1  1 1000 1000 1000 {"ifdef": "POSRES"}
+
 [ moleculetype ]
 ;molname       nrexcl
 HIH                1
 
 [ atoms ]
 ;id type resnr residu atom cgnr   charge
 1   $prot_default_bb_type     1     HIS     BB     1      0    
 2   TC4     1     HIH     SC1    2    0      ; three side chains in triangle
 3   TN6d    1     HIH     SC2    3    0      ; configuration, mimicking
 4   TQ2p    1     HIH     SC3    4    1      ; ring structure
 ;2   TC4     1     HIH     SC1    2    0      ; three side chains in triangle 
 ;3   TP3dq   1     HIH     SC2    3   +0.5    ; modelB
 ;4   TP3dq   1     HIH     SC3    4   +0.5    ; 
+5   VS      1     HIH     CA     1      0   0
+[ virtual_sitesn ]
+5 1 -- 1
+
 
 [bonds]
 #meta {"group": "Side chain bonds"}
 ;  i     j   funct   length  force.c.
   BB   SC1    1       0.336     7500 
 #meta {"group": "Side chain bonds", "ifdef": "FLEXIBLE"}
 ;  i     j   funct   length  
@@ -413,26 +525,32 @@
 
 [exclusions]
 ; We do not want non-bounded interactions within the residue.
 BB SC1 SC2 SC3
 SC1 SC2 SC3
 SC2 SC3
 
+[ position_restraints ]
+1  1  1 1000 1000 1000 {"ifdef": "POSRES"}
+
 ;;; PHENYLALANINE
 
 [ moleculetype ]
 ; molname       nrexcl
 PHE                1
 
 [ atoms ]
 ;id type resnr residu atom cgnr   charge
 1   $prot_default_bb_type     1     PHE     BB     1    0
-2   SC4    1     PHE     SC1    2    0    ; three side chains in triangle
-3   TC5    1     PHE     SC2    3    0    ; configuration, mimicking
-4   TC5    1     PHE     SC3    4    0    ; ring structure
+2   SC4    1     PHE     SC1    1    0    ; three side chains in triangle
+3   TC5    1     PHE     SC2    1    0    ; configuration, mimicking
+4   TC5    1     PHE     SC3    1    0    ; ring structure
+5   VS     1     PHE     CA     1      0   0
+[ virtual_sitesn ]
+5 1 -- 1
 
 [bonds]
 #meta {"group": "Side chain bonds"}
 ;  i     j   funct   length  force.c.
   BB   SC1    1       0.325     7500 	
 #meta {"group": "Side chain bonds", "ifdef": "FLEXIBLE"}
 ;  i     j   funct   length  
@@ -459,27 +577,34 @@
 
 [exclusions]
 ; We do not want non-bounded interactions within the residue.
 BB SC1 SC2 SC3
 SC1 SC2 SC3
 SC2 SC3
 
+[ position_restraints ]
+1  1  1 1000 1000 1000 {"ifdef": "POSRES"}
+
 ;;; TYROSINE
 
 [ moleculetype ]
 ; molname       nrexcl
 TYR                1
 
 [ atoms ]
 ;id type resnr residu atom cgnr   charge
 1   $prot_default_bb_type     1     TYR     BB     1    0
-2   TC4    1     TYR     SC1    2    0  
-3   TC5    1     TYR     SC2    3    0 
-4   TC5    1     TYR     SC3    4    0  
-5   TN6    1     TYR     SC4    5    0
+2   TC4    1     TYR     SC1    1    0  
+3   TC5    1     TYR     SC2    1    0 
+4   TC5    1     TYR     SC3    1    0  
+5   TN6    1     TYR     SC4    1    0
+6   VS     1     TYR     CA     1      0   0
+[ virtual_sitesn ]
+6 1 -- 1
+
 
 [bonds]
 #meta {"group": "Side chain bonds"}
 ;  i     j   funct   length  force.c.
   BB   SC1    1       0.325    5000 	
 #meta {"group": "Side chain bonds", "ifdef": "FLEXIBLE"}
 ;  i     j   funct   length  
@@ -511,28 +636,32 @@
 [exclusions]
 ; We do not want non-bounded interactions within the residue.
 BB SC1 SC2 SC3 SC4
 SC1 SC2 SC3 SC4
 SC2 SC3 SC4
 SC3 SC4
 
+[ position_restraints ]
+1  1  1 1000 1000 1000 {"ifdef": "POSRES"}
+
 ;;; TRYPTOPHAN
 
 [ moleculetype ]
 ;molname       nrexcl
 TRP                1
 
 [ atoms ]
 ;id type resnr residu atom cgnr   charge
 1   $prot_default_bb_type       1     TRP     BB     1    0
-2   TC4      1     TRP     SC1    2    0       36
-3   TN6d     1     TRP     SC2    3    0       36
-4   TC5      1     TRP     SC3    4    0        0
-5   TC5      1     TRP     SC4    5    0       36
-6   TC5      1     TRP     SC5    6    0       36
+2   TC4      1     TRP     SC1    1    0       36
+3   TN6d     1     TRP     SC2    1    0       36
+4   TC5      1     TRP     SC3    1    0        0
+5   TC5      1     TRP     SC4    1    0       36
+6   TC5      1     TRP     SC5    1    0       36
+7   VS       1     TRP     CA     1      0   0
 
 [ bonds ]
 #meta {"group": "Side chain bonds"}
 ;  i     j   funct   length  force.c.
   BB   SC1    1       0.315     5000 	
 #meta {"group": "Side chain bonds", "ifdef": "FLEXIBLE"}
 ;  i     j   funct   length  
@@ -559,27 +688,31 @@
 
 [ dihedrals ]
 ;  i     j    k    l   funct   angle  force.c.
  SC5   SC4  SC2  SC1       2   180.0    100.0
 
 [ virtual_sitesn ]
 SC3 SC5 SC4 SC2 SC1 -- 2
+7 1 -- 1
 
 ; prevents polyply warning about disconnected molecules
 [ edges ]
 SC3 SC5
 
 [exclusions]
 ; We do not want non-bounded interactions within the residue.
 BB SC1 SC2 SC3 SC4 SC5
 SC1 SC2 SC3 SC4 SC5
 SC2 SC3 SC4 SC5
 SC3 SC4 SC5
 SC4 SC5
 
+[ position_restraints ]
+1  1  1 1000 1000 1000 {"ifdef": "POSRES"}
+
 ;;; Links
 
 ;; Links for COIL. We apply them first as coil is the default.
 [ link ]
 resname $protein_resnames
 [ bonds ]
 ; (Modified by Paulo)
@@ -616,14 +749,75 @@
 ; (Modified by Paulo)
 -BB BB +BB 10 127 20 {"group": "BBB angles"}
 [ patterns ]
 -BB BB {"resname": $protein_resnames_non_pro} +BB 
 -BB {"resname": $protein_resnames_non_pro} BB +BB 
 -BB  BB +BB {"resname": $protein_resnames_non_pro}
 
+;; IDP specific corrections
+
+[ link ]
+resname $protein_resnames
+[ angles ]
+BB +BB +SC1 10 85 10 {"group": "idp-fix"}
+
+[ link ]
+resname $protein_resnames
+[ angles ]
+-SC1 -BB BB 10 85 10 {"group": "idp-fix"}
+
+[ link ]
+resname $protein_resnames
+[ dihedrals ]
+BB +BB ++BB +++BB 9 -120 -1 1 {"group": "idp-fix", "comment": "BB-BB-BB-BB-v1", "version":1}
+BB +BB ++BB +++BB 9 -120 -1 2 {"group": "idp-fix", "comment": "BB-BB-BB-BB-v2", "version":2}
+
+[ link ]
+resname $protein_resnames
+[ dihedrals ]
+SC1 BB +BB +SC1 9 -130 -1.5 1 {"group": "idp-fix", "version": 1, "comment": "SC1-BB-BB-SC1-v1"}
+SC1 BB +BB +SC1 9  100 -1.5 2 {"group": "idp-fix", "version": 2, "comment": "SC1-BB-BB-SC1-v2"}
+
+[ link ]
+[ atoms ]
+-SC1 {"resname": $protein_resnames}
+-BB  {"resname": $protein_resnames}
+ BB  {"resname": "GLY"}
++BB  {"resname": $protein_resnames}
+[ dihedrals ]
+-SC1 -BB BB +BB 1 115 -4.5 1 {"group": "idp-fix", "comment": "SC1-BB-BB(GLY)-BB"}
+
+[ link ]
+[ atoms ]
+-BB {"resname": $protein_resnames}
+ BB {"resname": "GLY"}
++BB {"resname": $protein_resnames}
++SC1 {"resname": $protein_resnames}
+[ dihedrals ]
+-BB BB +BB +SC1 1 0 -2.0 1 {"group": "idp-fix", "comment": "BB-BB(GLY)-BB-SC1"}
+
+[ link ]
+resname $protein_resnames
+[ exclusions ]
+#meta {"comment": "CA-BB-same"}
+CA  BB
+[ edges ]
+CA BB
+
+[ link ]
+resname $protein_resnames
+[ atoms ]
+CA { }
+BB { }
++BB { }
+[ exclusions ]
+#meta {"comment": "CA-BB"}
+CA +BB
+[ edges ]
+BB +BB
 
 ;; Protein termini. These links should be applied last.
 [ link ]
 resname $protein_resnames
 [ atoms ]
 BB {"replace": {"atype": "Q5", "charge": 1}}
 [ non-edges ]
```

### Comparing `polyply-1.6.1/polyply/data/martini3/cellulose.martini3.ff` & `polyply-1.7.0/polyply/data/martini3/cellulose.martini3.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/martini3/citations.bib` & `polyply-1.7.0/polyply/data/martini3/citations.bib`

 * *Files 13% similar despite different names*

```diff
@@ -54,7 +54,15 @@
   journal={Soft Matter},
   volume={18},
   number={40},
   pages={7887--7896},
   year={2022},
   publisher={Royal Society of Chemistry}
 }
+
+@article{M3_GO,
+title={GōMartini 3: From large conformational changes in proteins to environmental bias corrections},
+author={Souza, Paulo C. T. and Araujo, Luis P. Borges and Brasnett, Chris and Moreira, Rodrigo A. and Grunewald, Fabian and Park, Peter and Wang, Liguo and Razmazma, Hafez and Borges-Araujo, Ana C. and Cofas-Vargas, Luis F. and Monticelli, Luca and Mera-Adasme, Raul and Melo, Manuel N. and Wu, Sangwook and Marrink, Siewert J. and Poma, Adolfo B. and Thallmair, Sebastian},
+url={https://www.biorxiv.org/content/10.1101/2024.04.15.589479v1},
+doi={10.1101/2024.04.15.589479},
+year={2024},
+}
```

### Comparing `polyply-1.6.1/polyply/data/martini3/dextran.martini3.ff` & `polyply-1.7.0/polyply/data/martini3/dextran.martini3.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/martini3_beta/citations.bib` & `polyply-1.7.0/polyply/data/martini3_beta/citations.bib`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/oplsaaLigParGen/CH3.ff` & `polyply-1.7.0/polyply/data/oplsaaLigParGen/CH3.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/oplsaaLigParGen/OHter.ff` & `polyply-1.7.0/polyply/data/oplsaaLigParGen/OHter.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/oplsaaLigParGen/PEO.oplsaa.LigParGen.ff` & `polyply-1.7.0/polyply/data/oplsaaLigParGen/PEO.oplsaa.LigParGen.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/oplsaaLigParGen/PTMA.oplsaa.LigParGen.ff` & `polyply-1.7.0/polyply/data/oplsaaLigParGen/PTMA.oplsaa.LigParGen.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/oplsaaLigParGen/citations.bib` & `polyply-1.7.0/polyply/data/oplsaaLigParGen/citations.bib`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/oplsaaLigParGen/links.ff` & `polyply-1.7.0/polyply/data/oplsaaLigParGen/links.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/oplsaaLigParGen/links_PTMA.ff` & `polyply-1.7.0/polyply/data/oplsaaLigParGen/links_PTMA.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/parmbsc1/citations.bib` & `polyply-1.7.0/polyply/data/parmbsc1/citations.bib`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/data/parmbsc1/dna_final.ff` & `polyply-1.7.0/polyply/data/parmbsc1/dna_final.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/src/__init__.py` & `polyply-1.7.0/polyply/src/__init__.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/src/annotate_ligands.py` & `polyply-1.7.0/polyply/src/annotate_ligands.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/src/apply_links.py` & `polyply-1.7.0/polyply/src/apply_links.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/src/apply_modifications.py` & `polyply-1.7.0/polyply/src/apply_modifications.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/src/backmap.py` & `polyply-1.7.0/polyply/src/backmap.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/src/build_file_parser.py` & `polyply-1.7.0/polyply/src/build_file_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,14 +171,23 @@
         """
         Parses the lines in the '[volumes]'
         directive and stores it.
         """
         resname, volume = line.split()
         self.topology.volumes[resname] = float(volume)
 
+    @SectionLineParser.section_parser('bending')
+    def _bending(self, line, lineno=0):
+        """
+        Parses the lines in the '[bending]'
+        directive and stores it.
+        """
+        resA, resB, resC, bending_const = line.split()
+        self.topology.bending[(resA, resB, resC)] = float(bending_const)
+
     def finalize_section(self, previous_section, ended_section):
         """
         Called once a section has finished. Here we perform all
         operations that are required when a section has ended.
         Here comes a list of end-section wrap ups:
 
         Templates
```

### Comparing `polyply-1.6.1/polyply/src/build_system.py` & `polyply-1.7.0/polyply/src/build_system.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/src/check_residue_equivalence.py` & `polyply-1.7.0/polyply/src/check_residue_equivalence.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/src/ff_parser_sub.py` & `polyply-1.7.0/polyply/src/ff_parser_sub.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/src/gen_coords.py` & `polyply-1.7.0/polyply/src/gen_coords.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/src/gen_dna.py` & `polyply-1.7.0/polyply/src/gen_dna.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/src/gen_itp.py` & `polyply-1.7.0/polyply/src/gen_itp.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/src/gen_seq.py` & `polyply-1.7.0/polyply/src/gen_seq.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/src/generate_templates.py` & `polyply-1.7.0/polyply/src/generate_templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,27 +170,31 @@
     radius of gyration
     """
     n_atoms = len(coords)
     points = np.array(list(coords.values()))
     res_center_of_geometry = center_of_geometry(points)
     geom_vects = np.zeros((n_atoms, 3))
     idx = 0
-
+    radii = []
     for node, coord in coords.items():
         atom_key = block.nodes[node]["atype"]
         rad = float(nonbond_params[frozenset([atom_key, atom_key])]["nb1"])
         diff = coord - res_center_of_geometry
         if np.linalg.norm(diff) > treshold:
             geom_vects[idx, :] = diff + u_vect(diff) * rad
             idx += 1
-
-    if geom_vects.shape[0] > 1:
+        else:
+            radii.append(rad)
+    # make sure geom_vects is not just an array of zeros
+    # this can happen when multiple beads are stacked for
+    # example
+    if np.any(geom_vects):
         radgyr = radius_of_gyration(geom_vects)
     else:
-        radgyr = rad
+        radgyr = max(radii)
 
     return radgyr
 
 def map_from_CoG(coords):
     """
     Compute the center of geometry
     of `coords` and return each position
```

### Comparing `polyply-1.6.1/polyply/src/graph_utils.py` & `polyply-1.7.0/polyply/src/graph_utils.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/src/linalg_functions.py` & `polyply-1.7.0/polyply/src/linalg_functions.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/src/load_library.py` & `polyply-1.7.0/polyply/src/load_library.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/src/logging.py` & `polyply-1.7.0/polyply/src/logging.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/src/map_to_molecule.py` & `polyply-1.7.0/polyply/src/map_to_molecule.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/src/meta_molecule.py` & `polyply-1.7.0/polyply/src/meta_molecule.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/src/minimizer.py` & `polyply-1.7.0/polyply/src/minimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,16 @@
                 params = interaction.parameters
                 atom_coords = [positions[atom_to_idx[name]]
                                for name in atoms]
                 new = INTER_METHODS[inter_type](params, atom_coords)
                 energy += new
         return energy
 
-    opt_results = scipy.optimize.minimize(target_function, positions, method='L-BFGS-B',
+    opt_results = scipy.optimize.minimize(target_function, positions,
+                                          method='L-BFGS-B',
                                           options={'ftol': 0.001, 'maxiter': 100})
 
     # evaluate if optimization was successful
     positions = opt_results['x'].reshape((-1, 3))
     positions = renew_vs(positions, block, atom_to_idx)
 
     for node_key, idx in atom_to_idx.items():
```

### Comparing `polyply-1.6.1/polyply/src/nonbond_engine.py` & `polyply-1.7.0/polyply/src/nonbond_engine.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import random
 import itertools
 import numpy as np
 import scipy.spatial
 from polyply import jit
 from .topology import lorentz_berthelot_rule
-from .linalg_functions import not_exceeds_max_dimensions
+from .linalg_functions import angle, not_exceeds_max_dimensions
 
 def _lennard_jones_force(dist, point, ref, params):
     """
     Compute the Lennard-Jones force between two particles
     given their interaction parameters, the distance, and
     distance vector.
 
@@ -50,15 +51,14 @@
     return force
 
 # numba implementation if available
 lennard_jones_force = jit(_lennard_jones_force)
 
 POTENTIAL_FUNC = {"LJ": lennard_jones_force}
 
-
 def _n_particles(molecules):
     """
     Count the number of meta_molecule nodes
     in the topology.
     """
     return sum(map(len, molecules))
 
@@ -73,14 +73,16 @@
     """
 
     def __init__(self,
                  positions,
                  nodes_to_idx,
                  atom_types,
                  interaction_matrix,
+                 bending_matrix,
+                 torsion_matrix,
                  cut_off,
                  boxsize):
         """
         Parameters:
         -----------
         positions: np.ndarray
         nodes_to_idx: dict[(mol_idx, node_key)]
@@ -89,24 +91,32 @@
              index and node_key
         atomtypes:  np.ndarray
              array of atom_types corresponding to the atoms in positions
         interaction_matrix:  dict[frozenset(str, str), tuple(float, float)]
              Dict mapping the atom_types to LJ type interaction parameters,
              that is sigma, epsilon or C6, C12 depending on the potential
              used. Currently only the sigma epsilon form is implemented.
+        bending_matrix: dict[frozenset(str, str), float]
+             Dict mapping the residue types to a bending constant for the
+             bending probability
+        torsion_matrix: dict[frozenset(str, str), float]
+             Dict mapping the residue types to a torsion constant for the
+             torsion probability
         cut_off: float
              cut-off for which to compute the interaction in nm
         boxsize: np.ndarray
              box dimensions in nm
         """
 
         self.positions = positions
         self.nodes_to_gndx = nodes_to_idx
         self.atypes = np.asarray(atom_types, dtype=str)
         self.interaction_matrix = interaction_matrix
+        self.bending_matrix = bending_matrix
+        self.torsion_matrix = torsion_matrix
         self.cut_off = cut_off
         self.boxsize = boxsize
 
         self.defined_idxs = [list(np.where(self.positions[:, 0].reshape(-1) != np.inf)[0])]
         self.position_trees = [scipy.spatial.KDTree(positions[self.defined_idxs[-1]],
                                                     boxsize=boxsize)]
 
@@ -288,14 +298,50 @@
 
                 if gndx_pair not in exclusions:
                     other_atype = self.atypes[gndx_pair]
                     params = self.interaction_matrix[frozenset([current_atype, other_atype])]
                     force += POTENTIAL_FUNC[potential](dist, point, self.positions[gndx_pair], params)
         return force
 
+    def compute_bending_probability(self, lp, point, mol_idx, node_b, node_c):
+        """
+        Compute probability of an angle between three points (`point`, `node_b`,
+        `node_c`) according to a simple decay function modulated by a bending
+        constant `lp`. If lp is large the distribution increases with the highest
+        probability being at 180 degrees (i.e. more straight angles), whilst if lp
+        is low the angles occur with almost equal probability.
+
+        Parameters
+        ----------
+        lp: float
+            bending constant
+        point: np.ndarray(1, 3)
+            coordinates of the new point
+        mol_idx: int
+            index of the molecule at hand
+        node_b: abc.hashable
+            first predecessor of the node corresponding to `point`
+        node_c: abc.hashable
+            second predecessor of the node corresponding to `point`
+
+        Returns
+        -------
+        float
+            the probability
+        """
+        # get the missing positions
+        B_pos = self.get_point(mol_idx, node_b)
+        C_pos = self.get_point(mol_idx, node_c)
+        # compute angle
+        ang_val = angle(point, B_pos, C_pos)
+        # compute probability
+        # denominator is normalization
+        prob = np.exp(lp*ang_val/180)/(180*(np.exp(lp)-1)/lp)
+        return prob
+
     @classmethod
     def from_topology(cls, molecules, topology, box):
         """
         Create a class instance from a topology object,
         a list of molecules and a box.
 
         Parameters:
@@ -356,9 +402,11 @@
             vdw_radius = topology.volumes[resname]
             # as by model definition all epsilon values are set to 1
             inter_matrix[frozenset([resname, resname])] = (vdw_radius, 1.0)
 
         # dynamically set the cut-off as twice the largest vdw-radius
         cut_off = max(list(inter_matrix.values()))[0] * 2.
         nonbond_matrix = cls(positions, nodes_to_gndx,
-                             atom_types, inter_matrix, cut_off=cut_off, boxsize=box)
+                             atom_types, inter_matrix,
+                             cut_off=cut_off, boxsize=box,
+                             torsion_matrix=None, bending_matrix=topology.bending)
         return nonbond_matrix
```

### Comparing `polyply-1.6.1/polyply/src/persistence.py` & `polyply-1.7.0/polyply/src/persistence.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/src/polyply_parser.py` & `polyply-1.7.0/polyply/src/polyply_parser.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/src/processor.py` & `polyply-1.7.0/polyply/src/processor.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/src/random_walk.py` & `polyply-1.7.0/polyply/src/random_walk.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 import random
 import numpy as np
 from numpy.linalg import norm
 import networkx as nx
 from .processor import Processor
-from .linalg_functions import _vector_angle_degrees, not_exceeds_max_dimensions, norm_sphere, pbc_complete
+from .linalg_functions import angle, _vector_angle_degrees, not_exceeds_max_dimensions, norm_sphere, pbc_complete
 from .graph_utils import neighborhood
 from .meta_molecule import _find_starting_node
 """
 Processor implementing a random-walk to generate
 coordinates for a meta-molecule.
 """
 
@@ -242,14 +242,15 @@
         self.vector_sphere = vector_sphere
         self.success = False
         self.max_force = max_force
         self.step_fudge = step_fudge
         self.start_node = start_node
         self.nrewind = nrewind
         self.placed_nodes = []
+        self.prev_prob = 1
 
     def _rewind(self, current_step):
         nodes = [node for _, node in self.placed_nodes[-self.nrewind:-1]]
         self.nonbond_matrix.remove_positions(self.mol_idx, nodes)
         step_count = self.placed_nodes[-self.nrewind][0]
         self.placed_nodes = self.placed_nodes[:-self.nrewind]
         return step_count
@@ -275,14 +276,61 @@
                     return False
 
                 if current_distance < lower_bound:
                     return False
 
         return True
 
+    def bendiness(self, point, node):
+        """
+        Perform Monte-Carlo like sampling of bending probability.
+
+        Parameters
+        ----------
+        point: np.ndarray
+            new coordinate
+        node: `abc.hashable`
+            the current node for which to get a new point
+        """
+        b_node = list(self.molecule.search_tree.predecessors(node))[0]
+        c_nodes = list(self.molecule.search_tree.predecessors(b_node))
+
+        if len(c_nodes) != 1:
+            return True
+
+        c_node = c_nodes[0]
+        # get the atom types aka resnames
+        typea = self.molecule.nodes[node]['resname']
+        typeb = self.molecule.nodes[b_node]['resname']
+        typec = self.molecule.nodes[c_node]['resname']
+        # get the bending constant
+        lp = self.nonbond_matrix.bending_matrix.get((typea, typeb, typec), None)
+        if not lp:
+            return True
+
+        prob = self.nonbond_matrix.compute_bending_probability(lp,
+                                                               point,
+                                                               self.mol_idx,
+                                                               b_node,
+                                                               c_node)
+        if self.prev_prob < prob:
+            self.prev_prob = prob
+            return True
+
+        # compute test probability from uniform sampling of prob function
+        norm = 180/lp * (np.exp(lp)-1)
+        test_prob = random.uniform(np.exp(lp*1/180)/norm,
+                                   np.exp(lp*179/180)/norm)
+
+        if test_prob < prob:
+            self.prev_prob = prob
+            return True
+
+        return False
+
     def update_positions(self, vector_bundle, current_node, prev_node):
         """
         Take an array of unit vectors `vector_bundle` and generate the coordinates
         for `current_node` by adding a random vector to the position of the previous
         node `prev_node`. The length of that vector is defined as 2 times the vdw-radius
         of the two nodes. The position is updated in place.
 
@@ -304,15 +352,16 @@
         step_count = 0
         while True:
 
             new_point, index = _take_step(vector_bundle, step_length, last_point, self.maxdim)
             if fulfill_geometrical_constraints(new_point, self.molecule.nodes[current_node])\
                 and self.checks_milestones(current_node, new_point, step_length)\
                 and is_restricted(new_point, last_point, self.molecule.nodes[current_node])\
-                and not self._is_overlap(new_point, current_node):
+                and not self._is_overlap(new_point, current_node)\
+                and self.bendiness(new_point, current_node):
 
                     self.nonbond_matrix.add_positions(new_point,
                                                       self.mol_idx,
                                                       current_node,
                                                       start=False)
                     return True
 
@@ -352,18 +401,16 @@
                 self.success = False
                 return
 
         vector_bundle = self.vector_sphere.copy()
         count = 0
         path = list(meta_molecule.search_tree.edges)
         step_count = 0
-
         while step_count < len(path):
             prev_node, current_node = path[step_count]
-
             if not meta_molecule.nodes[current_node]["build"]:
                 step_count += 1
                 continue
 
             status = self.update_positions(vector_bundle,
                                            current_node,
                                            prev_node)
```

### Comparing `polyply-1.6.1/polyply/src/restraints.py` & `polyply-1.7.0/polyply/src/restraints.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/src/simple_seq_parsers.py` & `polyply-1.7.0/polyply/src/simple_seq_parsers.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/src/top_parser.py` & `polyply-1.7.0/polyply/src/top_parser.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/src/topology.py` & `polyply-1.7.0/polyply/src/topology.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,14 +211,18 @@
     force_field: a :class:`vermouth.forcefield.ForceField`
     nonbond_params: dict
         A dictionary of all nonbonded parameters
     types: dict
         A dictionary of all typed parameter
     defines: list
         A list of everything that is defined
+    volumes: dict
+        Volume constants for meta-models
+    bending: dict
+        Sequence dependent bending constants for meta-model
     box: np.array(3,1)
         Box vectors as a, b, c in nanometers
     """
 
     def __init__(self, force_field, name=None):
         super().__init__(force_field)
         self.name = name
@@ -228,14 +232,15 @@
         self.atom_types = {}
         self.types = defaultdict(lambda: defaultdict(list))
         self.nonbond_params = {}
         self.mol_idx_by_name = defaultdict(list)
         self.persistences = []
         self.distance_restraints = defaultdict(dict)
         self.volumes = {}
+        self.bending = {}
         self.box = None
 
     def preprocess(self):
         """
         Apply all defaults, generate pairs, convert non-bonded
         units. It performs most of the conversion which otherwise
         is done by grompp.
```

### Comparing `polyply-1.6.1/polyply/src/virtual_site_builder.py` & `polyply-1.7.0/polyply/src/virtual_site_builder.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/__init__.py` & `polyply-1.7.0/polyply/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/example_fixtures.py` & `polyply-1.7.0/polyply/tests/example_fixtures.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_annotate_lingads.py` & `polyply-1.7.0/polyply/tests/test_annotate_lingads.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_apply_links.py` & `polyply-1.7.0/polyply/tests/test_apply_links.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_backmap.py` & `polyply-1.7.0/polyply/tests/test_backmap.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_build_file_parser.py` & `polyply-1.7.0/polyply/tests/test_build_file_parser.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_build_system.py` & `polyply-1.7.0/polyply/tests/test_build_system.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/ff/aminoacids.ff` & `polyply-1.7.0/polyply/tests/test_data/ff/aminoacids.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_params/input/P3HT.martini.2.itp` & `polyply-1.7.0/polyply/tests/test_data/gen_params/input/P3HT.martini.2.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_params/input/PEO.martini.3.itp` & `polyply-1.7.0/polyply/tests/test_data/gen_params/input/PEO.martini.3.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_params/input/PPI.ff` & `polyply-1.7.0/polyply/tests/test_data/gen_params/input/PPI.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_params/input/PPI.json` & `polyply-1.7.0/polyply/tests/test_data/gen_params/input/PPI.json`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_params/input/PS.json` & `polyply-1.7.0/polyply/tests/test_data/gen_params/input/PS.json`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_params/input/PS.martini.2.itp` & `polyply-1.7.0/polyply/tests/test_data/gen_params/input/PS.martini.2.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_params/input/removal.ff` & `polyply-1.7.0/polyply/tests/test_data/gen_params/input/removal.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_params/input/test.ff` & `polyply-1.7.0/polyply/tests/test_data/gen_params/input/test.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_params/input/test_edge_attr.ff` & `polyply-1.7.0/polyply/tests/test_data/gen_params/input/test_edge_attr.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_params/input/test_edge_attr.json` & `polyply-1.7.0/polyply/tests/test_data/gen_params/input/test_edge_attr.json`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_params/logging/ERROR_block.ff` & `polyply-1.7.0/polyply/tests/test_data/gen_params/logging/ERROR_block.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_params/logging/ERROR_link.ff` & `polyply-1.7.0/polyply/tests/test_data/gen_params/logging/ERROR_link.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_params/logging/INFO_block.ff` & `polyply-1.7.0/polyply/tests/test_data/gen_params/logging/INFO_block.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_params/logging/INFO_link.ff` & `polyply-1.7.0/polyply/tests/test_data/gen_params/logging/INFO_link.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_params/logging/WARNING_block.ff` & `polyply-1.7.0/polyply/tests/test_data/gen_params/logging/WARNING_block.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_params/logging/WARNING_link.ff` & `polyply-1.7.0/polyply/tests/test_data/gen_params/logging/WARNING_link.ff`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_params/ref/G3.itp` & `polyply-1.7.0/polyply/tests/test_data/gen_params/ref/G3.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_params/ref/P3HT_10.itp` & `polyply-1.7.0/polyply/tests/test_data/gen_params/ref/P3HT_10.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_params/ref/PEO_10.itp` & `polyply-1.7.0/polyply/tests/test_data/gen_params/ref/PEO_10.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_params/ref/PS_10.itp` & `polyply-1.7.0/polyply/tests/test_data/gen_params/ref/PS_10.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_params/ref/test_edge_attr_ref.itp` & `polyply-1.7.0/polyply/tests/test_data/gen_params/ref/test_edge_attr_ref.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_params/ref/test_rev.itp` & `polyply-1.7.0/polyply/tests/test_data/gen_params/ref/test_rev.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_seq/input/molecule_0.itp` & `polyply-1.7.0/polyply/tests/test_data/gen_seq/input/molecule_0.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_seq/output/PEO_PS.json` & `polyply-1.7.0/polyply/tests/test_data/gen_seq/output/PEO_PS.json`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_seq/output/PPI.json` & `polyply-1.7.0/polyply/tests/test_data/gen_seq/output/PPI.json`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_seq/output/lysoPEG.json` & `polyply-1.7.0/polyply/tests/test_data/gen_seq/output/lysoPEG.json`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_seq/output/lyso_PEG.json` & `polyply-1.7.0/polyply/tests/test_data/gen_seq/output/lyso_PEG.json`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_seq/output/rand_PEG_PPO.json` & `polyply-1.7.0/polyply/tests/test_data/gen_seq/output/rand_PEG_PPO.json`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_seq/ref/PEO_PS_ref.json` & `polyply-1.7.0/polyply/tests/test_data/gen_seq/ref/PEO_PS_ref.json`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_seq/ref/PPI_ref.json` & `polyply-1.7.0/polyply/tests/test_data/gen_seq/ref/PPI_ref.json`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/gen_seq/ref/lyso_PEG.json` & `polyply-1.7.0/polyply/tests/test_data/gen_seq/ref/lyso_PEG.json`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/itp/PEO.itp` & `polyply-1.7.0/polyply/tests/test_data/itp/PEO.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/json/double_branch.json` & `polyply-1.7.0/polyply/tests/test_data/json/double_branch.json`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/json/hyperbranched.json` & `polyply-1.7.0/polyply/tests/test_data/json/hyperbranched.json`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/C12E4/polyply/C12E4.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/C12E4/polyply/C12E4.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PE/PE.json` & `polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PE/PE.json`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PE/polyply/PE.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PE/polyply/PE.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PMA/PMA.json` & `polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PMA/PMA.json`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PMA/polyply/PMA.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PMA/polyply/PMA.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PP/PP.json` & `polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PP/PP.json`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PP/polyply/PP.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PP/polyply/PP.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PS/PS.json` & `polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PS/PS.json`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PS/polyply/PS.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PS/polyply/PS.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PVA/PVA.json` & `polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PVA/PVA.json`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/2016H66/PVA/polyply/PVA.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/2016H66/PVA/polyply/PVA.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/gromos53A6/P3HT/polyply/P3HT.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/gromos53A6/P3HT/polyply/P3HT.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/ibi_cgm3/PTMA/polyply/PTMA.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/ibi_cgm3/PTMA/polyply/PTMA.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/ibi_gbcg/PTMA/polyply/PTMA.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/ibi_gbcg/PTMA/polyply/PTMA.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/PEL/DPPC.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/PEL/DPPC.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/PEL/polyply/PEL.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/PEL/polyply/PEL.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/PEO/polyply/PEO.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/PEO/polyply/PEO.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/PEO_PE/PEO_PE.json` & `polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/PEO_PE/PEO_PE.json`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/PEO_PE/polyply/PEO_PE.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/PEO_PE/polyply/PEO_PE.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/PS/polyply/PS.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/PS/polyply/PS.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/ssDNA/polyply/ssDNA.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/ssDNA/polyply/ssDNA.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/ssDNA/ssDNA.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/ssDNA/ssDNA.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/martini2/ssDNA/ssDNA.json` & `polyply-1.7.0/polyply/tests/test_data/library_tests/martini2/ssDNA/ssDNA.json`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/CEL/polyply/CEL.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/CEL/polyply/CEL.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/DEX/polyply/DEX.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/DEX/polyply/DEX.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/P3HT/polyply/P3HT.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/P3HT/polyply/P3HT.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PDMS/polyply/PDMS.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PDMS/polyply/PDMS.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PE/polyply/PE.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PE/polyply/PE.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PEO/polyply/PEO.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PEO/polyply/PEO.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PPE/polyply/PPE.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PPE/polyply/PPE.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PS/polyply/PS.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PS/polyply/PS.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/martini3/PTMA/polyply/PTMA.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/martini3/PTMA/polyply/PTMA.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/oplsaaLigParGen/PEO/polyply/PEO.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/oplsaaLigParGen/PEO/polyply/PEO.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/oplsaaLigParGen/PTMA/polyply/PTMA.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/oplsaaLigParGen/PTMA/polyply/PTMA.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/parmbsc1/DNA/DNA.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/parmbsc1/DNA/DNA.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/parmbsc1/DNA/polyply/DNA.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/parmbsc1/DNA/polyply/DNA.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/parmbsc1/DNA/ref.json` & `polyply-1.7.0/polyply/tests/test_data/library_tests/parmbsc1/DNA/ref.json`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/parmbsc1/dsDNA/polyply/DNA.itp` & `polyply-1.7.0/polyply/tests/test_data/library_tests/parmbsc1/dsDNA/polyply/DNA.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/library_tests/parmbsc1/dsDNA/ref.json` & `polyply-1.7.0/polyply/tests/test_data/library_tests/parmbsc1/dsDNA/ref.json`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/polyply/P3HT.martini.2.itp` & `polyply-1.7.0/polyply/tests/test_data/polyply/P3HT.martini.2.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/polyply/PDADMA.martini.2.itp` & `polyply-1.7.0/polyply/tests/test_data/polyply/PDADMA.martini.2.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/polyply/PE.martini.2.itp` & `polyply-1.7.0/polyply/tests/test_data/polyply/PE.martini.2.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/polyply/PEL_lipid.martini.2.itp` & `polyply-1.7.0/polyply/tests/test_data/polyply/PEL_lipid.martini.2.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/polyply/PEO.martini.2.itp` & `polyply-1.7.0/polyply/tests/test_data/polyply/PEO.martini.2.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/polyply/PEO.martini.3.itp` & `polyply-1.7.0/polyply/tests/test_data/polyply/PEO.martini.3.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/polyply/PP.martini.2.itp` & `polyply-1.7.0/polyply/tests/test_data/polyply/PP.martini.2.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/polyply/PS.martini.2.itp` & `polyply-1.7.0/polyply/tests/test_data/polyply/PS.martini.2.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/polyply/PSS.martini.2.itp` & `polyply-1.7.0/polyply/tests/test_data/polyply/PSS.martini.2.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/struc_build/PEO.itp` & `polyply-1.7.0/polyply/tests/test_data/struc_build/PEO.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/struc_build/martini_PEO_PS_CNP.itp` & `polyply-1.7.0/polyply/tests/test_data/struc_build/martini_PEO_PS_CNP.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/topology_test/complete.gro` & `polyply-1.7.0/polyply/tests/test_data/topology_test/complete.gro`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/topology_test/fail.gro` & `polyply-1.7.0/polyply/tests/test_data/topology_test/fail.gro`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/topology_test/ffnonbonded.itp` & `polyply-1.7.0/polyply/tests/test_data/topology_test/ffnonbonded.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/topology_test/molecule_0.itp` & `polyply-1.7.0/polyply/tests/test_data/topology_test/molecule_0.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/topology_test/test.gro` & `polyply-1.7.0/polyply/tests/test_data/topology_test/test.gro`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/topology_test/test.itp` & `polyply-1.7.0/polyply/tests/test_data/topology_test/test.itp`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_data/topology_test/test.pdb` & `polyply-1.7.0/polyply/tests/test_data/topology_test/test.pdb`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_ff_parser.py` & `polyply-1.7.0/polyply/tests/test_ff_parser.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_gen_coords.py` & `polyply-1.7.0/polyply/tests/test_gen_coords.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_gen_coords_logic.py` & `polyply-1.7.0/polyply/tests/test_gen_coords_logic.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_gen_dna.py` & `polyply-1.7.0/polyply/tests/test_gen_dna.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_gen_params.py` & `polyply-1.7.0/polyply/tests/test_gen_params.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_gen_seq.py` & `polyply-1.7.0/polyply/tests/test_gen_seq.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_generate_templates.py` & `polyply-1.7.0/polyply/tests/test_generate_templates.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import textwrap
 import pytest
 import numpy as np
 import math
 import networkx as nx
 import vermouth
 from vermouth.molecule import Interaction
+from vermouth.gmx.itp_read import read_itp
 import polyply
 from polyply import TEST_DATA
 from polyply.src.linalg_functions import center_of_geometry
 from polyply.src.generate_templates import (find_atoms,
                                             _expand_inital_coords,
                                             _relabel_interaction_atoms,
                                             compute_volume, map_from_CoG,
@@ -73,42 +74,14 @@
         block = ff.blocks['GLY']
         coords = _expand_inital_coords(block)
         assert len(coords) == 4
         for pos in coords.values():
             assert len(pos) == 3
 
       @staticmethod
-      def test_compute_volume():
-          lines = """
-          [ moleculetype ]
-          GLY 1
-
-          [ atoms ]
-          1 P1 1 ALA BB 1
-          2 P1 1 ALA SC1 2
-          3 P1 1 ALA SC2 3
-          4 P1 1 ALA SC3 3
-
-          [ bonds ]
-          1 2 1 0.2 100
-          2 3 1 0.6 700
-          3 4 1 0.2 700
-          """
-          meta_mol = polyply.MetaMolecule()
-          nonbond_params = {frozenset(["P1", "P1"]): {"nb1": 0.47, "nb2":0.5}}
-
-          lines = textwrap.dedent(lines).splitlines()
-          ff = vermouth.forcefield.ForceField(name='test_ff')
-          polyply.src.polyply_parser.read_polyply(lines, ff)
-          block = ff.blocks['GLY']
-          coords = _expand_inital_coords(block)
-          vol = compute_volume(block, coords, nonbond_params)
-          assert vol > 0.
-
-      @staticmethod
       def test_map_from_CoG():
          lines = """
          [ moleculetype ]
          GLY 1
          [ atoms ]
          1 P4 1 ALA BB 1
          2 P3 1 ALA SC1 2
@@ -245,7 +218,87 @@
       def test_find_interaction_involving_error(lines):
           lines = textwrap.dedent(lines).splitlines()
           ff = vermouth.forcefield.ForceField(name='test_ff')
           polyply.src.polyply_parser.read_polyply(lines, ff)
           block = ff.blocks['test']
           with pytest.raises(IOError):
                find_interaction_involving(block, 1, 2)
+
+@pytest.mark.parametrize('lines, coords, volume',
+    [("""
+      [ moleculetype ]
+      GLY 1
+      [ atoms ]
+      1 P1 1 ALA BB 1
+      2 P1 1 ALA SC1 2
+      3 P1 1 ALA SC2 3
+      4 P1 1 ALA SC3 3
+      [ bonds ]
+      1 2 1 0.2 100
+      2 3 1 0.6 700
+      3 4 1 0.2 700
+      """,
+      np.array([[0.00, 0.0, 0.0],
+                [0.47, 0.0, 0.0],
+                [0.94, 0.0, 0.0],
+                [1.41, 0.0, 0.0]]),
+      0.9689298220201501),
+    ("""
+      [ moleculetype ]
+      GLY 1
+      [ atoms ]
+      1 P2 1 ALA BB 1
+      2 P1 1 ALA SC1 2
+      3 P2 1 ALA SC2 3
+      4 P1 1 ALA SC3 3
+      [ bonds ]
+      1 2 1 0.2 100
+      2 3 1 0.6 700
+      3 4 1 0.2 700
+      """,
+      np.array([[0.00, 0.0, 0.0],
+                [0.47, 0.0, 0.0],
+                [0.94, 0.0, 0.0],
+                [1.41, 0.0, 0.0]]),
+      0.861408729930223),
+     ("""
+      [ moleculetype ]
+      GLY 1
+      [ atoms ]
+      1 P1 1 ALA BB 1
+      2 P1 1 ALA SC1 2
+      3 P1 1 ALA SC2 3
+      4 P1 1 ALA SC3 3
+      [ bonds ]
+      1 2 1 0.2 100
+      2 3 1 0.6 700
+      [ virtual_sitesn ]
+      4 1 1
+      """,
+      np.array([[0.00, 0.0, 0.0],
+                [0.47, 0.0, 0.0],
+                [0.94, 0.0, 0.0],
+                [0.00, 0.0, 0.0]]),
+      0.8391178403537848),
+     ("""
+      [ moleculetype ]
+      GLY 1
+      [ atoms ]
+      1 P1 1 ALA BB 1
+      """,
+      np.array([[0.00, 0.0, 0.0]]),
+      0.47),
+])
+def test_compute_volume(lines, coords, volume):
+    meta_mol = polyply.MetaMolecule()
+    nonbond_params = {frozenset(["P1", "P1"]): {"nb1": 0.47, "nb2":0.5},
+                      frozenset(["P2", "P2"]): {"nb1": 0.23, "nb2":0.5},
+                      frozenset(["P2", "P1"]): {"nb1": 0.35, "nb2":0.5},}
+
+    lines = textwrap.dedent(lines).splitlines()
+    ff = vermouth.forcefield.ForceField(name='test_ff')
+    read_itp(lines, ff)
+    block = ff.blocks['GLY']
+    coord_dict = {node: coord for node, coord in zip(block.nodes, coords)}
+    new_vol = compute_volume(block, coord_dict, nonbond_params)
+    print(new_vol)
+    assert np.isclose(new_vol, volume, atol=0.000001)
```

### Comparing `polyply-1.6.1/polyply/tests/test_graph_utils.py` & `polyply-1.7.0/polyply/tests/test_graph_utils.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_itp_files.py` & `polyply-1.7.0/polyply/tests/test_itp_files.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_lib_files.py` & `polyply-1.7.0/polyply/tests/test_lib_files.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_linalg.py` & `polyply-1.7.0/polyply/tests/test_linalg.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_load_library.py` & `polyply-1.7.0/polyply/tests/test_load_library.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_logging.py` & `polyply-1.7.0/polyply/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_map_to_molecule.py` & `polyply-1.7.0/polyply/tests/test_map_to_molecule.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_meta_molecule.py` & `polyply-1.7.0/polyply/tests/test_meta_molecule.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_nb_engine.py` & `polyply-1.7.0/polyply/tests/test_nb_engine.py`

 * *Files 15% similar despite different names*

```diff
@@ -168,14 +168,39 @@
      nb_engine.positions[:, :] = np.ones((5, 3), dtype=float)[:, :]
      # then we update them in the molecules and check if they are actually updated
      nb_engine.update_positions_in_molecules(topology.molecules)
      for mol_idx, mol in enumerate(topology.molecules):
          for node in mol.nodes:
             assert all(mol.nodes[node]["position"] == np.array([1., 1., 1.]))
 
+@pytest.mark.parametrize('lp, point, ref_prob',(
+                        # low lp, 180 degree,
+                        (0.001, np.array([0., 0., 2.]), 0.00555833379629605),
+                        # low lp, 90 degree,
+                        (0.001, np.array([0., 1., 1.]), 0.005555555324073842),
+                        # low lp, close to zero angle,
+                        (0.001, np.array([0., 0., 0.1]), 0.00555833379629605),
+                        # high lp, 180 degree,
+                        (10, np.array([0., 0., 2.]), 0.05555807788838943),
+                        # high lp, 90 degree,
+                        (10, np.array([0., 1., 1.]), 0.00037434738418303014),
+                        # high lp, close to 0 degree,
+                        (10, np.array([0., 0., 0.1]), 3.3299656173078084e-06),))
+def test_compute_bending_probability(topology, lp, point, ref_prob):
+    # we add two fixed positions to the first molecule
+    positions = [np.array([0., 0., 0,]), np.array([0., 0., 1.])]
+    for node, position in zip([0, 1], positions):
+        topology.molecules[0].nodes[node]["position"] = position
+
+    nb_engine =  NonBondEngine.from_topology(topology.molecules,
+                                             topology,
+                                             box=np.array([10., 10., 10.]))
+    prob = nb_engine.compute_bending_probability(lp, point, 0, 1, 0)
+    assert prob == pytest.approx(ref_prob, abs=10**-5)
+
 @pytest.mark.parametrize('mol_idx_a, mol_idx_b, node_a, node_b, expected',
                         ((0, 0, 0, 1, (0.53+0.67)/2.0),
                          (0, 2, 0, 0, (0.43+0.53)/2.0),
                          (0, 2, 1, 0, (0.43+0.67)/2.0)))
 def test_get_interaction(topology, mol_idx_a, mol_idx_b, node_a, node_b, expected):
      # initiate the nb_engine
      nb_engine =  NonBondEngine.from_topology(topology.molecules,
```

### Comparing `polyply-1.6.1/polyply/tests/test_optimize_geometry.py` & `polyply-1.7.0/polyply/tests/test_optimize_geometry.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_persistence.py` & `polyply-1.7.0/polyply/tests/test_persistence.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_polyply_input.py` & `polyply-1.7.0/polyply/tests/test_polyply_input.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_random_walk.py` & `polyply-1.7.0/polyply/tests/test_random_walk.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 Test that force field files are properly read.
 """
 import math
 import pytest
+import random
 import numpy as np
 from numpy.linalg import norm
 import networkx as nx
 import polyply
 from polyply import TEST_DATA
 from polyply.src.topology import Topology
 from polyply.src.nonbond_engine import NonBondEngine
@@ -184,14 +185,41 @@
 def test_is_overlap(nonbond_matrix, molecule, new_point, result):
     nb_matrix = add_positions(nonbond_matrix, 6)
     proccessor = RandomWalk(mol_idx=0, nonbond_matrix=nb_matrix)
     proccessor.molecule = molecule
     # node 4 is already placed and hence is skipped over
     assert proccessor._is_overlap(new_point, 7, nrexcl=1) == result
 
+@pytest.mark.parametrize('n_coords, new_point, prev_prob, lp, result', (
+    # only 1 previous node -> always True
+    (1, None, 1, 10, True,),
+    # no lp is given -> always True
+    (1, None, 1, None, True,),
+    # 180 degrees should be fine even with high prev prob
+    (2, np.array([1., 1., 1.11]), 1, 10, True),
+    # small angle and prev prob high
+    (2, np.array([1., 1.47, 0.1]), 1., 10, False),
+    # small angle and prev prob low
+    (2, np.array([1., 1.47, 0.1]), 0., 10, True),
+    # medium angle, prev prob high, unifrom prob low
+    (2, np.array([1., 1.57, 1.74]), 1., 10, True),
+))
+def test_bendiness(nonbond_matrix, molecule, n_coords, new_point, prev_prob, lp, result):
+    # set random seed for reproducability
+    random.seed(1)
+    nb_matrix = add_positions(nonbond_matrix, n_coords)
+    # the bending constant for a series of PEO monomers
+    # the value is the same as in the high test case from
+    # test nb matrix
+    nb_matrix.bending_matrix = {("PEO", "PEO", "PEO"): lp}
+    processor = RandomWalk(mol_idx=0, nonbond_matrix=nb_matrix)
+    processor.molecule = molecule
+    processor.prev_prob = prev_prob
+    assert processor.bendiness(new_point, n_coords) == result
+
 @pytest.mark.parametrize('new_point, restraint, result', (
    # distance restraint true upper_bound
    # ref_node, upper_bound, lower_bound
    (np.array([1., 1., 2.96]),
    [(0, 4.0, 0.0)],
     True
    ),
```

### Comparing `polyply-1.6.1/polyply/tests/test_residue_check.py` & `polyply-1.7.0/polyply/tests/test_residue_check.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_restraints.py` & `polyply-1.7.0/polyply/tests/test_restraints.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_simple_seq_parsers.py` & `polyply-1.7.0/polyply/tests/test_simple_seq_parsers.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_top_parser.py` & `polyply-1.7.0/polyply/tests/test_top_parser.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_topology.py` & `polyply-1.7.0/polyply/tests/test_topology.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply/tests/test_vs_builder.py` & `polyply-1.7.0/polyply/tests/test_vs_builder.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/polyply.egg-info/PKG-INFO` & `polyply-1.7.0/polyply.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyply
-Version: 1.6.1
+Version: 1.7.0
 Home-page: https://github.com/marrink-lab/polyply_1.0
 Author: Fabian Grunewald
 Author-email: f.grunewald@rug.nl
 License: Apache 2.0
 Keywords: molecular dynamics charmm gromos martini polymers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `polyply-1.6.1/polyply.egg-info/SOURCES.txt` & `polyply-1.7.0/polyply.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -236,16 +236,15 @@
 polyply/tests/test_data/library_tests/martini3/PDMS/polyply/command
 polyply/tests/test_data/library_tests/martini3/PE/polyply/PE.itp
 polyply/tests/test_data/library_tests/martini3/PE/polyply/command
 polyply/tests/test_data/library_tests/martini3/PEO/polyply/PEO.itp
 polyply/tests/test_data/library_tests/martini3/PEO/polyply/command
 polyply/tests/test_data/library_tests/martini3/PPE/polyply/PPE.itp
 polyply/tests/test_data/library_tests/martini3/PPE/polyply/command
-polyply/tests/test_data/library_tests/martini3/PROT/init.itp
-polyply/tests/test_data/library_tests/martini3/PROT/lysozyme_seq.json
+polyply/tests/test_data/library_tests/martini3/PROT/PNt.fasta
 polyply/tests/test_data/library_tests/martini3/PROT/polyply/PROT.itp
 polyply/tests/test_data/library_tests/martini3/PROT/polyply/command
 polyply/tests/test_data/library_tests/martini3/PS/polyply/PS.itp
 polyply/tests/test_data/library_tests/martini3/PS/polyply/command
 polyply/tests/test_data/library_tests/martini3/PTMA/polyply/PTMA.itp
 polyply/tests/test_data/library_tests/martini3/PTMA/polyply/command
 polyply/tests/test_data/library_tests/oplsaaLigParGen/PEO/polyply/PEO.itp
```

### Comparing `polyply-1.6.1/run_pylint.py` & `polyply-1.7.0/run_pylint.py`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/setup.cfg` & `polyply-1.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `polyply-1.6.1/setup.py` & `polyply-1.7.0/setup.py`

 * *Files identical despite different names*

