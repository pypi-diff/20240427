# Comparing `tmp/pyg_nightly-2.6.0.dev20240425.tar.gz` & `tmp/pyg_nightly-2.6.0.dev20240426.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyg_nightly-2.6.0.dev20240425.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyg_nightly-2.6.0.dev20240426.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyg_nightly-2.6.0.dev20240425.tar` & `pyg_nightly-2.6.0.dev20240426.tar`

### file list

```diff
@@ -1,609 +1,609 @@
--rw-r--r--   0        0        0    61057 2024-04-25 06:12:17.426540 pyg_nightly-2.6.0.dev20240425/README.md
--rw-r--r--   0        0        0     5269 2024-04-25 06:12:17.842535 pyg_nightly-2.6.0.dev20240425/pyproject.toml
--rw-r--r--   0        0        0     1209 2024-04-25 06:12:17.838535 pyg_nightly-2.6.0.dev20240425/torch_geometric/__init__.py
--rw-r--r--   0        0        0     1053 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/_compile.py
--rw-r--r--   0        0        0     1575 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/backend.py
--rw-r--r--   0        0        0    16514 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/config_store.py
--rw-r--r--   0        0        0      352 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/contrib/__init__.py
--rw-r--r--   0        0        0       23 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/contrib/datasets/__init__.py
--rw-r--r--   0        0        0      396 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/contrib/explain/__init__.py
--rw-r--r--   0        0        0    16972 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/contrib/explain/pgm_explainer.py
--rw-r--r--   0        0        0       72 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/contrib/nn/__init__.py
--rw-r--r--   0        0        0       23 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/contrib/nn/conv/__init__.py
--rw-r--r--   0        0        0      113 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/contrib/nn/models/__init__.py
--rw-r--r--   0        0        0    33280 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/contrib/nn/models/rbcd_attack.py
--rw-r--r--   0        0        0       23 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/contrib/transforms/__init__.py
--rw-r--r--   0        0        0     3882 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/data/__init__.py
--rw-r--r--   0        0        0     8767 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/data/batch.py
--rw-r--r--   0        0        0    12471 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/data/collate.py
--rw-r--r--   0        0        0    43328 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/data/data.py
--rw-r--r--   0        0        0    21267 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/data/database.py
--rw-r--r--   0        0        0     3083 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/data/datapipes.py
--rw-r--r--   0        0        0    16402 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/data/dataset.py
--rw-r--r--   0        0        0     1889 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/data/download.py
--rw-r--r--   0        0        0     2324 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/data/extract.py
--rw-r--r--   0        0        0    20205 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/data/feature_store.py
--rw-r--r--   0        0        0    13926 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/data/graph_store.py
--rw-r--r--   0        0        0    47550 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/data/hetero_data.py
--rw-r--r--   0        0        0     8294 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/data/hypergraph_data.py
--rw-r--r--   0        0        0    13513 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/data/in_memory_dataset.py
--rw-r--r--   0        0        0      178 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/data/lightning/__init__.py
--rw-r--r--   0        0        0    29244 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/data/lightning/datamodule.py
--rw-r--r--   0        0        0      463 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/data/makedirs.py
--rw-r--r--   0        0        0     6629 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/data/on_disk_dataset.py
--rw-r--r--   0        0        0     4503 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/data/remote_backend_utils.py
--rw-r--r--   0        0        0     5319 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/data/separate.py
--rw-r--r--   0        0        0    31582 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/data/storage.py
--rw-r--r--   0        0        0     5375 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/data/summary.py
--rw-r--r--   0        0        0    10055 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/data/temporal.py
--rw-r--r--   0        0        0     1089 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/data/view.py
--rw-r--r--   0        0        0     5770 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/__init__.py
--rw-r--r--   0        0        0     4471 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/actor.py
--rw-r--r--   0        0        0     5666 2024-04-25 06:12:17.486539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/airfrans.py
--rw-r--r--   0        0        0     3913 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/airports.py
--rw-r--r--   0        0        0     3179 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/amazon.py
--rw-r--r--   0        0        0     3362 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/amazon_book.py
--rw-r--r--   0        0        0     3964 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/amazon_products.py
--rw-r--r--   0        0        0     5178 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/aminer.py
--rw-r--r--   0        0        0     5455 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/aqsol.py
--rw-r--r--   0        0        0     5975 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/attributed_graph_dataset.py
--rw-r--r--   0        0        0     4258 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/ba2motif_dataset.py
--rw-r--r--   0        0        0     3700 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/ba_multi_shapes.py
--rw-r--r--   0        0        0     3904 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/ba_shapes.py
--rw-r--r--   0        0        0     4404 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/bitcoin_otc.py
--rw-r--r--   0        0        0     3959 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/brca_tgca.py
--rw-r--r--   0        0        0     4458 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/citation_full.py
--rw-r--r--   0        0        0     3138 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/coauthor.py
--rw-r--r--   0        0        0     4734 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/coma.py
--rw-r--r--   0        0        0     5311 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/cornell.py
--rw-r--r--   0        0        0     5416 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/dblp.py
--rw-r--r--   0        0        0     5707 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/dbp15k.py
--rw-r--r--   0        0        0     2511 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/deezer_europe.py
--rw-r--r--   0        0        0     4035 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/dgraph.py
--rw-r--r--   0        0        0     6041 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/dynamic_faust.py
--rw-r--r--   0        0        0     4605 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/elliptic.py
--rw-r--r--   0        0        0     3188 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/elliptic_temporal.py
--rw-r--r--   0        0        0     2834 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/email_eu_core.py
--rw-r--r--   0        0        0     7356 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/entities.py
--rw-r--r--   0        0        0     6103 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/explainer_dataset.py
--rw-r--r--   0        0        0     2431 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/facebook.py
--rw-r--r--   0        0        0    10554 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/fake.py
--rw-r--r--   0        0        0     4076 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/faust.py
--rw-r--r--   0        0        0     3964 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/flickr.py
--rw-r--r--   0        0        0     4080 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/freebase.py
--rw-r--r--   0        0        0     3598 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/gdelt.py
--rw-r--r--   0        0        0     3189 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/gdelt_lite.py
--rw-r--r--   0        0        0     9511 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/ged_dataset.py
--rw-r--r--   0        0        0     2820 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/gemsec.py
--rw-r--r--   0        0        0     4223 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/geometry.py
--rw-r--r--   0        0        0     2687 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/github.py
--rw-r--r--   0        0        0     6940 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/gnn_benchmark_dataset.py
--rw-r--r--   0        0        0      272 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/graph_generator/__init__.py
--rw-r--r--   0        0        0      965 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/graph_generator/ba_graph.py
--rw-r--r--   0        0        0      939 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/graph_generator/base.py
--rw-r--r--   0        0        0      918 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/graph_generator/er_graph.py
--rw-r--r--   0        0        0     1159 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/graph_generator/grid_graph.py
--rw-r--r--   0        0        0     2599 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/graph_generator/tree_graph.py
--rw-r--r--   0        0        0     4224 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/heterophilous_graph_dataset.py
--rw-r--r--   0        0        0     8846 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/hgb_dataset.py
--rw-r--r--   0        0        0     6763 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/hm.py
--rw-r--r--   0        0        0    11417 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/hydro_net.py
--rw-r--r--   0        0        0     4735 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/icews.py
--rw-r--r--   0        0        0     4611 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/igmc_dataset.py
--rw-r--r--   0        0        0     4223 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/imdb.py
--rw-r--r--   0        0        0     7293 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/infection_dataset.py
--rw-r--r--   0        0        0     3643 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/jodie.py
--rw-r--r--   0        0        0     3445 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/karate.py
--rw-r--r--   0        0        0     4572 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/last_fm.py
--rw-r--r--   0        0        0     2486 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/lastfm_asia.py
--rw-r--r--   0        0        0     6864 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/linkx_dataset.py
--rw-r--r--   0        0        0    11746 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/lrgb.py
--rw-r--r--   0        0        0     5244 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/malnet_tiny.py
--rw-r--r--   0        0        0    16734 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/md17.py
--rw-r--r--   0        0        0     3951 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/mixhop_synthetic_dataset.py
--rw-r--r--   0        0        0     3317 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/mnist_superpixels.py
--rw-r--r--   0        0        0     5347 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/modelnet.py
--rw-r--r--   0        0        0     7177 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/molecule_net.py
--rw-r--r--   0        0        0      272 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/motif_generator/__init__.py
--rw-r--r--   0        0        0      900 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/motif_generator/base.py
--rw-r--r--   0        0        0     1278 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/motif_generator/custom.py
--rw-r--r--   0        0        0      983 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/motif_generator/cycle.py
--rw-r--r--   0        0        0     1099 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/motif_generator/grid.py
--rw-r--r--   0        0        0      814 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/motif_generator/house.py
--rw-r--r--   0        0        0     4033 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/movie_lens.py
--rw-r--r--   0        0        0     6057 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/movie_lens_100k.py
--rw-r--r--   0        0        0     5396 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/movie_lens_1m.py
--rw-r--r--   0        0        0     3008 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/myket.py
--rw-r--r--   0        0        0     2863 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/nell.py
--rw-r--r--   0        0        0     5181 2024-04-25 06:12:17.490539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/neurograph.py
--rw-r--r--   0        0        0     7481 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/ogb_mag.py
--rw-r--r--   0        0        0     3585 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/omdb.py
--rw-r--r--   0        0        0     5161 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/ose_gvcs.py
--rw-r--r--   0        0        0     4162 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/particle.py
--rw-r--r--   0        0        0    12041 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/pascal.py
--rw-r--r--   0        0        0     4791 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/pascal_pf.py
--rw-r--r--   0        0        0     5897 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/pcpnet_dataset.py
--rw-r--r--   0        0        0     4207 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/pcqm4m.py
--rw-r--r--   0        0        0     7201 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/planetoid.py
--rw-r--r--   0        0        0     3045 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/polblogs.py
--rw-r--r--   0        0        0     4999 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/ppi.py
--rw-r--r--   0        0        0     3325 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/qm7.py
--rw-r--r--   0        0        0    17158 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/qm9.py
--rw-r--r--   0        0        0     5304 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/rcdd.py
--rw-r--r--   0        0        0     3122 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/reddit.py
--rw-r--r--   0        0        0     4282 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/reddit2.py
--rw-r--r--   0        0        0     4535 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/rel_link_pred_dataset.py
--rw-r--r--   0        0        0     4492 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/s3dis.py
--rw-r--r--   0        0        0     8816 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/sbm_dataset.py
--rw-r--r--   0        0        0     8504 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/shapenet.py
--rw-r--r--   0        0        0     6316 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/shrec2016.py
--rw-r--r--   0        0        0     9433 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/snap_dataset.py
--rw-r--r--   0        0        0     3278 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/suite_sparse.py
--rw-r--r--   0        0        0     4170 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/taobao.py
--rw-r--r--   0        0        0     4632 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/tosca.py
--rw-r--r--   0        0        0     7847 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/tu_dataset.py
--rw-r--r--   0        0        0     3658 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/twitch.py
--rw-r--r--   0        0        0     7001 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/upfd.py
--rw-r--r--   0        0        0      182 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/utils/__init__.py
--rw-r--r--   0        0        0     1835 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/utils/cheatsheet.py
--rw-r--r--   0        0        0     4889 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/webkb.py
--rw-r--r--   0        0        0     3884 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/wikics.py
--rw-r--r--   0        0        0     4947 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/wikidata.py
--rw-r--r--   0        0        0     6640 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/wikipedia_network.py
--rw-r--r--   0        0        0     7028 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/willow_object_class.py
--rw-r--r--   0        0        0     8158 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/word_net.py
--rw-r--r--   0        0        0     3959 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/yelp.py
--rw-r--r--   0        0        0     6347 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/zinc.py
--rw-r--r--   0        0        0     1295 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/debug.py
--rw-r--r--   0        0        0      858 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/deprecation.py
--rw-r--r--   0        0        0      589 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/distributed/__init__.py
--rw-r--r--   0        0        0      418 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/distributed/dist_context.py
--rw-r--r--   0        0        0     4933 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/distributed/dist_link_neighbor_loader.py
--rw-r--r--   0        0        0     6492 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/distributed/dist_loader.py
--rw-r--r--   0        0        0     4372 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/distributed/dist_neighbor_loader.py
--rw-r--r--   0        0        0    42406 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/distributed/dist_neighbor_sampler.py
--rw-r--r--   0        0        0     3309 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/distributed/event_loop.py
--rw-r--r--   0        0        0    19018 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/distributed/local_feature_store.py
--rw-r--r--   0        0        0     8408 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/distributed/local_graph_store.py
--rw-r--r--   0        0        0    14675 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/distributed/partition.py
--rw-r--r--   0        0        0     5753 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/distributed/rpc.py
--rw-r--r--   0        0        0     6567 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/distributed/utils.py
--rw-r--r--   0        0        0    64183 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/edge_index.py
--rw-r--r--   0        0        0     4756 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/experimental.py
--rw-r--r--   0        0        0      359 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/__init__.py
--rw-r--r--   0        0        0      496 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/algorithm/__init__.py
--rw-r--r--   0        0        0     4545 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/algorithm/attention_explainer.py
--rw-r--r--   0        0        0     6935 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/algorithm/base.py
--rw-r--r--   0        0        0    12857 2024-04-25 06:12:17.494539 pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/algorithm/captum.py
--rw-r--r--   0        0        0     7346 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/algorithm/captum_explainer.py
--rw-r--r--   0        0        0     2872 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/algorithm/dummy_explainer.py
--rw-r--r--   0        0        0    12454 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/algorithm/gnn_explainer.py
--rw-r--r--   0        0        0    21367 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/algorithm/graphmask_explainer.py
--rw-r--r--   0        0        0    10371 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/algorithm/pg_explainer.py
--rw-r--r--   0        0        0     2564 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/algorithm/utils.py
--rw-r--r--   0        0        0     7834 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/config.py
--rw-r--r--   0        0        0    10667 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/explainer.py
--rw-r--r--   0        0        0    14934 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/explanation.py
--rw-r--r--   0        0        0      301 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/metric/__init__.py
--rw-r--r--   0        0        0     1888 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/metric/basic.py
--rw-r--r--   0        0        0     3063 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/metric/faithfulness.py
--rw-r--r--   0        0        0     6157 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/metric/fidelity.py
--rw-r--r--   0        0        0     1815 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/__init__.py
--rw-r--r--   0        0        0      510 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/benchmark.py
--rw-r--r--   0        0        0     2371 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/checkpoint.py
--rw-r--r--   0        0        0      738 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/cmd_args.py
--rw-r--r--   0        0        0    17197 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/config.py
--rw-r--r--   0        0        0      389 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/contrib/__init__.py
--rw-r--r--   0        0        0      221 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/contrib/act/__init__.py
--rw-r--r--   0        0        0      221 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/contrib/config/__init__.py
--rw-r--r--   0        0        0      221 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/contrib/encoder/__init__.py
--rw-r--r--   0        0        0      221 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/contrib/head/__init__.py
--rw-r--r--   0        0        0      221 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/contrib/layer/__init__.py
--rw-r--r--   0        0        0     8435 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/contrib/layer/generalconv.py
--rw-r--r--   0        0        0      221 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/contrib/loader/__init__.py
--rw-r--r--   0        0        0      221 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/contrib/loss/__init__.py
--rw-r--r--   0        0        0      221 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/contrib/network/__init__.py
--rw-r--r--   0        0        0      221 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/contrib/optimizer/__init__.py
--rw-r--r--   0        0        0      221 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/contrib/pooling/__init__.py
--rw-r--r--   0        0        0      221 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/contrib/stage/__init__.py
--rw-r--r--   0        0        0      221 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/contrib/train/__init__.py
--rw-r--r--   0        0        0      221 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/contrib/transform/__init__.py
--rw-r--r--   0        0        0      375 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/imports.py
--rw-r--r--   0        0        0      521 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/init.py
--rw-r--r--   0        0        0    11605 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/loader.py
--rw-r--r--   0        0        0    11314 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/logger.py
--rw-r--r--   0        0        0     1445 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/loss.py
--rw-r--r--   0        0        0     3110 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/model_builder.py
--rw-r--r--   0        0        0     1121 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/models/__init__.py
--rw-r--r--   0        0        0      855 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/models/act.py
--rw-r--r--   0        0        0     3034 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/models/encoder.py
--rw-r--r--   0        0        0     6373 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/models/gnn.py
--rw-r--r--   0        0        0     4603 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/models/head.py
--rw-r--r--   0        0        0    12500 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/models/layer.py
--rw-r--r--   0        0        0      288 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/models/pooling.py
--rw-r--r--   0        0        0     1383 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/models/transform.py
--rw-r--r--   0        0        0     2544 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/optim.py
--rw-r--r--   0        0        0     3954 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/register.py
--rw-r--r--   0        0        0     2653 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/train.py
--rw-r--r--   0        0        0        0 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/utils/LICENSE
--rw-r--r--   0        0        0      641 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/utils/__init__.py
--rw-r--r--   0        0        0     9349 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/utils/agg_runs.py
--rw-r--r--   0        0        0     3045 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/utils/comp_budget.py
--rw-r--r--   0        0        0     1342 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/utils/device.py
--rw-r--r--   0        0        0      690 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/utils/epoch.py
--rw-r--r--   0        0        0     2049 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/utils/io.py
--rw-r--r--   0        0        0      624 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/utils/plot.py
--rw-r--r--   0        0        0      199 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/utils/tools.py
--rw-r--r--   0        0        0      790 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/home.py
--rw-r--r--   0        0        0    19216 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/inspector.py
--rw-r--r--   0        0        0      528 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/io/__init__.py
--rw-r--r--   0        0        0     6567 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/io/fs.py
--rw-r--r--   0        0        0     1177 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/io/npz.py
--rw-r--r--   0        0        0     1088 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/io/obj.py
--rw-r--r--   0        0        0     2762 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/io/off.py
--rw-r--r--   0        0        0     4667 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/io/planetoid.py
--rw-r--r--   0        0        0      489 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/io/ply.py
--rw-r--r--   0        0        0     1170 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/io/sdf.py
--rw-r--r--   0        0        0     4918 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/io/tu.py
--rw-r--r--   0        0        0      910 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/io/txt_array.py
--rw-r--r--   0        0        0      935 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/isinstance.py
--rw-r--r--   0        0        0      908 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/lazy_loader.py
--rw-r--r--   0        0        0     1835 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/__init__.py
--rw-r--r--   0        0        0     1615 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/base.py
--rw-r--r--   0        0        0     2106 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/cache.py
--rw-r--r--   0        0        0    13196 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/cluster.py
--rw-r--r--   0        0        0     1459 2024-04-25 06:12:17.498539 pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/data_list_loader.py
--rw-r--r--   0        0        0     3527 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/dataloader.py
--rw-r--r--   0        0        0     1685 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/dense_data_loader.py
--rw-r--r--   0        0        0     4163 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/dynamic_batch_sampler.py
--rw-r--r--   0        0        0     8448 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/graph_saint.py
--rw-r--r--   0        0        0     6012 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/hgt_loader.py
--rw-r--r--   0        0        0    31462 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/ibmb_loader.py
--rw-r--r--   0        0        0     3754 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/imbalanced_sampler.py
--rw-r--r--   0        0        0    16207 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/link_loader.py
--rw-r--r--   0        0        0    14383 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/link_neighbor_loader.py
--rw-r--r--   0        0        0    10931 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/mixin.py
--rw-r--r--   0        0        0    12452 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/neighbor_loader.py
--rw-r--r--   0        0        0     8513 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/neighbor_sampler.py
--rw-r--r--   0        0        0    11848 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/node_loader.py
--rw-r--r--   0        0        0     3236 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/prefetch.py
--rw-r--r--   0        0        0     2196 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/random_node_loader.py
--rw-r--r--   0        0        0     4173 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/shadow.py
--rw-r--r--   0        0        0     2248 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/temporal_dataloader.py
--rw-r--r--   0        0        0    14818 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/utils.py
--rw-r--r--   0        0        0     3518 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/zip_loader.py
--rw-r--r--   0        0        0      858 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/logging.py
--rw-r--r--   0        0        0      296 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/metrics/__init__.py
--rw-r--r--   0        0        0     7521 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/metrics/link_pred.py
--rw-r--r--   0        0        0      847 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/__init__.py
--rw-r--r--   0        0        0     1551 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/__init__.py
--rw-r--r--   0        0        0     3003 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/attention.py
--rw-r--r--   0        0        0     8230 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/base.py
--rw-r--r--   0        0        0    11011 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/basic.py
--rw-r--r--   0        0        0     2650 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/deep_sets.py
--rw-r--r--   0        0        0     6639 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/equilibrium.py
--rw-r--r--   0        0        0    12276 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/fused.py
--rw-r--r--   0        0        0     3801 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/gmt.py
--rw-r--r--   0        0        0     2193 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/gru.py
--rw-r--r--   0        0        0     4190 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/lcm.py
--rw-r--r--   0        0        0     2214 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/lstm.py
--rw-r--r--   0        0        0     2514 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/mlp.py
--rw-r--r--   0        0        0     8170 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/multi.py
--rw-r--r--   0        0        0     6189 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/quantile.py
--rw-r--r--   0        0        0     4638 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/scaler.py
--rw-r--r--   0        0        0     2446 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/set2set.py
--rw-r--r--   0        0        0     4207 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/set_transformer.py
--rw-r--r--   0        0        0     2507 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/sort.py
--rw-r--r--   0        0        0     8338 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/utils.py
--rw-r--r--   0        0        0     1126 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/variance_preserving.py
--rw-r--r--   0        0        0       76 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/attention/__init__.py
--rw-r--r--   0        0        0     7357 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/attention/performer.py
--rw-r--r--   0        0        0     3515 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/__init__.py
--rw-r--r--   0        0        0     3077 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/agnn_conv.py
--rw-r--r--   0        0        0     4387 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/antisymmetric_conv.py
--rw-r--r--   0        0        0     5983 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/appnp.py
--rw-r--r--   0        0        0     6585 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/arma_conv.py
--rw-r--r--   0        0        0     4014 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/cg_conv.py
--rw-r--r--   0        0        0     6423 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/cheb_conv.py
--rw-r--r--   0        0        0     5255 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/cluster_gcn_conv.py
--rw-r--r--   0        0        0     5648 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/collect.jinja
--rw-r--r--   0        0        0      251 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/cugraph/__init__.py
--rw-r--r--   0        0        0     6364 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/cugraph/base.py
--rw-r--r--   0        0        0     2874 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/cugraph/gat_conv.py
--rw-r--r--   0        0        0     4002 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/cugraph/rgcn_conv.py
--rw-r--r--   0        0        0     2830 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/cugraph/sage_conv.py
--rw-r--r--   0        0        0     2440 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/dir_gnn_conv.py
--rw-r--r--   0        0        0    12241 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/dna_conv.py
--rw-r--r--   0        0        0     5389 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/edge_conv.py
--rw-r--r--   0        0        0     2216 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/edge_updater.jinja
--rw-r--r--   0        0        0    10742 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/eg_conv.py
--rw-r--r--   0        0        0     9065 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/fa_conv.py
--rw-r--r--   0        0        0     4430 2024-04-25 06:12:17.502539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/feast_conv.py
--rw-r--r--   0        0        0     6314 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/film_conv.py
--rw-r--r--   0        0        0     4502 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/fused_gat_conv.py
--rw-r--r--   0        0        0    16091 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/gat_conv.py
--rw-r--r--   0        0        0     3518 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/gated_graph_conv.py
--rw-r--r--   0        0        0    13639 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/gatv2_conv.py
--rw-r--r--   0        0        0     7001 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/gcn2_conv.py
--rw-r--r--   0        0        0    10415 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/gcn_conv.py
--rw-r--r--   0        0        0     9722 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/gen_conv.py
--rw-r--r--   0        0        0     7591 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/general_conv.py
--rw-r--r--   0        0        0     7411 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/gin_conv.py
--rw-r--r--   0        0        0     8315 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/gmm_conv.py
--rw-r--r--   0        0        0     6672 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/gps_conv.py
--rw-r--r--   0        0        0     3905 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/graph_conv.py
--rw-r--r--   0        0        0     4951 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/gravnet_conv.py
--rw-r--r--   0        0        0     7198 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/han_conv.py
--rw-r--r--   0        0        0     6084 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/heat_conv.py
--rw-r--r--   0        0        0     6555 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/hetero_conv.py
--rw-r--r--   0        0        0     9043 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/hgt_conv.py
--rw-r--r--   0        0        0     8691 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/hypergraph_conv.py
--rw-r--r--   0        0        0     3494 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/le_conv.py
--rw-r--r--   0        0        0     2369 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/lg_conv.py
--rw-r--r--   0        0        0    43545 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/message_passing.py
--rw-r--r--   0        0        0     4340 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/mf_conv.py
--rw-r--r--   0        0        0     4554 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/mixhop_conv.py
--rw-r--r--   0        0        0     4759 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/nn_conv.py
--rw-r--r--   0        0        0     4908 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/pan_conv.py
--rw-r--r--   0        0        0     4892 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/pdn_conv.py
--rw-r--r--   0        0        0     8325 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/pna_conv.py
--rw-r--r--   0        0        0     4508 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/point_conv.py
--rw-r--r--   0        0        0     3278 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/point_gnn_conv.py
--rw-r--r--   0        0        0     5878 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/point_transformer_conv.py
--rw-r--r--   0        0        0     5363 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/ppf_conv.py
--rw-r--r--   0        0        0     7374 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/propagate.jinja
--rw-r--r--   0        0        0     5217 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/res_gated_graph_conv.py
--rw-r--r--   0        0        0    22863 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/rgat_conv.py
--rw-r--r--   0        0        0    15705 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/rgcn_conv.py
--rw-r--r--   0        0        0     5812 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/sage_conv.py
--rw-r--r--   0        0        0     4543 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/sg_conv.py
--rw-r--r--   0        0        0     6190 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/signed_conv.py
--rw-r--r--   0        0        0     3888 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/simple_conv.py
--rw-r--r--   0        0        0     6314 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/spline_conv.py
--rw-r--r--   0        0        0     5131 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/ssg_conv.py
--rw-r--r--   0        0        0    12420 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/supergat_conv.py
--rw-r--r--   0        0        0     4164 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/tag_conv.py
--rw-r--r--   0        0        0    10407 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/transformer_conv.py
--rw-r--r--   0        0        0      852 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/utils/__init__.py
--rw-r--r--   0        0        0     2792 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/utils/cheatsheet.py
--rw-r--r--   0        0        0     3140 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/wl_conv.py
--rw-r--r--   0        0        0     2777 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/wl_conv_continuous.py
--rw-r--r--   0        0        0     5956 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/x_conv.py
--rw-r--r--   0        0        0     4764 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/data_parallel.py
--rw-r--r--   0        0        0      847 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/dense/__init__.py
--rw-r--r--   0        0        0     4238 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/dense/dense_gat_conv.py
--rw-r--r--   0        0        0     3002 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/dense/dense_gcn_conv.py
--rw-r--r--   0        0        0     2361 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/dense/dense_gin_conv.py
--rw-r--r--   0        0        0     2751 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/dense/dense_graph_conv.py
--rw-r--r--   0        0        0     2672 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/dense/dense_sage_conv.py
--rw-r--r--   0        0        0     3051 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/dense/diff_pool.py
--rw-r--r--   0        0        0     6115 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/dense/dmon_pool.py
--rw-r--r--   0        0        0    17702 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/dense/linear.py
--rw-r--r--   0        0        0     4111 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/dense/mincut_pool.py
--rw-r--r--   0        0        0     3115 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/encoding.py
--rw-r--r--   0        0        0      129 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/functional/__init__.py
--rw-r--r--   0        0        0     1549 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/functional/bro.py
--rw-r--r--   0        0        0      863 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/functional/gini.py
--rw-r--r--   0        0        0    16055 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/fx.py
--rw-r--r--   0        0        0     1088 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/glob.py
--rw-r--r--   0        0        0     2457 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/inits.py
--rw-r--r--   0        0        0      290 2024-04-25 06:12:17.506539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/kge/__init__.py
--rw-r--r--   0        0        0     5902 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/kge/base.py
--rw-r--r--   0        0        0     3234 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/kge/complex.py
--rw-r--r--   0        0        0     2462 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/kge/distmult.py
--rw-r--r--   0        0        0      771 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/kge/loader.py
--rw-r--r--   0        0        0     3208 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/kge/rotate.py
--rw-r--r--   0        0        0     3088 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/kge/transe.py
--rw-r--r--   0        0        0     8937 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/lr_scheduler.py
--rw-r--r--   0        0        0     9512 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/model_hub.py
--rw-r--r--   0        0        0     1909 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/__init__.py
--rw-r--r--   0        0        0     6634 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/attentive_fp.py
--rw-r--r--   0        0        0    10770 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/autoencoder.py
--rw-r--r--   0        0        0    31225 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/basic_gnn.py
--rw-r--r--   0        0        0     3971 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/captum.py
--rw-r--r--   0        0        0     6827 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/correct_and_smooth.py
--rw-r--r--   0        0        0     4197 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/deep_graph_infomax.py
--rw-r--r--   0        0        0     4339 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/deepgcn.py
--rw-r--r--   0        0        0    36186 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/dimenet.py
--rw-r--r--   0        0        0     5107 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/dimenet_utils.py
--rw-r--r--   0        0        0     7873 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/gnnff.py
--rw-r--r--   0        0        0     9246 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/graph_mixer.py
--rw-r--r--   0        0        0     5395 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/graph_unet.py
--rw-r--r--   0        0        0     3450 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/jumping_knowledge.py
--rw-r--r--   0        0        0     3908 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/label_prop.py
--rw-r--r--   0        0        0    12465 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/lightgcn.py
--rw-r--r--   0        0        0     5812 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/linkx.py
--rw-r--r--   0        0        0     2580 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/mask_label.py
--rw-r--r--   0        0        0     6540 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/meta.py
--rw-r--r--   0        0        0    10870 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/metapath2vec.py
--rw-r--r--   0        0        0    10315 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/mlp.py
--rw-r--r--   0        0        0     2378 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/neural_fingerprint.py
--rw-r--r--   0        0        0     7731 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/node2vec.py
--rw-r--r--   0        0        0     3538 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/pmlp.py
--rw-r--r--   0        0        0     8986 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/re_net.py
--rw-r--r--   0        0        0     2808 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/rect.py
--rw-r--r--   0        0        0    11796 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/rev_gnn.py
--rw-r--r--   0        0        0    16619 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/schnet.py
--rw-r--r--   0        0        0     9839 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/signed_gcn.py
--rw-r--r--   0        0        0    11878 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/tgn.py
--rw-r--r--   0        0        0    43192 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/visnet.py
--rw-r--r--   0        0        0     2373 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/module_dict.py
--rw-r--r--   0        0        0      669 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/norm/__init__.py
--rw-r--r--   0        0        0     8283 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/norm/batch_norm.py
--rw-r--r--   0        0        0     4722 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/norm/diff_group_norm.py
--rw-r--r--   0        0        0     2727 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/norm/graph_norm.py
--rw-r--r--   0        0        0     1491 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/norm/graph_size_norm.py
--rw-r--r--   0        0        0     4685 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/norm/instance_norm.py
--rw-r--r--   0        0        0     7831 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/norm/layer_norm.py
--rw-r--r--   0        0        0     1322 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/norm/mean_subtraction_norm.py
--rw-r--r--   0        0        0     1662 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/norm/msg_norm.py
--rw-r--r--   0        0        0     2824 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/norm/pair_norm.py
--rw-r--r--   0        0        0     2410 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/parameter_dict.py
--rw-r--r--   0        0        0    14129 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/__init__.py
--rw-r--r--   0        0        0     3967 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/approx_knn.py
--rw-r--r--   0        0        0     6683 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/asap.py
--rw-r--r--   0        0        0     3966 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/avg_pool.py
--rw-r--r--   0        0        0      287 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/connect/__init__.py
--rw-r--r--   0        0        0     4094 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/connect/base.py
--rw-r--r--   0        0        0     2190 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/connect/filter_edges.py
--rw-r--r--   0        0        0      273 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/consecutive.py
--rw-r--r--   0        0        0     1601 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/decimation.py
--rw-r--r--   0        0        0     8581 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/edge_pool.py
--rw-r--r--   0        0        0     3492 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/glob.py
--rw-r--r--   0        0        0     1291 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/graclus.py
--rw-r--r--   0        0        0    11343 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/knn.py
--rw-r--r--   0        0        0     4262 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/max_pool.py
--rw-r--r--   0        0        0     5377 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/mem_pool.py
--rw-r--r--   0        0        0     4366 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/pan_pool.py
--rw-r--r--   0        0        0      737 2024-04-25 06:12:17.510539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/pool.py
--rw-r--r--   0        0        0     5838 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/sag_pool.py
--rw-r--r--   0        0        0      254 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/select/__init__.py
--rw-r--r--   0        0        0     3311 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/select/base.py
--rw-r--r--   0        0        0     5305 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/select/topk.py
--rw-r--r--   0        0        0     5159 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/topk_pool.py
--rw-r--r--   0        0        0     2736 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/voxel_grid.py
--rw-r--r--   0        0        0      426 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/reshape.py
--rw-r--r--   0        0        0     6155 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/resolver.py
--rw-r--r--   0        0        0     1054 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/sequential.jinja
--rw-r--r--   0        0        0     5534 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/sequential.py
--rw-r--r--   0        0        0     5821 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/summary.py
--rw-r--r--   0        0        0     1282 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/to_fixed_size_transformer.py
--rw-r--r--   0        0        0     6519 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/to_hetero_module.py
--rw-r--r--   0        0        0    18407 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/to_hetero_transformer.py
--rw-r--r--   0        0        0    23121 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/to_hetero_with_bases_transformer.py
--rw-r--r--   0        0        0      129 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/unpool/__init__.py
--rw-r--r--   0        0        0     2586 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/unpool/knn_interpolate.py
--rw-r--r--   0        0        0      863 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/profile/__init__.py
--rw-r--r--   0        0        0     5256 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/profile/benchmark.py
--rw-r--r--   0        0        0    11793 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/profile/profile.py
--rw-r--r--   0        0        0    16640 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/profile/profiler.py
--rw-r--r--   0        0        0     5497 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/profile/utils.py
--rw-r--r--   0        0        0     1273 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/resolver.py
--rw-r--r--   0        0        0      512 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/sampler/__init__.py
--rw-r--r--   0        0        0    25968 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/sampler/base.py
--rw-r--r--   0        0        0     2721 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/sampler/hgt_sampler.py
--rw-r--r--   0        0        0    33850 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/sampler/neighbor_sampler.py
--rw-r--r--   0        0        0     5492 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/sampler/utils.py
--rw-r--r--   0        0        0      372 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/seed.py
--rw-r--r--   0        0        0     1060 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/template.py
--rw-r--r--   0        0        0     1227 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/testing/__init__.py
--rw-r--r--   0        0        0     4606 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/testing/asserts.py
--rw-r--r--   0        0        0     2604 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/testing/data.py
--rw-r--r--   0        0        0     8160 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/testing/decorators.py
--rw-r--r--   0        0        0     2227 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/testing/distributed.py
--rw-r--r--   0        0        0     2158 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/testing/feature_store.py
--rw-r--r--   0        0        0     1044 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/testing/graph_store.py
--rw-r--r--   0        0        0     4181 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/__init__.py
--rw-r--r--   0        0        0    14223 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/add_metapaths.py
--rw-r--r--   0        0        0     6065 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/add_positional_encoding.py
--rw-r--r--   0        0        0     2085 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/add_remaining_self_loops.py
--rw-r--r--   0        0        0     2024 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/add_self_loops.py
--rw-r--r--   0        0        0     1298 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/base_transform.py
--rw-r--r--   0        0        0     2464 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/cartesian.py
--rw-r--r--   0        0        0      645 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/center.py
--rw-r--r--   0        0        0     1658 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/compose.py
--rw-r--r--   0        0        0     2005 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/constant.py
--rw-r--r--   0        0        0     1264 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/delaunay.py
--rw-r--r--   0        0        0     2360 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/distance.py
--rw-r--r--   0        0        0     1083 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/face_to_edge.py
--rw-r--r--   0        0        0     3056 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/feature_propagation.py
--rw-r--r--   0        0        0     2426 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/fixed_points.py
--rw-r--r--   0        0        0     1397 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/gcn_norm.py
--rw-r--r--   0        0        0    20201 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/gdc.py
--rw-r--r--   0        0        0     1028 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/generate_mesh_normals.py
--rw-r--r--   0        0        0     2564 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/grid_sampling.py
--rw-r--r--   0        0        0     4102 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/half_hop.py
--rw-r--r--   0        0        0     2536 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/knn_graph.py
--rw-r--r--   0        0        0     2497 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/laplacian_lambda_max.py
--rw-r--r--   0        0        0     2161 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/largest_connected_components.py
--rw-r--r--   0        0        0     3730 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/line_graph.py
--rw-r--r--   0        0        0     1997 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/linear_transformation.py
--rw-r--r--   0        0        0     2144 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/local_cartesian.py
--rw-r--r--   0        0        0     1480 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/local_degree_profile.py
--rw-r--r--   0        0        0     4813 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/mask.py
--rw-r--r--   0        0        0     6088 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/node_property_split.py
--rw-r--r--   0        0        0     1028 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/normalize_features.py
--rw-r--r--   0        0        0     1782 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/normalize_rotation.py
--rw-r--r--   0        0        0      666 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/normalize_scale.py
--rw-r--r--   0        0        0     1584 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/one_hot_degree.py
--rw-r--r--   0        0        0    21047 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/pad.py
--rw-r--r--   0        0        0     1794 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/point_pair_features.py
--rw-r--r--   0        0        0     2213 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/polar.py
--rw-r--r--   0        0        0     2043 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/radius_graph.py
--rw-r--r--   0        0        0     1033 2024-04-25 06:12:17.514539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/random_flip.py
--rw-r--r--   0        0        0     1721 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/random_jitter.py
--rw-r--r--   0        0        0    15174 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/random_link_split.py
--rw-r--r--   0        0        0     5853 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/random_node_split.py
--rw-r--r--   0        0        0     1946 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/random_rotate.py
--rw-r--r--   0        0        0     1261 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/random_scale.py
--rw-r--r--   0        0        0     1365 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/random_shear.py
--rw-r--r--   0        0        0     1929 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/remove_duplicated_edges.py
--rw-r--r--   0        0        0     2449 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/remove_isolated_nodes.py
--rw-r--r--   0        0        0      932 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/remove_training_classes.py
--rw-r--r--   0        0        0     6509 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/rooted_subgraph.py
--rw-r--r--   0        0        0     2280 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/sample_points.py
--rw-r--r--   0        0        0     2329 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/sign.py
--rw-r--r--   0        0        0     2320 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/spherical.py
--rw-r--r--   0        0        0     1009 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/svd_feature_reduction.py
--rw-r--r--   0        0        0     1659 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/target_indegree.py
--rw-r--r--   0        0        0     2456 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/to_dense.py
--rw-r--r--   0        0        0     1470 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/to_device.py
--rw-r--r--   0        0        0     5580 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/to_sparse_tensor.py
--rw-r--r--   0        0        0     2697 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/to_superpixels.py
--rw-r--r--   0        0        0     2972 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/to_undirected.py
--rw-r--r--   0        0        0     1295 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/two_hop.py
--rw-r--r--   0        0        0     2860 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/virtual_node.py
--rw-r--r--   0        0        0    13230 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/typing.py
--rw-r--r--   0        0        0     4790 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/__init__.py
--rw-r--r--   0        0        0     2347 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_assortativity.py
--rw-r--r--   0        0        0     6769 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_coalesce.py
--rw-r--r--   0        0        0     1017 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_degree.py
--rw-r--r--   0        0        0     2562 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_grid.py
--rw-r--r--   0        0        0     5090 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_homophily.py
--rw-r--r--   0        0        0     1283 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_index_sort.py
--rw-r--r--   0        0        0     1403 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_lexsort.py
--rw-r--r--   0        0        0    14672 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_negative_sampling.py
--rw-r--r--   0        0        0     1167 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_normalized_cut.py
--rw-r--r--   0        0        0     1404 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_one_hot.py
--rw-r--r--   0        0        0    13389 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_scatter.py
--rw-r--r--   0        0        0     1976 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_segment.py
--rw-r--r--   0        0        0     2439 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_select.py
--rw-r--r--   0        0        0     3242 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_softmax.py
--rw-r--r--   0        0        0     4500 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_sort_edge_index.py
--rw-r--r--   0        0        0     5794 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_spmm.py
--rw-r--r--   0        0        0    18311 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_subgraph.py
--rw-r--r--   0        0        0     3606 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_to_dense_adj.py
--rw-r--r--   0        0        0     4582 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_to_dense_batch.py
--rw-r--r--   0        0        0     3569 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_train_test_split_edges.py
--rw-r--r--   0        0        0     5300 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_tree_decomposition.py
--rw-r--r--   0        0        0     8307 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_trim_to_layer.py
--rw-r--r--   0        0        0     2378 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_unbatch.py
--rw-r--r--   0        0        0     8601 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/augmentation.py
--rw-r--r--   0        0        0    21740 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/convert.py
--rw-r--r--   0        0        0     3047 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/cross_entropy.py
--rw-r--r--   0        0        0    11416 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/dropout.py
--rw-r--r--   0        0        0     1675 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/embedding.py
--rw-r--r--   0        0        0      703 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/functions.py
--rw-r--r--   0        0        0     4668 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/geodesic.py
--rw-r--r--   0        0        0     5542 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/hetero.py
--rw-r--r--   0        0        0     3588 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/isolated.py
--rw-r--r--   0        0        0     3695 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/laplacian.py
--rw-r--r--   0        0        0    23051 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/loop.py
--rw-r--r--   0        0        0     5918 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/map.py
--rw-r--r--   0        0        0     2340 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/mask.py
--rw-r--r--   0        0        0     4387 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/mesh_laplacian.py
--rw-r--r--   0        0        0      699 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/mixin.py
--rw-r--r--   0        0        0     3310 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/nested.py
--rw-r--r--   0        0        0     3750 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/noise_scheduler.py
--rw-r--r--   0        0        0     2176 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/num_nodes.py
--rw-r--r--   0        0        0     4055 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/ppr.py
--rw-r--r--   0        0        0     5148 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/random.py
--rw-r--r--   0        0        0      815 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/repeat.py
--rw-r--r--   0        0        0     6242 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/smiles.py
--rw-r--r--   0        0        0    25330 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/sparse.py
--rw-r--r--   0        0        0     6222 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/undirected.py
--rw-r--r--   0        0        0      154 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/visualization/__init__.py
--rw-r--r--   0        0        0     4813 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/visualization/graph.py
--rw-r--r--   0        0        0      477 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/visualization/influence.py
--rw-r--r--   0        0        0      413 2024-04-25 06:12:17.518539 pyg_nightly-2.6.0.dev20240425/torch_geometric/warnings.py
--rw-r--r--   0        0        0    64205 1970-01-01 00:00:00.000000 pyg_nightly-2.6.0.dev20240425/PKG-INFO
+-rw-r--r--   0        0        0    59764 2024-04-26 06:12:57.817215 pyg_nightly-2.6.0.dev20240426/README.md
+-rw-r--r--   0        0        0     5269 2024-04-26 06:12:58.409211 pyg_nightly-2.6.0.dev20240426/pyproject.toml
+-rw-r--r--   0        0        0     1209 2024-04-26 06:12:58.405211 pyg_nightly-2.6.0.dev20240426/torch_geometric/__init__.py
+-rw-r--r--   0        0        0     1053 2024-04-26 06:12:57.865214 pyg_nightly-2.6.0.dev20240426/torch_geometric/_compile.py
+-rw-r--r--   0        0        0     1575 2024-04-26 06:12:57.865214 pyg_nightly-2.6.0.dev20240426/torch_geometric/backend.py
+-rw-r--r--   0        0        0    16514 2024-04-26 06:12:57.865214 pyg_nightly-2.6.0.dev20240426/torch_geometric/config_store.py
+-rw-r--r--   0        0        0      352 2024-04-26 06:12:57.865214 pyg_nightly-2.6.0.dev20240426/torch_geometric/contrib/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-26 06:12:57.865214 pyg_nightly-2.6.0.dev20240426/torch_geometric/contrib/datasets/__init__.py
+-rw-r--r--   0        0        0      396 2024-04-26 06:12:57.865214 pyg_nightly-2.6.0.dev20240426/torch_geometric/contrib/explain/__init__.py
+-rw-r--r--   0        0        0    16972 2024-04-26 06:12:57.865214 pyg_nightly-2.6.0.dev20240426/torch_geometric/contrib/explain/pgm_explainer.py
+-rw-r--r--   0        0        0       72 2024-04-26 06:12:57.865214 pyg_nightly-2.6.0.dev20240426/torch_geometric/contrib/nn/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-26 06:12:57.865214 pyg_nightly-2.6.0.dev20240426/torch_geometric/contrib/nn/conv/__init__.py
+-rw-r--r--   0        0        0      113 2024-04-26 06:12:57.865214 pyg_nightly-2.6.0.dev20240426/torch_geometric/contrib/nn/models/__init__.py
+-rw-r--r--   0        0        0    33280 2024-04-26 06:12:57.865214 pyg_nightly-2.6.0.dev20240426/torch_geometric/contrib/nn/models/rbcd_attack.py
+-rw-r--r--   0        0        0       23 2024-04-26 06:12:57.865214 pyg_nightly-2.6.0.dev20240426/torch_geometric/contrib/transforms/__init__.py
+-rw-r--r--   0        0        0     3882 2024-04-26 06:12:57.865214 pyg_nightly-2.6.0.dev20240426/torch_geometric/data/__init__.py
+-rw-r--r--   0        0        0     8767 2024-04-26 06:12:57.865214 pyg_nightly-2.6.0.dev20240426/torch_geometric/data/batch.py
+-rw-r--r--   0        0        0    12525 2024-04-26 06:12:57.865214 pyg_nightly-2.6.0.dev20240426/torch_geometric/data/collate.py
+-rw-r--r--   0        0        0    43328 2024-04-26 06:12:57.865214 pyg_nightly-2.6.0.dev20240426/torch_geometric/data/data.py
+-rw-r--r--   0        0        0    21306 2024-04-26 06:12:57.865214 pyg_nightly-2.6.0.dev20240426/torch_geometric/data/database.py
+-rw-r--r--   0        0        0     3083 2024-04-26 06:12:57.865214 pyg_nightly-2.6.0.dev20240426/torch_geometric/data/datapipes.py
+-rw-r--r--   0        0        0    16402 2024-04-26 06:12:57.865214 pyg_nightly-2.6.0.dev20240426/torch_geometric/data/dataset.py
+-rw-r--r--   0        0        0     1889 2024-04-26 06:12:57.865214 pyg_nightly-2.6.0.dev20240426/torch_geometric/data/download.py
+-rw-r--r--   0        0        0     2324 2024-04-26 06:12:57.865214 pyg_nightly-2.6.0.dev20240426/torch_geometric/data/extract.py
+-rw-r--r--   0        0        0    20205 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/data/feature_store.py
+-rw-r--r--   0        0        0    13926 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/data/graph_store.py
+-rw-r--r--   0        0        0    47550 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/data/hetero_data.py
+-rw-r--r--   0        0        0     8294 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/data/hypergraph_data.py
+-rw-r--r--   0        0        0    13513 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/data/in_memory_dataset.py
+-rw-r--r--   0        0        0      178 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/data/lightning/__init__.py
+-rw-r--r--   0        0        0    29244 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/data/lightning/datamodule.py
+-rw-r--r--   0        0        0      463 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/data/makedirs.py
+-rw-r--r--   0        0        0     6629 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/data/on_disk_dataset.py
+-rw-r--r--   0        0        0     4503 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/data/remote_backend_utils.py
+-rw-r--r--   0        0        0     5319 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/data/separate.py
+-rw-r--r--   0        0        0    31582 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/data/storage.py
+-rw-r--r--   0        0        0     5375 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/data/summary.py
+-rw-r--r--   0        0        0    10055 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/data/temporal.py
+-rw-r--r--   0        0        0     1089 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/data/view.py
+-rw-r--r--   0        0        0     5770 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/__init__.py
+-rw-r--r--   0        0        0     4471 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/actor.py
+-rw-r--r--   0        0        0     5666 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/airfrans.py
+-rw-r--r--   0        0        0     3913 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/airports.py
+-rw-r--r--   0        0        0     3179 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/amazon.py
+-rw-r--r--   0        0        0     3362 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/amazon_book.py
+-rw-r--r--   0        0        0     3964 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/amazon_products.py
+-rw-r--r--   0        0        0     5178 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/aminer.py
+-rw-r--r--   0        0        0     5455 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/aqsol.py
+-rw-r--r--   0        0        0     5975 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/attributed_graph_dataset.py
+-rw-r--r--   0        0        0     4258 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/ba2motif_dataset.py
+-rw-r--r--   0        0        0     3700 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/ba_multi_shapes.py
+-rw-r--r--   0        0        0     3904 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/ba_shapes.py
+-rw-r--r--   0        0        0     4404 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/bitcoin_otc.py
+-rw-r--r--   0        0        0     3959 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/brca_tgca.py
+-rw-r--r--   0        0        0     4458 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/citation_full.py
+-rw-r--r--   0        0        0     3138 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/coauthor.py
+-rw-r--r--   0        0        0     4734 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/coma.py
+-rw-r--r--   0        0        0     5311 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/cornell.py
+-rw-r--r--   0        0        0     5416 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/dblp.py
+-rw-r--r--   0        0        0     5707 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/dbp15k.py
+-rw-r--r--   0        0        0     2511 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/deezer_europe.py
+-rw-r--r--   0        0        0     4035 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/dgraph.py
+-rw-r--r--   0        0        0     6041 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/dynamic_faust.py
+-rw-r--r--   0        0        0     4605 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/elliptic.py
+-rw-r--r--   0        0        0     3188 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/elliptic_temporal.py
+-rw-r--r--   0        0        0     2834 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/email_eu_core.py
+-rw-r--r--   0        0        0     7356 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/entities.py
+-rw-r--r--   0        0        0     6103 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/explainer_dataset.py
+-rw-r--r--   0        0        0     2431 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/facebook.py
+-rw-r--r--   0        0        0    10554 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/fake.py
+-rw-r--r--   0        0        0     4076 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/faust.py
+-rw-r--r--   0        0        0     3964 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/flickr.py
+-rw-r--r--   0        0        0     4080 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/freebase.py
+-rw-r--r--   0        0        0     3598 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/gdelt.py
+-rw-r--r--   0        0        0     3189 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/gdelt_lite.py
+-rw-r--r--   0        0        0     9511 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/ged_dataset.py
+-rw-r--r--   0        0        0     2820 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/gemsec.py
+-rw-r--r--   0        0        0     4223 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/geometry.py
+-rw-r--r--   0        0        0     2687 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/github.py
+-rw-r--r--   0        0        0     6940 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/gnn_benchmark_dataset.py
+-rw-r--r--   0        0        0      272 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/graph_generator/__init__.py
+-rw-r--r--   0        0        0      965 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/graph_generator/ba_graph.py
+-rw-r--r--   0        0        0      939 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/graph_generator/base.py
+-rw-r--r--   0        0        0      918 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/graph_generator/er_graph.py
+-rw-r--r--   0        0        0     1159 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/graph_generator/grid_graph.py
+-rw-r--r--   0        0        0     2599 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/graph_generator/tree_graph.py
+-rw-r--r--   0        0        0     4224 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/heterophilous_graph_dataset.py
+-rw-r--r--   0        0        0     8846 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/hgb_dataset.py
+-rw-r--r--   0        0        0     6763 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/hm.py
+-rw-r--r--   0        0        0    11417 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/hydro_net.py
+-rw-r--r--   0        0        0     4735 2024-04-26 06:12:57.869214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/icews.py
+-rw-r--r--   0        0        0     4611 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/igmc_dataset.py
+-rw-r--r--   0        0        0     4223 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/imdb.py
+-rw-r--r--   0        0        0     7293 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/infection_dataset.py
+-rw-r--r--   0        0        0     3643 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/jodie.py
+-rw-r--r--   0        0        0     3445 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/karate.py
+-rw-r--r--   0        0        0     4572 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/last_fm.py
+-rw-r--r--   0        0        0     2486 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/lastfm_asia.py
+-rw-r--r--   0        0        0     6864 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/linkx_dataset.py
+-rw-r--r--   0        0        0    11746 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/lrgb.py
+-rw-r--r--   0        0        0     5244 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/malnet_tiny.py
+-rw-r--r--   0        0        0    16734 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/md17.py
+-rw-r--r--   0        0        0     3951 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/mixhop_synthetic_dataset.py
+-rw-r--r--   0        0        0     3317 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/mnist_superpixels.py
+-rw-r--r--   0        0        0     5347 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/modelnet.py
+-rw-r--r--   0        0        0     7177 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/molecule_net.py
+-rw-r--r--   0        0        0      272 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/motif_generator/__init__.py
+-rw-r--r--   0        0        0      900 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/motif_generator/base.py
+-rw-r--r--   0        0        0     1278 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/motif_generator/custom.py
+-rw-r--r--   0        0        0      983 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/motif_generator/cycle.py
+-rw-r--r--   0        0        0     1099 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/motif_generator/grid.py
+-rw-r--r--   0        0        0      814 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/motif_generator/house.py
+-rw-r--r--   0        0        0     4033 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/movie_lens.py
+-rw-r--r--   0        0        0     6057 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/movie_lens_100k.py
+-rw-r--r--   0        0        0     5396 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/movie_lens_1m.py
+-rw-r--r--   0        0        0     3008 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/myket.py
+-rw-r--r--   0        0        0     2863 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/nell.py
+-rw-r--r--   0        0        0     5181 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/neurograph.py
+-rw-r--r--   0        0        0     7481 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/ogb_mag.py
+-rw-r--r--   0        0        0     3585 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/omdb.py
+-rw-r--r--   0        0        0     5161 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/ose_gvcs.py
+-rw-r--r--   0        0        0     4162 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/particle.py
+-rw-r--r--   0        0        0    12041 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/pascal.py
+-rw-r--r--   0        0        0     4791 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/pascal_pf.py
+-rw-r--r--   0        0        0     5897 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/pcpnet_dataset.py
+-rw-r--r--   0        0        0     4207 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/pcqm4m.py
+-rw-r--r--   0        0        0     7201 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/planetoid.py
+-rw-r--r--   0        0        0     3045 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/polblogs.py
+-rw-r--r--   0        0        0     4999 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/ppi.py
+-rw-r--r--   0        0        0     3325 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/qm7.py
+-rw-r--r--   0        0        0    17158 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/qm9.py
+-rw-r--r--   0        0        0     5304 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/rcdd.py
+-rw-r--r--   0        0        0     3122 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/reddit.py
+-rw-r--r--   0        0        0     4282 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/reddit2.py
+-rw-r--r--   0        0        0     4535 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/rel_link_pred_dataset.py
+-rw-r--r--   0        0        0     4553 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/s3dis.py
+-rw-r--r--   0        0        0     8816 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/sbm_dataset.py
+-rw-r--r--   0        0        0     8504 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/shapenet.py
+-rw-r--r--   0        0        0     6316 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/shrec2016.py
+-rw-r--r--   0        0        0     9433 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/snap_dataset.py
+-rw-r--r--   0        0        0     3278 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/suite_sparse.py
+-rw-r--r--   0        0        0     4170 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/taobao.py
+-rw-r--r--   0        0        0     4632 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/tosca.py
+-rw-r--r--   0        0        0     7847 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/tu_dataset.py
+-rw-r--r--   0        0        0     3658 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/twitch.py
+-rw-r--r--   0        0        0     7001 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/upfd.py
+-rw-r--r--   0        0        0      182 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/utils/__init__.py
+-rw-r--r--   0        0        0     1835 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/utils/cheatsheet.py
+-rw-r--r--   0        0        0     4889 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/webkb.py
+-rw-r--r--   0        0        0     3884 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/wikics.py
+-rw-r--r--   0        0        0     4947 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/wikidata.py
+-rw-r--r--   0        0        0     6640 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/wikipedia_network.py
+-rw-r--r--   0        0        0     7028 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/willow_object_class.py
+-rw-r--r--   0        0        0     8158 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/word_net.py
+-rw-r--r--   0        0        0     3959 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/yelp.py
+-rw-r--r--   0        0        0     6347 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/zinc.py
+-rw-r--r--   0        0        0     1295 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/debug.py
+-rw-r--r--   0        0        0      858 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/deprecation.py
+-rw-r--r--   0        0        0      589 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/distributed/__init__.py
+-rw-r--r--   0        0        0      418 2024-04-26 06:12:57.873214 pyg_nightly-2.6.0.dev20240426/torch_geometric/distributed/dist_context.py
+-rw-r--r--   0        0        0     4933 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/distributed/dist_link_neighbor_loader.py
+-rw-r--r--   0        0        0     6492 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/distributed/dist_loader.py
+-rw-r--r--   0        0        0     4372 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/distributed/dist_neighbor_loader.py
+-rw-r--r--   0        0        0    42406 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/distributed/dist_neighbor_sampler.py
+-rw-r--r--   0        0        0     3309 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/distributed/event_loop.py
+-rw-r--r--   0        0        0    19018 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/distributed/local_feature_store.py
+-rw-r--r--   0        0        0     8408 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/distributed/local_graph_store.py
+-rw-r--r--   0        0        0    14675 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/distributed/partition.py
+-rw-r--r--   0        0        0     5753 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/distributed/rpc.py
+-rw-r--r--   0        0        0     6567 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/distributed/utils.py
+-rw-r--r--   0        0        0    67415 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/edge_index.py
+-rw-r--r--   0        0        0     4756 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/experimental.py
+-rw-r--r--   0        0        0      359 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/__init__.py
+-rw-r--r--   0        0        0      496 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/algorithm/__init__.py
+-rw-r--r--   0        0        0     4545 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/algorithm/attention_explainer.py
+-rw-r--r--   0        0        0     6935 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/algorithm/base.py
+-rw-r--r--   0        0        0    12857 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/algorithm/captum.py
+-rw-r--r--   0        0        0     7346 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/algorithm/captum_explainer.py
+-rw-r--r--   0        0        0     2872 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/algorithm/dummy_explainer.py
+-rw-r--r--   0        0        0    12454 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/algorithm/gnn_explainer.py
+-rw-r--r--   0        0        0    21367 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/algorithm/graphmask_explainer.py
+-rw-r--r--   0        0        0    10371 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/algorithm/pg_explainer.py
+-rw-r--r--   0        0        0     2564 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/algorithm/utils.py
+-rw-r--r--   0        0        0     7834 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/config.py
+-rw-r--r--   0        0        0    10667 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/explainer.py
+-rw-r--r--   0        0        0    14934 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/explanation.py
+-rw-r--r--   0        0        0      301 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/metric/__init__.py
+-rw-r--r--   0        0        0     1888 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/metric/basic.py
+-rw-r--r--   0        0        0     3063 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/metric/faithfulness.py
+-rw-r--r--   0        0        0     6157 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/metric/fidelity.py
+-rw-r--r--   0        0        0     1815 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/__init__.py
+-rw-r--r--   0        0        0      510 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/benchmark.py
+-rw-r--r--   0        0        0     2371 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/checkpoint.py
+-rw-r--r--   0        0        0      738 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/cmd_args.py
+-rw-r--r--   0        0        0    17197 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/config.py
+-rw-r--r--   0        0        0      389 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/contrib/__init__.py
+-rw-r--r--   0        0        0      221 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/contrib/act/__init__.py
+-rw-r--r--   0        0        0      221 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/contrib/config/__init__.py
+-rw-r--r--   0        0        0      221 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/contrib/encoder/__init__.py
+-rw-r--r--   0        0        0      221 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/contrib/head/__init__.py
+-rw-r--r--   0        0        0      221 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/contrib/layer/__init__.py
+-rw-r--r--   0        0        0     8435 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/contrib/layer/generalconv.py
+-rw-r--r--   0        0        0      221 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/contrib/loader/__init__.py
+-rw-r--r--   0        0        0      221 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/contrib/loss/__init__.py
+-rw-r--r--   0        0        0      221 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/contrib/network/__init__.py
+-rw-r--r--   0        0        0      221 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/contrib/optimizer/__init__.py
+-rw-r--r--   0        0        0      221 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/contrib/pooling/__init__.py
+-rw-r--r--   0        0        0      221 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/contrib/stage/__init__.py
+-rw-r--r--   0        0        0      221 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/contrib/train/__init__.py
+-rw-r--r--   0        0        0      221 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/contrib/transform/__init__.py
+-rw-r--r--   0        0        0      375 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/imports.py
+-rw-r--r--   0        0        0      521 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/init.py
+-rw-r--r--   0        0        0    11605 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/loader.py
+-rw-r--r--   0        0        0    11314 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/logger.py
+-rw-r--r--   0        0        0     1445 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/loss.py
+-rw-r--r--   0        0        0     3110 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/model_builder.py
+-rw-r--r--   0        0        0     1121 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/models/__init__.py
+-rw-r--r--   0        0        0      855 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/models/act.py
+-rw-r--r--   0        0        0     3034 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/models/encoder.py
+-rw-r--r--   0        0        0     6373 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/models/gnn.py
+-rw-r--r--   0        0        0     4603 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/models/head.py
+-rw-r--r--   0        0        0    12500 2024-04-26 06:12:57.877214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/models/layer.py
+-rw-r--r--   0        0        0      288 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/models/pooling.py
+-rw-r--r--   0        0        0     1383 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/models/transform.py
+-rw-r--r--   0        0        0     2544 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/optim.py
+-rw-r--r--   0        0        0     3954 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/register.py
+-rw-r--r--   0        0        0     2653 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/train.py
+-rw-r--r--   0        0        0        0 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/utils/LICENSE
+-rw-r--r--   0        0        0      641 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/utils/__init__.py
+-rw-r--r--   0        0        0     9349 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/utils/agg_runs.py
+-rw-r--r--   0        0        0     3045 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/utils/comp_budget.py
+-rw-r--r--   0        0        0     1342 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/utils/device.py
+-rw-r--r--   0        0        0      690 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/utils/epoch.py
+-rw-r--r--   0        0        0     2049 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/utils/io.py
+-rw-r--r--   0        0        0      624 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/utils/plot.py
+-rw-r--r--   0        0        0      199 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/utils/tools.py
+-rw-r--r--   0        0        0      790 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/home.py
+-rw-r--r--   0        0        0    19216 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/inspector.py
+-rw-r--r--   0        0        0      528 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/io/__init__.py
+-rw-r--r--   0        0        0     6567 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/io/fs.py
+-rw-r--r--   0        0        0     1177 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/io/npz.py
+-rw-r--r--   0        0        0     1088 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/io/obj.py
+-rw-r--r--   0        0        0     2762 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/io/off.py
+-rw-r--r--   0        0        0     4667 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/io/planetoid.py
+-rw-r--r--   0        0        0      489 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/io/ply.py
+-rw-r--r--   0        0        0     1170 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/io/sdf.py
+-rw-r--r--   0        0        0     4930 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/io/tu.py
+-rw-r--r--   0        0        0      910 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/io/txt_array.py
+-rw-r--r--   0        0        0      935 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/isinstance.py
+-rw-r--r--   0        0        0      908 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/lazy_loader.py
+-rw-r--r--   0        0        0     1835 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/__init__.py
+-rw-r--r--   0        0        0     1615 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/base.py
+-rw-r--r--   0        0        0     2106 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/cache.py
+-rw-r--r--   0        0        0    13196 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/cluster.py
+-rw-r--r--   0        0        0     1459 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/data_list_loader.py
+-rw-r--r--   0        0        0     3527 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/dataloader.py
+-rw-r--r--   0        0        0     1685 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/dense_data_loader.py
+-rw-r--r--   0        0        0     4163 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/dynamic_batch_sampler.py
+-rw-r--r--   0        0        0     8448 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/graph_saint.py
+-rw-r--r--   0        0        0     6012 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/hgt_loader.py
+-rw-r--r--   0        0        0    31462 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/ibmb_loader.py
+-rw-r--r--   0        0        0     3754 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/imbalanced_sampler.py
+-rw-r--r--   0        0        0    16207 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/link_loader.py
+-rw-r--r--   0        0        0    14383 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/link_neighbor_loader.py
+-rw-r--r--   0        0        0    10931 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/mixin.py
+-rw-r--r--   0        0        0    12452 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/neighbor_loader.py
+-rw-r--r--   0        0        0     8513 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/neighbor_sampler.py
+-rw-r--r--   0        0        0    11848 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/node_loader.py
+-rw-r--r--   0        0        0     3236 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/prefetch.py
+-rw-r--r--   0        0        0     2196 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/random_node_loader.py
+-rw-r--r--   0        0        0     4173 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/shadow.py
+-rw-r--r--   0        0        0     2248 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/temporal_dataloader.py
+-rw-r--r--   0        0        0    14901 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/utils.py
+-rw-r--r--   0        0        0     3518 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/zip_loader.py
+-rw-r--r--   0        0        0      858 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/logging.py
+-rw-r--r--   0        0        0      296 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/metrics/__init__.py
+-rw-r--r--   0        0        0     7521 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/metrics/link_pred.py
+-rw-r--r--   0        0        0      847 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/__init__.py
+-rw-r--r--   0        0        0     1551 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/__init__.py
+-rw-r--r--   0        0        0     3003 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/attention.py
+-rw-r--r--   0        0        0     8230 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/base.py
+-rw-r--r--   0        0        0    11011 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/basic.py
+-rw-r--r--   0        0        0     2650 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/deep_sets.py
+-rw-r--r--   0        0        0     6639 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/equilibrium.py
+-rw-r--r--   0        0        0    12276 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/fused.py
+-rw-r--r--   0        0        0     3801 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/gmt.py
+-rw-r--r--   0        0        0     2193 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/gru.py
+-rw-r--r--   0        0        0     4190 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/lcm.py
+-rw-r--r--   0        0        0     2214 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/lstm.py
+-rw-r--r--   0        0        0     2514 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/mlp.py
+-rw-r--r--   0        0        0     8170 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/multi.py
+-rw-r--r--   0        0        0     6189 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/quantile.py
+-rw-r--r--   0        0        0     4638 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/scaler.py
+-rw-r--r--   0        0        0     2446 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/set2set.py
+-rw-r--r--   0        0        0     4207 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/set_transformer.py
+-rw-r--r--   0        0        0     2507 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/sort.py
+-rw-r--r--   0        0        0     8338 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/utils.py
+-rw-r--r--   0        0        0     1126 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/variance_preserving.py
+-rw-r--r--   0        0        0       76 2024-04-26 06:12:57.881214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/attention/__init__.py
+-rw-r--r--   0        0        0     7357 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/attention/performer.py
+-rw-r--r--   0        0        0     3515 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/__init__.py
+-rw-r--r--   0        0        0     3077 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/agnn_conv.py
+-rw-r--r--   0        0        0     4387 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/antisymmetric_conv.py
+-rw-r--r--   0        0        0     5983 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/appnp.py
+-rw-r--r--   0        0        0     6585 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/arma_conv.py
+-rw-r--r--   0        0        0     4014 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/cg_conv.py
+-rw-r--r--   0        0        0     6423 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/cheb_conv.py
+-rw-r--r--   0        0        0     5255 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/cluster_gcn_conv.py
+-rw-r--r--   0        0        0     5648 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/collect.jinja
+-rw-r--r--   0        0        0      251 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/cugraph/__init__.py
+-rw-r--r--   0        0        0     6364 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/cugraph/base.py
+-rw-r--r--   0        0        0     2874 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/cugraph/gat_conv.py
+-rw-r--r--   0        0        0     4002 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/cugraph/rgcn_conv.py
+-rw-r--r--   0        0        0     2830 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/cugraph/sage_conv.py
+-rw-r--r--   0        0        0     2440 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/dir_gnn_conv.py
+-rw-r--r--   0        0        0    12241 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/dna_conv.py
+-rw-r--r--   0        0        0     5389 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/edge_conv.py
+-rw-r--r--   0        0        0     2216 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/edge_updater.jinja
+-rw-r--r--   0        0        0    10742 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/eg_conv.py
+-rw-r--r--   0        0        0     9065 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/fa_conv.py
+-rw-r--r--   0        0        0     4430 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/feast_conv.py
+-rw-r--r--   0        0        0     6314 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/film_conv.py
+-rw-r--r--   0        0        0     4502 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/fused_gat_conv.py
+-rw-r--r--   0        0        0    16091 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/gat_conv.py
+-rw-r--r--   0        0        0     3518 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/gated_graph_conv.py
+-rw-r--r--   0        0        0    13639 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/gatv2_conv.py
+-rw-r--r--   0        0        0     7001 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/gcn2_conv.py
+-rw-r--r--   0        0        0    10415 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/gcn_conv.py
+-rw-r--r--   0        0        0     9722 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/gen_conv.py
+-rw-r--r--   0        0        0     7591 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/general_conv.py
+-rw-r--r--   0        0        0     7411 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/gin_conv.py
+-rw-r--r--   0        0        0     8315 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/gmm_conv.py
+-rw-r--r--   0        0        0     6672 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/gps_conv.py
+-rw-r--r--   0        0        0     3905 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/graph_conv.py
+-rw-r--r--   0        0        0     4951 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/gravnet_conv.py
+-rw-r--r--   0        0        0     7198 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/han_conv.py
+-rw-r--r--   0        0        0     6084 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/heat_conv.py
+-rw-r--r--   0        0        0     6555 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/hetero_conv.py
+-rw-r--r--   0        0        0     9043 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/hgt_conv.py
+-rw-r--r--   0        0        0     8691 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/hypergraph_conv.py
+-rw-r--r--   0        0        0     3494 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/le_conv.py
+-rw-r--r--   0        0        0     2369 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/lg_conv.py
+-rw-r--r--   0        0        0    43545 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/message_passing.py
+-rw-r--r--   0        0        0     4340 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/mf_conv.py
+-rw-r--r--   0        0        0     4554 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/mixhop_conv.py
+-rw-r--r--   0        0        0     4759 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/nn_conv.py
+-rw-r--r--   0        0        0     4908 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/pan_conv.py
+-rw-r--r--   0        0        0     4892 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/pdn_conv.py
+-rw-r--r--   0        0        0     8325 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/pna_conv.py
+-rw-r--r--   0        0        0     4508 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/point_conv.py
+-rw-r--r--   0        0        0     3278 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/point_gnn_conv.py
+-rw-r--r--   0        0        0     5878 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/point_transformer_conv.py
+-rw-r--r--   0        0        0     5363 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/ppf_conv.py
+-rw-r--r--   0        0        0     7374 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/propagate.jinja
+-rw-r--r--   0        0        0     5217 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/res_gated_graph_conv.py
+-rw-r--r--   0        0        0    22863 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/rgat_conv.py
+-rw-r--r--   0        0        0    15705 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/rgcn_conv.py
+-rw-r--r--   0        0        0     5812 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/sage_conv.py
+-rw-r--r--   0        0        0     4543 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/sg_conv.py
+-rw-r--r--   0        0        0     6190 2024-04-26 06:12:57.885214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/signed_conv.py
+-rw-r--r--   0        0        0     3888 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/simple_conv.py
+-rw-r--r--   0        0        0     6314 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/spline_conv.py
+-rw-r--r--   0        0        0     5131 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/ssg_conv.py
+-rw-r--r--   0        0        0    12420 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/supergat_conv.py
+-rw-r--r--   0        0        0     4164 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/tag_conv.py
+-rw-r--r--   0        0        0    10407 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/transformer_conv.py
+-rw-r--r--   0        0        0      852 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/utils/__init__.py
+-rw-r--r--   0        0        0     2792 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/utils/cheatsheet.py
+-rw-r--r--   0        0        0     3140 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/wl_conv.py
+-rw-r--r--   0        0        0     2777 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/wl_conv_continuous.py
+-rw-r--r--   0        0        0     5956 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/x_conv.py
+-rw-r--r--   0        0        0     4764 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/data_parallel.py
+-rw-r--r--   0        0        0      847 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/dense/__init__.py
+-rw-r--r--   0        0        0     4238 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/dense/dense_gat_conv.py
+-rw-r--r--   0        0        0     3002 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/dense/dense_gcn_conv.py
+-rw-r--r--   0        0        0     2361 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/dense/dense_gin_conv.py
+-rw-r--r--   0        0        0     2751 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/dense/dense_graph_conv.py
+-rw-r--r--   0        0        0     2672 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/dense/dense_sage_conv.py
+-rw-r--r--   0        0        0     3051 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/dense/diff_pool.py
+-rw-r--r--   0        0        0     6115 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/dense/dmon_pool.py
+-rw-r--r--   0        0        0    17702 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/dense/linear.py
+-rw-r--r--   0        0        0     4111 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/dense/mincut_pool.py
+-rw-r--r--   0        0        0     3115 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/encoding.py
+-rw-r--r--   0        0        0      129 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/functional/__init__.py
+-rw-r--r--   0        0        0     1549 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/functional/bro.py
+-rw-r--r--   0        0        0      863 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/functional/gini.py
+-rw-r--r--   0        0        0    16055 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/fx.py
+-rw-r--r--   0        0        0     1088 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/glob.py
+-rw-r--r--   0        0        0     2457 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/inits.py
+-rw-r--r--   0        0        0      290 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/kge/__init__.py
+-rw-r--r--   0        0        0     5902 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/kge/base.py
+-rw-r--r--   0        0        0     3234 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/kge/complex.py
+-rw-r--r--   0        0        0     2462 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/kge/distmult.py
+-rw-r--r--   0        0        0      771 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/kge/loader.py
+-rw-r--r--   0        0        0     3208 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/kge/rotate.py
+-rw-r--r--   0        0        0     3088 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/kge/transe.py
+-rw-r--r--   0        0        0     8937 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/lr_scheduler.py
+-rw-r--r--   0        0        0     9512 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/model_hub.py
+-rw-r--r--   0        0        0     1909 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/__init__.py
+-rw-r--r--   0        0        0     6634 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/attentive_fp.py
+-rw-r--r--   0        0        0    10770 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/autoencoder.py
+-rw-r--r--   0        0        0    31225 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/basic_gnn.py
+-rw-r--r--   0        0        0     3971 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/captum.py
+-rw-r--r--   0        0        0     6827 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/correct_and_smooth.py
+-rw-r--r--   0        0        0     4197 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/deep_graph_infomax.py
+-rw-r--r--   0        0        0     4339 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/deepgcn.py
+-rw-r--r--   0        0        0    36186 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/dimenet.py
+-rw-r--r--   0        0        0     5107 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/dimenet_utils.py
+-rw-r--r--   0        0        0     7873 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/gnnff.py
+-rw-r--r--   0        0        0     9246 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/graph_mixer.py
+-rw-r--r--   0        0        0     5395 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/graph_unet.py
+-rw-r--r--   0        0        0     3450 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/jumping_knowledge.py
+-rw-r--r--   0        0        0     3908 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/label_prop.py
+-rw-r--r--   0        0        0    12465 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/lightgcn.py
+-rw-r--r--   0        0        0     5812 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/linkx.py
+-rw-r--r--   0        0        0     2580 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/mask_label.py
+-rw-r--r--   0        0        0     6540 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/meta.py
+-rw-r--r--   0        0        0    10870 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/metapath2vec.py
+-rw-r--r--   0        0        0    10315 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/mlp.py
+-rw-r--r--   0        0        0     2378 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/neural_fingerprint.py
+-rw-r--r--   0        0        0     7731 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/node2vec.py
+-rw-r--r--   0        0        0     3538 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/pmlp.py
+-rw-r--r--   0        0        0     8986 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/re_net.py
+-rw-r--r--   0        0        0     2808 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/rect.py
+-rw-r--r--   0        0        0    11796 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/rev_gnn.py
+-rw-r--r--   0        0        0    16619 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/schnet.py
+-rw-r--r--   0        0        0     9839 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/signed_gcn.py
+-rw-r--r--   0        0        0    11878 2024-04-26 06:12:57.889214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/tgn.py
+-rw-r--r--   0        0        0    43192 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/visnet.py
+-rw-r--r--   0        0        0     2373 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/module_dict.py
+-rw-r--r--   0        0        0      669 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/norm/__init__.py
+-rw-r--r--   0        0        0     8283 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/norm/batch_norm.py
+-rw-r--r--   0        0        0     4722 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/norm/diff_group_norm.py
+-rw-r--r--   0        0        0     2727 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/norm/graph_norm.py
+-rw-r--r--   0        0        0     1491 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/norm/graph_size_norm.py
+-rw-r--r--   0        0        0     4685 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/norm/instance_norm.py
+-rw-r--r--   0        0        0     7831 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/norm/layer_norm.py
+-rw-r--r--   0        0        0     1322 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/norm/mean_subtraction_norm.py
+-rw-r--r--   0        0        0     1662 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/norm/msg_norm.py
+-rw-r--r--   0        0        0     2824 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/norm/pair_norm.py
+-rw-r--r--   0        0        0     2410 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/parameter_dict.py
+-rw-r--r--   0        0        0    14129 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/__init__.py
+-rw-r--r--   0        0        0     3967 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/approx_knn.py
+-rw-r--r--   0        0        0     6683 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/asap.py
+-rw-r--r--   0        0        0     3966 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/avg_pool.py
+-rw-r--r--   0        0        0      287 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/connect/__init__.py
+-rw-r--r--   0        0        0     4094 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/connect/base.py
+-rw-r--r--   0        0        0     2190 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/connect/filter_edges.py
+-rw-r--r--   0        0        0      273 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/consecutive.py
+-rw-r--r--   0        0        0     1601 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/decimation.py
+-rw-r--r--   0        0        0     8581 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/edge_pool.py
+-rw-r--r--   0        0        0     3492 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/glob.py
+-rw-r--r--   0        0        0     1291 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/graclus.py
+-rw-r--r--   0        0        0    11343 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/knn.py
+-rw-r--r--   0        0        0     4262 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/max_pool.py
+-rw-r--r--   0        0        0     5377 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/mem_pool.py
+-rw-r--r--   0        0        0     4366 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/pan_pool.py
+-rw-r--r--   0        0        0      737 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/pool.py
+-rw-r--r--   0        0        0     5838 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/sag_pool.py
+-rw-r--r--   0        0        0      254 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/select/__init__.py
+-rw-r--r--   0        0        0     3311 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/select/base.py
+-rw-r--r--   0        0        0     5305 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/select/topk.py
+-rw-r--r--   0        0        0     5159 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/topk_pool.py
+-rw-r--r--   0        0        0     2736 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/voxel_grid.py
+-rw-r--r--   0        0        0      426 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/reshape.py
+-rw-r--r--   0        0        0     6155 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/resolver.py
+-rw-r--r--   0        0        0     1054 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/sequential.jinja
+-rw-r--r--   0        0        0     5534 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/sequential.py
+-rw-r--r--   0        0        0     5821 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/summary.py
+-rw-r--r--   0        0        0     1282 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/to_fixed_size_transformer.py
+-rw-r--r--   0        0        0     6519 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/to_hetero_module.py
+-rw-r--r--   0        0        0    18407 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/to_hetero_transformer.py
+-rw-r--r--   0        0        0    23121 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/to_hetero_with_bases_transformer.py
+-rw-r--r--   0        0        0      129 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/unpool/__init__.py
+-rw-r--r--   0        0        0     2586 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/unpool/knn_interpolate.py
+-rw-r--r--   0        0        0      863 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/profile/__init__.py
+-rw-r--r--   0        0        0     5256 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/profile/benchmark.py
+-rw-r--r--   0        0        0    11793 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/profile/profile.py
+-rw-r--r--   0        0        0    16640 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/profile/profiler.py
+-rw-r--r--   0        0        0     5497 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/profile/utils.py
+-rw-r--r--   0        0        0     1273 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/resolver.py
+-rw-r--r--   0        0        0      512 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/sampler/__init__.py
+-rw-r--r--   0        0        0    25968 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/sampler/base.py
+-rw-r--r--   0        0        0     2721 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/sampler/hgt_sampler.py
+-rw-r--r--   0        0        0    33850 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/sampler/neighbor_sampler.py
+-rw-r--r--   0        0        0     5492 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/sampler/utils.py
+-rw-r--r--   0        0        0      372 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/seed.py
+-rw-r--r--   0        0        0     1060 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/template.py
+-rw-r--r--   0        0        0     1227 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/testing/__init__.py
+-rw-r--r--   0        0        0     4606 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/testing/asserts.py
+-rw-r--r--   0        0        0     2604 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/testing/data.py
+-rw-r--r--   0        0        0     8160 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/testing/decorators.py
+-rw-r--r--   0        0        0     2227 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/testing/distributed.py
+-rw-r--r--   0        0        0     2158 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/testing/feature_store.py
+-rw-r--r--   0        0        0     1044 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/testing/graph_store.py
+-rw-r--r--   0        0        0     4181 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/__init__.py
+-rw-r--r--   0        0        0    14235 2024-04-26 06:12:57.893214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/add_metapaths.py
+-rw-r--r--   0        0        0     6065 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/add_positional_encoding.py
+-rw-r--r--   0        0        0     2085 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/add_remaining_self_loops.py
+-rw-r--r--   0        0        0     2024 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/add_self_loops.py
+-rw-r--r--   0        0        0     1298 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/base_transform.py
+-rw-r--r--   0        0        0     2464 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/cartesian.py
+-rw-r--r--   0        0        0      645 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/center.py
+-rw-r--r--   0        0        0     1658 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/compose.py
+-rw-r--r--   0        0        0     2005 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/constant.py
+-rw-r--r--   0        0        0     1264 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/delaunay.py
+-rw-r--r--   0        0        0     2360 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/distance.py
+-rw-r--r--   0        0        0     1083 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/face_to_edge.py
+-rw-r--r--   0        0        0     3056 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/feature_propagation.py
+-rw-r--r--   0        0        0     2426 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/fixed_points.py
+-rw-r--r--   0        0        0     1397 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/gcn_norm.py
+-rw-r--r--   0        0        0    20201 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/gdc.py
+-rw-r--r--   0        0        0     1028 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/generate_mesh_normals.py
+-rw-r--r--   0        0        0     2564 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/grid_sampling.py
+-rw-r--r--   0        0        0     4102 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/half_hop.py
+-rw-r--r--   0        0        0     2536 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/knn_graph.py
+-rw-r--r--   0        0        0     2497 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/laplacian_lambda_max.py
+-rw-r--r--   0        0        0     2161 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/largest_connected_components.py
+-rw-r--r--   0        0        0     3730 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/line_graph.py
+-rw-r--r--   0        0        0     1997 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/linear_transformation.py
+-rw-r--r--   0        0        0     2144 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/local_cartesian.py
+-rw-r--r--   0        0        0     1480 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/local_degree_profile.py
+-rw-r--r--   0        0        0     4813 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/mask.py
+-rw-r--r--   0        0        0     6088 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/node_property_split.py
+-rw-r--r--   0        0        0     1028 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/normalize_features.py
+-rw-r--r--   0        0        0     1782 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/normalize_rotation.py
+-rw-r--r--   0        0        0      666 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/normalize_scale.py
+-rw-r--r--   0        0        0     1584 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/one_hot_degree.py
+-rw-r--r--   0        0        0    21047 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/pad.py
+-rw-r--r--   0        0        0     1794 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/point_pair_features.py
+-rw-r--r--   0        0        0     2213 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/polar.py
+-rw-r--r--   0        0        0     2043 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/radius_graph.py
+-rw-r--r--   0        0        0     1033 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/random_flip.py
+-rw-r--r--   0        0        0     1721 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/random_jitter.py
+-rw-r--r--   0        0        0    15174 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/random_link_split.py
+-rw-r--r--   0        0        0     5853 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/random_node_split.py
+-rw-r--r--   0        0        0     1946 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/random_rotate.py
+-rw-r--r--   0        0        0     1261 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/random_scale.py
+-rw-r--r--   0        0        0     1365 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/random_shear.py
+-rw-r--r--   0        0        0     1929 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/remove_duplicated_edges.py
+-rw-r--r--   0        0        0     2449 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/remove_isolated_nodes.py
+-rw-r--r--   0        0        0      932 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/remove_training_classes.py
+-rw-r--r--   0        0        0     6509 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/rooted_subgraph.py
+-rw-r--r--   0        0        0     2280 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/sample_points.py
+-rw-r--r--   0        0        0     2329 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/sign.py
+-rw-r--r--   0        0        0     2320 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/spherical.py
+-rw-r--r--   0        0        0     1009 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/svd_feature_reduction.py
+-rw-r--r--   0        0        0     1659 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/target_indegree.py
+-rw-r--r--   0        0        0     2456 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/to_dense.py
+-rw-r--r--   0        0        0     1470 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/to_device.py
+-rw-r--r--   0        0        0     5580 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/to_sparse_tensor.py
+-rw-r--r--   0        0        0     2697 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/to_superpixels.py
+-rw-r--r--   0        0        0     2972 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/to_undirected.py
+-rw-r--r--   0        0        0     1313 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/two_hop.py
+-rw-r--r--   0        0        0     2860 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/virtual_node.py
+-rw-r--r--   0        0        0    13230 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/typing.py
+-rw-r--r--   0        0        0     4790 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/__init__.py
+-rw-r--r--   0        0        0     2347 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_assortativity.py
+-rw-r--r--   0        0        0     6769 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_coalesce.py
+-rw-r--r--   0        0        0     1017 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_degree.py
+-rw-r--r--   0        0        0     2562 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_grid.py
+-rw-r--r--   0        0        0     5090 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_homophily.py
+-rw-r--r--   0        0        0     1283 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_index_sort.py
+-rw-r--r--   0        0        0     1403 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_lexsort.py
+-rw-r--r--   0        0        0    14672 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_negative_sampling.py
+-rw-r--r--   0        0        0     1167 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_normalized_cut.py
+-rw-r--r--   0        0        0     1404 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_one_hot.py
+-rw-r--r--   0        0        0    13389 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_scatter.py
+-rw-r--r--   0        0        0     1976 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_segment.py
+-rw-r--r--   0        0        0     2439 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_select.py
+-rw-r--r--   0        0        0     3242 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_softmax.py
+-rw-r--r--   0        0        0     4500 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_sort_edge_index.py
+-rw-r--r--   0        0        0     5794 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_spmm.py
+-rw-r--r--   0        0        0    18311 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_subgraph.py
+-rw-r--r--   0        0        0     3606 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_to_dense_adj.py
+-rw-r--r--   0        0        0     4582 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_to_dense_batch.py
+-rw-r--r--   0        0        0     3569 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_train_test_split_edges.py
+-rw-r--r--   0        0        0     5300 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_tree_decomposition.py
+-rw-r--r--   0        0        0     8307 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_trim_to_layer.py
+-rw-r--r--   0        0        0     2378 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_unbatch.py
+-rw-r--r--   0        0        0     8601 2024-04-26 06:12:57.897214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/augmentation.py
+-rw-r--r--   0        0        0    21740 2024-04-26 06:12:57.901214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/convert.py
+-rw-r--r--   0        0        0     3047 2024-04-26 06:12:57.901214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/cross_entropy.py
+-rw-r--r--   0        0        0    11416 2024-04-26 06:12:57.901214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/dropout.py
+-rw-r--r--   0        0        0     1675 2024-04-26 06:12:57.901214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/embedding.py
+-rw-r--r--   0        0        0      703 2024-04-26 06:12:57.901214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/functions.py
+-rw-r--r--   0        0        0     4668 2024-04-26 06:12:57.901214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/geodesic.py
+-rw-r--r--   0        0        0     5542 2024-04-26 06:12:57.901214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/hetero.py
+-rw-r--r--   0        0        0     3588 2024-04-26 06:12:57.901214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/isolated.py
+-rw-r--r--   0        0        0     3695 2024-04-26 06:12:57.901214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/laplacian.py
+-rw-r--r--   0        0        0    23051 2024-04-26 06:12:57.901214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/loop.py
+-rw-r--r--   0        0        0     5918 2024-04-26 06:12:57.901214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/map.py
+-rw-r--r--   0        0        0     2340 2024-04-26 06:12:57.901214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/mask.py
+-rw-r--r--   0        0        0     4387 2024-04-26 06:12:57.901214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/mesh_laplacian.py
+-rw-r--r--   0        0        0      699 2024-04-26 06:12:57.901214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/mixin.py
+-rw-r--r--   0        0        0     3310 2024-04-26 06:12:57.901214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/nested.py
+-rw-r--r--   0        0        0     3750 2024-04-26 06:12:57.901214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/noise_scheduler.py
+-rw-r--r--   0        0        0     2176 2024-04-26 06:12:57.901214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/num_nodes.py
+-rw-r--r--   0        0        0     4055 2024-04-26 06:12:57.901214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/ppr.py
+-rw-r--r--   0        0        0     5148 2024-04-26 06:12:57.901214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/random.py
+-rw-r--r--   0        0        0      815 2024-04-26 06:12:57.901214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/repeat.py
+-rw-r--r--   0        0        0     6242 2024-04-26 06:12:57.901214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/smiles.py
+-rw-r--r--   0        0        0    25330 2024-04-26 06:12:57.901214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/sparse.py
+-rw-r--r--   0        0        0     6222 2024-04-26 06:12:57.901214 pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/undirected.py
+-rw-r--r--   0        0        0      154 2024-04-26 06:12:57.901214 pyg_nightly-2.6.0.dev20240426/torch_geometric/visualization/__init__.py
+-rw-r--r--   0        0        0     4813 2024-04-26 06:12:57.901214 pyg_nightly-2.6.0.dev20240426/torch_geometric/visualization/graph.py
+-rw-r--r--   0        0        0      477 2024-04-26 06:12:57.901214 pyg_nightly-2.6.0.dev20240426/torch_geometric/visualization/influence.py
+-rw-r--r--   0        0        0      413 2024-04-26 06:12:57.901214 pyg_nightly-2.6.0.dev20240426/torch_geometric/warnings.py
+-rw-r--r--   0        0        0    62912 1970-01-01 00:00:00.000000 pyg_nightly-2.6.0.dev20240426/PKG-INFO
```

### Comparing `pyg_nightly-2.6.0.dev20240425/README.md` & `pyg_nightly-2.6.0.dev20240426/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 [![Slack][slack-image]][slack-url]
 
 **[Documentation](https://pytorch-geometric.readthedocs.io)** | **[Paper](https://arxiv.org/abs/1903.02428)** | **[Colab Notebooks and Video Tutorials](https://pytorch-geometric.readthedocs.io/en/latest/get_started/colabs.html)** | **[External Resources](https://pytorch-geometric.readthedocs.io/en/latest/external/resources.html)** | **[OGB Examples](https://github.com/snap-stanford/ogb/tree/master/examples)**
 
 **PyG** *(PyTorch Geometric)* is a library built upon [PyTorch](https://pytorch.org/) to easily write and train Graph Neural Networks (GNNs) for a wide range of applications related to structured data.
 
 It consists of various methods for deep learning on graphs and other irregular structures, also known as *[geometric deep learning](http://geometricdeeplearning.com/)*, from a variety of published papers.
-In addition, it consists of easy-to-use mini-batch loaders for operating on many small and single giant graphs, [multi GPU-support](https://github.com/pyg-team/pytorch_geometric/tree/master/examples/multi_gpu), [`torch.compile`](https://pytorch-geometric.readthedocs.io/en/latest/advanced/compile.html) support, [`DataPipe`](https://github.com/pyg-team/pytorch_geometric/blob/master/examples/datapipe.py) support, a large number of common benchmark datasets (based on simple interfaces to create your own), the [GraphGym](https://pytorch-geometric.readthedocs.io/en/latest/advanced/graphgym.html) experiment manager, and helpful transforms, both for learning on arbitrary graphs as well as on 3D meshes or point clouds.
+In addition, it consists of easy-to-use mini-batch loaders for operating on many small and single giant graphs, [multi GPU-support](https://github.com/pyg-team/pytorch_geometric/tree/master/examples/multi_gpu), [`torch.compile`](https://pytorch-geometric.readthedocs.io/en/latest/advanced/compile.html) support, [`DataPipe`](https://github.com/pyg-team/pytorch_geometric/blob/master/examples/datapipe.py) support, a large number of common benchmark datasets (based on simple interfaces to create your own), and helpful transforms, both for learning on arbitrary graphs as well as on 3D meshes or point clouds.
 
 **[Click here to join our Slack community!][slack-url]**
 
 <p align="center">
   <a href="https://medium.com/stanford-cs224w"><img style="max-width: 941px" src="https://data.pyg.org/img/cs224w_tutorials.png" /></a>
 </p>
 
@@ -43,15 +43,14 @@
 - **Comprehensive and well-maintained GNN models**:
   Most of the state-of-the-art Graph Neural Network architectures have been implemented by library developers or authors of research papers and are ready to be applied.
 - **Great flexibility**:
   Existing PyG models can easily be extended for conducting your own research with GNNs.
   Making modifications to existing models or creating new architectures is simple, thanks to its easy-to-use message passing API, and a variety of operators and utility functions.
 - **Large-scale real-world GNN models**:
   We focus on the need of GNN applications in challenging real-world scenarios, and support learning on diverse types of graphs, including but not limited to: scalable GNNs for graphs with millions of nodes; dynamic GNNs for node predictions over time; heterogeneous GNNs with multiple node types and edge types.
-- **GraphGym integration**: GraphGym lets users easily reproduce GNN experiments, is able to launch and analyze thousands of different GNN configurations, and is customizable by registering new modules to a GNN learning pipeline.
 
 ## Quick Tour for New Users
 
 In this quick tour, we highlight the ease of creating and training a GNN model with only a few lines of code.
 
 ### Train your own GNN model
 
@@ -135,28 +134,14 @@
     def message(self, x_j: Tensor, x_i: Tensor) -> Tensor:
         # x_j: Source node features of shape [num_edges, in_channels]
         # x_i: Target node features of shape [num_edges, in_channels]
         edge_features = torch.cat([x_i, x_j - x_i], dim=-1)
         return self.mlp(edge_features)  # shape [num_edges, out_channels]
 ```
 
-### Manage experiments with GraphGym
-
-GraphGym allows you to manage and launch GNN experiments, using a highly modularized pipeline (see [here](https://pytorch-geometric.readthedocs.io/en/latest/advanced/graphgym.html) for the accompanying tutorial).
-
-```
-git clone https://github.com/pyg-team/pytorch_geometric.git
-cd pytorch_geometric/graphgym
-bash run_single.sh  # run a single GNN experiment (node/edge/graph-level)
-bash run_batch.sh   # run a batch of GNN experiments, using differnt GNN designs/datasets/tasks
-```
-
-Users are highly encouraged to check out the [documentation](https://pytorch-geometric.readthedocs.io/en/latest), which contains additional tutorials on the essential functionalities of PyG, including data handling, creation of datasets and a full list of implemented methods, transforms, and datasets.
-For a quick start, check out our [examples](https://github.com/pyg-team/pytorch_geometric/tree/master/examples) in `examples/`.
-
 ## Architecture Overview
 
 PyG provides a multi-layer framework that enables users to build Graph Neural Network solutions on both low and high levels.
 It comprises of the following components:
 
 - The PyG **engine** utilizes the powerful PyTorch deep learning framework with full [`torch.compile`](https://pytorch-geometric.readthedocs.io/en/latest/advanced/compile.html) and [TorchScript](https://pytorch-geometric.readthedocs.io/en/latest/advanced/jit.html) support, as well as additions of efficient CPU/CUDA libraries for operating on sparse data, *e.g.*, [`pyg-lib`](https://github.com/pyg-team/pyg-lib).
 - The PyG **storage** handles data processing, transformation and loading pipelines. It is capable of handling and processing large-scale graph datasets, and provides effective solutions for heterogeneous graphs. It further provides a variety of sampling solutions, which enable training of GNNs on large-scale graphs.
```

### Comparing `pyg_nightly-2.6.0.dev20240425/pyproject.toml` & `pyg_nightly-2.6.0.dev20240426/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires=["flit_core >=3.2,<4"]
 build-backend="flit_core.buildapi"
 
 [project]
 name="pyg-nightly"
-version="2.6.0.dev20240425"
+version="2.6.0.dev20240426"
 authors=[
     {name="Matthias Fey", email="matthias@pyg.org"},
 ]
 description="Graph Neural Network Library for PyTorch"
 readme="README.md"
 requires-python=">=3.8"
 keywords=[
```

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/__init__.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from .experimental import (is_experimental_mode_enabled, experimental_mode,
                            set_experimental_mode)
 from .lazy_loader import LazyLoader
 
 contrib = LazyLoader('contrib', globals(), 'torch_geometric.contrib')
 graphgym = LazyLoader('graphgym', globals(), 'torch_geometric.graphgym')
 
-__version__ = '2.6.0.dev20240425'
+__version__ = '2.6.0.dev20240426'
 
 __all__ = [
     'EdgeIndex',
     'seed_everything',
     'get_home_dir',
     'set_home_dir',
     'compile',
```

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/_compile.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/_compile.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/backend.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/backend.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/config_store.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/config_store.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/contrib/explain/pgm_explainer.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/contrib/explain/pgm_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/contrib/nn/models/rbcd_attack.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/contrib/nn/models/rbcd_attack.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/data/__init__.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/data/batch.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/data/batch.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/data/collate.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/data/collate.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,16 @@
             for nested_tensor in values:
                 tensors.extend(nested_tensor.unbind())
             value = torch.nested.nested_tensor(tensors)
 
             return value, slices, incs
 
         out = None
-        if torch.utils.data.get_worker_info() is not None:
+        if (torch.utils.data.get_worker_info() is not None
+                and not isinstance(elem, EdgeIndex)):
             # Write directly into shared memory to avoid an extra copy:
             numel = sum(value.numel() for value in values)
             if torch_geometric.typing.WITH_PT20:
                 storage = elem.untyped_storage()._new_shared(
                     numel * elem.element_size(), device=elem.device)
             elif torch_geometric.typing.WITH_PT112:
                 storage = elem.storage()._new_shared(numel, device=elem.device)
```

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/data/data.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/data/data.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/data/database.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/data/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -462,15 +462,16 @@
                 meta = torch.tensor([
                     num_rows if num_rows is not None else -1,
                     num_cols if num_cols is not None else -1,
                     SORT_ORDER_TO_INDEX[col._sort_order],
                     col.is_undirected,
                 ], dtype=torch.long)
 
-                out.append(meta.numpy().tobytes() + col.numpy().tobytes())
+                out.append(meta.numpy().tobytes() +
+                           col.as_tensor().numpy().tobytes())
 
             elif isinstance(schema, TensorInfo):
                 assert isinstance(col, Tensor)
                 out.append(col.numpy().tobytes())
 
             elif schema in {int, float, str}:
                 out.append(col)
```

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/data/datapipes.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/data/datapipes.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/data/dataset.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/data/dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/data/download.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/data/download.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/data/extract.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/data/extract.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/data/feature_store.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/data/feature_store.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/data/graph_store.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/data/graph_store.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/data/hetero_data.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/data/hetero_data.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/data/hypergraph_data.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/data/hypergraph_data.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/data/in_memory_dataset.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/data/in_memory_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/data/lightning/datamodule.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/data/lightning/datamodule.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/data/on_disk_dataset.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/data/on_disk_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/data/remote_backend_utils.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/data/remote_backend_utils.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/data/separate.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/data/separate.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/data/storage.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/data/storage.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/data/summary.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/data/summary.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/data/temporal.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/data/temporal.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/data/view.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/data/view.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/__init__.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/actor.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/actor.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/airfrans.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/airfrans.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/airports.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/airports.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/amazon.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/amazon.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/amazon_book.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/amazon_book.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/amazon_products.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/amazon_products.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/aminer.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/aminer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/aqsol.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/aqsol.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/attributed_graph_dataset.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/attributed_graph_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/ba2motif_dataset.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/ba2motif_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/ba_multi_shapes.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/ba_multi_shapes.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/ba_shapes.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/ba_shapes.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/bitcoin_otc.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/bitcoin_otc.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/brca_tgca.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/brca_tgca.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/citation_full.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/citation_full.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/coauthor.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/coauthor.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/coma.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/coma.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/cornell.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/cornell.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/dblp.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/dblp.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/dbp15k.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/dbp15k.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/deezer_europe.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/deezer_europe.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/dgraph.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/dgraph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/dynamic_faust.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/dynamic_faust.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/elliptic.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/elliptic.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/elliptic_temporal.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/elliptic_temporal.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/email_eu_core.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/email_eu_core.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/entities.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/entities.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/explainer_dataset.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/explainer_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/facebook.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/facebook.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/fake.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/fake.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/faust.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/faust.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/flickr.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/flickr.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/freebase.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/freebase.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/gdelt.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/gdelt.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/gdelt_lite.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/gdelt_lite.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/ged_dataset.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/ged_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/gemsec.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/gemsec.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/geometry.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/geometry.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/github.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/github.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/gnn_benchmark_dataset.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/gnn_benchmark_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/graph_generator/ba_graph.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/graph_generator/ba_graph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/graph_generator/base.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/graph_generator/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/graph_generator/er_graph.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/graph_generator/er_graph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/graph_generator/grid_graph.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/graph_generator/grid_graph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/graph_generator/tree_graph.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/graph_generator/tree_graph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/heterophilous_graph_dataset.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/heterophilous_graph_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/hgb_dataset.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/hgb_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/hm.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/hm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/hydro_net.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/hydro_net.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/icews.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/icews.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/igmc_dataset.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/igmc_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/imdb.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/imdb.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/infection_dataset.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/infection_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/jodie.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/jodie.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/karate.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/karate.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/last_fm.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/last_fm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/lastfm_asia.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/lastfm_asia.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/linkx_dataset.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/linkx_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/lrgb.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/lrgb.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/malnet_tiny.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/malnet_tiny.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/md17.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/md17.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/mixhop_synthetic_dataset.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/mixhop_synthetic_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/mnist_superpixels.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/mnist_superpixels.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/modelnet.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/modelnet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/molecule_net.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/molecule_net.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/motif_generator/base.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/motif_generator/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/motif_generator/custom.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/motif_generator/custom.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/motif_generator/cycle.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/motif_generator/cycle.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/motif_generator/grid.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/motif_generator/grid.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/motif_generator/house.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/motif_generator/house.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/movie_lens.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/movie_lens.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/movie_lens_100k.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/movie_lens_100k.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/movie_lens_1m.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/movie_lens_1m.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/myket.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/myket.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/nell.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/nell.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/neurograph.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/neurograph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/ogb_mag.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/ogb_mag.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/omdb.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/omdb.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/ose_gvcs.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/ose_gvcs.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/particle.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/particle.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/pascal.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/pascal.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/pascal_pf.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/pascal_pf.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/pcpnet_dataset.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/pcpnet_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/pcqm4m.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/pcqm4m.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/planetoid.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/planetoid.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/polblogs.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/polblogs.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/ppi.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/ppi.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/qm7.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/qm7.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/qm9.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/qm9.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/rcdd.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/rcdd.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/reddit.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/reddit.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/reddit2.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/reddit2.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/rel_link_pred_dataset.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/rel_link_pred_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/s3dis.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/s3dis.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import os.path as osp
 from typing import Callable, List, Optional
 
 import torch
+from torch import Tensor
 
 from torch_geometric.data import (
     Data,
     InMemoryDataset,
     download_url,
     extract_zip,
 )
@@ -87,15 +88,16 @@
 
         with open(self.raw_paths[0], 'r') as f:
             filenames = [x.split('/')[-1] for x in f.read().split('\n')[:-1]]
 
         with open(self.raw_paths[1], 'r') as f:
             rooms = f.read().split('\n')[:-1]
 
-        xs, ys = [], []
+        xs: List[Tensor] = []
+        ys: List[Tensor] = []
         for filename in filenames:
             h5 = h5py.File(osp.join(self.raw_dir, filename))
             xs += torch.from_numpy(h5['data'][:]).unbind(0)
             ys += torch.from_numpy(h5['label'][:]).to(torch.long).unbind(0)
 
         test_area = f'Area_{self.test_area}'
         train_data_list, test_data_list = [], []
```

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/sbm_dataset.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/sbm_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/shapenet.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/shapenet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/shrec2016.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/shrec2016.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/snap_dataset.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/snap_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/suite_sparse.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/suite_sparse.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/taobao.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/taobao.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/tosca.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/tosca.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/tu_dataset.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/tu_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/twitch.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/twitch.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/upfd.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/upfd.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/utils/cheatsheet.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/utils/cheatsheet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/webkb.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/webkb.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/wikics.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/wikics.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/wikidata.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/wikidata.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/wikipedia_network.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/wikipedia_network.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/willow_object_class.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/willow_object_class.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/word_net.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/word_net.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/yelp.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/yelp.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/datasets/zinc.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/datasets/zinc.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/debug.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/debug.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/deprecation.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/deprecation.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/distributed/__init__.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/distributed/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/distributed/dist_link_neighbor_loader.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/distributed/dist_link_neighbor_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/distributed/dist_loader.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/distributed/dist_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/distributed/dist_neighbor_loader.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/distributed/dist_neighbor_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/distributed/dist_neighbor_sampler.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/distributed/dist_neighbor_sampler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/distributed/event_loop.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/distributed/event_loop.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/distributed/local_feature_store.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/distributed/local_feature_store.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/distributed/local_graph_store.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/distributed/local_graph_store.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/distributed/partition.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/distributed/partition.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/distributed/rpc.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/distributed/rpc.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/distributed/utils.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/distributed/utils.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/edge_index.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/edge_index.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 import functools
 import typing
 from enum import Enum
 from typing import (
     Any,
     Callable,
     Dict,
+    Iterable,
     List,
     Literal,
     NamedTuple,
     Optional,
     Sequence,
     Set,
     Tuple,
     Type,
     Union,
     get_args,
     overload,
 )
 
 import torch
+import torch.utils._pytree as pytree
 from torch import Tensor
 
 import torch_geometric.typing
 from torch_geometric import is_compiling
 from torch_geometric.typing import SparseTensor
 
+aten = torch.ops.aten
+
 HANDLED_FUNCTIONS: Dict[Callable, Callable] = {}
 
 if torch_geometric.typing.WITH_PT20:
     SUPPORTED_DTYPES: Set[torch.dtype] = {
         torch.int32,
         torch.int64,
     }
@@ -132,15 +136,15 @@
                          f"(got {tensor.dim()} dimensions)")
     if not torch.jit.is_tracing() and tensor.size(0) != 2:
         raise ValueError(f"'EdgeIndex' needs to have a shape of "
                          f"[2, *] (got {list(tensor.size())})")
 
 
 def assert_contiguous(tensor: Tensor) -> None:
-    if not tensor.is_contiguous():
+    if not tensor[0].is_contiguous() or not tensor[1].is_contiguous():
         raise ValueError("'EdgeIndex' needs to be contiguous. Please call "
                          "`edge_index.contiguous()` before proceeding.")
 
 
 def assert_symmetric(size: Tuple[Optional[int], Optional[int]]) -> None:
     if (not torch.jit.is_tracing() and size[0] is not None
             and size[1] is not None and size[0] != size[1]):
@@ -225,15 +229,15 @@
         out = edge_index.flip(0) @ torch.randn(3, 16)
         assert out.size() == (3, 16)
     """
     # See "https://pytorch.org/docs/stable/notes/extending.html"
     # for a basic tutorial on how to subclass `torch.Tensor`.
 
     # The underlying tensor representation:
-    _data: Optional[Tensor] = None
+    _data: Tensor
 
     # The size of the underlying sparse matrix:
     _sparse_size: Tuple[Optional[int], Optional[int]] = (None, None)
 
     # Whether the `edge_index` represented is non-sorted (`None`), or sorted
     # based on row or column values.
     _sort_order: Optional[SortOrder] = None
@@ -256,14 +260,15 @@
     # A cached "1"-value vector for `torch.sparse` matrix multiplication:
     _value: Optional[Tensor] = None
 
     # Whenever we perform a concatenation of edge indices, we cache the
     # original metadata to be able to reconstruct individual edge indices:
     _cat_metadata: Optional[CatMetadata] = None
 
+    @staticmethod
     def __new__(
         cls: Type,
         data: Any,
         *args: Any,
         sparse_size: Optional[Tuple[Optional[int], Optional[int]]] = None,
         sort_order: Optional[Union[str, SortOrder]] = None,
         is_undirected: bool = False,
@@ -332,23 +337,27 @@
         if is_undirected:
             assert_symmetric(sparse_size)
             if sparse_size[0] is not None and sparse_size[1] is None:
                 sparse_size = (sparse_size[0], sparse_size[0])
             elif sparse_size[0] is None and sparse_size[1] is not None:
                 sparse_size = (sparse_size[1], sparse_size[1])
 
-        if torch_geometric.typing.WITH_PT112:
-            out = super().__new__(cls, data)
-        else:
-            out = Tensor._make_subclass(cls, data)
+        out = Tensor._make_wrapper_subclass(  # type: ignore
+            cls,
+            size=data.size(),
+            strides=data.stride(),
+            dtype=data.dtype,
+            device=data.device,
+            layout=data.layout,
+            requires_grad=False,
+        )
+        assert isinstance(out, EdgeIndex)
 
         # Attach metadata:
-        assert isinstance(out, EdgeIndex)
-        if torch_geometric.typing.WITH_PT22:
-            out._data = data
+        out._data = data
         out._sparse_size = sparse_size
         out._sort_order = None if sort_order is None else SortOrder(sort_order)
         out._is_undirected = is_undirected
         out._indptr = indptr
 
         if isinstance(data, cls):  # If passed `EdgeIndex`, inherit metadata:
             out._T_perm = data._T_perm
@@ -374,49 +383,51 @@
 
         In particular, it ensures that
 
         * it only holds valid indices.
         * the sort order is correctly set.
         * indices are bidirectional in case it is specified as undirected.
         """
-        assert_valid_dtype(self)
-        assert_two_dimensional(self)
-        assert_contiguous(self)
+        assert_valid_dtype(self._data)
+        assert_two_dimensional(self._data)
+        assert_contiguous(self._data)
         if self.is_undirected:
             assert_symmetric(self.sparse_size())
 
-        if self.numel() > 0 and self.min() < 0:
+        if self.numel() > 0 and self._data.min() < 0:
             raise ValueError(f"'{self.__class__.__name__}' contains negative "
                              f"indices (got {int(self.min())})")
 
         if (self.numel() > 0 and self.num_rows is not None
-                and self[0].max() >= self.num_rows):
+                and self._data[0].max() >= self.num_rows):
             raise ValueError(f"'{self.__class__.__name__}' contains larger "
                              f"indices than its number of rows "
-                             f"(got {int(self[0].max())}, but expected values "
-                             f"smaller than {self.num_rows})")
+                             f"(got {int(self._data[0].max())}, but expected "
+                             f"values smaller than {self.num_rows})")
 
         if (self.numel() > 0 and self.num_cols is not None
-                and self[1].max() >= self.num_cols):
+                and self._data[1].max() >= self.num_cols):
             raise ValueError(f"'{self.__class__.__name__}' contains larger "
                              f"indices than its number of columns "
-                             f"(got {int(self[1].max())}, but expected values "
-                             f"smaller than {self.num_cols})")
+                             f"(got {int(self._data[1].max())}, but expected "
+                             f"values smaller than {self.num_cols})")
 
-        if self.is_sorted_by_row and (self[0].diff() < 0).any():
+        if self.is_sorted_by_row and (self._data[0].diff() < 0).any():
             raise ValueError(f"'{self.__class__.__name__}' is not sorted by "
                              f"row indices")
 
-        if self.is_sorted_by_col and (self[1].diff() < 0).any():
+        if self.is_sorted_by_col and (self._data[1].diff() < 0).any():
             raise ValueError(f"'{self.__class__.__name__}' is not sorted by "
                              f"column indices")
 
         if self.is_undirected:
-            flat_index1 = (self[0] * self.get_num_rows() + self[1]).sort()[0]
-            flat_index2 = (self[1] * self.get_num_cols() + self[0]).sort()[0]
+            flat_index1 = self._data[0] * self.get_num_rows() + self._data[1]
+            flat_index1 = flat_index1.sort()[0]
+            flat_index2 = self._data[1] * self.get_num_cols() + self._data[0]
+            flat_index2 = flat_index2.sort()[0]
             if not torch.equal(flat_index1, flat_index2):
                 raise ValueError(f"'{self.__class__.__name__}' is not "
                                  f"undirected")
 
         return self
 
     # Properties ##############################################################
@@ -507,19 +518,19 @@
         """
         if dim is not None:
             size = self._sparse_size[dim]
             if size is not None:
                 return size
 
             if self.is_undirected:
-                size = int(self.max()) + 1 if self.numel() > 0 else 0
+                size = int(self._data.max()) + 1 if self.numel() > 0 else 0
                 self._sparse_size = (size, size)
                 return size
 
-            size = int(self[dim].max()) + 1 if self.numel() > 0 else 0
+            size = int(self._data[dim].max()) + 1 if self.numel() > 0 else 0
             self._sparse_size = set_tuple_item(self._sparse_size, dim, size)
             return size
 
         return torch.Size((self.get_sparse_size(0), self.get_sparse_size(1)))
 
     def sparse_resize_(  # type: ignore
         self,
@@ -596,48 +607,49 @@
             return self._indptr
 
         if self.is_undirected and self._T_indptr is not None:
             return self._T_indptr
 
         dim = 0 if self.is_sorted_by_row else 1
         self._indptr = torch._convert_indices_from_coo_to_csr(
-            self[dim],
+            self._data[dim],
             self.get_sparse_size(dim),
             out_int32=self.dtype != torch.int64,
         )
 
         return self._indptr
 
     @assert_sorted
     def _sort_by_transpose(self) -> Tuple[Tuple[Tensor, Tensor], Tensor]:
         from torch_geometric.utils import index_sort
 
         dim = 1 if self.is_sorted_by_row else 0
 
         if self._T_perm is None:
-            index, perm = index_sort(self[dim], self.get_sparse_size(dim))
+            max_index = self.get_sparse_size(dim)
+            index, perm = index_sort(self._data[dim], max_index)
             self._T_index = set_tuple_item(self._T_index, dim, index)
-            self._T_perm = perm
+            self._T_perm = perm.to(self.dtype)
 
         if self._T_index[1 - dim] is None:
             self._T_index = set_tuple_item(  #
-                self._T_index, 1 - dim, self[1 - dim][self._T_perm])
+                self._T_index, 1 - dim, self._data[1 - dim][self._T_perm])
 
         row, col = self._T_index
         assert row is not None and col is not None
 
         return (row, col), self._T_perm
 
     @assert_sorted
-    def get_csr(self) -> Tuple[Tuple[Tensor, Tensor], Union[Tensor, slice]]:
+    def get_csr(self) -> Tuple[Tuple[Tensor, Tensor], Optional[Tensor]]:
         r"""Returns the compressed CSR representation
         :obj:`(rowptr, col), perm` in case :class:`EdgeIndex` is sorted.
         """
         if self.is_sorted_by_row:
-            return (self.get_indptr(), self[1]), slice(None, None, None)
+            return (self.get_indptr(), self._data[1]), None
 
         assert self.is_sorted_by_col
         (row, col), perm = self._sort_by_transpose()
 
         if self._T_indptr is not None:
             rowptr = self._T_indptr
         elif self.is_undirected and self._indptr is not None:
@@ -648,20 +660,20 @@
                 self.get_num_rows(),
                 out_int32=self.dtype != torch.int64,
             )
 
         return (rowptr, col), perm
 
     @assert_sorted
-    def get_csc(self) -> Tuple[Tuple[Tensor, Tensor], Union[Tensor, slice]]:
+    def get_csc(self) -> Tuple[Tuple[Tensor, Tensor], Optional[Tensor]]:
         r"""Returns the compressed CSC representation
         :obj:`(colptr, row), perm` in case :class:`EdgeIndex` is sorted.
         """
         if self.is_sorted_by_col:
-            return (self.get_indptr(), self[0]), slice(None, None, None)
+            return (self.get_indptr(), self._data[0]), None
 
         assert self.is_sorted_by_row
         (row, col), perm = self._sort_by_transpose()
 
         if self._T_indptr is not None:
             colptr = self._T_indptr
         elif self.is_undirected and self._indptr is not None:
@@ -706,19 +718,38 @@
             if not no_transpose:
                 self.get_csr()
 
         return self
 
     # Methods #################################################################
 
+    def share_memory_(self) -> 'EdgeIndex':
+        self._data.share_memory_()
+        if self._indptr is not None:
+            self._indptr.share_memory_()
+        if self._T_perm is not None:
+            self._T_perm.share_memory_()
+        if self._T_index[0] is not None:
+            self._T_index[0].share_memory_()
+        if self._T_index[1] is not None:
+            self._T_index[1].share_memory_()
+        if self._T_indptr is not None:
+            self._T_indptr.share_memory_()
+        if self._value is not None:
+            self._value.share_memory_()
+        return self
+
+    def is_shared(self) -> bool:
+        return self._data.is_shared()
+
     def as_tensor(self) -> Tensor:
         r"""Zero-copies the :class:`EdgeIndex` representation back to a
         :class:`torch.Tensor` representation.
         """
-        return self.as_subclass(Tensor)
+        return self._data
 
     def sort_by(
         self,
         sort_order: Union[str, SortOrder],
         stable: bool = False,
     ) -> 'SortReturnType':
         r"""Sorts the elements by row or column indices.
@@ -731,28 +762,28 @@
                 (default: :obj:`False`)
         """
         from torch_geometric.utils import index_sort
 
         sort_order = SortOrder(sort_order)
 
         if self._sort_order == sort_order:  # Nothing to do.
-            return SortReturnType(self, slice(None, None, None))
+            return SortReturnType(self, None)
 
         if self.is_sorted:
             (row, col), perm = self._sort_by_transpose()
             edge_index = torch.stack([row, col], dim=0)
 
         # Otherwise, perform sorting:
         elif sort_order == SortOrder.ROW:
-            row, perm = index_sort(self[0], self.get_num_rows(), stable)
-            edge_index = torch.stack([row, self[1][perm]], dim=0)
+            row, perm = index_sort(self._data[0], self.get_num_rows(), stable)
+            edge_index = torch.stack([row, self._data[1][perm]], dim=0)
 
         else:
-            col, perm = index_sort(self[1], self.get_num_cols(), stable)
-            edge_index = torch.stack([self[0][perm], col], dim=0)
+            col, perm = index_sort(self._data[1], self.get_num_cols(), stable)
+            edge_index = torch.stack([self._data[0][perm], col], dim=0)
 
         out = self.__class__(edge_index)
 
         # We can inherit metadata and (mostly) cache:
         out._sparse_size = self.sparse_size()
         out._sort_order = sort_order
         out._is_undirected = self.is_undirected
@@ -794,30 +825,30 @@
         dtype = value.dtype if value is not None else dtype
 
         size = self.get_sparse_size()
         if value is not None and value.dim() > 1:
             size = size + value.size()[1:]  # type: ignore
 
         out = torch.full(size, fill_value, dtype=dtype, device=self.device)
-        out[self[0], self[1]] = value if value is not None else 1
+        out[self._data[0], self._data[1]] = value if value is not None else 1
 
         return out
 
     def to_sparse_coo(self, value: Optional[Tensor] = None) -> Tensor:
         r"""Converts :class:`EdgeIndex` into a :pytorch:`null`
         :class:`torch.sparse_coo_tensor`.
 
         Args:
             value (torch.Tensor, optional): The values for non-zero elements.
                 If not specified, non-zero elements will be assigned a value of
                 :obj:`1.0`. (default: :obj:`None`)
         """
         value = self._get_value() if value is None else value
         out = torch.sparse_coo_tensor(
-            indices=self.as_tensor(),
+            indices=self._data,
             values=value,
             size=self.get_sparse_size(),
             device=self.device,
             requires_grad=value.requires_grad,
         )
 
         if self.is_sorted_by_row:
@@ -834,15 +865,18 @@
 
         Args:
             value (torch.Tensor, optional): The values for non-zero elements.
                 If not specified, non-zero elements will be assigned a value of
                 :obj:`1.0`. (default: :obj:`None`)
         """
         (rowptr, col), perm = self.get_csr()
-        value = self._get_value() if value is None else value[perm]
+        if value is not None and perm is not None:
+            value = value[perm]
+        elif value is None:
+            value = self._get_value()
 
         return torch.sparse_csr_tensor(
             crow_indices=rowptr,
             col_indices=col,
             values=value,
             size=self.get_sparse_size(),
             device=self.device,
@@ -862,15 +896,18 @@
                 :obj:`1.0`. (default: :obj:`None`)
         """
         if not torch_geometric.typing.WITH_PT112:
             raise NotImplementedError(
                 "'to_sparse_csc' not supported for PyTorch < 1.12")
 
         (colptr, row), perm = self.get_csc()
-        value = self._get_value() if value is None else value[perm]
+        if value is not None and perm is not None:
+            value = value[perm]
+        elif value is None:
+            value = self._get_value()
 
         return torch.sparse_csc_tensor(
             ccol_indices=colptr,
             row_indices=row,
             values=value,
             size=self.get_sparse_size(),
             device=self.device,
@@ -912,24 +949,24 @@
         Requires that :obj:`torch-sparse` is installed.
 
         Args:
             value (torch.Tensor, optional): The values for non-zero elements.
                 (default: :obj:`None`)
         """
         return SparseTensor(
-            row=self[0],
-            col=self[1],
+            row=self._data[0],
+            col=self._data[1],
             rowptr=self._indptr if self.is_sorted_by_row else None,
             value=value,
             sparse_sizes=self.get_sparse_size(),
             is_sorted=self.is_sorted_by_row,
             trust_data=True,
         )
 
-    # TODO investigate how to avoid overlapping return types here.
+    # TODO Investigate how to avoid overlapping return types here.
     @overload
     def matmul(  # type: ignore
         self,
         other: 'EdgeIndex',
         input_value: Optional[Tensor] = None,
         other_value: Optional[Tensor] = None,
         reduce: ReduceType = 'sum',
@@ -1034,15 +1071,15 @@
                              f"(got {start})")
 
         if dim == 0:
             (rowptr, col), _ = self.get_csr()
             rowptr = rowptr.narrow(0, start, length + 1)
 
             if rowptr.numel() < 2:
-                row, col = self[0, :0], self[1, :0]
+                row, col = self._data[0, :0], self._data[1, :0]
                 rowptr = None
                 num_rows = 0
             else:
                 col = col[rowptr[0]:rowptr[-1]]
                 rowptr = rowptr - rowptr[0]
                 num_rows = rowptr.numel() - 1
 
@@ -1064,15 +1101,15 @@
             return edge_index
 
         else:  # dim == 0:
             (colptr, row), _ = self.get_csc()
             colptr = colptr.narrow(0, start, length + 1)
 
             if colptr.numel() < 2:
-                row, col = self[0, :0], self[1, :0]
+                row, col = self._data[0, :0], self._data[1, :0]
                 colptr = None
                 num_cols = 0
             else:
                 row = row[colptr[0]:colptr[-1]]
                 colptr = colptr - colptr[0]
                 num_cols = colptr.numel() - 1
 
@@ -1089,42 +1126,66 @@
                 torch.stack([row, col], dim=0),
                 sparse_size=(self.sparse_size(0), num_cols),
                 sort_order='col',
             )
             edge_index._indptr = colptr
             return edge_index
 
+    # PyTorch/Python builtins #################################################
+
     def __tensor_flatten__(self) -> Tuple[List[str], Tuple[Any, ...]]:
-        if not torch_geometric.typing.WITH_PT22:  # pragma: no cover
-            raise RuntimeError("'torch.compile' with 'EdgeIndex' only "
-                               "supported from PyTorch 2.2 onwards")
-        assert self._data is not None
-        # TODO Add `_T_index`.
-        attrs = ['_data', '_indptr', '_T_perm', '_T_indptr']
-        return attrs, ()
+        attrs = ['_data']
+        if self._indptr is not None:
+            attrs.append('_indptr')
+        if self._T_perm is not None:
+            attrs.append('_T_perm')
+        # TODO We cannot save `_T_index` for now since it is stored as tuple.
+        if self._T_indptr is not None:
+            attrs.append('_T_indptr')
+
+        ctx = (
+            self._sparse_size,
+            self._sort_order,
+            self._is_undirected,
+            self._cat_metadata,
+        )
+
+        return attrs, ctx
 
     @staticmethod
     def __tensor_unflatten__(
-        inner_tensors: Tuple[Any],
+        inner_tensors: Dict[str, Any],
         ctx: Tuple[Any, ...],
-        *args: Any,
-        **kwargs: Any,
+        outer_size: Tuple[int, ...],
+        outer_stride: Tuple[int, ...],
     ) -> 'EdgeIndex':
-        if not torch_geometric.typing.WITH_PT22:  # pragma: no cover
-            raise RuntimeError("'torch.compile' with 'EdgeIndex' only "
-                               "supported from PyTorch 2.2 onwards")
-        raise NotImplementedError
+        edge_index = EdgeIndex(
+            inner_tensors['_data'],
+            sparse_size=ctx[0],
+            sort_order=ctx[1],
+            is_undirected=ctx[2],
+        )
+
+        edge_index._indptr = inner_tensors.get('_indptr', None)
+        edge_index._T_perm = inner_tensors.get('_T_perm', None)
+        edge_index._T_indptr = inner_tensors.get('_T_indptr', None)
+        edge_index._cat_metadata = ctx[3]
+
+        return edge_index
+
+    # Prevent auto-wrapping outputs back into the proper subclass type:
+    __torch_function__ = torch._C._disabled_torch_function_impl
 
     @classmethod
-    def __torch_function__(
+    def __torch_dispatch__(
         cls: Type,
-        func: Callable,
-        types: Tuple[Type, ...],
-        args: Tuple[Any, ...] = (),
-        kwargs: Optional[Dict[str, Any]] = None,
+        func: Callable[..., Any],
+        types: Iterable[Type[Any]],
+        args: Iterable[Tuple[Any, ...]] = (),
+        kwargs: Optional[Dict[Any, Any]] = None,
     ) -> Any:
         # `EdgeIndex` should be treated as a regular PyTorch tensor for all
         # standard PyTorch functionalities. However,
         # * some of its metadata can be transferred to new functions, e.g.,
         #   `torch.cat(dim=1)` can inherit the sparse matrix size, or
         #   `torch.narrow(dim=1)` can inherit cached pointers.
         # * not all operations lead to valid `EdgeIndex` tensors again, e.g.,
@@ -1132,77 +1193,102 @@
         #   `torch.cat(dim=0) violates the [2, *] shape assumption.
 
         # To account for this, we hold a number of `HANDLED_FUNCTIONS` that
         # implement specific functions for valid `EdgeIndex` routines.
         if func in HANDLED_FUNCTIONS:
             return HANDLED_FUNCTIONS[func](*args, **(kwargs or {}))
 
-        # For all other PyTorch functions, we return a vanilla PyTorch tensor.
-        _types = tuple(Tensor if issubclass(t, cls) else t for t in types)
-        return Tensor.__torch_function__(func, _types, args, kwargs)
-
-
-class SortReturnType(NamedTuple):
-    values: EdgeIndex
-    indices: Union[Tensor, slice]
+        # For all other PyTorch functions, we treat them as vanilla tensors.
+        args = pytree.tree_map_only(EdgeIndex, lambda x: x._data, args)
+        if kwargs is not None:
+            kwargs = pytree.tree_map_only(EdgeIndex, lambda x: x._data, kwargs)
+        return func(*args, **(kwargs or {}))
+
+    def __repr__(self) -> str:  # type: ignore
+        prefix = f'{self.__class__.__name__}('
+        indent = len(prefix)
+        tensor_str = torch._tensor_str._tensor_str(self._data, indent)
 
-
-@implements(Tensor.__repr__)
-def __repr__(
-    tensor: EdgeIndex,
-    *,
-    tensor_contents: Optional[str] = None,
-) -> str:
-    # Monkey-patch `torch._tensor_str._add_suffixes`. There might exist better
-    # solutions to attach additional metadata, but this seems to be the most
-    # straightforward one to inherit most of the `torch.Tensor` print logic:
-    orig_fn = torch._tensor_str._add_suffixes
-
-    def _add_suffixes(
-        tensor_str: str,
-        suffixes: List[str],
-        indent: int,
-        force_newline: bool,
-    ) -> str:
-
-        num_rows, num_cols = tensor.sparse_size()
+        suffixes = []
+        num_rows, num_cols = self.sparse_size()
         if num_rows is not None or num_cols is not None:
             size_repr = f"({num_rows or '?'}, {num_cols or '?'})"
             suffixes.append(f'sparse_size={size_repr}')
+        suffixes.append(f'nnz={self._data.size(1)}')
+        if (self.device.type != torch._C._get_default_device()
+                or (self.device.type == 'cuda'
+                    and torch.cuda.current_device() != self.device.index)
+                or (self.device.type == 'mps')):
+            suffixes.append(f"device='{self.device}'")
+        if self.dtype != torch.int64:
+            suffixes.append(f'dtype={self.dtype}')
+        if self.is_sorted:
+            suffixes.append(f'sort_order={self.sort_order}')
+        if self.is_undirected:
+            suffixes.append('is_undirected=True')
 
-        suffixes.append(f'nnz={tensor.size(1)}')
+        return torch._tensor_str._add_suffixes(prefix + tensor_str, suffixes,
+                                               indent, force_newline=False)
 
-        if tensor.is_sorted:
-            suffixes.append(f'sort_order={tensor.sort_order}')
+    # Helpers #################################################################
 
-        if tensor.is_undirected:
-            suffixes.append('is_undirected=True')
+    def _shallow_copy(self) -> 'EdgeIndex':
+        out = EdgeIndex(self._data)
+        out._sparse_size = self._sparse_size
+        out._sort_order = self._sort_order
+        out._is_undirected = self._is_undirected
+        out._indptr = self._indptr
+        out._T_perm = self._T_perm
+        out._T_index = self._T_index
+        out._T_indptr = self._T_indptr
+        out._value = self._value
+        out._cat_metadata = self._cat_metadata
+        return out
 
-        return orig_fn(tensor_str, suffixes, indent, force_newline)
+    def _clear_metadata(self) -> 'EdgeIndex':
+        self._sparse_size = (None, None)
+        self._sort_order = None
+        self._is_undirected = False
+        self._indptr = None
+        self._T_perm = None
+        self._T_index = (None, None)
+        self._T_indptr = None
+        self._value = None
+        self._cat_metadata = None
+        return self
 
-    torch._tensor_str._add_suffixes = _add_suffixes
-    out = torch._tensor_str._str(tensor, tensor_contents=tensor_contents)
-    torch._tensor_str._add_suffixes = orig_fn
-    return out
+
+class SortReturnType(NamedTuple):
+    values: EdgeIndex
+    indices: Optional[Tensor]
 
 
 def apply_(
     tensor: EdgeIndex,
     fn: Callable,
     *args: Any,
     **kwargs: Any,
-) -> EdgeIndex:
+) -> Union[EdgeIndex, Tensor]:
 
-    out = Tensor.__torch_function__(fn, (Tensor, ), (tensor, ) + args, kwargs)
-    out = out.as_subclass(EdgeIndex)
+    data = fn(tensor._data, *args, **kwargs)
+
+    if data.dtype not in SUPPORTED_DTYPES:
+        return data
+
+    if tensor._data.data_ptr() != data.data_ptr():
+        out = EdgeIndex(data)
+    else:  # In-place:
+        tensor._data = data
+        out = tensor
 
     # Copy metadata:
-    out._sparse_size = tensor.sparse_size()
+    out._sparse_size = tensor._sparse_size
     out._sort_order = tensor._sort_order
     out._is_undirected = tensor._is_undirected
+    out._cat_metadata = tensor._cat_metadata
 
     # Convert cache (but do not consider `_value`):
     if tensor._indptr is not None:
         out._indptr = fn(tensor._indptr, *args, **kwargs)
 
     if tensor._T_perm is not None:
         out._T_perm = fn(tensor._T_perm, *args, **kwargs)
@@ -1216,85 +1302,64 @@
 
     if tensor._T_indptr is not None:
         out._T_indptr = fn(tensor._T_indptr, *args, **kwargs)
 
     return out
 
 
-@implements(torch.clone)
-@implements(Tensor.clone)
-def clone(tensor: EdgeIndex) -> EdgeIndex:
-    return apply_(tensor, Tensor.clone)
-
-
-@implements(Tensor.to)
-def to(
+@implements(aten.clone.default)
+def _clone(
     tensor: EdgeIndex,
-    *args: Any,
-    **kwargs: Any,
-) -> Union[EdgeIndex, Tensor]:
-    out = apply_(tensor, Tensor.to, *args, **kwargs)
-    return out if out.dtype in SUPPORTED_DTYPES else out.as_tensor()
-
-
-@implements(Tensor.int)
-def _int(tensor: EdgeIndex) -> EdgeIndex:
-    return to(tensor, torch.int32)
-
-
-@implements(Tensor.long)
-def long(tensor: EdgeIndex, *args: Any, **kwargs: Any) -> EdgeIndex:
-    return to(tensor, torch.int64)
-
-
-@implements(Tensor.cpu)
-def cpu(tensor: EdgeIndex, *args: Any, **kwargs: Any) -> EdgeIndex:
-    return apply_(tensor, Tensor.cpu, *args, **kwargs)
-
-
-@implements(Tensor.cuda)
-def cuda(  # pragma: no cover
-    tensor: EdgeIndex,
-    *args: Any,
-    **kwargs: Any,
+    *,
+    memory_format: torch.memory_format = torch.preserve_format,
 ) -> EdgeIndex:
-    return apply_(tensor, Tensor.cuda, *args, **kwargs)
-
-
-@implements(Tensor.share_memory_)
-def share_memory_(tensor: EdgeIndex) -> EdgeIndex:
-    return apply_(tensor, Tensor.share_memory_)
+    out = apply_(tensor, aten.clone.default, memory_format=memory_format)
+    assert isinstance(out, EdgeIndex)
+    return out
 
 
-@implements(Tensor.contiguous)
-def contiguous(tensor: EdgeIndex) -> EdgeIndex:
-    return apply_(tensor, Tensor.contiguous)
+@implements(aten._to_copy.default)
+def _to_copy(
+    tensor: EdgeIndex,
+    *,
+    dtype: Optional[torch.dtype] = None,
+    layout: Optional[torch.layout] = None,
+    device: Optional[torch.device] = None,
+    pin_memory: bool = False,
+    non_blocking: bool = False,
+    memory_format: Optional[torch.memory_format] = None,
+) -> Union[EdgeIndex, Tensor]:
+    return apply_(
+        tensor,
+        aten._to_copy.default,
+        dtype=dtype,
+        layout=layout,
+        device=device,
+        pin_memory=pin_memory,
+        non_blocking=non_blocking,
+        memory_format=memory_format,
+    )
 
 
-@implements(torch.cat)
-def cat(
+@implements(aten.cat.default)
+def _cat(
     tensors: List[Union[EdgeIndex, Tensor]],
     dim: int = 0,
-    *,
-    out: Optional[Tensor] = None,
 ) -> Union[EdgeIndex, Tensor]:
 
-    if len(tensors) == 1:
-        return tensors[0]
-
-    output = Tensor.__torch_function__(torch.cat, (Tensor, ), (tensors, dim),
-                                       dict(out=out))
+    data_list = pytree.tree_map_only(EdgeIndex, lambda x: x._data, tensors)
+    data = aten.cat.default(data_list, dim=dim)
 
     if dim != 1 and dim != -1:  # No valid `EdgeIndex` anymore.
-        return output
+        return data
 
     if any([not isinstance(tensor, EdgeIndex) for tensor in tensors]):
-        return output
+        return data
 
-    output = output.as_subclass(EdgeIndex)
+    out = EdgeIndex(data)
 
     nnz_list = [t.size(1) for t in tensors]
     sparse_size_list = [t.sparse_size() for t in tensors]  # type: ignore
     sort_order_list = [t._sort_order for t in tensors]  # type: ignore
     is_undirected_list = [t.is_undirected for t in tensors]  # type: ignore
 
     # Post-process `sparse_size`:
@@ -1310,42 +1375,37 @@
     for _, num_cols in sparse_size_list:
         if num_cols is None:
             total_num_cols = None
             break
         assert isinstance(total_num_cols, int)
         num_cols = max(num_cols, total_num_cols)
 
-    output._sparse_size = (num_rows, num_cols)
+    out._sparse_size = (num_rows, num_cols)
 
     # Post-process `is_undirected`:
-    output._is_undirected = all(is_undirected_list)
+    out._is_undirected = all(is_undirected_list)
 
-    output._cat_metadata = CatMetadata(
+    out._cat_metadata = CatMetadata(
         nnz=nnz_list,
         sparse_size=sparse_size_list,
         sort_order=sort_order_list,
         is_undirected=is_undirected_list,
     )
 
-    return output
+    return out
 
 
-@implements(torch.flip)
-@implements(Tensor.flip)
-def flip(
+@implements(aten.flip.default)
+def _flip(
     input: EdgeIndex,
-    dims: Union[int, List[int], Tuple[int, ...]],
-) -> Union[EdgeIndex, Tensor]:
-
-    if isinstance(dims, int):
-        dims = [dims]
-    assert isinstance(dims, (tuple, list))
+    dims: Union[List[int], Tuple[int, ...]],
+) -> EdgeIndex:
 
-    out = Tensor.__torch_function__(torch.flip, (Tensor, ), (input, dims))
-    out = out.as_subclass(EdgeIndex)
+    data = aten.flip.default(input._data, dims)
+    out = EdgeIndex(data)
 
     out._value = input._value
     out._is_undirected = input.is_undirected
 
     # Flip metadata and cache:
     if 0 in dims or -2 in dims:
         out._sparse_size = input.sparse_size()[::-1]
@@ -1360,246 +1420,278 @@
         out._T_perm = input._T_perm
         out._T_index = input._T_index[::-1]
         out._T_indptr = input._indptr
 
     return out
 
 
-@implements(torch.index_select)
-@implements(Tensor.index_select)
-def index_select(
+@implements(aten.index_select.default)
+def _index_select(
     input: EdgeIndex,
     dim: int,
     index: Tensor,
-    *,
-    out: Optional[Tensor] = None,
 ) -> Union[EdgeIndex, Tensor]:
 
-    output = Tensor.__torch_function__(  #
-        torch.index_select, (Tensor, ), (input, dim, index), dict(out=out))
+    out = aten.index_select.default(input._data, dim, index)
 
     if dim == 1 or dim == -1:
-        output = output.as_subclass(EdgeIndex)
-        output._sparse_size = input.sparse_size()
+        out = EdgeIndex(out)
+        out._sparse_size = input.sparse_size()
 
-    return output
+    return out
 
 
-@implements(torch.narrow)
-@implements(Tensor.narrow)
-def narrow(
+@implements(aten.slice.Tensor)
+def _slice(
     input: EdgeIndex,
     dim: int,
-    start: Union[int, Tensor],
-    length: int,
+    start: Optional[int] = None,
+    end: Optional[int] = None,
+    step: int = 1,
 ) -> Union[EdgeIndex, Tensor]:
 
-    out = Tensor.__torch_function__(  #
-        torch.narrow, (Tensor, ), (input, dim, start, length))
+    if ((start is None or start <= 0)
+            and (end is None or end > input.size(dim)) and step == 1):
+        return input._shallow_copy()  # No-op.
+
+    out = aten.slice.Tensor(input._data, dim, start, end, step)
 
     if dim == 1 or dim == -1:
-        out = out.as_subclass(EdgeIndex)
+        if step != 1:
+            out = out.contiguous()
+
+        out = EdgeIndex(out)
         out._sparse_size = input.sparse_size()
         # NOTE We could potentially maintain `rowptr`/`colptr` attributes here,
         # but it is not really clear if this is worth it. The most important
         # information, the sort order, needs to be maintained though:
-        out._sort_order = input._sort_order
+        if step >= 0:
+            out._sort_order = input._sort_order
+        else:
+            if input._sort_order == SortOrder.ROW:
+                out._sort_order = SortOrder.COL
+            elif input._sort_order == SortOrder.COL:
+                out._sort_order = SortOrder.ROW
 
     return out
 
 
-@implements(Tensor.__getitem__)
-def getitem(input: EdgeIndex, index: Any) -> Union[EdgeIndex, Tensor]:
-    out = Tensor.__torch_function__(  #
-        Tensor.__getitem__, (Tensor, ), (input, index))
-
-    # There exists 3 possible index types that map back to a valid `EdgeIndex`,
-    # and all include selecting/filtering in the last dimension only:
-    def is_last_dim_select(i: Any) -> bool:
-        # Maps to true for `__getitem__` requests of the form
-        # `tensor[..., index]` or `tensor[:, index]`.
-        if not isinstance(i, tuple) or len(i) != 2:
-            return False
-        if i[0] == Ellipsis:
-            return True
-        if not isinstance(i[0], slice):
-            return False
-        return i[0].start is None and i[0].stop is None and i[0].step is None
+@implements(aten.index.Tensor)
+def _index(
+    input: Union[EdgeIndex, Tensor],
+    indices: List[Optional[Union[Tensor, EdgeIndex]]],
+) -> Union[EdgeIndex, Tensor]:
+
+    if not isinstance(input, EdgeIndex):
+        indices = pytree.tree_map_only(EdgeIndex, lambda x: x._data, indices)
+        return aten.index.Tensor(input, indices)
+
+    out = aten.index.Tensor(input._data, indices)
+
+    if len(indices) != 2 or indices[0] is not None:
+        return out
 
-    is_valid = is_last_dim_select(index)
+    index = indices[1]
+    assert isinstance(index, Tensor)
 
     # 1. `edge_index[:, mask]` or `edge_index[..., mask]`.
-    if (is_valid and isinstance(index[1], Tensor)
-            and index[1].dtype in (torch.bool, torch.uint8)):
-        out = out.as_subclass(EdgeIndex)
+    if index.dtype in (torch.bool, torch.uint8):
+        out = EdgeIndex(out)
         out._sparse_size = input.sparse_size()
         out._sort_order = input._sort_order
 
-    # 2. `edge_index[:, index]` or `edge_index[..., index]`.
-    elif is_valid and isinstance(index[1], Tensor):
-        out = out.as_subclass(EdgeIndex)
+    else:  # 2. `edge_index[:, index]` or `edge_index[..., index]`.
+        out = EdgeIndex(out)
         out._sparse_size = input.sparse_size()
 
-    # 3. `edge_index[:, slice]` or `edge_index[..., slice]`.
-    elif is_valid and isinstance(index[1], slice):
-        out = out.as_subclass(EdgeIndex)
-        out._sparse_size = input.sparse_size()
-        if index[1].step is None or index[1].step > 0:
-            out._sort_order = input._sort_order
-
     return out
 
 
-def postprocess_add_(
+@implements(aten.add.Tensor)
+def _add(
     input: EdgeIndex,
-    other: Union[int, Tensor],
-    out: Tensor,
+    other: Union[int, Tensor, EdgeIndex],
+    *,
     alpha: int = 1,
 ) -> Union[EdgeIndex, Tensor]:
 
+    out = aten.add.Tensor(
+        input._data,
+        other._data if isinstance(other, EdgeIndex) else other,
+        alpha=alpha,
+    )
+
     if out.dtype not in SUPPORTED_DTYPES:
         return out
     if out.dim() != 2 or out.size(0) != 2:
         return out
 
-    output: EdgeIndex = out.as_subclass(EdgeIndex)
+    out = EdgeIndex(out)
+
+    if isinstance(other, Tensor) and other.numel() <= 1:
+        other = int(other)
 
     if isinstance(other, int):
         size = maybe_add(input._sparse_size, other, alpha)
         assert len(size) == 2
-        output._sparse_size = size
-        output._sort_order = input._sort_order
-        output._is_undirected = input.is_undirected
-        output._T_perm = input._T_perm
-
-    elif isinstance(other, Tensor) and other.numel() <= 1:
-        size = maybe_add(input._sparse_size, int(other), alpha)
-        assert len(size) == 2
-        output._sparse_size = size
-        output._sort_order = input._sort_order
-        output._is_undirected = input.is_undirected
-        output._T_perm = input._T_perm
+        out._sparse_size = size
+        out._sort_order = input._sort_order
+        out._is_undirected = input.is_undirected
+        out._T_perm = input._T_perm
 
     elif isinstance(other, Tensor) and other.size() == (2, 1):
         size = maybe_add(input._sparse_size, other.view(-1).tolist(), alpha)
         assert len(size) == 2
-        output._sparse_size = size
-        output._sort_order = input._sort_order
-        output._T_perm = input._T_perm
+        out._sparse_size = size
+        out._sort_order = input._sort_order
         if torch.equal(other[0], other[1]):
-            output._is_undirected = input.is_undirected
+            out._is_undirected = input.is_undirected
+        out._T_perm = input._T_perm
 
     elif isinstance(other, EdgeIndex):
         size = maybe_add(input._sparse_size, other._sparse_size, alpha)
         assert len(size) == 2
-        output._sparse_size = size
+        out._sparse_size = size
 
-    return output
+    return out
 
 
-@implements(torch.add)
-@implements(Tensor.add)
-def add(
+@implements(aten.add_.Tensor)
+def add_(
     input: EdgeIndex,
-    other: Union[int, Tensor],
+    other: Union[int, Tensor, EdgeIndex],
     *,
     alpha: int = 1,
-    out: Optional[Tensor] = None,
-) -> Union[EdgeIndex, Tensor]:
+) -> EdgeIndex:
 
-    output = Tensor.__torch_function__(  #
-        torch.add, (Tensor, ), (input, other), dict(alpha=alpha, out=out))
+    sparse_size = input._sparse_size
+    sort_order = input._sort_order
+    is_undirected = input._is_undirected
+    T_perm = input._T_perm
+    input._clear_metadata()
+
+    aten.add_.Tensor(
+        input._data,
+        other._data if isinstance(other, EdgeIndex) else other,
+        alpha=alpha,
+    )
 
-    return postprocess_add_(input, other, output, alpha)
+    if isinstance(other, Tensor) and other.numel() <= 1:
+        other = int(other)
 
+    if isinstance(other, int):
+        size = maybe_add(sparse_size, other, alpha)
+        assert len(size) == 2
+        input._sparse_size = size
+        input._sort_order = sort_order
+        input._is_undirected = is_undirected
+        input._T_perm = T_perm
 
-@implements(Tensor.add_)
-def add_(
-    input: EdgeIndex,
-    other: Union[int, Tensor],
-    *,
-    alpha: int = 1,
-) -> Union[EdgeIndex, Tensor]:
+    elif isinstance(other, Tensor) and other.size() == (2, 1):
+        size = maybe_add(sparse_size, other.view(-1).tolist(), alpha)
+        assert len(size) == 2
+        input._sparse_size = size
+        input._sort_order = sort_order
+        if torch.equal(other[0], other[1]):
+            input._is_undirected = is_undirected
+        input._T_perm = T_perm
 
-    output = Tensor.__torch_function__(  #
-        Tensor.add_, (Tensor, ), (input, other), dict(alpha=alpha))
+    elif isinstance(other, EdgeIndex):
+        size = maybe_add(sparse_size, other._sparse_size, alpha)
+        assert len(size) == 2
+        input._sparse_size = size
 
-    return postprocess_add_(input, other, output, alpha)
+    return input
 
 
-def postprocess_sub_(
+@implements(aten.sub.Tensor)
+def _sub(
     input: EdgeIndex,
-    other: Union[int, Tensor],
-    out: Tensor,
+    other: Union[int, Tensor, EdgeIndex],
+    *,
     alpha: int = 1,
 ) -> Union[EdgeIndex, Tensor]:
 
+    out = aten.sub.Tensor(
+        input._data,
+        other._data if isinstance(other, EdgeIndex) else other,
+        alpha=alpha,
+    )
+
     if out.dtype not in SUPPORTED_DTYPES:
         return out
     if out.dim() != 2 or out.size(0) != 2:
         return out
 
-    output: EdgeIndex = out.as_subclass(EdgeIndex)
+    out = EdgeIndex(out)
+
+    if isinstance(other, Tensor) and other.numel() <= 1:
+        other = int(other)
 
     if isinstance(other, int):
         size = maybe_sub(input._sparse_size, other, alpha)
         assert len(size) == 2
-        output._sparse_size = size
-        output._sort_order = input._sort_order
-        output._is_undirected = input.is_undirected
-        output._T_perm = input._T_perm
-
-    elif isinstance(other, Tensor) and other.numel() <= 1:
-        size = maybe_sub(input._sparse_size, int(other), alpha)
-        assert len(size) == 2
-        output._sparse_size = size
-        output._sort_order = input._sort_order
-        output._is_undirected = input.is_undirected
-        output._T_perm = input._T_perm
+        out._sparse_size = size
+        out._sort_order = input._sort_order
+        out._is_undirected = input.is_undirected
+        out._T_perm = input._T_perm
 
     elif isinstance(other, Tensor) and other.size() == (2, 1):
         size = maybe_sub(input._sparse_size, other.view(-1).tolist(), alpha)
         assert len(size) == 2
-        output._sparse_size = size
-        output._sort_order = input._sort_order
-        output._T_perm = input._T_perm
+        out._sparse_size = size
+        out._sort_order = input._sort_order
         if torch.equal(other[0], other[1]):
-            output._is_undirected = input.is_undirected
+            out._is_undirected = input.is_undirected
+        out._T_perm = input._T_perm
 
-    return output
+    return out
 
 
-@implements(torch.sub)
-@implements(Tensor.sub)
-def sub(
+@implements(aten.sub_.Tensor)
+def sub_(
     input: EdgeIndex,
-    other: Union[int, Tensor],
+    other: Union[int, Tensor, EdgeIndex],
     *,
     alpha: int = 1,
-    out: Optional[Tensor] = None,
-) -> Union[EdgeIndex, Tensor]:
-
-    output = Tensor.__torch_function__(  #
-        torch.sub, (Tensor, ), (input, other), dict(alpha=alpha, out=out))
+) -> EdgeIndex:
 
-    return postprocess_sub_(input, other, output, alpha)
+    sparse_size = input._sparse_size
+    sort_order = input._sort_order
+    is_undirected = input._is_undirected
+    T_perm = input._T_perm
+    input._clear_metadata()
+
+    aten.sub_.Tensor(
+        input._data,
+        other._data if isinstance(other, EdgeIndex) else other,
+        alpha=alpha,
+    )
 
+    if isinstance(other, Tensor) and other.numel() <= 1:
+        other = int(other)
 
-@implements(Tensor.sub_)
-def sub_(
-    input: EdgeIndex,
-    other: Union[int, Tensor],
-    *,
-    alpha: int = 1,
-) -> Union[EdgeIndex, Tensor]:
+    if isinstance(other, int):
+        size = maybe_sub(sparse_size, other, alpha)
+        assert len(size) == 2
+        input._sparse_size = size
+        input._sort_order = sort_order
+        input._is_undirected = is_undirected
+        input._T_perm = T_perm
 
-    output = Tensor.__torch_function__(  #
-        Tensor.sub_, (Tensor, ), (input, other), dict(alpha=alpha))
+    elif isinstance(other, Tensor) and other.size() == (2, 1):
+        size = maybe_sub(sparse_size, other.view(-1).tolist(), alpha)
+        assert len(size) == 2
+        input._sparse_size = size
+        input._sort_order = sort_order
+        if torch.equal(other[0], other[1]):
+            input._is_undirected = is_undirected
+        input._T_perm = T_perm
 
-    return postprocess_sub_(input, other, output, alpha)
+    return input
 
 
 # Sparse-Dense Matrix Multiplication ##########################################
 
 
 def _torch_sparse_spmm(
     input: EdgeIndex,
@@ -1695,15 +1787,15 @@
             assert ctx.reduce == 'sum'
 
             if not ctx.transpose:
                 if value is None and input.is_undirected:
                     adj = input.to_sparse_csr(value)
                 else:
                     (colptr, row), perm = input.get_csc()
-                    if value is not None:
+                    if value is not None and perm is not None:
                         value = value[perm]
                     else:
                         value = input._get_value()
                     adj = torch.sparse_csr_tensor(
                         crow_indices=colptr,
                         col_indices=row,
                         values=value,
@@ -1711,15 +1803,15 @@
                         device=input.device,
                     )
             else:
                 if value is None and input.is_undirected:
                     adj = input.to_sparse_csc(value).t()
                 else:
                     (rowptr, col), perm = input.get_csr()
-                    if value is not None:
+                    if value is not None and perm is not None:
                         value = value[perm]
                     else:
                         value = input._get_value()
                     adj = torch.sparse_csr_tensor(
                         crow_indices=rowptr,
                         col_indices=col,
                         values=value,
@@ -1742,20 +1834,20 @@
     value: Optional[Tensor] = None,
     reduce: ReduceType = 'sum',
     transpose: bool = False,
 ) -> Tensor:
     from torch_geometric.utils import scatter
 
     if not transpose:
-        other_j = other[input[1]]
-        index = input[0]
+        other_j = other[input._data[1]]
+        index = input._data[0]
         dim_size = input.get_sparse_size(0)
     else:
-        other_j = other[input[0]]
-        index = input[1]
+        other_j = other[input._data[0]]
+        index = input._data[1]
         dim_size = input.get_sparse_size(1)
 
     other_j = other_j * value.view(-1, 1) if value is not None else other_j
     return scatter(other_j, index, 0, dim_size=dim_size, reduce=reduce)
 
 
 def _spmm(
@@ -1856,32 +1948,48 @@
     elif out.layout == torch.sparse_coo:  # pragma: no cover
         out = out.coalesce()
         edge_index = out.indices()
 
     else:
         raise NotImplementedError
 
-    edge_index = edge_index.as_subclass(EdgeIndex)
+    edge_index = EdgeIndex(edge_index)
     edge_index._sort_order = SortOrder.ROW
     edge_index._sparse_size = (out.size(0), out.size(1))
     edge_index._indptr = rowptr
 
     return edge_index, out.values()
 
 
-@implements(torch.mm)
-@implements(torch.matmul)
-@implements(Tensor.matmul)
-def _matmul1(
+@implements(aten.mm.default)
+def _mm(
     input: EdgeIndex,
     other: Union[Tensor, EdgeIndex],
 ) -> Union[Tensor, Tuple[EdgeIndex, Tensor]]:
     return matmul(input, other)
 
 
-@implements(torch.sparse.mm)
-def _matmul2(
+@implements(aten._sparse_addmm.default)
+def _addmm(
+    input: Tensor,
     mat1: EdgeIndex,
-    mat2: Union[Tensor, EdgeIndex],
-    reduce: ReduceType = 'sum',
-) -> Union[Tensor, Tuple[EdgeIndex, Tensor]]:
-    return matmul(mat1, mat2, reduce=reduce)
+    mat2: Tensor,
+    beta: float = 1.0,
+    alpha: float = 1.0,
+) -> Tensor:
+    assert input.abs().sum() == 0.0
+    out = matmul(mat1, mat2)
+    assert isinstance(out, Tensor)
+    return alpha * out if alpha != 1.0 else out
+
+
+if hasattr(aten, '_sparse_mm_reduce_impl'):
+
+    @implements(aten._sparse_mm_reduce_impl.default)
+    def _mm_reduce(
+        mat1: EdgeIndex,
+        mat2: Tensor,
+        reduce: ReduceType = 'sum',
+    ) -> Tuple[Tensor, Tensor]:
+        out = matmul(mat1, mat2, reduce=reduce)
+        assert isinstance(out, Tensor)
+        return out, out  # We return a dummy tensor for `argout` for now.
```

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/experimental.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/experimental.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/algorithm/attention_explainer.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/algorithm/attention_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/algorithm/base.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/algorithm/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/algorithm/captum.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/algorithm/captum.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/algorithm/captum_explainer.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/algorithm/captum_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/algorithm/dummy_explainer.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/algorithm/dummy_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/algorithm/gnn_explainer.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/algorithm/gnn_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/algorithm/graphmask_explainer.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/algorithm/graphmask_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/algorithm/pg_explainer.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/algorithm/pg_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/algorithm/utils.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/algorithm/utils.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/config.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/config.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/explainer.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/explanation.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/explanation.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/metric/basic.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/metric/basic.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/metric/faithfulness.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/metric/faithfulness.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/explain/metric/fidelity.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/explain/metric/fidelity.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/__init__.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/checkpoint.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/checkpoint.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/cmd_args.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/cmd_args.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/config.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/config.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/contrib/layer/generalconv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/contrib/layer/generalconv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/init.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/init.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/loader.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/logger.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/logger.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/loss.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/loss.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/model_builder.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/model_builder.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/models/__init__.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/models/act.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/models/act.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/models/encoder.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/models/encoder.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/models/gnn.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/models/gnn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/models/head.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/models/head.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/models/layer.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/models/layer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/models/transform.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/models/transform.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/optim.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/optim.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/register.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/register.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/train.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/train.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/utils/__init__.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/utils/agg_runs.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/utils/agg_runs.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/utils/comp_budget.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/utils/comp_budget.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/utils/device.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/utils/device.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/utils/epoch.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/utils/epoch.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/utils/io.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/utils/io.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/graphgym/utils/plot.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/graphgym/utils/plot.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/home.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/home.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/inspector.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/inspector.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/io/__init__.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/io/fs.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/io/fs.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/io/npz.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/io/npz.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/io/obj.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/io/obj.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/io/off.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/io/off.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/io/planetoid.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/io/planetoid.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/io/sdf.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/io/sdf.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/io/tu.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/io/tu.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     node_label = torch.empty((batch.size(0), 0))
     if 'node_labels' in names:
         node_label = read_file(folder, prefix, 'node_labels', torch.long)
         if node_label.dim() == 1:
             node_label = node_label.unsqueeze(-1)
         node_label = node_label - node_label.min(dim=0)[0]
-        node_labels = node_label.unbind(dim=-1)
+        node_labels = list(node_label.unbind(dim=-1))
         node_labels = [one_hot(x) for x in node_labels]
         if len(node_labels) == 1:
             node_label = node_labels[0]
         else:
             node_label = torch.cat(node_labels, dim=-1)
 
     edge_attribute = torch.empty((edge_index.size(1), 0))
@@ -52,15 +52,15 @@
 
     edge_label = torch.empty((edge_index.size(1), 0))
     if 'edge_labels' in names:
         edge_label = read_file(folder, prefix, 'edge_labels', torch.long)
         if edge_label.dim() == 1:
             edge_label = edge_label.unsqueeze(-1)
         edge_label = edge_label - edge_label.min(dim=0)[0]
-        edge_labels = edge_label.unbind(dim=-1)
+        edge_labels = list(edge_label.unbind(dim=-1))
         edge_labels = [one_hot(e) for e in edge_labels]
         if len(edge_labels) == 1:
             edge_label = edge_labels[0]
         else:
             edge_label = torch.cat(edge_labels, dim=-1)
 
     x = cat([node_attribute, node_label])
```

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/io/txt_array.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/io/txt_array.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/isinstance.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/isinstance.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/lazy_loader.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/__init__.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/base.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/cache.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/cache.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/cluster.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/cluster.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/data_list_loader.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/data_list_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/dataloader.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/dataloader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/dense_data_loader.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/dense_data_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/dynamic_batch_sampler.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/dynamic_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/graph_saint.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/graph_saint.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/hgt_loader.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/hgt_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/ibmb_loader.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/ibmb_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/imbalanced_sampler.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/imbalanced_sampler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/link_loader.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/link_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/link_neighbor_loader.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/link_neighbor_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/mixin.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/mixin.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/neighbor_loader.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/neighbor_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/neighbor_sampler.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/neighbor_sampler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/node_loader.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/node_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/prefetch.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/prefetch.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/random_node_loader.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/random_node_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/shadow.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/shadow.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/temporal_dataloader.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/temporal_dataloader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/utils.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from typing import Any, Dict, Optional, Tuple, Union
 
 import numpy as np
 import torch
 from torch import Tensor
 
 import torch_geometric.typing
-from torch_geometric import EdgeIndex
 from torch_geometric.data import (
     Data,
     FeatureStore,
     GraphStore,
     HeteroData,
     TensorAttr,
     remote_backend_utils,
@@ -101,21 +100,23 @@
 
 def filter_edge_store_(store: EdgeStorage, out_store: EdgeStorage, row: Tensor,
                        col: Tensor, index: OptTensor, perm: OptTensor = None):
     # Filters a edge storage object to only hold the edges in `index`,
     # which represents the new graph as denoted by `(row, col)`:
     for key, value in store.items():
         if key == 'edge_index':
+            edge_index = torch.stack([row, col], dim=0).to(value.device)
             # TODO Integrate `EdgeIndex` into `custom_store`.
-            out_store.edge_index = EdgeIndex(
-                torch.stack([row, col], dim=0).to(value.device),
-                sparse_size=out_store.size(),
-                sort_order='col',
-                # TODO Support `is_undirected`.
-            )
+            # edge_index = EdgeIndex(
+            #     torch.stack([row, col], dim=0).to(value.device),
+            #     sparse_size=out_store.size(),
+            #     sort_order='col',
+            #     # TODO Support `is_undirected`.
+            # )
+            out_store.edge_index = edge_index
 
         elif key == 'adj_t':
             # NOTE: We expect `(row, col)` to be sorted by `col` (CSC layout).
             row = row.to(value.device())
             col = col.to(value.device())
             edge_attr = value.storage.value()
             if edge_attr is not None:
```

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/loader/zip_loader.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/loader/zip_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/logging.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/logging.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/metrics/link_pred.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/metrics/link_pred.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/__init__.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/__init__.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/attention.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/attention.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/base.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/basic.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/basic.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/deep_sets.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/deep_sets.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/equilibrium.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/equilibrium.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/fused.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/fused.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/gmt.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/gmt.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/gru.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/gru.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/lcm.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/lcm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/lstm.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/lstm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/mlp.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/mlp.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/multi.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/multi.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/quantile.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/quantile.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/scaler.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/scaler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/set2set.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/set2set.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/set_transformer.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/set_transformer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/sort.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/sort.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/utils.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/utils.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/aggr/variance_preserving.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/aggr/variance_preserving.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/attention/performer.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/attention/performer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/__init__.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/agnn_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/agnn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/antisymmetric_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/antisymmetric_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/appnp.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/appnp.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/arma_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/arma_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/cg_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/cg_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/cheb_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/cheb_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/cluster_gcn_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/cluster_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/collect.jinja` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/collect.jinja`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/cugraph/base.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/cugraph/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/cugraph/gat_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/cugraph/gat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/cugraph/rgcn_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/cugraph/rgcn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/cugraph/sage_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/cugraph/sage_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/dir_gnn_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/dir_gnn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/dna_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/dna_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/edge_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/edge_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/edge_updater.jinja` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/edge_updater.jinja`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/eg_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/eg_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/fa_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/fa_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/feast_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/feast_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/film_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/film_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/fused_gat_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/fused_gat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/gat_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/gat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/gated_graph_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/gated_graph_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/gatv2_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/gatv2_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/gcn2_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/gcn2_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/gcn_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/gcn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/gen_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/gen_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/general_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/general_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/gin_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/gin_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/gmm_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/gmm_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/gps_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/gps_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/graph_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/graph_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/gravnet_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/gravnet_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/han_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/han_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/heat_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/heat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/hetero_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/hetero_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/hgt_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/hgt_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/hypergraph_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/hypergraph_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/le_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/le_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/lg_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/lg_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/message_passing.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/message_passing.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/mf_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/mf_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/mixhop_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/mixhop_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/nn_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/nn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/pan_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/pan_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/pdn_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/pdn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/pna_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/pna_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/point_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/point_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/point_gnn_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/point_gnn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/point_transformer_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/point_transformer_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/ppf_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/ppf_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/propagate.jinja` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/propagate.jinja`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/res_gated_graph_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/res_gated_graph_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/rgat_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/rgat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/rgcn_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/rgcn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/sage_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/sage_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/sg_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/sg_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/signed_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/signed_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/simple_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/simple_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/spline_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/spline_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/ssg_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/ssg_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/supergat_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/supergat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/tag_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/tag_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/transformer_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/transformer_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/utils/__init__.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/utils/cheatsheet.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/utils/cheatsheet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/wl_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/wl_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/wl_conv_continuous.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/wl_conv_continuous.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/conv/x_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/conv/x_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/data_parallel.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/data_parallel.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/dense/__init__.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/dense/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/dense/dense_gat_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/dense/dense_gat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/dense/dense_gcn_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/dense/dense_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/dense/dense_gin_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/dense/dense_gin_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/dense/dense_graph_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/dense/dense_graph_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/dense/dense_sage_conv.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/dense/dense_sage_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/dense/diff_pool.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/dense/diff_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/dense/dmon_pool.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/dense/dmon_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/dense/linear.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/dense/linear.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/dense/mincut_pool.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/dense/mincut_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/encoding.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/encoding.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/functional/bro.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/functional/bro.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/functional/gini.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/functional/gini.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/fx.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/fx.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/glob.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/glob.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/inits.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/inits.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/kge/base.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/kge/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/kge/complex.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/kge/complex.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/kge/distmult.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/kge/distmult.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/kge/loader.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/kge/loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/kge/rotate.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/kge/rotate.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/kge/transe.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/kge/transe.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/lr_scheduler.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/model_hub.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/model_hub.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/__init__.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/attentive_fp.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/attentive_fp.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/autoencoder.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/autoencoder.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/basic_gnn.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/basic_gnn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/captum.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/captum.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/correct_and_smooth.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/correct_and_smooth.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/deep_graph_infomax.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/deep_graph_infomax.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/deepgcn.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/deepgcn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/dimenet.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/dimenet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/dimenet_utils.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/dimenet_utils.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/gnnff.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/gnnff.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/graph_mixer.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/graph_mixer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/graph_unet.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/graph_unet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/jumping_knowledge.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/jumping_knowledge.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/label_prop.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/label_prop.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/lightgcn.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/lightgcn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/linkx.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/linkx.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/mask_label.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/mask_label.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/meta.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/meta.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/metapath2vec.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/metapath2vec.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/mlp.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/mlp.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/neural_fingerprint.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/neural_fingerprint.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/node2vec.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/node2vec.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/pmlp.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/pmlp.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/re_net.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/re_net.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/rect.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/rect.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/rev_gnn.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/rev_gnn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/schnet.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/schnet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/signed_gcn.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/signed_gcn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/tgn.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/tgn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/models/visnet.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/models/visnet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/module_dict.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/module_dict.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/norm/__init__.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/norm/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/norm/batch_norm.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/norm/batch_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/norm/diff_group_norm.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/norm/diff_group_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/norm/graph_norm.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/norm/graph_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/norm/graph_size_norm.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/norm/graph_size_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/norm/instance_norm.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/norm/instance_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/norm/layer_norm.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/norm/layer_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/norm/mean_subtraction_norm.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/norm/mean_subtraction_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/norm/msg_norm.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/norm/msg_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/norm/pair_norm.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/norm/pair_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/parameter_dict.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/parameter_dict.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/__init__.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/approx_knn.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/approx_knn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/asap.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/asap.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/avg_pool.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/avg_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/connect/base.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/connect/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/connect/filter_edges.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/connect/filter_edges.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/decimation.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/decimation.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/edge_pool.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/edge_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/glob.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/glob.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/graclus.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/graclus.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/knn.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/knn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/max_pool.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/max_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/mem_pool.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/mem_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/pan_pool.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/pan_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/pool.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/sag_pool.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/sag_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/select/base.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/select/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/select/topk.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/select/topk.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/topk_pool.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/topk_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/pool/voxel_grid.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/pool/voxel_grid.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/resolver.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/resolver.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/sequential.jinja` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/sequential.jinja`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/sequential.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/sequential.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/summary.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/summary.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/to_fixed_size_transformer.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/to_fixed_size_transformer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/to_hetero_module.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/to_hetero_module.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/to_hetero_transformer.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/to_hetero_transformer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/to_hetero_with_bases_transformer.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/to_hetero_with_bases_transformer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/nn/unpool/knn_interpolate.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/nn/unpool/knn_interpolate.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/profile/__init__.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/profile/benchmark.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/profile/benchmark.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/profile/profile.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/profile/profile.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/profile/profiler.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/profile/profiler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/profile/utils.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/profile/utils.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/resolver.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/resolver.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/sampler/__init__.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/sampler/base.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/sampler/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/sampler/hgt_sampler.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/sampler/hgt_sampler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/sampler/neighbor_sampler.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/sampler/neighbor_sampler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/sampler/utils.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/sampler/utils.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/template.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/template.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/testing/__init__.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/testing/asserts.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/testing/asserts.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/testing/data.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/testing/data.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/testing/decorators.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/testing/decorators.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/testing/distributed.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/testing/distributed.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/testing/feature_store.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/testing/feature_store.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/testing/graph_store.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/testing/graph_store.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/__init__.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/add_metapaths.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/add_metapaths.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
                     edge_weight = None
 
                 if self.max_sample is not None:
                     edge_index, edge_weight = self._sample(
                         edge_index, edge_weight)
 
             new_edge_type = (metapath[0][0], f'metapath_{j}', metapath[-1][-1])
-            data[new_edge_type].edge_index = edge_index
+            data[new_edge_type].edge_index = edge_index.as_tensor()
             if self.weighted:
                 data[new_edge_type].edge_weight = edge_weight
             data.metapath_dict[new_edge_type] = metapath
 
         postprocess(data, edge_types, self.drop_orig_edge_types,
                     self.keep_same_node_type, self.drop_unconnected_node_types)
```

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/add_positional_encoding.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/add_positional_encoding.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/add_remaining_self_loops.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/add_remaining_self_loops.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/add_self_loops.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/add_self_loops.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/base_transform.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/base_transform.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/cartesian.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/cartesian.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/center.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/center.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/compose.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/compose.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/constant.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/constant.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/delaunay.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/delaunay.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/distance.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/distance.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/face_to_edge.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/face_to_edge.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/feature_propagation.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/feature_propagation.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/fixed_points.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/fixed_points.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/gcn_norm.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/gcn_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/gdc.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/gdc.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/generate_mesh_normals.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/generate_mesh_normals.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/grid_sampling.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/grid_sampling.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/half_hop.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/half_hop.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/knn_graph.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/knn_graph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/laplacian_lambda_max.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/laplacian_lambda_max.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/largest_connected_components.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/largest_connected_components.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/line_graph.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/line_graph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/linear_transformation.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/linear_transformation.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/local_cartesian.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/local_cartesian.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/local_degree_profile.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/local_degree_profile.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/mask.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/mask.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/node_property_split.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/node_property_split.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/normalize_features.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/normalize_features.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/normalize_rotation.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/normalize_rotation.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/normalize_scale.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/normalize_scale.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/one_hot_degree.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/one_hot_degree.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/pad.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/pad.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/point_pair_features.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/point_pair_features.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/polar.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/polar.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/radius_graph.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/radius_graph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/random_flip.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/random_flip.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/random_jitter.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/random_jitter.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/random_link_split.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/random_link_split.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/random_node_split.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/random_node_split.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/random_rotate.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/random_rotate.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/random_scale.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/random_scale.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/random_shear.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/random_shear.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/remove_duplicated_edges.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/remove_duplicated_edges.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/remove_isolated_nodes.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/remove_isolated_nodes.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/remove_training_classes.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/remove_training_classes.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/rooted_subgraph.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/rooted_subgraph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/sample_points.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/sample_points.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/sign.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/sign.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/spherical.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/spherical.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/svd_feature_reduction.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/svd_feature_reduction.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/target_indegree.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/target_indegree.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/to_dense.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/to_dense.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/to_device.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/to_device.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/to_sparse_tensor.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/to_sparse_tensor.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/to_superpixels.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/to_superpixels.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/to_undirected.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/to_undirected.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/two_hop.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/two_hop.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def forward(self, data: Data) -> Data:
         assert data.edge_index is not None
         edge_index, edge_attr = data.edge_index, data.edge_attr
         N = data.num_nodes
 
         edge_index = EdgeIndex(edge_index, sparse_size=(N, N))
         edge_index = edge_index.sort_by('row')[0]
-        edge_index2, _ = edge_index @ edge_index
+        edge_index2 = edge_index.matmul(edge_index)[0].as_tensor()
         edge_index2, _ = remove_self_loops(edge_index2)
         edge_index = torch.cat([edge_index, edge_index2], dim=1)
 
         if edge_attr is not None:
             # We treat newly added edge features as "zero-features":
             edge_attr2 = edge_attr.new_zeros(edge_index2.size(1),
                                              *edge_attr.size()[1:])
```

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/transforms/virtual_node.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/transforms/virtual_node.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/typing.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/typing.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/__init__.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_assortativity.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_assortativity.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_coalesce.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_coalesce.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_degree.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_degree.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_grid.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_grid.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_homophily.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_homophily.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_index_sort.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_index_sort.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_lexsort.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_lexsort.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_negative_sampling.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_negative_sampling.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_normalized_cut.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_normalized_cut.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_one_hot.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_one_hot.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_scatter.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_scatter.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_segment.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_segment.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_select.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_select.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_softmax.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_softmax.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_sort_edge_index.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_sort_edge_index.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_spmm.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_spmm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_subgraph.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_subgraph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_to_dense_adj.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_to_dense_adj.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_to_dense_batch.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_to_dense_batch.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_train_test_split_edges.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_train_test_split_edges.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_tree_decomposition.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_tree_decomposition.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_trim_to_layer.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_trim_to_layer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/_unbatch.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/_unbatch.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/augmentation.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/convert.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/convert.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/cross_entropy.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/dropout.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/dropout.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/embedding.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/embedding.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/functions.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/functions.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/geodesic.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/geodesic.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/hetero.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/hetero.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/isolated.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/isolated.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/laplacian.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/laplacian.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/loop.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/loop.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/map.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/map.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/mask.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/mask.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/mesh_laplacian.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/mesh_laplacian.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/mixin.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/mixin.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/nested.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/nested.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/noise_scheduler.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/noise_scheduler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/num_nodes.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/num_nodes.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/ppr.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/ppr.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/random.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/random.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/repeat.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/repeat.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/smiles.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/smiles.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/sparse.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/sparse.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/utils/undirected.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/utils/undirected.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/torch_geometric/visualization/graph.py` & `pyg_nightly-2.6.0.dev20240426/torch_geometric/visualization/graph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240425/PKG-INFO` & `pyg_nightly-2.6.0.dev20240426/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyg-nightly
-Version: 2.6.0.dev20240425
+Version: 2.6.0.dev20240426
 Summary: Graph Neural Network Library for PyTorch
 Keywords: deep-learning,pytorch,geometric-deep-learning,graph-neural-networks,graph-convolutional-networks
 Author-email: Matthias Fey <matthias@pyg.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -88,15 +88,15 @@
 [![Slack][slack-image]][slack-url]
 
 **[Documentation](https://pytorch-geometric.readthedocs.io)** | **[Paper](https://arxiv.org/abs/1903.02428)** | **[Colab Notebooks and Video Tutorials](https://pytorch-geometric.readthedocs.io/en/latest/get_started/colabs.html)** | **[External Resources](https://pytorch-geometric.readthedocs.io/en/latest/external/resources.html)** | **[OGB Examples](https://github.com/snap-stanford/ogb/tree/master/examples)**
 
 **PyG** *(PyTorch Geometric)* is a library built upon [PyTorch](https://pytorch.org/) to easily write and train Graph Neural Networks (GNNs) for a wide range of applications related to structured data.
 
 It consists of various methods for deep learning on graphs and other irregular structures, also known as *[geometric deep learning](http://geometricdeeplearning.com/)*, from a variety of published papers.
-In addition, it consists of easy-to-use mini-batch loaders for operating on many small and single giant graphs, [multi GPU-support](https://github.com/pyg-team/pytorch_geometric/tree/master/examples/multi_gpu), [`torch.compile`](https://pytorch-geometric.readthedocs.io/en/latest/advanced/compile.html) support, [`DataPipe`](https://github.com/pyg-team/pytorch_geometric/blob/master/examples/datapipe.py) support, a large number of common benchmark datasets (based on simple interfaces to create your own), the [GraphGym](https://pytorch-geometric.readthedocs.io/en/latest/advanced/graphgym.html) experiment manager, and helpful transforms, both for learning on arbitrary graphs as well as on 3D meshes or point clouds.
+In addition, it consists of easy-to-use mini-batch loaders for operating on many small and single giant graphs, [multi GPU-support](https://github.com/pyg-team/pytorch_geometric/tree/master/examples/multi_gpu), [`torch.compile`](https://pytorch-geometric.readthedocs.io/en/latest/advanced/compile.html) support, [`DataPipe`](https://github.com/pyg-team/pytorch_geometric/blob/master/examples/datapipe.py) support, a large number of common benchmark datasets (based on simple interfaces to create your own), and helpful transforms, both for learning on arbitrary graphs as well as on 3D meshes or point clouds.
 
 **[Click here to join our Slack community!][slack-url]**
 
 <p align="center">
   <a href="https://medium.com/stanford-cs224w"><img style="max-width: 941px" src="https://data.pyg.org/img/cs224w_tutorials.png" /></a>
 </p>
 
@@ -119,15 +119,14 @@
 - **Comprehensive and well-maintained GNN models**:
   Most of the state-of-the-art Graph Neural Network architectures have been implemented by library developers or authors of research papers and are ready to be applied.
 - **Great flexibility**:
   Existing PyG models can easily be extended for conducting your own research with GNNs.
   Making modifications to existing models or creating new architectures is simple, thanks to its easy-to-use message passing API, and a variety of operators and utility functions.
 - **Large-scale real-world GNN models**:
   We focus on the need of GNN applications in challenging real-world scenarios, and support learning on diverse types of graphs, including but not limited to: scalable GNNs for graphs with millions of nodes; dynamic GNNs for node predictions over time; heterogeneous GNNs with multiple node types and edge types.
-- **GraphGym integration**: GraphGym lets users easily reproduce GNN experiments, is able to launch and analyze thousands of different GNN configurations, and is customizable by registering new modules to a GNN learning pipeline.
 
 ## Quick Tour for New Users
 
 In this quick tour, we highlight the ease of creating and training a GNN model with only a few lines of code.
 
 ### Train your own GNN model
 
@@ -211,28 +210,14 @@
     def message(self, x_j: Tensor, x_i: Tensor) -> Tensor:
         # x_j: Source node features of shape [num_edges, in_channels]
         # x_i: Target node features of shape [num_edges, in_channels]
         edge_features = torch.cat([x_i, x_j - x_i], dim=-1)
         return self.mlp(edge_features)  # shape [num_edges, out_channels]
 ```
 
-### Manage experiments with GraphGym
-
-GraphGym allows you to manage and launch GNN experiments, using a highly modularized pipeline (see [here](https://pytorch-geometric.readthedocs.io/en/latest/advanced/graphgym.html) for the accompanying tutorial).
-
-```
-git clone https://github.com/pyg-team/pytorch_geometric.git
-cd pytorch_geometric/graphgym
-bash run_single.sh  # run a single GNN experiment (node/edge/graph-level)
-bash run_batch.sh   # run a batch of GNN experiments, using differnt GNN designs/datasets/tasks
-```
-
-Users are highly encouraged to check out the [documentation](https://pytorch-geometric.readthedocs.io/en/latest), which contains additional tutorials on the essential functionalities of PyG, including data handling, creation of datasets and a full list of implemented methods, transforms, and datasets.
-For a quick start, check out our [examples](https://github.com/pyg-team/pytorch_geometric/tree/master/examples) in `examples/`.
-
 ## Architecture Overview
 
 PyG provides a multi-layer framework that enables users to build Graph Neural Network solutions on both low and high levels.
 It comprises of the following components:
 
 - The PyG **engine** utilizes the powerful PyTorch deep learning framework with full [`torch.compile`](https://pytorch-geometric.readthedocs.io/en/latest/advanced/compile.html) and [TorchScript](https://pytorch-geometric.readthedocs.io/en/latest/advanced/jit.html) support, as well as additions of efficient CPU/CUDA libraries for operating on sparse data, *e.g.*, [`pyg-lib`](https://github.com/pyg-team/pyg-lib).
 - The PyG **storage** handles data processing, transformation and loading pipelines. It is capable of handling and processing large-scale graph datasets, and provides effective solutions for heterogeneous graphs. It further provides a variety of sampling solutions, which enable training of GNNs on large-scale graphs.
```

