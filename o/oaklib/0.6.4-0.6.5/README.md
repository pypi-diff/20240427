# Comparing `tmp/oaklib-0.6.4.tar.gz` & `tmp/oaklib-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oaklib-0.6.4.tar", max compression
+gzip compressed data, was "oaklib-0.6.5.tar", max compression
```

## Comparing `oaklib-0.6.4.tar` & `oaklib-0.6.5.tar`

### file list

```diff
@@ -1,316 +1,316 @@
--rw-r--r--   0        0        0    11357 2024-04-25 00:55:39.708864 oaklib-0.6.4/LICENSE
--rw-r--r--   0        0        0     7258 2024-04-25 00:55:39.708864 oaklib-0.6.4/README.md
--rw-r--r--   0        0        0     3500 2024-04-25 00:56:12.428821 oaklib-0.6.4/pyproject.toml
--rw-r--r--   0        0        0      272 2024-04-25 00:55:39.876864 oaklib-0.6.4/src/oaklib/__init__.py
--rw-r--r--   0        0        0   231404 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/cli.py
--rw-r--r--   0        0        0       64 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/conf/__init__.py
--rw-r--r--   0        0        0      372 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/conf/go-human-input-spec.yaml
--rw-r--r--   0        0        0      162 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/conf/go-pombase-input-spec.yaml
--rw-r--r--   0        0        0      109 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/conf/hpoa-g2p-input-spec.yaml
--rw-r--r--   0        0        0      106 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/conf/hpoa-input-spec.yaml
--rw-r--r--   0        0        0     1903 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml
--rw-r--r--   0        0        0     1011 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/conf/mondo-g2d-input-spec.yaml
--rw-r--r--   0        0        0      109 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/conf/mondo-gencc-input-spec.yaml
--rw-r--r--   0        0        0      529 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/conf/mondo-hpoa-g2d-input-spec.yaml
--rw-r--r--   0        0        0      118 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/conf/mondo-medgen-g2d-input-spec.yaml
--rw-r--r--   0        0        0     4730 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/conf/obograph-style.json
--rw-r--r--   0        0        0      256 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/conf/omo-to-skos.sssom.tsv
--rw-r--r--   0        0        0      131 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/conf/value-set-expander.conf.yaml
--rw-r--r--   0        0        0      149 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/constants.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/converters/__init__.py
--rw-r--r--   0        0        0     1461 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/converters/data_model_converter.py
--rw-r--r--   0        0        0     2547 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/converters/logical_definition_flattener.py
--rw-r--r--   0        0        0     2446 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/converters/obo_graph_to_cx_converter.py
--rw-r--r--   0        0        0    12105 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/converters/obo_graph_to_fhir_converter.py
--rw-r--r--   0        0        0     7719 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/converters/obo_graph_to_obo_format_converter.py
--rw-r--r--   0        0        0     6100 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py
--rw-r--r--   0        0        0       60 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/__init__.py
--rw-r--r--   0        0        0     4034 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/association.owl.ttl
--rw-r--r--   0        0        0    38339 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/association.py
--rw-r--r--   0        0        0    13058 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/association.yaml
--rw-r--r--   0        0        0     6165 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/class_enrichment.owl.ttl
--rw-r--r--   0        0        0    13288 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/class_enrichment.py
--rw-r--r--   0        0        0     3262 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/class_enrichment.yaml
--rw-r--r--   0        0        0    19083 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/cross_ontology_diff.owl.ttl
--rw-r--r--   0        0        0    24250 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/cross_ontology_diff.py
--rw-r--r--   0        0        0    10687 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/cross_ontology_diff.yaml
--rw-r--r--   0        0        0    29418 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/cx.py
--rw-r--r--   0        0        0     6314 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/cx.yaml
--rw-r--r--   0        0        0    15826 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/fhir.owl.ttl
--rw-r--r--   0        0        0    35746 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/fhir.py
--rw-r--r--   0        0        0     5064 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/fhir.yaml
--rw-r--r--   0        0        0    14566 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/input_specification.py
--rw-r--r--   0        0        0     3560 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/input_specification.yaml
--rw-r--r--   0        0        0    15776 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/item_list.py
--rw-r--r--   0        0        0     6339 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/item_list.yaml
--rw-r--r--   0        0        0     8984 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/lexical_index.owl.ttl
--rw-r--r--   0        0        0    17296 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/lexical_index.py
--rw-r--r--   0        0        0     6429 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/lexical_index.schema.json
--rw-r--r--   0        0        0     4016 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/lexical_index.yaml
--rw-r--r--   0        0        0    26474 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/mapping_cluster_datamodel.py
--rw-r--r--   0        0        0     7317 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/mapping_cluster_datamodel.yaml
--rw-r--r--   0        0        0   226115 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl
--rw-r--r--   0        0        0    30133 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/mapping_rules_datamodel.py
--rw-r--r--   0        0        0    12889 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/mapping_rules_datamodel.schema.json
--rw-r--r--   0        0        0     3634 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/mapping_rules_datamodel.yaml
--rw-r--r--   0        0        0    25354 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/obograph.owl.ttl
--rw-r--r--   0        0        0    51109 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/obograph.py
--rw-r--r--   0        0        0    22375 2024-04-25 00:55:39.880864 oaklib-0.6.4/src/oaklib/datamodels/obograph.schema.json
--rw-r--r--   0        0        0    19600 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/obograph.yaml
--rw-r--r--   0        0        0    59793 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/ontology_metadata.owl.ttl
--rw-r--r--   0        0        0   116914 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/ontology_metadata.py
--rw-r--r--   0        0        0    95288 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/ontology_metadata.schema.json
--rw-r--r--   0        0        0    31452 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/ontology_metadata.yaml
--rw-r--r--   0        0        0    14759 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/oxo.owl.ttl
--rw-r--r--   0        0        0    21914 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/oxo.py
--rw-r--r--   0        0        0     4392 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/oxo.yaml
--rw-r--r--   0        0        0     3348 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/search.py
--rw-r--r--   0        0        0    16948 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/search_datamodel.owl.ttl
--rw-r--r--   0        0        0    25157 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/search_datamodel.py
--rw-r--r--   0        0        0     6684 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/search_datamodel.yaml
--rw-r--r--   0        0        0      287 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/settings.py
--rw-r--r--   0        0        0    12826 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/similarity.owl.ttl
--rw-r--r--   0        0        0    22645 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/similarity.py
--rw-r--r--   0        0        0     5690 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/similarity.yaml
--rw-r--r--   0        0        0    31217 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl
--rw-r--r--   0        0        0    50743 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/summary_statistics_datamodel.py
--rw-r--r--   0        0        0    21176 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/summary_statistics_datamodel.schema.json
--rw-r--r--   0        0        0    16246 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/summary_statistics_datamodel.yaml
--rw-r--r--   0        0        0    23481 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/synonymizer_datamodel.py
--rw-r--r--   0        0        0     2476 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/synonymizer_datamodel.yaml
--rw-r--r--   0        0        0     9909 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/taxon_constraints.owl.ttl
--rw-r--r--   0        0        0    18432 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/taxon_constraints.py
--rw-r--r--   0        0        0     5880 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/taxon_constraints.yaml
--rw-r--r--   0        0        0    11599 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/text_annotator.owl.ttl
--rw-r--r--   0        0        0    21645 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/text_annotator.py
--rw-r--r--   0        0        0     2464 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/text_annotator.schema.json
--rw-r--r--   0        0        0     4996 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/text_annotator.yaml
--rw-r--r--   0        0        0    13670 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/validation_datamodel.owl.ttl
--rw-r--r--   0        0        0    33912 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/validation_datamodel.py
--rw-r--r--   0        0        0    10783 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/validation_datamodel.schema.json
--rw-r--r--   0        0        0     9005 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/validation_datamodel.yaml
--rw-r--r--   0        0        0     6640 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/value_set_configuration.owl.ttl
--rw-r--r--   0        0        0     8458 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/value_set_configuration.py
--rw-r--r--   0        0        0     2276 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/value_set_configuration.yaml
--rw-r--r--   0        0        0     6595 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/datamodels/vocabulary.py
--rw-r--r--   0        0        0     6452 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/implementations/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/implementations/aggregator/__init__.py
--rw-r--r--   0        0        0     6377 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/implementations/aggregator/aggregator_implementation.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/implementations/agrkb/__init__.py
--rw-r--r--   0        0        0     8848 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/implementations/agrkb/agrkb_implementation.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/implementations/amigo/__init__.py
--rw-r--r--   0        0        0    16195 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/implementations/amigo/amigo_implementation.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/implementations/cx/__init__.py
--rw-r--r--   0        0        0     1985 2024-04-25 00:55:39.884863 oaklib-0.6.4/src/oaklib/implementations/cx/cx_implementation.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/eutils/__init__.py
--rw-r--r--   0        0        0     2180 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/eutils/eutils_implementation.py
--rw-r--r--   0        0        0     1055 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/eutils/pubmed_implementation.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/fhir/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/funowl/__init__.py
--rw-r--r--   0        0        0     8473 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/funowl/funowl_implementation.py
--rw-r--r--   0        0        0     3565 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/gilda.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/kgx/__init__.py
--rw-r--r--   0        0        0    30523 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/kgx/kgx_implementation.py
--rw-r--r--   0        0        0    28777 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/llm_implementation.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/monarch/__init__.py
--rw-r--r--   0        0        0     7034 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/monarch/monarch_implementation.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/ncbi/__init__.py
--rw-r--r--   0        0        0     7034 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/ncbi/ncbi_gene_implementation.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/neo4j/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/obograph/__init__.py
--rw-r--r--   0        0        0    17122 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/obograph/obograph_implementation.py
--rw-r--r--   0        0        0      267 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/ols/__init__.py
--rw-r--r--   0        0        0      132 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/ols/constants.py
--rw-r--r--   0        0        0     8071 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/ols/ols_implementation.py
--rw-r--r--   0        0        0      686 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/ols/oxo_utils.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/ontobee/__init__.py
--rw-r--r--   0        0        0     2641 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/ontobee/ontobee_implementation.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/ontoportal/__init__.py
--rw-r--r--   0        0        0      382 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/ontoportal/agroportal_implementation.py
--rw-r--r--   0        0        0     1250 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/ontoportal/bioportal_implementation.py
--rw-r--r--   0        0        0      378 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/ontoportal/ecoportal_implementation.py
--rw-r--r--   0        0        0      378 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/ontoportal/matportal_implementation.py
--rw-r--r--   0        0        0    13670 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/owlery/__init__.py
--rw-r--r--   0        0        0      427 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/owlery/owlery_implementation.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/pantherdb/__init__.py
--rw-r--r--   0        0        0    12625 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/pantherdb/pantherdb_implementation.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/pronto/__init__.py
--rw-r--r--   0        0        0    37863 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/pronto/pronto_implementation.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/robot/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/scigraph/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/semsimian/__init__.py
--rw-r--r--   0        0        0      247 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/semsimian/profiler.py
--rw-r--r--   0        0        0    11605 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/semsimian/semsimian_implementation.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/simpleobo/__init__.py
--rw-r--r--   0        0        0    46328 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/simpleobo/simple_obo_implementation.py
--rw-r--r--   0        0        0    23081 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/simpleobo/simple_obo_parser.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/skos/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/solor/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/solr/__init__.py
--rw-r--r--   0        0        0       96 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/sparql/__init__.py
--rw-r--r--   0        0        0    38067 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/sparql/abstract_sparql_implementation.py
--rw-r--r--   0        0        0      885 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/sparql/lov_implementation.py
--rw-r--r--   0        0        0     1721 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/sparql/oak_metamodel_implementation.py
--rw-r--r--   0        0        0     2658 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/sparql/sparql_implementation.py
--rw-r--r--   0        0        0     2325 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/sparql/sparql_query.py
--rw-r--r--   0        0        0       96 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/sqldb/__init__.py
--rw-r--r--   0        0        0   115796 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/sqldb/sql_implementation.py
--rw-r--r--   0        0        0     1903 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/sqldb/sqlite_utils.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/tabular/__init__.py
--rw-r--r--   0        0        0    19432 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/tabular/robot_template_implementation.py
--rw-r--r--   0        0        0     3279 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/tabular/tabular_implementation.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.888863 oaklib-0.6.4/src/oaklib/implementations/tccm/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/implementations/translator/__init__.py
--rw-r--r--   0        0        0     5442 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/implementations/translator/translator_implementation.py
--rw-r--r--   0        0        0      108 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/implementations/ubergraph/__init__.py
--rw-r--r--   0        0        0    20090 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/implementations/ubergraph/ubergraph_implementation.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/implementations/umls/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/implementations/uniprot/__init__.py
--rw-r--r--   0        0        0    14740 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/implementations/uniprot/uniprot_implementation.py
--rw-r--r--   0        0        0       96 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/implementations/wikidata/__init__.py
--rw-r--r--   0        0        0    17267 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/implementations/wikidata/wikidata_implementation.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/indexes/__init__.py
--rw-r--r--   0        0        0     3089 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/indexes/edge_index.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/inference/__init__.py
--rw-r--r--   0        0        0      748 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/inference/owl_reasoner.py
--rw-r--r--   0        0        0      105 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/inference/reasoner.py
--rw-r--r--   0        0        0     6960 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/inference/relation_graph_reasoner.py
--rw-r--r--   0        0        0      913 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/__init__.py
--rw-r--r--   0        0        0    28686 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/association_provider_interface.py
--rw-r--r--   0        0        0    55465 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/basic_ontology_interface.py
--rw-r--r--   0        0        0     9243 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/class_enrichment_calculation_interface.py
--rw-r--r--   0        0        0    21219 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/differ_interface.py
--rw-r--r--   0        0        0     3222 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/dumper_interface.py
--rw-r--r--   0        0        0      788 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/embedding_provider_interface.py
--rw-r--r--   0        0        0    13680 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/mapping_provider_interface.py
--rw-r--r--   0        0        0     3262 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/merge_interface.py
--rw-r--r--   0        0        0     3103 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/metadata_interface.py
--rw-r--r--   0        0        0    24049 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/obograph_interface.py
--rw-r--r--   0        0        0     1003 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/obolegacy_interface.py
--rw-r--r--   0        0        0      786 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/ontology_generator_interface.py
--rw-r--r--   0        0        0      784 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/ontology_interface.py
--rw-r--r--   0        0        0    13645 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/owl_interface.py
--rw-r--r--   0        0        0     8606 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/patcher_interface.py
--rw-r--r--   0        0        0     1955 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/rdf_interface.py
--rw-r--r--   0        0        0     2287 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/relation_graph_interface.py
--rw-r--r--   0        0        0     3759 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/search_interface.py
--rw-r--r--   0        0        0    16173 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/semsim_interface.py
--rw-r--r--   0        0        0     1063 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/skos_interface.py
--rw-r--r--   0        0        0     2113 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/subsetter_interface.py
--rw-r--r--   0        0        0    10140 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/summary_statistics_interface.py
--rw-r--r--   0        0        0    18295 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/taxon_constraint_interface.py
--rw-r--r--   0        0        0    10076 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/text_annotator_interface.py
--rw-r--r--   0        0        0    12915 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/interfaces/validator_interface.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/__init__.py
--rw-r--r--   0        0        0     2091 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/heatmap_writer.py
--rw-r--r--   0        0        0     1698 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/html_writer.py
--rw-r--r--   0        0        0     1565 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/obograph_writer.py
--rw-r--r--   0        0        0     3444 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/rollup_report_writer.py
--rw-r--r--   0        0        0      739 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_axiom_writer.py
--rw-r--r--   0        0        0     9012 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_csv_writer.py
--rw-r--r--   0        0        0     1284 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_fhir_writer.py
--rw-r--r--   0        0        0     2524 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_info_writer.py
--rw-r--r--   0        0        0      785 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_json_lines_writer.py
--rw-r--r--   0        0        0     1806 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_json_writer.py
--rw-r--r--   0        0        0      741 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_kgcl_writer.py
--rw-r--r--   0        0        0     2672 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_markdown_writer.py
--rw-r--r--   0        0        0     1152 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_nl_writer.py
--rw-r--r--   0        0        0     1117 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_obo_json_writer.py
--rw-r--r--   0        0        0     3485 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_obo_writer.py
--rw-r--r--   0        0        0     1270 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_owl_functional_writer.py
--rw-r--r--   0        0        0     2244 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_rdf_writer.py
--rw-r--r--   0        0        0     5126 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_writer.py
--rw-r--r--   0        0        0     1318 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/io/streaming_yaml_writer.py
--rw-r--r--   0        0        0      113 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/mappers/__init__.py
--rw-r--r--   0        0        0     3956 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/mappers/base_mapper.py
--rw-r--r--   0        0        0     1979 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/mappers/ontology_metadata_mapper.py
--rw-r--r--   0        0        0     2363 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/parsers/__init__.py
--rw-r--r--   0        0        0     1525 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/parsers/association_parser.py
--rw-r--r--   0        0        0      522 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/parsers/association_parser_factory.py
--rw-r--r--   0        0        0     4732 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/parsers/boomer_parser.py
--rw-r--r--   0        0        0     2148 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/parsers/gaf_association_parser.py
--rw-r--r--   0        0        0     2101 2024-04-25 00:55:39.892863 oaklib-0.6.4/src/oaklib/parsers/gencc_association_parser.py
--rw-r--r--   0        0        0     1131 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/parsers/hpoa_association_parser.py
--rw-r--r--   0        0        0     1673 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/parsers/hpoa_g2d_association_parser.py
--rw-r--r--   0        0        0      603 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/parsers/hpoa_g2p_association_parser.py
--rw-r--r--   0        0        0      654 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/parsers/kgx_association_parser.py
--rw-r--r--   0        0        0     1672 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/parsers/mim2gene_association_parser.py
--rw-r--r--   0        0        0      526 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/parsers/pairwise_association_parser.py
--rw-r--r--   0        0        0     1433 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/parsers/parser_base.py
--rw-r--r--   0        0        0      708 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/parsers/phaf_association_parser.py
--rw-r--r--   0        0        0     8681 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/parsers/xaf_association_parser.py
--rw-r--r--   0        0        0     2210 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/resource.py
--rw-r--r--   0        0        0    15958 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/selector.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/transformers/__init__.py
--rw-r--r--   0        0        0      589 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/transformers/chained_ontology_transformer.py
--rw-r--r--   0        0        0     2757 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/transformers/edge_filter_transformer.py
--rw-r--r--   0        0        0     1257 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/transformers/graph_transformer.py
--rw-r--r--   0        0        0     1804 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/transformers/node_filter_transformer.py
--rw-r--r--   0        0        0      470 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/transformers/ontology_transformer.py
--rw-r--r--   0        0        0     6353 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/transformers/sep_transformer.py
--rw-r--r--   0        0        0     1768 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/transformers/transformers_factory.py
--rw-r--r--   0        0        0      177 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/types.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/__init__.py
--rw-r--r--   0        0        0     1613 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/apikey_manager.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/associations/__init__.py
--rw-r--r--   0        0        0    13441 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/associations/association_differ.py
--rw-r--r--   0        0        0     3427 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/associations/association_index.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/axioms/__init__.py
--rw-r--r--   0        0        0     7694 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/axioms/disjointness_axiom_analyzer.py
--rw-r--r--   0        0        0     4093 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/axioms/logical_definition_analyzer.py
--rw-r--r--   0        0        0     8829 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/axioms/logical_definition_summarizer.py
--rw-r--r--   0        0        0     2436 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/axioms/logical_definition_utilities.py
--rw-r--r--   0        0        0     1540 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/basic_utils.py
--rw-r--r--   0        0        0     1356 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/format_utilities.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/graph/__init__.py
--rw-r--r--   0        0        0     2491 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/graph/networkx_bridge.py
--rw-r--r--   0        0        0     2857 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/graph/relationship_walker.py
--rw-r--r--   0        0        0      993 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/identifier_utils.py
--rw-r--r--   0        0        0      999 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/iterator_utils.py
--rw-r--r--   0        0        0     1015 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/keyval_cache.py
--rw-r--r--   0        0        0     3425 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/kgcl_utilities.py
--rw-r--r--   0        0        0      850 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/label_utilities.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/lexical/__init__.py
--rw-r--r--   0        0        0    19249 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/lexical/lexical_indexer.py
--rw-r--r--   0        0        0    10235 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/lexical/patternizer.py
--rw-r--r--   0        0        0     6881 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/lexical/synonymizer.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/mapping/__init__.py
--rw-r--r--   0        0        0    14422 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/mapping/boomer_utils.py
--rw-r--r--   0        0        0    15527 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/mapping/cross_ontology_diffs.py
--rw-r--r--   0        0        0      751 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/mapping/mapping_propagator.py
--rw-r--r--   0        0        0    10929 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/mapping/mapping_validation.py
--rw-r--r--   0        0        0     2558 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/mapping/sssom_utils.py
--rw-r--r--   0        0        0      690 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/ner_utilities.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/nlp/__init__.py
--rw-r--r--   0        0        0     3358 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/nlp/natual_language_generation.py
--rw-r--r--   0        0        0      136 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/oboformat_utils.py
--rw-r--r--   0        0        0    30409 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/obograph_utils.py
--rw-r--r--   0        0        0     2275 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/ontology_builder.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/publication_utils/__init__.py
--rw-r--r--   0        0        0     5283 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/publication_utils/doi_wrapper.py
--rw-r--r--   0        0        0      924 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/publication_utils/pubdb_wrapper.py
--rw-r--r--   0        0        0     6575 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/publication_utils/pubmed_wrapper.py
--rw-r--r--   0        0        0      380 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/rate_limiter.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/reasoning/__init__.py
--rw-r--r--   0        0        0      569 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/reasoning/relation_graph.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/semsim/__init__.py
--rw-r--r--   0        0        0     2545 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/semsim/similarity_utils.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/stats/__init__.py
--rw-r--r--   0        0        0     1511 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/stats/hypergeometric.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/subsets/__init__.py
--rw-r--r--   0        0        0     2819 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/subsets/slimmer_utils.py
--rw-r--r--   0        0        0     4701 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/subsets/subset_analysis.py
--rw-r--r--   0        0        0    12015 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/subsets/value_set_expander.py
--rw-r--r--   0        0        0    18045 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/table_filler.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/taxon/__init__.py
--rw-r--r--   0        0        0     1743 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/taxon/taxon_constraint_utils.py
--rw-r--r--   0        0        0        0 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/validation/__init__.py
--rw-r--r--   0        0        0    11118 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/validation/definition_ontology_rule.py
--rw-r--r--   0        0        0     7492 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/validation/disjointness_rule.py
--rw-r--r--   0        0        0     1729 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/validation/lint_utils.py
--rw-r--r--   0        0        0     1402 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/validation/ontology_rule.py
--rw-r--r--   0        0        0     1275 2024-04-25 00:55:39.896864 oaklib-0.6.4/src/oaklib/utilities/validation/rule_runner.py
--rw-r--r--   0        0        0      122 2024-04-25 00:55:39.900864 oaklib-0.6.4/src/oaklib/utilities/writers/__init__.py
--rw-r--r--   0        0        0    16522 2024-04-25 00:55:39.900864 oaklib-0.6.4/src/oaklib/utilities/writers/change_handler.py
--rw-r--r--   0        0        0     9171 1970-01-01 00:00:00.000000 oaklib-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-27 02:05:43.507818 oaklib-0.6.5/LICENSE
+-rw-r--r--   0        0        0     7258 2024-04-27 02:05:43.507818 oaklib-0.6.5/README.md
+-rw-r--r--   0        0        0     3522 2024-04-27 02:06:20.159785 oaklib-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0      272 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/__init__.py
+-rw-r--r--   0        0        0   231525 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/cli.py
+-rw-r--r--   0        0        0       64 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/conf/__init__.py
+-rw-r--r--   0        0        0      372 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/conf/go-human-input-spec.yaml
+-rw-r--r--   0        0        0      162 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/conf/go-pombase-input-spec.yaml
+-rw-r--r--   0        0        0      109 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/conf/hpoa-g2p-input-spec.yaml
+-rw-r--r--   0        0        0      106 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/conf/hpoa-input-spec.yaml
+-rw-r--r--   0        0        0     1903 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml
+-rw-r--r--   0        0        0     1011 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/conf/mondo-g2d-input-spec.yaml
+-rw-r--r--   0        0        0      109 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/conf/mondo-gencc-input-spec.yaml
+-rw-r--r--   0        0        0      529 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/conf/mondo-hpoa-g2d-input-spec.yaml
+-rw-r--r--   0        0        0      118 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/conf/mondo-medgen-g2d-input-spec.yaml
+-rw-r--r--   0        0        0     4730 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/conf/obograph-style.json
+-rw-r--r--   0        0        0      256 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/conf/omo-to-skos.sssom.tsv
+-rw-r--r--   0        0        0      131 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/conf/value-set-expander.conf.yaml
+-rw-r--r--   0        0        0      149 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/constants.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/converters/__init__.py
+-rw-r--r--   0        0        0     1461 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/converters/data_model_converter.py
+-rw-r--r--   0        0        0     2547 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/converters/logical_definition_flattener.py
+-rw-r--r--   0        0        0     2446 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/converters/obo_graph_to_cx_converter.py
+-rw-r--r--   0        0        0    12105 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/converters/obo_graph_to_fhir_converter.py
+-rw-r--r--   0        0        0     7719 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/converters/obo_graph_to_obo_format_converter.py
+-rw-r--r--   0        0        0     6100 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py
+-rw-r--r--   0        0        0       60 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/__init__.py
+-rw-r--r--   0        0        0     4034 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/association.owl.ttl
+-rw-r--r--   0        0        0    38339 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/association.py
+-rw-r--r--   0        0        0    13058 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/association.yaml
+-rw-r--r--   0        0        0     6165 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/class_enrichment.owl.ttl
+-rw-r--r--   0        0        0    13288 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/class_enrichment.py
+-rw-r--r--   0        0        0     3262 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/class_enrichment.yaml
+-rw-r--r--   0        0        0    19083 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/cross_ontology_diff.owl.ttl
+-rw-r--r--   0        0        0    24250 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/cross_ontology_diff.py
+-rw-r--r--   0        0        0    10687 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/cross_ontology_diff.yaml
+-rw-r--r--   0        0        0    29418 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/cx.py
+-rw-r--r--   0        0        0     6314 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/cx.yaml
+-rw-r--r--   0        0        0    15826 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/fhir.owl.ttl
+-rw-r--r--   0        0        0    35746 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/fhir.py
+-rw-r--r--   0        0        0     5064 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/fhir.yaml
+-rw-r--r--   0        0        0    14566 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/input_specification.py
+-rw-r--r--   0        0        0     3560 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/input_specification.yaml
+-rw-r--r--   0        0        0    15776 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/item_list.py
+-rw-r--r--   0        0        0     6339 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/item_list.yaml
+-rw-r--r--   0        0        0     8984 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/lexical_index.owl.ttl
+-rw-r--r--   0        0        0    17296 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/lexical_index.py
+-rw-r--r--   0        0        0     6429 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/lexical_index.schema.json
+-rw-r--r--   0        0        0     4016 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/lexical_index.yaml
+-rw-r--r--   0        0        0    26474 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/mapping_cluster_datamodel.py
+-rw-r--r--   0        0        0     7317 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/mapping_cluster_datamodel.yaml
+-rw-r--r--   0        0        0   226115 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl
+-rw-r--r--   0        0        0    33955 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/mapping_rules_datamodel.py
+-rw-r--r--   0        0        0    12889 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/mapping_rules_datamodel.schema.json
+-rw-r--r--   0        0        0     4155 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/mapping_rules_datamodel.yaml
+-rw-r--r--   0        0        0    25354 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/obograph.owl.ttl
+-rw-r--r--   0        0        0    51109 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/obograph.py
+-rw-r--r--   0        0        0    22375 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/obograph.schema.json
+-rw-r--r--   0        0        0    19600 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/obograph.yaml
+-rw-r--r--   0        0        0    59793 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/ontology_metadata.owl.ttl
+-rw-r--r--   0        0        0   116914 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/ontology_metadata.py
+-rw-r--r--   0        0        0    95288 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/ontology_metadata.schema.json
+-rw-r--r--   0        0        0    31452 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/ontology_metadata.yaml
+-rw-r--r--   0        0        0    14759 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/oxo.owl.ttl
+-rw-r--r--   0        0        0    21914 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/oxo.py
+-rw-r--r--   0        0        0     4392 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/oxo.yaml
+-rw-r--r--   0        0        0     3348 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/search.py
+-rw-r--r--   0        0        0    16948 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/search_datamodel.owl.ttl
+-rw-r--r--   0        0        0    25157 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/search_datamodel.py
+-rw-r--r--   0        0        0     6684 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/search_datamodel.yaml
+-rw-r--r--   0        0        0      287 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/settings.py
+-rw-r--r--   0        0        0    12826 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/similarity.owl.ttl
+-rw-r--r--   0        0        0    22645 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/similarity.py
+-rw-r--r--   0        0        0     5690 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/similarity.yaml
+-rw-r--r--   0        0        0    31217 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl
+-rw-r--r--   0        0        0    50743 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/summary_statistics_datamodel.py
+-rw-r--r--   0        0        0    21176 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/summary_statistics_datamodel.schema.json
+-rw-r--r--   0        0        0    16246 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/summary_statistics_datamodel.yaml
+-rw-r--r--   0        0        0    23481 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/synonymizer_datamodel.py
+-rw-r--r--   0        0        0     2476 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/synonymizer_datamodel.yaml
+-rw-r--r--   0        0        0     9909 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/taxon_constraints.owl.ttl
+-rw-r--r--   0        0        0    18432 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/taxon_constraints.py
+-rw-r--r--   0        0        0     5880 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/taxon_constraints.yaml
+-rw-r--r--   0        0        0    11599 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/text_annotator.owl.ttl
+-rw-r--r--   0        0        0    21645 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/text_annotator.py
+-rw-r--r--   0        0        0     2464 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/text_annotator.schema.json
+-rw-r--r--   0        0        0     4996 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/text_annotator.yaml
+-rw-r--r--   0        0        0    13670 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/datamodels/validation_datamodel.owl.ttl
+-rw-r--r--   0        0        0    33912 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/datamodels/validation_datamodel.py
+-rw-r--r--   0        0        0    10783 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/datamodels/validation_datamodel.schema.json
+-rw-r--r--   0        0        0     9005 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/datamodels/validation_datamodel.yaml
+-rw-r--r--   0        0        0     6640 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/datamodels/value_set_configuration.owl.ttl
+-rw-r--r--   0        0        0     8458 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/datamodels/value_set_configuration.py
+-rw-r--r--   0        0        0     2276 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/datamodels/value_set_configuration.yaml
+-rw-r--r--   0        0        0     6595 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/datamodels/vocabulary.py
+-rw-r--r--   0        0        0     6452 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/aggregator/__init__.py
+-rw-r--r--   0        0        0     6377 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/aggregator/aggregator_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/agrkb/__init__.py
+-rw-r--r--   0        0        0     8848 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/agrkb/agrkb_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/amigo/__init__.py
+-rw-r--r--   0        0        0    16195 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/amigo/amigo_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/cx/__init__.py
+-rw-r--r--   0        0        0     1985 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/cx/cx_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/eutils/__init__.py
+-rw-r--r--   0        0        0     2180 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/eutils/eutils_implementation.py
+-rw-r--r--   0        0        0     1055 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/eutils/pubmed_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/fhir/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/funowl/__init__.py
+-rw-r--r--   0        0        0     8473 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/funowl/funowl_implementation.py
+-rw-r--r--   0        0        0     3565 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/gilda.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/kgx/__init__.py
+-rw-r--r--   0        0        0    30523 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/kgx/kgx_implementation.py
+-rw-r--r--   0        0        0    28777 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/llm_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/monarch/__init__.py
+-rw-r--r--   0        0        0     7034 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/monarch/monarch_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/ncbi/__init__.py
+-rw-r--r--   0        0        0     7034 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/ncbi/ncbi_gene_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/neo4j/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/obograph/__init__.py
+-rw-r--r--   0        0        0    17122 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/obograph/obograph_implementation.py
+-rw-r--r--   0        0        0      267 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/ols/__init__.py
+-rw-r--r--   0        0        0      132 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/ols/constants.py
+-rw-r--r--   0        0        0     8071 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/ols/ols_implementation.py
+-rw-r--r--   0        0        0      686 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/ols/oxo_utils.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/ontobee/__init__.py
+-rw-r--r--   0        0        0     2641 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/ontobee/ontobee_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/ontoportal/__init__.py
+-rw-r--r--   0        0        0      382 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/ontoportal/agroportal_implementation.py
+-rw-r--r--   0        0        0     1250 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/ontoportal/bioportal_implementation.py
+-rw-r--r--   0        0        0      378 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/ontoportal/ecoportal_implementation.py
+-rw-r--r--   0        0        0      378 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/ontoportal/matportal_implementation.py
+-rw-r--r--   0        0        0    13670 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/owlery/__init__.py
+-rw-r--r--   0        0        0      427 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/owlery/owlery_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/pantherdb/__init__.py
+-rw-r--r--   0        0        0    12625 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/pantherdb/pantherdb_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/pronto/__init__.py
+-rw-r--r--   0        0        0    37863 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/pronto/pronto_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/robot/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/scigraph/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/semsimian/__init__.py
+-rw-r--r--   0        0        0      247 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/semsimian/profiler.py
+-rw-r--r--   0        0        0    11605 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/semsimian/semsimian_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/simpleobo/__init__.py
+-rw-r--r--   0        0        0    46328 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/simpleobo/simple_obo_implementation.py
+-rw-r--r--   0        0        0    23081 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/simpleobo/simple_obo_parser.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/skos/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/solor/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/solr/__init__.py
+-rw-r--r--   0        0        0       96 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/sparql/__init__.py
+-rw-r--r--   0        0        0    38067 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/sparql/abstract_sparql_implementation.py
+-rw-r--r--   0        0        0      885 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/sparql/lov_implementation.py
+-rw-r--r--   0        0        0     1721 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/sparql/oak_metamodel_implementation.py
+-rw-r--r--   0        0        0     2658 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/sparql/sparql_implementation.py
+-rw-r--r--   0        0        0     2325 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/sparql/sparql_query.py
+-rw-r--r--   0        0        0       96 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/sqldb/__init__.py
+-rw-r--r--   0        0        0   115796 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/sqldb/sql_implementation.py
+-rw-r--r--   0        0        0     1903 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/sqldb/sqlite_utils.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/tabular/__init__.py
+-rw-r--r--   0        0        0    19432 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/tabular/robot_template_implementation.py
+-rw-r--r--   0        0        0     3279 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/tabular/tabular_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/tccm/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/translator/__init__.py
+-rw-r--r--   0        0        0     5442 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/translator/translator_implementation.py
+-rw-r--r--   0        0        0      108 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/ubergraph/__init__.py
+-rw-r--r--   0        0        0    20090 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/ubergraph/ubergraph_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/umls/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/uniprot/__init__.py
+-rw-r--r--   0        0        0    14740 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/uniprot/uniprot_implementation.py
+-rw-r--r--   0        0        0       96 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/wikidata/__init__.py
+-rw-r--r--   0        0        0    17267 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/wikidata/wikidata_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/indexes/__init__.py
+-rw-r--r--   0        0        0     3089 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/indexes/edge_index.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/inference/__init__.py
+-rw-r--r--   0        0        0      748 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/inference/owl_reasoner.py
+-rw-r--r--   0        0        0      105 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/inference/reasoner.py
+-rw-r--r--   0        0        0     6960 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/inference/relation_graph_reasoner.py
+-rw-r--r--   0        0        0      913 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/__init__.py
+-rw-r--r--   0        0        0    28686 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/association_provider_interface.py
+-rw-r--r--   0        0        0    55465 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/basic_ontology_interface.py
+-rw-r--r--   0        0        0     9243 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/class_enrichment_calculation_interface.py
+-rw-r--r--   0        0        0    21219 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/differ_interface.py
+-rw-r--r--   0        0        0     3222 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/dumper_interface.py
+-rw-r--r--   0        0        0      788 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/embedding_provider_interface.py
+-rw-r--r--   0        0        0    13680 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/mapping_provider_interface.py
+-rw-r--r--   0        0        0     3262 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/merge_interface.py
+-rw-r--r--   0        0        0     3103 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/metadata_interface.py
+-rw-r--r--   0        0        0    24049 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/obograph_interface.py
+-rw-r--r--   0        0        0     1003 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/obolegacy_interface.py
+-rw-r--r--   0        0        0      786 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/ontology_generator_interface.py
+-rw-r--r--   0        0        0      784 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/ontology_interface.py
+-rw-r--r--   0        0        0    13645 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/owl_interface.py
+-rw-r--r--   0        0        0     8606 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/patcher_interface.py
+-rw-r--r--   0        0        0     1955 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/rdf_interface.py
+-rw-r--r--   0        0        0     2287 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/relation_graph_interface.py
+-rw-r--r--   0        0        0     3759 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/search_interface.py
+-rw-r--r--   0        0        0    16173 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/semsim_interface.py
+-rw-r--r--   0        0        0     1063 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/skos_interface.py
+-rw-r--r--   0        0        0     2113 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/subsetter_interface.py
+-rw-r--r--   0        0        0    10140 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/summary_statistics_interface.py
+-rw-r--r--   0        0        0    18295 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/taxon_constraint_interface.py
+-rw-r--r--   0        0        0    10076 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/text_annotator_interface.py
+-rw-r--r--   0        0        0    12915 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/validator_interface.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/io/__init__.py
+-rw-r--r--   0        0        0     2091 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/io/heatmap_writer.py
+-rw-r--r--   0        0        0     1698 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/io/html_writer.py
+-rw-r--r--   0        0        0     1565 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/io/obograph_writer.py
+-rw-r--r--   0        0        0     3444 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/io/rollup_report_writer.py
+-rw-r--r--   0        0        0      739 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/io/streaming_axiom_writer.py
+-rw-r--r--   0        0        0     9012 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/io/streaming_csv_writer.py
+-rw-r--r--   0        0        0     1284 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/io/streaming_fhir_writer.py
+-rw-r--r--   0        0        0     2524 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/io/streaming_info_writer.py
+-rw-r--r--   0        0        0      785 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/io/streaming_json_lines_writer.py
+-rw-r--r--   0        0        0     1806 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/io/streaming_json_writer.py
+-rw-r--r--   0        0        0      741 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/io/streaming_kgcl_writer.py
+-rw-r--r--   0        0        0     2672 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/io/streaming_markdown_writer.py
+-rw-r--r--   0        0        0     1152 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/io/streaming_nl_writer.py
+-rw-r--r--   0        0        0     1117 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/io/streaming_obo_json_writer.py
+-rw-r--r--   0        0        0     3485 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/io/streaming_obo_writer.py
+-rw-r--r--   0        0        0     1270 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/io/streaming_owl_functional_writer.py
+-rw-r--r--   0        0        0     2244 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/io/streaming_rdf_writer.py
+-rw-r--r--   0        0        0     5126 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/io/streaming_writer.py
+-rw-r--r--   0        0        0     1318 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/io/streaming_yaml_writer.py
+-rw-r--r--   0        0        0      113 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/mappers/__init__.py
+-rw-r--r--   0        0        0     3956 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/mappers/base_mapper.py
+-rw-r--r--   0        0        0     1979 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/mappers/ontology_metadata_mapper.py
+-rw-r--r--   0        0        0     2363 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/__init__.py
+-rw-r--r--   0        0        0     1525 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/association_parser.py
+-rw-r--r--   0        0        0      522 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/association_parser_factory.py
+-rw-r--r--   0        0        0     4732 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/boomer_parser.py
+-rw-r--r--   0        0        0     2148 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/gaf_association_parser.py
+-rw-r--r--   0        0        0     2101 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/gencc_association_parser.py
+-rw-r--r--   0        0        0     1131 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/hpoa_association_parser.py
+-rw-r--r--   0        0        0     1673 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/hpoa_g2d_association_parser.py
+-rw-r--r--   0        0        0      603 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/hpoa_g2p_association_parser.py
+-rw-r--r--   0        0        0      654 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/kgx_association_parser.py
+-rw-r--r--   0        0        0     1672 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/mim2gene_association_parser.py
+-rw-r--r--   0        0        0      526 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/pairwise_association_parser.py
+-rw-r--r--   0        0        0     1433 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/parser_base.py
+-rw-r--r--   0        0        0      708 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/phaf_association_parser.py
+-rw-r--r--   0        0        0     8681 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/xaf_association_parser.py
+-rw-r--r--   0        0        0     2210 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/resource.py
+-rw-r--r--   0        0        0    15958 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/selector.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/transformers/__init__.py
+-rw-r--r--   0        0        0      589 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/transformers/chained_ontology_transformer.py
+-rw-r--r--   0        0        0     2757 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/transformers/edge_filter_transformer.py
+-rw-r--r--   0        0        0     1257 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/transformers/graph_transformer.py
+-rw-r--r--   0        0        0     1804 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/transformers/node_filter_transformer.py
+-rw-r--r--   0        0        0      470 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/transformers/ontology_transformer.py
+-rw-r--r--   0        0        0     6353 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/transformers/sep_transformer.py
+-rw-r--r--   0        0        0     1768 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/transformers/transformers_factory.py
+-rw-r--r--   0        0        0      177 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/types.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/__init__.py
+-rw-r--r--   0        0        0     1613 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/apikey_manager.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/associations/__init__.py
+-rw-r--r--   0        0        0    13441 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/associations/association_differ.py
+-rw-r--r--   0        0        0     3427 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/associations/association_index.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/axioms/__init__.py
+-rw-r--r--   0        0        0     7694 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/axioms/disjointness_axiom_analyzer.py
+-rw-r--r--   0        0        0     4093 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/axioms/logical_definition_analyzer.py
+-rw-r--r--   0        0        0     8829 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/axioms/logical_definition_summarizer.py
+-rw-r--r--   0        0        0     2436 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/axioms/logical_definition_utilities.py
+-rw-r--r--   0        0        0     1540 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/basic_utils.py
+-rw-r--r--   0        0        0     1356 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/format_utilities.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/graph/__init__.py
+-rw-r--r--   0        0        0     2491 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/graph/networkx_bridge.py
+-rw-r--r--   0        0        0     2857 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/graph/relationship_walker.py
+-rw-r--r--   0        0        0      993 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/identifier_utils.py
+-rw-r--r--   0        0        0      999 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/iterator_utils.py
+-rw-r--r--   0        0        0     1015 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/keyval_cache.py
+-rw-r--r--   0        0        0     3425 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/kgcl_utilities.py
+-rw-r--r--   0        0        0      850 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/label_utilities.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/lexical/__init__.py
+-rw-r--r--   0        0        0    19249 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/lexical/lexical_indexer.py
+-rw-r--r--   0        0        0    10235 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/lexical/patternizer.py
+-rw-r--r--   0        0        0     6881 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/lexical/synonymizer.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/mapping/__init__.py
+-rw-r--r--   0        0        0    14422 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/mapping/boomer_utils.py
+-rw-r--r--   0        0        0    15527 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/mapping/cross_ontology_diffs.py
+-rw-r--r--   0        0        0      751 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/mapping/mapping_propagator.py
+-rw-r--r--   0        0        0    10929 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/mapping/mapping_validation.py
+-rw-r--r--   0        0        0     2558 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/mapping/sssom_utils.py
+-rw-r--r--   0        0        0      690 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/ner_utilities.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/nlp/__init__.py
+-rw-r--r--   0        0        0     3358 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/nlp/natual_language_generation.py
+-rw-r--r--   0        0        0      136 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/oboformat_utils.py
+-rw-r--r--   0        0        0    30409 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/obograph_utils.py
+-rw-r--r--   0        0        0     2275 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/ontology_builder.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/publication_utils/__init__.py
+-rw-r--r--   0        0        0     5283 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/publication_utils/doi_wrapper.py
+-rw-r--r--   0        0        0      924 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/publication_utils/pubdb_wrapper.py
+-rw-r--r--   0        0        0     6575 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/publication_utils/pubmed_wrapper.py
+-rw-r--r--   0        0        0      380 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/rate_limiter.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/reasoning/__init__.py
+-rw-r--r--   0        0        0      569 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/reasoning/relation_graph.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/semsim/__init__.py
+-rw-r--r--   0        0        0     2545 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/semsim/similarity_utils.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/stats/__init__.py
+-rw-r--r--   0        0        0     1511 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/stats/hypergeometric.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/subsets/__init__.py
+-rw-r--r--   0        0        0     2819 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/subsets/slimmer_utils.py
+-rw-r--r--   0        0        0     4701 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/subsets/subset_analysis.py
+-rw-r--r--   0        0        0    12015 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/subsets/value_set_expander.py
+-rw-r--r--   0        0        0    18045 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/table_filler.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/taxon/__init__.py
+-rw-r--r--   0        0        0     1743 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/taxon/taxon_constraint_utils.py
+-rw-r--r--   0        0        0        0 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/validation/__init__.py
+-rw-r--r--   0        0        0    11118 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/validation/definition_ontology_rule.py
+-rw-r--r--   0        0        0     7492 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/validation/disjointness_rule.py
+-rw-r--r--   0        0        0     1729 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/validation/lint_utils.py
+-rw-r--r--   0        0        0     1402 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/validation/ontology_rule.py
+-rw-r--r--   0        0        0     1275 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/validation/rule_runner.py
+-rw-r--r--   0        0        0      122 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/writers/__init__.py
+-rw-r--r--   0        0        0    16522 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/writers/change_handler.py
+-rw-r--r--   0        0        0     9214 1970-01-01 00:00:00.000000 oaklib-0.6.5/PKG-INFO
```

### Comparing `oaklib-0.6.4/LICENSE` & `oaklib-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/README.md` & `oaklib-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/pyproject.toml` & `oaklib-0.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oaklib"
-version = "v0.6.4"
+version = "v0.6.5"
 description = "Ontology Access Kit: Python library for common ontology operations over a variety of backends"
 authors = ["cmungall <cjm@berkeleybop.org>"]
 
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0.0"
@@ -39,14 +39,15 @@
 eutils = ">=0.6.0"
 requests-cache = "^1.0.1"
 click = "*"
 urllib3 = {version = "< 2", optional = true}
 pydantic = "*"
 jsonlines = "^4.0.0"
 tenacity = "^8.2.3"
+defusedxml = "^0.7.1"
 
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 Sphinx = ">=6.1.3"
 pandas = ">=1.5.1"
 jupyter = ">=1.0.0"
```

### Comparing `oaklib-0.6.4/src/oaklib/cli.py` & `oaklib-0.6.5/src/oaklib/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -4063,14 +4063,18 @@
 
        https://incatools.github.io/ontology-access-kit/interfaces/mapping-provider
 
     Data model:
 
        https://w3id.org/oak/mapping-provider
 
+    More examples:
+
+       https://github.com/INCATools/ontology-access-kit/blob/main/notebooks/Commands/Mappings.ipynb
+
     """
     impl = settings.impl
     writer = _get_writer(output_type, impl, StreamingYamlWriter, datamodel=sssom_schema)
     writer.output = output
     writer.autolabel = autolabel
     if not isinstance(impl, MappingProviderInterface):
         raise NotImplementedError(f"Cannot execute this using {impl} of type {type(impl)}")
```

### Comparing `oaklib-0.6.4/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml` & `oaklib-0.6.5/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/conf/mondo-g2d-input-spec.yaml` & `oaklib-0.6.5/src/oaklib/conf/mondo-g2d-input-spec.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/conf/mondo-hpoa-g2d-input-spec.yaml` & `oaklib-0.6.5/src/oaklib/conf/mondo-hpoa-g2d-input-spec.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/conf/obograph-style.json` & `oaklib-0.6.5/src/oaklib/conf/obograph-style.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/converters/data_model_converter.py` & `oaklib-0.6.5/src/oaklib/converters/data_model_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/converters/logical_definition_flattener.py` & `oaklib-0.6.5/src/oaklib/converters/logical_definition_flattener.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/converters/obo_graph_to_cx_converter.py` & `oaklib-0.6.5/src/oaklib/converters/obo_graph_to_cx_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/converters/obo_graph_to_fhir_converter.py` & `oaklib-0.6.5/src/oaklib/converters/obo_graph_to_fhir_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/converters/obo_graph_to_obo_format_converter.py` & `oaklib-0.6.5/src/oaklib/converters/obo_graph_to_obo_format_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py` & `oaklib-0.6.5/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/association.owl.ttl` & `oaklib-0.6.5/src/oaklib/datamodels/association.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/association.py` & `oaklib-0.6.5/src/oaklib/datamodels/association.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/association.yaml` & `oaklib-0.6.5/src/oaklib/datamodels/association.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/class_enrichment.owl.ttl` & `oaklib-0.6.5/src/oaklib/datamodels/class_enrichment.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/class_enrichment.py` & `oaklib-0.6.5/src/oaklib/datamodels/class_enrichment.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/class_enrichment.yaml` & `oaklib-0.6.5/src/oaklib/datamodels/class_enrichment.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/cross_ontology_diff.owl.ttl` & `oaklib-0.6.5/src/oaklib/datamodels/cross_ontology_diff.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/cross_ontology_diff.py` & `oaklib-0.6.5/src/oaklib/datamodels/cross_ontology_diff.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/cross_ontology_diff.yaml` & `oaklib-0.6.5/src/oaklib/datamodels/cross_ontology_diff.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/cx.py` & `oaklib-0.6.5/src/oaklib/datamodels/cx.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/cx.yaml` & `oaklib-0.6.5/src/oaklib/datamodels/cx.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/fhir.owl.ttl` & `oaklib-0.6.5/src/oaklib/datamodels/fhir.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/fhir.py` & `oaklib-0.6.5/src/oaklib/datamodels/fhir.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/fhir.yaml` & `oaklib-0.6.5/src/oaklib/datamodels/fhir.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/input_specification.py` & `oaklib-0.6.5/src/oaklib/datamodels/input_specification.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/input_specification.yaml` & `oaklib-0.6.5/src/oaklib/datamodels/input_specification.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/item_list.py` & `oaklib-0.6.5/src/oaklib/datamodels/item_list.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/item_list.yaml` & `oaklib-0.6.5/src/oaklib/datamodels/item_list.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/lexical_index.owl.ttl` & `oaklib-0.6.5/src/oaklib/datamodels/lexical_index.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/lexical_index.py` & `oaklib-0.6.5/src/oaklib/datamodels/lexical_index.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/lexical_index.schema.json` & `oaklib-0.6.5/src/oaklib/datamodels/lexical_index.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/lexical_index.yaml` & `oaklib-0.6.5/src/oaklib/datamodels/lexical_index.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/mapping_cluster_datamodel.py` & `oaklib-0.6.5/src/oaklib/datamodels/mapping_cluster_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/mapping_cluster_datamodel.yaml` & `oaklib-0.6.5/src/oaklib/datamodels/mapping_cluster_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl` & `oaklib-0.6.5/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/mapping_rules_datamodel.py` & `oaklib-0.6.5/src/oaklib/datamodels/mapping_rules_datamodel.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,63 @@
-# Auto generated from mapping_rules_datamodel.yaml by pythongen.py version: 0.9.0
-# Generation date: 2023-04-12T14:50:11
+# Auto generated from mapping_rules_datamodel.yaml by pythongen.py version: 0.0.1
+# Generation date: 2024-04-25T10:18:46
 # Schema: mapping-rules-datamodel
 #
 # id: https://w3id.org/oak/mapping-rules-datamodel
-# description: A datamodel for specifying lexical mapping rules.
+# description: A datamodel for specifying lexical mapping rules
 # license: https://creativecommons.org/publicdomain/zero/1.0/
 
 import dataclasses
+import re
+from jsonasobj2 import JsonObj, as_dict
+from typing import Optional, List, Union, Dict, ClassVar, Any
 from dataclasses import dataclass
-from typing import Any, ClassVar, Dict, List, Optional, Union
+from datetime import date, datetime
+from linkml_runtime.linkml_model.meta import EnumDefinition, PermissibleValue, PvFormulaOptions
 
-from jsonasobj2 import as_dict
-from linkml_runtime.linkml_model.meta import (
-    EnumDefinition,
-    PermissibleValue,
-)
-from linkml_runtime.utils.curienamespace import CurieNamespace
-from linkml_runtime.utils.dataclass_extensions_376 import (
-    dataclasses_init_fn_with_kwargs,
-)
-from linkml_runtime.utils.enumerations import EnumDefinitionImpl
-from linkml_runtime.utils.metamodelcore import (
-    Bool,
-    URIorCURIE,
-    empty_dict,
-    empty_list,
-)
 from linkml_runtime.utils.slot import Slot
-from linkml_runtime.utils.yamlutils import (
-    YAMLRoot,
-    extended_str,
-)
-from rdflib import URIRef
-
-from oaklib.datamodels.synonymizer_datamodel import Synonymizer, Test
+from linkml_runtime.utils.metamodelcore import empty_list, empty_dict, bnode
+from linkml_runtime.utils.yamlutils import YAMLRoot, extended_str, extended_float, extended_int
+from linkml_runtime.utils.dataclass_extensions_376 import dataclasses_init_fn_with_kwargs
+from linkml_runtime.utils.formatutils import camelcase, underscore, sfx
+from linkml_runtime.utils.enumerations import EnumDefinitionImpl
+from rdflib import Namespace, URIRef
+from linkml_runtime.utils.curienamespace import CurieNamespace
+from linkml_runtime.linkml_model.types import Boolean, Float, String, Uriorcurie
+from linkml_runtime.utils.metamodelcore import Bool, URIorCURIE
 
 metamodel_version = "1.7.0"
 version = None
 
 # Overwrite dataclasses _init_fn to add **kwargs in __init__
 dataclasses._init_fn = dataclasses_init_fn_with_kwargs
 
 # Namespaces
-LINKML = CurieNamespace("linkml", "https://w3id.org/linkml/")
-MAPPINGRULES = CurieNamespace("mappingrules", "https://w3id.org/oak/mapping-rules-datamodel/")
-ONTOLEXINDEX = CurieNamespace("ontolexindex", "https://w3id.org/oak/lexical-index/")
-OWL = CurieNamespace("owl", "http://www.w3.org/2002/07/owl#")
-PAV = CurieNamespace("pav", "http://purl.org/pav/")
-PROV = CurieNamespace("prov", "http://www.w3.org/ns/prov#")
-RDF = CurieNamespace("rdf", "http://www.w3.org/1999/02/22-rdf-syntax-ns#")
-RDFS = CurieNamespace("rdfs", "http://www.w3.org/2000/01/rdf-schema#")
-SCHEMA = CurieNamespace("schema", "http://schema.org/")
-SH = CurieNamespace("sh", "https://w3id.org/shacl/")
-SKOS = CurieNamespace("skos", "http://www.w3.org/2004/02/skos/core#")
-XSD = CurieNamespace("xsd", "http://www.w3.org/2001/XMLSchema#")
+LINKML = CurieNamespace('linkml', 'https://w3id.org/linkml/')
+MAPPINGRULES = CurieNamespace('mappingrules', 'https://w3id.org/oak/mapping-rules-datamodel/')
+ONTOLEXINDEX = CurieNamespace('ontolexindex', 'https://w3id.org/oak/lexical-index/')
+OWL = CurieNamespace('owl', 'http://www.w3.org/2002/07/owl#')
+PAV = CurieNamespace('pav', 'http://purl.org/pav/')
+PROV = CurieNamespace('prov', 'http://www.w3.org/ns/prov#')
+RDF = CurieNamespace('rdf', 'http://www.w3.org/1999/02/22-rdf-syntax-ns#')
+RDFS = CurieNamespace('rdfs', 'http://www.w3.org/2000/01/rdf-schema#')
+SCHEMA = CurieNamespace('schema', 'http://schema.org/')
+SH = CurieNamespace('sh', 'https://w3id.org/shacl/')
+SKOS = CurieNamespace('skos', 'http://www.w3.org/2004/02/skos/core#')
+SYNONYMIZER = CurieNamespace('synonymizer', 'https://w3id.org/oak/synonymizer-datamodel/')
+XSD = CurieNamespace('xsd', 'http://www.w3.org/2001/XMLSchema#')
 DEFAULT_ = MAPPINGRULES
 
 
 # Types
+class RegularExpressionString(String):
+    type_class_uri = XSD["string"]
+    type_class_curie = "xsd:string"
+    type_name = "RegularExpressionString"
+    type_model_uri = MAPPINGRULES.RegularExpressionString
 
 
 # Class references
 class LexicalGroupingTerm(extended_str):
     pass
 
 
@@ -70,49 +66,43 @@
 
 
 @dataclass
 class MappingRuleCollection(YAMLRoot):
     """
     A collection of mapping rules
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = MAPPINGRULES.MappingRuleCollection
+    class_class_uri: ClassVar[URIRef] = MAPPINGRULES["MappingRuleCollection"]
     class_class_curie: ClassVar[str] = "mappingrules:MappingRuleCollection"
     class_name: ClassVar[str] = "MappingRuleCollection"
     class_model_uri: ClassVar[URIRef] = MAPPINGRULES.MappingRuleCollection
 
-    rules: Optional[Union[Union[dict, "MappingRule"], List[Union[dict, "MappingRule"]]]] = (
-        empty_list()
-    )
+    rules: Optional[Union[Union[dict, "MappingRule"], List[Union[dict, "MappingRule"]]]] = empty_list()
     minimum_confidence: Optional[float] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if not isinstance(self.rules, list):
             self.rules = [self.rules] if self.rules is not None else []
-        self.rules = [
-            v if isinstance(v, MappingRule) else MappingRule(**as_dict(v)) for v in self.rules
-        ]
+        self.rules = [v if isinstance(v, MappingRule) else MappingRule(**as_dict(v)) for v in self.rules]
 
         if self.minimum_confidence is not None and not isinstance(self.minimum_confidence, float):
             self.minimum_confidence = float(self.minimum_confidence)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class MappingRule(YAMLRoot):
     """
     An individual mapping rule, if preconditions match the postconditions are applied
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = MAPPINGRULES.MappingRule
+    class_class_uri: ClassVar[URIRef] = MAPPINGRULES["MappingRule"]
     class_class_curie: ClassVar[str] = "mappingrules:MappingRule"
     class_name: ClassVar[str] = "MappingRule"
     class_model_uri: ClassVar[URIRef] = MAPPINGRULES.MappingRule
 
     description: Optional[str] = None
     oneway: Optional[Union[bool, Bool]] = False
     preconditions: Optional[Union[dict, "Precondition"]] = None
@@ -139,101 +129,66 @@
 
 
 @dataclass
 class Precondition(YAMLRoot):
     """
     A pattern to be matched against an individual SSSOM mapping
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = MAPPINGRULES.Precondition
+    class_class_uri: ClassVar[URIRef] = MAPPINGRULES["Precondition"]
     class_class_curie: ClassVar[str] = "mappingrules:Precondition"
     class_name: ClassVar[str] = "Precondition"
     class_model_uri: ClassVar[URIRef] = MAPPINGRULES.Precondition
 
     subject_source_one_of: Optional[Union[str, List[str]]] = empty_list()
     object_source_one_of: Optional[Union[str, List[str]]] = empty_list()
     mapping_source_one_of: Optional[Union[str, List[str]]] = empty_list()
     subject_match_field_one_of: Optional[Union[str, List[str]]] = empty_list()
     object_match_field_one_of: Optional[Union[str, List[str]]] = empty_list()
     transformations_included_in: Optional[Union[str, List[str]]] = empty_list()
     predicate_id_one_of: Optional[Union[str, List[str]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if not isinstance(self.subject_source_one_of, list):
-            self.subject_source_one_of = (
-                [self.subject_source_one_of] if self.subject_source_one_of is not None else []
-            )
-        self.subject_source_one_of = [
-            v if isinstance(v, str) else str(v) for v in self.subject_source_one_of
-        ]
+            self.subject_source_one_of = [self.subject_source_one_of] if self.subject_source_one_of is not None else []
+        self.subject_source_one_of = [v if isinstance(v, str) else str(v) for v in self.subject_source_one_of]
 
         if not isinstance(self.object_source_one_of, list):
-            self.object_source_one_of = (
-                [self.object_source_one_of] if self.object_source_one_of is not None else []
-            )
-        self.object_source_one_of = [
-            v if isinstance(v, str) else str(v) for v in self.object_source_one_of
-        ]
+            self.object_source_one_of = [self.object_source_one_of] if self.object_source_one_of is not None else []
+        self.object_source_one_of = [v if isinstance(v, str) else str(v) for v in self.object_source_one_of]
 
         if not isinstance(self.mapping_source_one_of, list):
-            self.mapping_source_one_of = (
-                [self.mapping_source_one_of] if self.mapping_source_one_of is not None else []
-            )
-        self.mapping_source_one_of = [
-            v if isinstance(v, str) else str(v) for v in self.mapping_source_one_of
-        ]
+            self.mapping_source_one_of = [self.mapping_source_one_of] if self.mapping_source_one_of is not None else []
+        self.mapping_source_one_of = [v if isinstance(v, str) else str(v) for v in self.mapping_source_one_of]
 
         if not isinstance(self.subject_match_field_one_of, list):
-            self.subject_match_field_one_of = (
-                [self.subject_match_field_one_of]
-                if self.subject_match_field_one_of is not None
-                else []
-            )
-        self.subject_match_field_one_of = [
-            v if isinstance(v, str) else str(v) for v in self.subject_match_field_one_of
-        ]
+            self.subject_match_field_one_of = [self.subject_match_field_one_of] if self.subject_match_field_one_of is not None else []
+        self.subject_match_field_one_of = [v if isinstance(v, str) else str(v) for v in self.subject_match_field_one_of]
 
         if not isinstance(self.object_match_field_one_of, list):
-            self.object_match_field_one_of = (
-                [self.object_match_field_one_of]
-                if self.object_match_field_one_of is not None
-                else []
-            )
-        self.object_match_field_one_of = [
-            v if isinstance(v, str) else str(v) for v in self.object_match_field_one_of
-        ]
+            self.object_match_field_one_of = [self.object_match_field_one_of] if self.object_match_field_one_of is not None else []
+        self.object_match_field_one_of = [v if isinstance(v, str) else str(v) for v in self.object_match_field_one_of]
 
         if not isinstance(self.transformations_included_in, list):
-            self.transformations_included_in = (
-                [self.transformations_included_in]
-                if self.transformations_included_in is not None
-                else []
-            )
-        self.transformations_included_in = [
-            v if isinstance(v, str) else str(v) for v in self.transformations_included_in
-        ]
+            self.transformations_included_in = [self.transformations_included_in] if self.transformations_included_in is not None else []
+        self.transformations_included_in = [v if isinstance(v, str) else str(v) for v in self.transformations_included_in]
 
         if not isinstance(self.predicate_id_one_of, list):
-            self.predicate_id_one_of = (
-                [self.predicate_id_one_of] if self.predicate_id_one_of is not None else []
-            )
-        self.predicate_id_one_of = [
-            v if isinstance(v, str) else str(v) for v in self.predicate_id_one_of
-        ]
+            self.predicate_id_one_of = [self.predicate_id_one_of] if self.predicate_id_one_of is not None else []
+        self.predicate_id_one_of = [v if isinstance(v, str) else str(v) for v in self.predicate_id_one_of]
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class Postcondition(YAMLRoot):
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = MAPPINGRULES.Postcondition
+    class_class_uri: ClassVar[URIRef] = MAPPINGRULES["Postcondition"]
     class_class_curie: ClassVar[str] = "mappingrules:Postcondition"
     class_name: ClassVar[str] = "Postcondition"
     class_model_uri: ClassVar[URIRef] = MAPPINGRULES.Postcondition
 
     predicate_id: Optional[str] = None
     weight: Optional[float] = None
 
@@ -248,110 +203,77 @@
 
 
 @dataclass
 class LexicalIndex(YAMLRoot):
     """
     An index over an ontology keyed by lexical unit
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = ONTOLEXINDEX.LexicalIndex
+    class_class_uri: ClassVar[URIRef] = ONTOLEXINDEX["LexicalIndex"]
     class_class_curie: ClassVar[str] = "ontolexindex:LexicalIndex"
     class_name: ClassVar[str] = "LexicalIndex"
     class_model_uri: ClassVar[URIRef] = MAPPINGRULES.LexicalIndex
 
-    groupings: Optional[
-        Union[
-            Dict[Union[str, LexicalGroupingTerm], Union[dict, "LexicalGrouping"]],
-            List[Union[dict, "LexicalGrouping"]],
-        ]
-    ] = empty_dict()
-    pipelines: Optional[
-        Union[
-            Dict[
-                Union[str, LexicalTransformationPipelineName],
-                Union[dict, "LexicalTransformationPipeline"],
-            ],
-            List[Union[dict, "LexicalTransformationPipeline"]],
-        ]
-    ] = empty_dict()
-
-    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
-        self._normalize_inlined_as_dict(
-            slot_name="groupings", slot_type=LexicalGrouping, key_name="term", keyed=True
-        )
-
-        self._normalize_inlined_as_dict(
-            slot_name="pipelines",
-            slot_type=LexicalTransformationPipeline,
-            key_name="name",
-            keyed=True,
-        )
+    groupings: Optional[Union[Dict[Union[str, LexicalGroupingTerm], Union[dict, "LexicalGrouping"]], List[Union[dict, "LexicalGrouping"]]]] = empty_dict()
+    pipelines: Optional[Union[Dict[Union[str, LexicalTransformationPipelineName], Union[dict, "LexicalTransformationPipeline"]], List[Union[dict, "LexicalTransformationPipeline"]]]] = empty_dict()
+
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        self._normalize_inlined_as_dict(slot_name="groupings", slot_type=LexicalGrouping, key_name="term", keyed=True)
+
+        self._normalize_inlined_as_dict(slot_name="pipelines", slot_type=LexicalTransformationPipeline, key_name="name", keyed=True)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class LexicalGrouping(YAMLRoot):
     """
     A grouping of ontology elements by a shared lexical term
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = ONTOLEXINDEX.LexicalGrouping
+    class_class_uri: ClassVar[URIRef] = ONTOLEXINDEX["LexicalGrouping"]
     class_class_curie: ClassVar[str] = "ontolexindex:LexicalGrouping"
     class_name: ClassVar[str] = "LexicalGrouping"
     class_model_uri: ClassVar[URIRef] = MAPPINGRULES.LexicalGrouping
 
     term: Union[str, LexicalGroupingTerm] = None
-    relationships: Optional[
-        Union[Union[dict, "RelationshipToTerm"], List[Union[dict, "RelationshipToTerm"]]]
-    ] = empty_list()
+    relationships: Optional[Union[Union[dict, "RelationshipToTerm"], List[Union[dict, "RelationshipToTerm"]]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.term):
             self.MissingRequiredField("term")
         if not isinstance(self.term, LexicalGroupingTerm):
             self.term = LexicalGroupingTerm(self.term)
 
         if not isinstance(self.relationships, list):
             self.relationships = [self.relationships] if self.relationships is not None else []
-        self.relationships = [
-            v if isinstance(v, RelationshipToTerm) else RelationshipToTerm(**as_dict(v))
-            for v in self.relationships
-        ]
+        self.relationships = [v if isinstance(v, RelationshipToTerm) else RelationshipToTerm(**as_dict(v)) for v in self.relationships]
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class RelationshipToTerm(YAMLRoot):
     """
     A relationship of an ontology element to a lexical term
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = ONTOLEXINDEX.RelationshipToTerm
+    class_class_uri: ClassVar[URIRef] = ONTOLEXINDEX["RelationshipToTerm"]
     class_class_curie: ClassVar[str] = "ontolexindex:RelationshipToTerm"
     class_name: ClassVar[str] = "RelationshipToTerm"
     class_model_uri: ClassVar[URIRef] = MAPPINGRULES.RelationshipToTerm
 
     predicate: Optional[Union[str, URIorCURIE]] = None
     element: Optional[Union[str, URIorCURIE]] = None
     element_term: Optional[str] = None
     source: Optional[Union[str, URIorCURIE]] = None
-    pipeline: Optional[
-        Union[
-            Union[str, LexicalTransformationPipelineName],
-            List[Union[str, LexicalTransformationPipelineName]],
-        ]
-    ] = empty_list()
+    pipeline: Optional[Union[Union[str, LexicalTransformationPipelineName], List[Union[str, LexicalTransformationPipelineName]]]] = empty_list()
     synonymized: Optional[Union[bool, Bool]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self.predicate is not None and not isinstance(self.predicate, URIorCURIE):
             self.predicate = URIorCURIE(self.predicate)
 
         if self.element is not None and not isinstance(self.element, URIorCURIE):
@@ -361,87 +283,70 @@
             self.element_term = str(self.element_term)
 
         if self.source is not None and not isinstance(self.source, URIorCURIE):
             self.source = URIorCURIE(self.source)
 
         if not isinstance(self.pipeline, list):
             self.pipeline = [self.pipeline] if self.pipeline is not None else []
-        self.pipeline = [
-            (
-                v
-                if isinstance(v, LexicalTransformationPipelineName)
-                else LexicalTransformationPipelineName(v)
-            )
-            for v in self.pipeline
-        ]
+        self.pipeline = [v if isinstance(v, LexicalTransformationPipelineName) else LexicalTransformationPipelineName(v) for v in self.pipeline]
 
         if self.synonymized is not None and not isinstance(self.synonymized, Bool):
             self.synonymized = Bool(self.synonymized)
 
         super().__post_init__(**kwargs)
 
 
 class Activity(YAMLRoot):
     """
     Generic grouping for any lexical operation
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = PROV.Activity
+    class_class_uri: ClassVar[URIRef] = PROV["Activity"]
     class_class_curie: ClassVar[str] = "prov:Activity"
     class_name: ClassVar[str] = "Activity"
     class_model_uri: ClassVar[URIRef] = MAPPINGRULES.Activity
 
 
 @dataclass
 class LexicalTransformationPipeline(Activity):
     """
     A collection of atomic lexical transformations that are applied in serial fashion
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = ONTOLEXINDEX.LexicalTransformationPipeline
+    class_class_uri: ClassVar[URIRef] = ONTOLEXINDEX["LexicalTransformationPipeline"]
     class_class_curie: ClassVar[str] = "ontolexindex:LexicalTransformationPipeline"
     class_name: ClassVar[str] = "LexicalTransformationPipeline"
     class_model_uri: ClassVar[URIRef] = MAPPINGRULES.LexicalTransformationPipeline
 
     name: Union[str, LexicalTransformationPipelineName] = None
-    transformations: Optional[
-        Union[Union[dict, "LexicalTransformation"], List[Union[dict, "LexicalTransformation"]]]
-    ] = empty_list()
+    transformations: Optional[Union[Union[dict, "LexicalTransformation"], List[Union[dict, "LexicalTransformation"]]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.name):
             self.MissingRequiredField("name")
         if not isinstance(self.name, LexicalTransformationPipelineName):
             self.name = LexicalTransformationPipelineName(self.name)
 
         if not isinstance(self.transformations, list):
-            self.transformations = (
-                [self.transformations] if self.transformations is not None else []
-            )
-        self.transformations = [
-            v if isinstance(v, LexicalTransformation) else LexicalTransformation(**as_dict(v))
-            for v in self.transformations
-        ]
+            self.transformations = [self.transformations] if self.transformations is not None else []
+        self.transformations = [v if isinstance(v, LexicalTransformation) else LexicalTransformation(**as_dict(v)) for v in self.transformations]
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class LexicalTransformation(Activity):
     """
     An atomic lexical transformation applied on a term (string) yielding a transformed string
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = ONTOLEXINDEX.LexicalTransformation
+    class_class_uri: ClassVar[URIRef] = ONTOLEXINDEX["LexicalTransformation"]
     class_class_curie: ClassVar[str] = "ontolexindex:LexicalTransformation"
     class_name: ClassVar[str] = "LexicalTransformation"
     class_model_uri: ClassVar[URIRef] = MAPPINGRULES.LexicalTransformation
 
     type: Optional[Union[str, "TransformationType"]] = None
     params: Optional[Union[Union[dict, "Any"], List[Union[dict, "Any"]]]] = empty_list()
 
@@ -450,435 +355,279 @@
             self.type = TransformationType(self.type)
 
         super().__post_init__(**kwargs)
 
 
 Any = Any
 
+@dataclass
+class RuleSet(YAMLRoot):
+    """
+    A set of rules for generating synonyms or alternate lexical elements.
+    """
+    _inherited_slots: ClassVar[List[str]] = []
+
+    class_class_uri: ClassVar[URIRef] = SYNONYMIZER["RuleSet"]
+    class_class_curie: ClassVar[str] = "synonymizer:RuleSet"
+    class_name: ClassVar[str] = "RuleSet"
+    class_model_uri: ClassVar[URIRef] = MAPPINGRULES.RuleSet
+
+    rules: Optional[Union[Union[dict, "Synonymizer"], List[Union[dict, "Synonymizer"]]]] = empty_list()
+    prefix: Optional[str] = None
+
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        if not isinstance(self.rules, list):
+            self.rules = [self.rules] if self.rules is not None else []
+        self.rules = [v if isinstance(v, Synonymizer) else Synonymizer(**as_dict(v)) for v in self.rules]
+
+        if self.prefix is not None and not isinstance(self.prefix, str):
+            self.prefix = str(self.prefix)
+
+        super().__post_init__(**kwargs)
+
+
+@dataclass
+class Synonymizer(YAMLRoot):
+    """
+    Specification of a rule for generating a synonym or alternate lexical element.
+    """
+    _inherited_slots: ClassVar[List[str]] = []
+
+    class_class_uri: ClassVar[URIRef] = SYNONYMIZER["Synonymizer"]
+    class_class_curie: ClassVar[str] = "synonymizer:Synonymizer"
+    class_name: ClassVar[str] = "Synonymizer"
+    class_model_uri: ClassVar[URIRef] = MAPPINGRULES.Synonymizer
+
+    description: Optional[str] = None
+    match: Optional[Union[str, RegularExpressionString]] = None
+    match_scope: Optional[str] = None
+    replacement: Optional[Union[str, RegularExpressionString]] = None
+    qualifier: Optional[str] = None
+    prefix: Optional[str] = None
+    in_place: Optional[Union[bool, Bool]] = None
+    tests: Optional[Union[Union[dict, "Test"], List[Union[dict, "Test"]]]] = empty_list()
+
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        if self.description is not None and not isinstance(self.description, str):
+            self.description = str(self.description)
+
+        if self.match is not None and not isinstance(self.match, RegularExpressionString):
+            self.match = RegularExpressionString(self.match)
+
+        if self.match_scope is not None and not isinstance(self.match_scope, str):
+            self.match_scope = str(self.match_scope)
+
+        if self.replacement is not None and not isinstance(self.replacement, RegularExpressionString):
+            self.replacement = RegularExpressionString(self.replacement)
+
+        if self.qualifier is not None and not isinstance(self.qualifier, str):
+            self.qualifier = str(self.qualifier)
+
+        if self.prefix is not None and not isinstance(self.prefix, str):
+            self.prefix = str(self.prefix)
+
+        if self.in_place is not None and not isinstance(self.in_place, Bool):
+            self.in_place = Bool(self.in_place)
+
+        if not isinstance(self.tests, list):
+            self.tests = [self.tests] if self.tests is not None else []
+        self.tests = [v if isinstance(v, Test) else Test(**as_dict(v)) for v in self.tests]
+
+        super().__post_init__(**kwargs)
+
+
+@dataclass
+class Test(YAMLRoot):
+    """
+    A unit test for a rule, specifies an intended output for an input
+    """
+    _inherited_slots: ClassVar[List[str]] = []
+
+    class_class_uri: ClassVar[URIRef] = SYNONYMIZER["Test"]
+    class_class_curie: ClassVar[str] = "synonymizer:Test"
+    class_name: ClassVar[str] = "Test"
+    class_model_uri: ClassVar[URIRef] = MAPPINGRULES.Test
+
+    input: Optional[str] = None
+    output: Optional[str] = None
+    prefix: Optional[str] = None
+
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        if self.input is not None and not isinstance(self.input, str):
+            self.input = str(self.input)
+
+        if self.output is not None and not isinstance(self.output, str):
+            self.output = str(self.output)
+
+        if self.prefix is not None and not isinstance(self.prefix, str):
+            self.prefix = str(self.prefix)
+
+        super().__post_init__(**kwargs)
+
 
 # Enumerations
 class TransformationType(EnumDefinitionImpl):
     """
     A controlled datamodels of the types of transformation that can be applied to
     """
-
     Stemming = PermissibleValue(
         text="Stemming",
-        description="Removal of the last few characters of a word to yield a stem term for each word in the term",
-    )
+        description="Removal of the last few characters of a word to yield a stem term for each word in the term")
     Lemmatization = PermissibleValue(
         text="Lemmatization",
-        description="Contextual reduction of a word to its base form for each word in the term",
-    )
+        description="Contextual reduction of a word to its base form for each word in the term")
     WordOrderNormalization = PermissibleValue(
         text="WordOrderNormalization",
-        description="reorder words in the term to a standard order such that comparisons are order-independent",
-    )
+        description="reorder words in the term to a standard order such that comparisons are order-independent")
     Depluralization = PermissibleValue(
         text="Depluralization",
-        description="Transform plural form to singular form for each word in a term",
-    )
+        description="Transform plural form to singular form for each word in a term")
     CaseNormalization = PermissibleValue(
         text="CaseNormalization",
-        description="Transform term to a standard case, typically lowercase",
-    )
+        description="Transform term to a standard case, typically lowercase")
     WhitespaceNormalization = PermissibleValue(
         text="WhitespaceNormalization",
-        description="Trim whitespace, condense whitespace runs, and transform all non-space whitespace to spaces",
-    )
+        description="Trim whitespace, condense whitespace runs, and transform all non-space whitespace to spaces")
     TermExpanson = PermissibleValue(
-        text="TermExpanson", description="Expand terms using a dictionary"
-    )
+        text="TermExpanson",
+        description="Expand terms using a dictionary")
     Synonymization = PermissibleValue(
-        text="Synonymization", description="Applying synonymizer rules from matcher_rules.yaml"
-    )
+        text="Synonymization",
+        description="Applying synonymizer rules from matcher_rules.yaml")
 
     _defn = EnumDefinition(
         name="TransformationType",
         description="A controlled datamodels of the types of transformation that can be applied to",
     )
 
-
 # Slots
 class slots:
     pass
 
+slots.mappingRuleCollection__rules = Slot(uri=MAPPINGRULES.rules, name="mappingRuleCollection__rules", curie=MAPPINGRULES.curie('rules'),
+                   model_uri=MAPPINGRULES.mappingRuleCollection__rules, domain=None, range=Optional[Union[Union[dict, MappingRule], List[Union[dict, MappingRule]]]])
+
+slots.mappingRuleCollection__minimum_confidence = Slot(uri=MAPPINGRULES.minimum_confidence, name="mappingRuleCollection__minimum_confidence", curie=MAPPINGRULES.curie('minimum_confidence'),
+                   model_uri=MAPPINGRULES.mappingRuleCollection__minimum_confidence, domain=None, range=Optional[float])
+
+slots.mappingRule__description = Slot(uri=MAPPINGRULES.description, name="mappingRule__description", curie=MAPPINGRULES.curie('description'),
+                   model_uri=MAPPINGRULES.mappingRule__description, domain=None, range=Optional[str])
+
+slots.mappingRule__oneway = Slot(uri=MAPPINGRULES.oneway, name="mappingRule__oneway", curie=MAPPINGRULES.curie('oneway'),
+                   model_uri=MAPPINGRULES.mappingRule__oneway, domain=None, range=Optional[Union[bool, Bool]])
+
+slots.mappingRule__preconditions = Slot(uri=SH.condition, name="mappingRule__preconditions", curie=SH.curie('condition'),
+                   model_uri=MAPPINGRULES.mappingRule__preconditions, domain=None, range=Optional[Union[dict, Precondition]])
+
+slots.mappingRule__postconditions = Slot(uri=MAPPINGRULES.postconditions, name="mappingRule__postconditions", curie=MAPPINGRULES.curie('postconditions'),
+                   model_uri=MAPPINGRULES.mappingRule__postconditions, domain=None, range=Optional[Union[dict, Postcondition]])
+
+slots.mappingRule__synonymizer = Slot(uri=MAPPINGRULES.synonymizer, name="mappingRule__synonymizer", curie=MAPPINGRULES.curie('synonymizer'),
+                   model_uri=MAPPINGRULES.mappingRule__synonymizer, domain=None, range=Optional[Union[dict, Synonymizer]])
+
+slots.precondition__subject_source_one_of = Slot(uri=MAPPINGRULES.subject_source_one_of, name="precondition__subject_source_one_of", curie=MAPPINGRULES.curie('subject_source_one_of'),
+                   model_uri=MAPPINGRULES.precondition__subject_source_one_of, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.precondition__object_source_one_of = Slot(uri=MAPPINGRULES.object_source_one_of, name="precondition__object_source_one_of", curie=MAPPINGRULES.curie('object_source_one_of'),
+                   model_uri=MAPPINGRULES.precondition__object_source_one_of, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.precondition__mapping_source_one_of = Slot(uri=MAPPINGRULES.mapping_source_one_of, name="precondition__mapping_source_one_of", curie=MAPPINGRULES.curie('mapping_source_one_of'),
+                   model_uri=MAPPINGRULES.precondition__mapping_source_one_of, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.precondition__subject_match_field_one_of = Slot(uri=MAPPINGRULES.subject_match_field_one_of, name="precondition__subject_match_field_one_of", curie=MAPPINGRULES.curie('subject_match_field_one_of'),
+                   model_uri=MAPPINGRULES.precondition__subject_match_field_one_of, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.precondition__object_match_field_one_of = Slot(uri=MAPPINGRULES.object_match_field_one_of, name="precondition__object_match_field_one_of", curie=MAPPINGRULES.curie('object_match_field_one_of'),
+                   model_uri=MAPPINGRULES.precondition__object_match_field_one_of, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.precondition__transformations_included_in = Slot(uri=MAPPINGRULES.transformations_included_in, name="precondition__transformations_included_in", curie=MAPPINGRULES.curie('transformations_included_in'),
+                   model_uri=MAPPINGRULES.precondition__transformations_included_in, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.precondition__predicate_id_one_of = Slot(uri=MAPPINGRULES.predicate_id_one_of, name="precondition__predicate_id_one_of", curie=MAPPINGRULES.curie('predicate_id_one_of'),
+                   model_uri=MAPPINGRULES.precondition__predicate_id_one_of, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.postcondition__predicate_id = Slot(uri=MAPPINGRULES.predicate_id, name="postcondition__predicate_id", curie=MAPPINGRULES.curie('predicate_id'),
+                   model_uri=MAPPINGRULES.postcondition__predicate_id, domain=None, range=Optional[str])
+
+slots.postcondition__weight = Slot(uri=MAPPINGRULES.weight, name="postcondition__weight", curie=MAPPINGRULES.curie('weight'),
+                   model_uri=MAPPINGRULES.postcondition__weight, domain=None, range=Optional[float])
+
+slots.lexicalIndex__groupings = Slot(uri=ONTOLEXINDEX.groupings, name="lexicalIndex__groupings", curie=ONTOLEXINDEX.curie('groupings'),
+                   model_uri=MAPPINGRULES.lexicalIndex__groupings, domain=None, range=Optional[Union[Dict[Union[str, LexicalGroupingTerm], Union[dict, LexicalGrouping]], List[Union[dict, LexicalGrouping]]]])
+
+slots.lexicalIndex__pipelines = Slot(uri=ONTOLEXINDEX.pipelines, name="lexicalIndex__pipelines", curie=ONTOLEXINDEX.curie('pipelines'),
+                   model_uri=MAPPINGRULES.lexicalIndex__pipelines, domain=None, range=Optional[Union[Dict[Union[str, LexicalTransformationPipelineName], Union[dict, LexicalTransformationPipeline]], List[Union[dict, LexicalTransformationPipeline]]]])
+
+slots.lexicalGrouping__term = Slot(uri=ONTOLEXINDEX.term, name="lexicalGrouping__term", curie=ONTOLEXINDEX.curie('term'),
+                   model_uri=MAPPINGRULES.lexicalGrouping__term, domain=None, range=URIRef)
+
+slots.lexicalGrouping__relationships = Slot(uri=ONTOLEXINDEX.relationships, name="lexicalGrouping__relationships", curie=ONTOLEXINDEX.curie('relationships'),
+                   model_uri=MAPPINGRULES.lexicalGrouping__relationships, domain=None, range=Optional[Union[Union[dict, RelationshipToTerm], List[Union[dict, RelationshipToTerm]]]])
+
+slots.relationshipToTerm__predicate = Slot(uri=ONTOLEXINDEX.predicate, name="relationshipToTerm__predicate", curie=ONTOLEXINDEX.curie('predicate'),
+                   model_uri=MAPPINGRULES.relationshipToTerm__predicate, domain=None, range=Optional[Union[str, URIorCURIE]])
+
+slots.relationshipToTerm__element = Slot(uri=ONTOLEXINDEX.element, name="relationshipToTerm__element", curie=ONTOLEXINDEX.curie('element'),
+                   model_uri=MAPPINGRULES.relationshipToTerm__element, domain=None, range=Optional[Union[str, URIorCURIE]])
+
+slots.relationshipToTerm__element_term = Slot(uri=ONTOLEXINDEX.element_term, name="relationshipToTerm__element_term", curie=ONTOLEXINDEX.curie('element_term'),
+                   model_uri=MAPPINGRULES.relationshipToTerm__element_term, domain=None, range=Optional[str])
+
+slots.relationshipToTerm__source = Slot(uri=ONTOLEXINDEX.source, name="relationshipToTerm__source", curie=ONTOLEXINDEX.curie('source'),
+                   model_uri=MAPPINGRULES.relationshipToTerm__source, domain=None, range=Optional[Union[str, URIorCURIE]])
+
+slots.relationshipToTerm__pipeline = Slot(uri=ONTOLEXINDEX.pipeline, name="relationshipToTerm__pipeline", curie=ONTOLEXINDEX.curie('pipeline'),
+                   model_uri=MAPPINGRULES.relationshipToTerm__pipeline, domain=None, range=Optional[Union[Union[str, LexicalTransformationPipelineName], List[Union[str, LexicalTransformationPipelineName]]]])
+
+slots.relationshipToTerm__synonymized = Slot(uri=ONTOLEXINDEX.synonymized, name="relationshipToTerm__synonymized", curie=ONTOLEXINDEX.curie('synonymized'),
+                   model_uri=MAPPINGRULES.relationshipToTerm__synonymized, domain=None, range=Optional[Union[bool, Bool]])
+
+slots.lexicalTransformationPipeline__name = Slot(uri=ONTOLEXINDEX.name, name="lexicalTransformationPipeline__name", curie=ONTOLEXINDEX.curie('name'),
+                   model_uri=MAPPINGRULES.lexicalTransformationPipeline__name, domain=None, range=URIRef)
+
+slots.lexicalTransformationPipeline__transformations = Slot(uri=ONTOLEXINDEX.transformations, name="lexicalTransformationPipeline__transformations", curie=ONTOLEXINDEX.curie('transformations'),
+                   model_uri=MAPPINGRULES.lexicalTransformationPipeline__transformations, domain=None, range=Optional[Union[Union[dict, LexicalTransformation], List[Union[dict, LexicalTransformation]]]])
+
+slots.lexicalTransformation__type = Slot(uri=ONTOLEXINDEX.type, name="lexicalTransformation__type", curie=ONTOLEXINDEX.curie('type'),
+                   model_uri=MAPPINGRULES.lexicalTransformation__type, domain=None, range=Optional[Union[str, "TransformationType"]])
+
+slots.lexicalTransformation__params = Slot(uri=ONTOLEXINDEX.params, name="lexicalTransformation__params", curie=ONTOLEXINDEX.curie('params'),
+                   model_uri=MAPPINGRULES.lexicalTransformation__params, domain=None, range=Optional[Union[Union[dict, Any], List[Union[dict, Any]]]])
+
+slots.ruleSet__rules = Slot(uri=SYNONYMIZER.rules, name="ruleSet__rules", curie=SYNONYMIZER.curie('rules'),
+                   model_uri=MAPPINGRULES.ruleSet__rules, domain=None, range=Optional[Union[Union[dict, Synonymizer], List[Union[dict, Synonymizer]]]])
+
+slots.ruleSet__prefix = Slot(uri=SYNONYMIZER.prefix, name="ruleSet__prefix", curie=SYNONYMIZER.curie('prefix'),
+                   model_uri=MAPPINGRULES.ruleSet__prefix, domain=None, range=Optional[str])
+
+slots.synonymizer__description = Slot(uri=SYNONYMIZER.description, name="synonymizer__description", curie=SYNONYMIZER.curie('description'),
+                   model_uri=MAPPINGRULES.synonymizer__description, domain=None, range=Optional[str])
+
+slots.synonymizer__match = Slot(uri=SYNONYMIZER.match, name="synonymizer__match", curie=SYNONYMIZER.curie('match'),
+                   model_uri=MAPPINGRULES.synonymizer__match, domain=None, range=Optional[Union[str, RegularExpressionString]])
+
+slots.synonymizer__match_scope = Slot(uri=SYNONYMIZER.match_scope, name="synonymizer__match_scope", curie=SYNONYMIZER.curie('match_scope'),
+                   model_uri=MAPPINGRULES.synonymizer__match_scope, domain=None, range=Optional[str])
+
+slots.synonymizer__replacement = Slot(uri=SYNONYMIZER.replacement, name="synonymizer__replacement", curie=SYNONYMIZER.curie('replacement'),
+                   model_uri=MAPPINGRULES.synonymizer__replacement, domain=None, range=Optional[Union[str, RegularExpressionString]])
+
+slots.synonymizer__qualifier = Slot(uri=SYNONYMIZER.qualifier, name="synonymizer__qualifier", curie=SYNONYMIZER.curie('qualifier'),
+                   model_uri=MAPPINGRULES.synonymizer__qualifier, domain=None, range=Optional[str])
+
+slots.synonymizer__prefix = Slot(uri=SYNONYMIZER.prefix, name="synonymizer__prefix", curie=SYNONYMIZER.curie('prefix'),
+                   model_uri=MAPPINGRULES.synonymizer__prefix, domain=None, range=Optional[str])
+
+slots.synonymizer__in_place = Slot(uri=SYNONYMIZER.in_place, name="synonymizer__in_place", curie=SYNONYMIZER.curie('in_place'),
+                   model_uri=MAPPINGRULES.synonymizer__in_place, domain=None, range=Optional[Union[bool, Bool]])
+
+slots.synonymizer__tests = Slot(uri=SYNONYMIZER.tests, name="synonymizer__tests", curie=SYNONYMIZER.curie('tests'),
+                   model_uri=MAPPINGRULES.synonymizer__tests, domain=None, range=Optional[Union[Union[dict, Test], List[Union[dict, Test]]]])
+
+slots.test__input = Slot(uri=SYNONYMIZER.input, name="test__input", curie=SYNONYMIZER.curie('input'),
+                   model_uri=MAPPINGRULES.test__input, domain=None, range=Optional[str])
+
+slots.test__output = Slot(uri=SYNONYMIZER.output, name="test__output", curie=SYNONYMIZER.curie('output'),
+                   model_uri=MAPPINGRULES.test__output, domain=None, range=Optional[str])
 
-slots.mappingRuleCollection__rules = Slot(
-    uri=MAPPINGRULES.rules,
-    name="mappingRuleCollection__rules",
-    curie=MAPPINGRULES.curie("rules"),
-    model_uri=MAPPINGRULES.mappingRuleCollection__rules,
-    domain=None,
-    range=Optional[Union[Union[dict, MappingRule], List[Union[dict, MappingRule]]]],
-)
-
-slots.mappingRuleCollection__minimum_confidence = Slot(
-    uri=MAPPINGRULES.minimum_confidence,
-    name="mappingRuleCollection__minimum_confidence",
-    curie=MAPPINGRULES.curie("minimum_confidence"),
-    model_uri=MAPPINGRULES.mappingRuleCollection__minimum_confidence,
-    domain=None,
-    range=Optional[float],
-)
-
-slots.mappingRule__description = Slot(
-    uri=MAPPINGRULES.description,
-    name="mappingRule__description",
-    curie=MAPPINGRULES.curie("description"),
-    model_uri=MAPPINGRULES.mappingRule__description,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.mappingRule__oneway = Slot(
-    uri=MAPPINGRULES.oneway,
-    name="mappingRule__oneway",
-    curie=MAPPINGRULES.curie("oneway"),
-    model_uri=MAPPINGRULES.mappingRule__oneway,
-    domain=None,
-    range=Optional[Union[bool, Bool]],
-)
-
-slots.mappingRule__preconditions = Slot(
-    uri=SH.condition,
-    name="mappingRule__preconditions",
-    curie=SH.curie("condition"),
-    model_uri=MAPPINGRULES.mappingRule__preconditions,
-    domain=None,
-    range=Optional[Union[dict, Precondition]],
-)
-
-slots.mappingRule__postconditions = Slot(
-    uri=MAPPINGRULES.postconditions,
-    name="mappingRule__postconditions",
-    curie=MAPPINGRULES.curie("postconditions"),
-    model_uri=MAPPINGRULES.mappingRule__postconditions,
-    domain=None,
-    range=Optional[Union[dict, Postcondition]],
-)
-
-slots.mappingRule__synonymizer = Slot(
-    uri=MAPPINGRULES.synonymizer,
-    name="mappingRule__synonymizer",
-    curie=MAPPINGRULES.curie("synonymizer"),
-    model_uri=MAPPINGRULES.mappingRule__synonymizer,
-    domain=None,
-    range=Optional[Union[dict, Synonymizer]],
-)
-
-slots.precondition__subject_source_one_of = Slot(
-    uri=MAPPINGRULES.subject_source_one_of,
-    name="precondition__subject_source_one_of",
-    curie=MAPPINGRULES.curie("subject_source_one_of"),
-    model_uri=MAPPINGRULES.precondition__subject_source_one_of,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.precondition__object_source_one_of = Slot(
-    uri=MAPPINGRULES.object_source_one_of,
-    name="precondition__object_source_one_of",
-    curie=MAPPINGRULES.curie("object_source_one_of"),
-    model_uri=MAPPINGRULES.precondition__object_source_one_of,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.precondition__mapping_source_one_of = Slot(
-    uri=MAPPINGRULES.mapping_source_one_of,
-    name="precondition__mapping_source_one_of",
-    curie=MAPPINGRULES.curie("mapping_source_one_of"),
-    model_uri=MAPPINGRULES.precondition__mapping_source_one_of,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.precondition__subject_match_field_one_of = Slot(
-    uri=MAPPINGRULES.subject_match_field_one_of,
-    name="precondition__subject_match_field_one_of",
-    curie=MAPPINGRULES.curie("subject_match_field_one_of"),
-    model_uri=MAPPINGRULES.precondition__subject_match_field_one_of,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.precondition__object_match_field_one_of = Slot(
-    uri=MAPPINGRULES.object_match_field_one_of,
-    name="precondition__object_match_field_one_of",
-    curie=MAPPINGRULES.curie("object_match_field_one_of"),
-    model_uri=MAPPINGRULES.precondition__object_match_field_one_of,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.precondition__transformations_included_in = Slot(
-    uri=MAPPINGRULES.transformations_included_in,
-    name="precondition__transformations_included_in",
-    curie=MAPPINGRULES.curie("transformations_included_in"),
-    model_uri=MAPPINGRULES.precondition__transformations_included_in,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.precondition__predicate_id_one_of = Slot(
-    uri=MAPPINGRULES.predicate_id_one_of,
-    name="precondition__predicate_id_one_of",
-    curie=MAPPINGRULES.curie("predicate_id_one_of"),
-    model_uri=MAPPINGRULES.precondition__predicate_id_one_of,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.postcondition__predicate_id = Slot(
-    uri=MAPPINGRULES.predicate_id,
-    name="postcondition__predicate_id",
-    curie=MAPPINGRULES.curie("predicate_id"),
-    model_uri=MAPPINGRULES.postcondition__predicate_id,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.postcondition__weight = Slot(
-    uri=MAPPINGRULES.weight,
-    name="postcondition__weight",
-    curie=MAPPINGRULES.curie("weight"),
-    model_uri=MAPPINGRULES.postcondition__weight,
-    domain=None,
-    range=Optional[float],
-)
-
-slots.synonymizer__the_rule = Slot(
-    uri=MAPPINGRULES.the_rule,
-    name="synonymizer__the_rule",
-    curie=MAPPINGRULES.curie("the_rule"),
-    model_uri=MAPPINGRULES.synonymizer__the_rule,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.synonymizer__match = Slot(
-    uri=MAPPINGRULES.match,
-    name="synonymizer__match",
-    curie=MAPPINGRULES.curie("match"),
-    model_uri=MAPPINGRULES.synonymizer__match,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.synonymizer__match_scope = Slot(
-    uri=MAPPINGRULES.match_scope,
-    name="synonymizer__match_scope",
-    curie=MAPPINGRULES.curie("match_scope"),
-    model_uri=MAPPINGRULES.synonymizer__match_scope,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.synonymizer__replacement = Slot(
-    uri=MAPPINGRULES.replacement,
-    name="synonymizer__replacement",
-    curie=MAPPINGRULES.curie("replacement"),
-    model_uri=MAPPINGRULES.synonymizer__replacement,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.synonymizer__qualifier = Slot(
-    uri=MAPPINGRULES.qualifier,
-    name="synonymizer__qualifier",
-    curie=MAPPINGRULES.curie("qualifier"),
-    model_uri=MAPPINGRULES.synonymizer__qualifier,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.synonymizer__prefix = Slot(
-    uri=MAPPINGRULES.prefix,
-    name="synonymizer__prefix",
-    curie=MAPPINGRULES.curie("prefix"),
-    model_uri=MAPPINGRULES.synonymizer__prefix,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.synonymizer__tests = Slot(
-    uri=MAPPINGRULES.tests,
-    name="synonymizer__tests",
-    curie=MAPPINGRULES.curie("tests"),
-    model_uri=MAPPINGRULES.synonymizer__tests,
-    domain=None,
-    range=Optional[Union[dict, Test]],
-)
-
-slots.test__input = Slot(
-    uri=MAPPINGRULES.input,
-    name="test__input",
-    curie=MAPPINGRULES.curie("input"),
-    model_uri=MAPPINGRULES.test__input,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.test__output = Slot(
-    uri=MAPPINGRULES.output,
-    name="test__output",
-    curie=MAPPINGRULES.curie("output"),
-    model_uri=MAPPINGRULES.test__output,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.test__prefix = Slot(
-    uri=MAPPINGRULES.prefix,
-    name="test__prefix",
-    curie=MAPPINGRULES.curie("prefix"),
-    model_uri=MAPPINGRULES.test__prefix,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.lexicalIndex__groupings = Slot(
-    uri=ONTOLEXINDEX.groupings,
-    name="lexicalIndex__groupings",
-    curie=ONTOLEXINDEX.curie("groupings"),
-    model_uri=MAPPINGRULES.lexicalIndex__groupings,
-    domain=None,
-    range=Optional[
-        Union[
-            Dict[Union[str, LexicalGroupingTerm], Union[dict, LexicalGrouping]],
-            List[Union[dict, LexicalGrouping]],
-        ]
-    ],
-)
-
-slots.lexicalIndex__pipelines = Slot(
-    uri=ONTOLEXINDEX.pipelines,
-    name="lexicalIndex__pipelines",
-    curie=ONTOLEXINDEX.curie("pipelines"),
-    model_uri=MAPPINGRULES.lexicalIndex__pipelines,
-    domain=None,
-    range=Optional[
-        Union[
-            Dict[
-                Union[str, LexicalTransformationPipelineName],
-                Union[dict, LexicalTransformationPipeline],
-            ],
-            List[Union[dict, LexicalTransformationPipeline]],
-        ]
-    ],
-)
-
-slots.lexicalGrouping__term = Slot(
-    uri=ONTOLEXINDEX.term,
-    name="lexicalGrouping__term",
-    curie=ONTOLEXINDEX.curie("term"),
-    model_uri=MAPPINGRULES.lexicalGrouping__term,
-    domain=None,
-    range=URIRef,
-)
-
-slots.lexicalGrouping__relationships = Slot(
-    uri=ONTOLEXINDEX.relationships,
-    name="lexicalGrouping__relationships",
-    curie=ONTOLEXINDEX.curie("relationships"),
-    model_uri=MAPPINGRULES.lexicalGrouping__relationships,
-    domain=None,
-    range=Optional[Union[Union[dict, RelationshipToTerm], List[Union[dict, RelationshipToTerm]]]],
-)
-
-slots.relationshipToTerm__predicate = Slot(
-    uri=ONTOLEXINDEX.predicate,
-    name="relationshipToTerm__predicate",
-    curie=ONTOLEXINDEX.curie("predicate"),
-    model_uri=MAPPINGRULES.relationshipToTerm__predicate,
-    domain=None,
-    range=Optional[Union[str, URIorCURIE]],
-)
-
-slots.relationshipToTerm__element = Slot(
-    uri=ONTOLEXINDEX.element,
-    name="relationshipToTerm__element",
-    curie=ONTOLEXINDEX.curie("element"),
-    model_uri=MAPPINGRULES.relationshipToTerm__element,
-    domain=None,
-    range=Optional[Union[str, URIorCURIE]],
-)
-
-slots.relationshipToTerm__element_term = Slot(
-    uri=ONTOLEXINDEX.element_term,
-    name="relationshipToTerm__element_term",
-    curie=ONTOLEXINDEX.curie("element_term"),
-    model_uri=MAPPINGRULES.relationshipToTerm__element_term,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.relationshipToTerm__source = Slot(
-    uri=ONTOLEXINDEX.source,
-    name="relationshipToTerm__source",
-    curie=ONTOLEXINDEX.curie("source"),
-    model_uri=MAPPINGRULES.relationshipToTerm__source,
-    domain=None,
-    range=Optional[Union[str, URIorCURIE]],
-)
-
-slots.relationshipToTerm__pipeline = Slot(
-    uri=ONTOLEXINDEX.pipeline,
-    name="relationshipToTerm__pipeline",
-    curie=ONTOLEXINDEX.curie("pipeline"),
-    model_uri=MAPPINGRULES.relationshipToTerm__pipeline,
-    domain=None,
-    range=Optional[
-        Union[
-            Union[str, LexicalTransformationPipelineName],
-            List[Union[str, LexicalTransformationPipelineName]],
-        ]
-    ],
-)
-
-slots.relationshipToTerm__synonymized = Slot(
-    uri=ONTOLEXINDEX.synonymized,
-    name="relationshipToTerm__synonymized",
-    curie=ONTOLEXINDEX.curie("synonymized"),
-    model_uri=MAPPINGRULES.relationshipToTerm__synonymized,
-    domain=None,
-    range=Optional[Union[bool, Bool]],
-)
-
-slots.lexicalTransformationPipeline__name = Slot(
-    uri=ONTOLEXINDEX.name,
-    name="lexicalTransformationPipeline__name",
-    curie=ONTOLEXINDEX.curie("name"),
-    model_uri=MAPPINGRULES.lexicalTransformationPipeline__name,
-    domain=None,
-    range=URIRef,
-)
-
-slots.lexicalTransformationPipeline__transformations = Slot(
-    uri=ONTOLEXINDEX.transformations,
-    name="lexicalTransformationPipeline__transformations",
-    curie=ONTOLEXINDEX.curie("transformations"),
-    model_uri=MAPPINGRULES.lexicalTransformationPipeline__transformations,
-    domain=None,
-    range=Optional[
-        Union[Union[dict, LexicalTransformation], List[Union[dict, LexicalTransformation]]]
-    ],
-)
-
-slots.lexicalTransformation__type = Slot(
-    uri=ONTOLEXINDEX.type,
-    name="lexicalTransformation__type",
-    curie=ONTOLEXINDEX.curie("type"),
-    model_uri=MAPPINGRULES.lexicalTransformation__type,
-    domain=None,
-    range=Optional[Union[str, "TransformationType"]],
-)
-
-slots.lexicalTransformation__params = Slot(
-    uri=ONTOLEXINDEX.params,
-    name="lexicalTransformation__params",
-    curie=ONTOLEXINDEX.curie("params"),
-    model_uri=MAPPINGRULES.lexicalTransformation__params,
-    domain=None,
-    range=Optional[Union[Union[dict, Any], List[Union[dict, Any]]]],
-)
+slots.test__prefix = Slot(uri=SYNONYMIZER.prefix, name="test__prefix", curie=SYNONYMIZER.curie('prefix'),
+                   model_uri=MAPPINGRULES.test__prefix, domain=None, range=Optional[str])
```

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/mapping_rules_datamodel.schema.json` & `oaklib-0.6.5/src/oaklib/datamodels/mapping_rules_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/mapping_rules_datamodel.yaml` & `oaklib-0.6.5/src/oaklib/datamodels/synonymizer_datamodel.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-id: https://w3id.org/oak/mapping-rules-datamodel
-title: Mapping Rules Datamodel
-name: mapping-rules-datamodel
+id: https://w3id.org/oak/synonymizer-datamodel
+title: Synonymizer Datamodel
+name: synonymizer_datamodel
 description: >-
-  A datamodel for specifying lexical mapping rules
+  A datamodel for specifying synonymization rules
 license: https://creativecommons.org/publicdomain/zero/1.0/
 
 prefixes:
   linkml: https://w3id.org/linkml/
-  mappingrules: https://w3id.org/oak/mapping-rules-datamodel/
+  synonymizer: https://w3id.org/oak/synonymizer-datamodel/
   skos: http://www.w3.org/2004/02/skos/core#
   pav: http://purl.org/pav/
   schema: http://schema.org/
   sh: https://w3id.org/shacl/
   prov: http://www.w3.org/ns/prov#
 
-default_prefix: mappingrules
+default_prefix: synonymizer
 default_range: string
 
 default_curi_maps:
   - semweb_context
 
 emit_prefixes:
   - linkml
@@ -26,108 +26,68 @@
   - rdfs
   - xsd
   - owl
 
 imports:
   - linkml:types
   - lexical_index
-  - synonymizer_datamodel
 
 
+types:
+  RegularExpressionString:
+    typeof: string
+
 
 #==================================
 # Classes                         #
 #==================================
 classes:
-  MappingRuleCollection:
-    tree_root: true
-    description: A collection of mapping rules
-    attributes:
-      rules:
-        description: all rules
-        range: MappingRule
-        multivalued: true
-        inlined: true
-      minimum_confidence:
-        range: float
 
-  MappingRule:
-    description: An individual mapping rule, if preconditions match the postconditions are applied
+  RuleSet:
+    description: A set of rules for generating synonyms or alternate lexical elements.
     attributes:
-      description:
-      oneway:
-        ifabsent: False
-        range: boolean
-        description: if true then subject and object can be switched and predicate inverted
-      preconditions:
-        range: Precondition
-        slot_uri: sh:condition
-        description: all of the criteria that must be true before a rule is fired
-      postconditions:
-        range: Postcondition
-        description: conditions that apply if preconditions match
-      synonymizer:
+      rules:
+        description: A list of rules for generating synonyms or alternate lexical elements.
         range: Synonymizer
-        description: Normalizing rules to labels. 
-
-  Precondition:
-    description: A pattern to be matched against an individual SSSOM mapping
-    attributes:
-      subject_source_one_of:
-        multivalued: true
-      object_source_one_of:
-        multivalued: true
-      mapping_source_one_of:
-        multivalued: true
-      subject_match_field_one_of:
-        multivalued: true
-      object_match_field_one_of:
-        multivalued: true
-      transformations_included_in:
-        multivalued: true
-      predicate_id_one_of:
         multivalued: true
-
-  Postcondition:
-    attributes:
-      predicate_id:
-        comments:
-          - if the rule is invertible, then the predicate is inverted, e.g. skos broad becomes narrow
-      weight:
-        description: Weighting of the rule, positive increases the confidence, negative decreases
-        range: float
-        see_also:
-          - https://en.wikipedia.org/wiki/Logit
-          - https://upload.wikimedia.org/wikipedia/commons/5/57/Logit.png
+      prefix:
+        description: The prefix that qualifies for the rule.
+        range: string
 
   Synonymizer:
+   description: Specification of a rule for generating a synonym or alternate lexical element.
    attributes:
     description:
       description: Description of the rule.
       range: string
     match:
       description: Reg-ex rule to match substrings in labels.
-      range: string
+      range: RegularExpressionString
     match_scope:
-      description: Scope of the reg-ex rule
+      description: Synonym scope of the reg-ex rule, e.g. exact, narrow
       range: string
     replacement:
       description: Reg-ex rule to replace substrings in labels
-      range: string
+      range: RegularExpressionString
     qualifier:
       description: Type of match for the new synonym generated.
       range: string
     prefix:
       description: The rule applies to nodes of a specific prefix.
       range: string
+    in_place:
+      description: Whether the rule is applied in place or not.
+      range: boolean
     tests:
       description: Unit tests for each rules.
       range: Test
+      multivalued: true
   
   Test:
+   description: A unit test for a rule, specifies an intended output for an input
    attributes:
     input:
      description: Input string for the rule.
     output:
      description: Output based on the rule.
     prefix:
       description: The prefix that qualifies for the rule.
```

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/obograph.owl.ttl` & `oaklib-0.6.5/src/oaklib/datamodels/obograph.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/obograph.py` & `oaklib-0.6.5/src/oaklib/datamodels/obograph.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/obograph.schema.json` & `oaklib-0.6.5/src/oaklib/datamodels/obograph.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/obograph.yaml` & `oaklib-0.6.5/src/oaklib/datamodels/obograph.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/ontology_metadata.owl.ttl` & `oaklib-0.6.5/src/oaklib/datamodels/ontology_metadata.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/ontology_metadata.py` & `oaklib-0.6.5/src/oaklib/datamodels/ontology_metadata.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/ontology_metadata.schema.json` & `oaklib-0.6.5/src/oaklib/datamodels/ontology_metadata.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/ontology_metadata.yaml` & `oaklib-0.6.5/src/oaklib/datamodels/ontology_metadata.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/oxo.owl.ttl` & `oaklib-0.6.5/src/oaklib/datamodels/oxo.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/oxo.py` & `oaklib-0.6.5/src/oaklib/datamodels/oxo.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/oxo.yaml` & `oaklib-0.6.5/src/oaklib/datamodels/oxo.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/search.py` & `oaklib-0.6.5/src/oaklib/datamodels/search.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/search_datamodel.owl.ttl` & `oaklib-0.6.5/src/oaklib/datamodels/search_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/search_datamodel.py` & `oaklib-0.6.5/src/oaklib/datamodels/search_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/search_datamodel.yaml` & `oaklib-0.6.5/src/oaklib/datamodels/search_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/similarity.owl.ttl` & `oaklib-0.6.5/src/oaklib/datamodels/similarity.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/similarity.py` & `oaklib-0.6.5/src/oaklib/datamodels/similarity.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/similarity.yaml` & `oaklib-0.6.5/src/oaklib/datamodels/similarity.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl` & `oaklib-0.6.5/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/summary_statistics_datamodel.py` & `oaklib-0.6.5/src/oaklib/datamodels/summary_statistics_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/summary_statistics_datamodel.schema.json` & `oaklib-0.6.5/src/oaklib/datamodels/summary_statistics_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/summary_statistics_datamodel.yaml` & `oaklib-0.6.5/src/oaklib/datamodels/summary_statistics_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/synonymizer_datamodel.py` & `oaklib-0.6.5/src/oaklib/datamodels/synonymizer_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/synonymizer_datamodel.yaml` & `oaklib-0.6.5/src/oaklib/datamodels/value_set_configuration.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,94 +1,98 @@
-id: https://w3id.org/oak/synonymizer-datamodel
-title: Synonymizer Datamodel
-name: synonymizer_datamodel
+id: https://w3id.org/linkml/value-set-configuration
+title: Value Set Configuration
+name: value-set-configuration
 description: >-
-  A datamodel for specifying synonymization rules
+  A datamodel for configuring value sets and value set expabsions
 license: https://creativecommons.org/publicdomain/zero/1.0/
 
 prefixes:
+  vsconf: https://w3id.org/linkml/value-set-configuration/
   linkml: https://w3id.org/linkml/
-  synonymizer: https://w3id.org/oak/synonymizer-datamodel/
-  skos: http://www.w3.org/2004/02/skos/core#
-  pav: http://purl.org/pav/
   schema: http://schema.org/
   sh: https://w3id.org/shacl/
-  prov: http://www.w3.org/ns/prov#
+  oa: http://www.w3.org/ns/oa#
 
-default_prefix: synonymizer
+default_prefix: vsconf
 default_range: string
 
-default_curi_maps:
-  - semweb_context
-
-emit_prefixes:
-  - linkml
-  - rdf
-  - rdfs
-  - xsd
-  - owl
-
 imports:
   - linkml:types
-  - lexical_index
-
-
-types:
-  RegularExpressionString:
-    typeof: string
 
 
 #==================================
 # Classes                         #
 #==================================
 classes:
-
-  RuleSet:
-    description: A set of rules for generating synonyms or alternate lexical elements.
+  ValueSetConfiguration:
+    description: configuration for value sets
     attributes:
-      rules:
-        description: A list of rules for generating synonyms or alternate lexical elements.
-        range: Synonymizer
+      default_resolver:
+        range: Resolver
+        inlined: true
+      resource_resolvers:
+        range: Resolver
+        multivalued: true
+        inlined: true
+      prefix_resolvers:
+        range: Resolver
         multivalued: true
-      prefix:
-        description: The prefix that qualifies for the rule.
+        inlined: true
+
+  Resolver:
+    description: A mechanism for resolving using an ontology
+    attributes:
+      name:
+        range: string
+        key: true
+        description: The name of the resource or prefix
+      shorthand_prefix:
+      shorthand:
+        description: A shorthand for the resolver, using the OAK shorthand syntax
+      method:
+        range: ResolverMethod
+        description: >-
+          The method used to resolve the value set.
+      url:
+        range: uri
+
+  NamedResolver:
+    description: A resolver that is associated with a named resource or prefix
+    is_a: Resolver
+    attributes:
+      name:
         range: string
+        key: true
+        description: The name of the resource or prefix
+
+enums:
+  ResolverMethod:
+    permissible_values:
+      SemanticSQL:
+        annotations:
+          prefix: sqlite:obo
+      OLS:
+        annotations:
+          prefix: ols
+      BioPortal:
+        annotations:
+          prefix: bioportal
+      OntoBee:
+        annotations:
+          prefix: ontobee
+      Ubergraph:
+        annotations:
+          prefix: ubergraph
+      TCCM:
+      SPARQL:
+      LOV:
+        annotations:
+          prefix: lov
+      Pronto:
+        annotations:
+          prefix: pronto
+      Uniprot:
+        annotations:
+          prefix: uniprot
+
+
 
-  Synonymizer:
-   description: Specification of a rule for generating a synonym or alternate lexical element.
-   attributes:
-    description:
-      description: Description of the rule.
-      range: string
-    match:
-      description: Reg-ex rule to match substrings in labels.
-      range: RegularExpressionString
-    match_scope:
-      description: Synonym scope of the reg-ex rule, e.g. exact, narrow
-      range: string
-    replacement:
-      description: Reg-ex rule to replace substrings in labels
-      range: RegularExpressionString
-    qualifier:
-      description: Type of match for the new synonym generated.
-      range: string
-    prefix:
-      description: The rule applies to nodes of a specific prefix.
-      range: string
-    in_place:
-      description: Whether the rule is applied in place or not.
-      range: boolean
-    tests:
-      description: Unit tests for each rules.
-      range: Test
-      multivalued: true
-  
-  Test:
-   description: A unit test for a rule, specifies an intended output for an input
-   attributes:
-    input:
-     description: Input string for the rule.
-    output:
-     description: Output based on the rule.
-    prefix:
-      description: The prefix that qualifies for the rule.
-
```

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/taxon_constraints.owl.ttl` & `oaklib-0.6.5/src/oaklib/datamodels/taxon_constraints.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/taxon_constraints.py` & `oaklib-0.6.5/src/oaklib/datamodels/taxon_constraints.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/taxon_constraints.yaml` & `oaklib-0.6.5/src/oaklib/datamodels/taxon_constraints.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/text_annotator.owl.ttl` & `oaklib-0.6.5/src/oaklib/datamodels/text_annotator.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/text_annotator.py` & `oaklib-0.6.5/src/oaklib/datamodels/text_annotator.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/text_annotator.schema.json` & `oaklib-0.6.5/src/oaklib/datamodels/text_annotator.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/text_annotator.yaml` & `oaklib-0.6.5/src/oaklib/datamodels/text_annotator.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/validation_datamodel.owl.ttl` & `oaklib-0.6.5/src/oaklib/datamodels/validation_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/validation_datamodel.py` & `oaklib-0.6.5/src/oaklib/datamodels/validation_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/validation_datamodel.schema.json` & `oaklib-0.6.5/src/oaklib/datamodels/validation_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/validation_datamodel.yaml` & `oaklib-0.6.5/src/oaklib/datamodels/validation_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/value_set_configuration.owl.ttl` & `oaklib-0.6.5/src/oaklib/datamodels/value_set_configuration.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/value_set_configuration.py` & `oaklib-0.6.5/src/oaklib/datamodels/value_set_configuration.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/datamodels/vocabulary.py` & `oaklib-0.6.5/src/oaklib/datamodels/vocabulary.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/__init__.py` & `oaklib-0.6.5/src/oaklib/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/aggregator/aggregator_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/aggregator/aggregator_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/agrkb/agrkb_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/agrkb/agrkb_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/amigo/amigo_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/amigo/amigo_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/cx/cx_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/cx/cx_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/eutils/eutils_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/eutils/eutils_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/eutils/pubmed_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/eutils/pubmed_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/funowl/funowl_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/funowl/funowl_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/gilda.py` & `oaklib-0.6.5/src/oaklib/implementations/gilda.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/kgx/kgx_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/kgx/kgx_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/llm_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/llm_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/monarch/monarch_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/monarch/monarch_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/ncbi/ncbi_gene_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/ncbi/ncbi_gene_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/obograph/obograph_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/obograph/obograph_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/ols/ols_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/ols/ols_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/ols/oxo_utils.py` & `oaklib-0.6.5/src/oaklib/implementations/ols/oxo_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/ontobee/ontobee_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/ontobee/ontobee_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/ontoportal/bioportal_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/ontoportal/bioportal_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py` & `oaklib-0.6.5/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/pantherdb/pantherdb_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/pantherdb/pantherdb_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/pronto/pronto_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/pronto/pronto_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/semsimian/semsimian_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/semsimian/semsimian_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/simpleobo/simple_obo_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/simpleobo/simple_obo_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/simpleobo/simple_obo_parser.py` & `oaklib-0.6.5/src/oaklib/implementations/simpleobo/simple_obo_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/sparql/abstract_sparql_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/sparql/abstract_sparql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/sparql/lov_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/sparql/lov_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/sparql/oak_metamodel_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/sparql/oak_metamodel_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/sparql/sparql_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/sparql/sparql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/sparql/sparql_query.py` & `oaklib-0.6.5/src/oaklib/implementations/sparql/sparql_query.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/sqldb/sql_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/sqldb/sql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/sqldb/sqlite_utils.py` & `oaklib-0.6.5/src/oaklib/implementations/sqldb/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/tabular/robot_template_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/tabular/robot_template_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/tabular/tabular_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/tabular/tabular_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/translator/translator_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/translator/translator_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/ubergraph/ubergraph_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/ubergraph/ubergraph_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/uniprot/uniprot_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/uniprot/uniprot_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/implementations/wikidata/wikidata_implementation.py` & `oaklib-0.6.5/src/oaklib/implementations/wikidata/wikidata_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/indexes/edge_index.py` & `oaklib-0.6.5/src/oaklib/indexes/edge_index.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/inference/owl_reasoner.py` & `oaklib-0.6.5/src/oaklib/inference/owl_reasoner.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/inference/relation_graph_reasoner.py` & `oaklib-0.6.5/src/oaklib/inference/relation_graph_reasoner.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/interfaces/__init__.py` & `oaklib-0.6.5/src/oaklib/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/interfaces/association_provider_interface.py` & `oaklib-0.6.5/src/oaklib/interfaces/association_provider_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/interfaces/basic_ontology_interface.py` & `oaklib-0.6.5/src/oaklib/interfaces/basic_ontology_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/interfaces/class_enrichment_calculation_interface.py` & `oaklib-0.6.5/src/oaklib/interfaces/class_enrichment_calculation_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/interfaces/differ_interface.py` & `oaklib-0.6.5/src/oaklib/interfaces/differ_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/interfaces/dumper_interface.py` & `oaklib-0.6.5/src/oaklib/interfaces/dumper_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/interfaces/embedding_provider_interface.py` & `oaklib-0.6.5/src/oaklib/interfaces/embedding_provider_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/interfaces/mapping_provider_interface.py` & `oaklib-0.6.5/src/oaklib/interfaces/mapping_provider_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/interfaces/merge_interface.py` & `oaklib-0.6.5/src/oaklib/interfaces/merge_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/interfaces/metadata_interface.py` & `oaklib-0.6.5/src/oaklib/interfaces/metadata_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/interfaces/obograph_interface.py` & `oaklib-0.6.5/src/oaklib/interfaces/obograph_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/interfaces/obolegacy_interface.py` & `oaklib-0.6.5/src/oaklib/interfaces/obolegacy_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/interfaces/ontology_generator_interface.py` & `oaklib-0.6.5/src/oaklib/interfaces/ontology_generator_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/interfaces/ontology_interface.py` & `oaklib-0.6.5/src/oaklib/interfaces/ontology_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/interfaces/owl_interface.py` & `oaklib-0.6.5/src/oaklib/interfaces/owl_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/interfaces/patcher_interface.py` & `oaklib-0.6.5/src/oaklib/interfaces/patcher_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/interfaces/rdf_interface.py` & `oaklib-0.6.5/src/oaklib/interfaces/rdf_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/interfaces/relation_graph_interface.py` & `oaklib-0.6.5/src/oaklib/interfaces/relation_graph_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/interfaces/search_interface.py` & `oaklib-0.6.5/src/oaklib/interfaces/search_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/interfaces/semsim_interface.py` & `oaklib-0.6.5/src/oaklib/interfaces/semsim_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/interfaces/skos_interface.py` & `oaklib-0.6.5/src/oaklib/interfaces/skos_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/interfaces/subsetter_interface.py` & `oaklib-0.6.5/src/oaklib/interfaces/subsetter_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/interfaces/summary_statistics_interface.py` & `oaklib-0.6.5/src/oaklib/interfaces/summary_statistics_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/interfaces/taxon_constraint_interface.py` & `oaklib-0.6.5/src/oaklib/interfaces/taxon_constraint_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/interfaces/text_annotator_interface.py` & `oaklib-0.6.5/src/oaklib/interfaces/text_annotator_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/interfaces/validator_interface.py` & `oaklib-0.6.5/src/oaklib/interfaces/validator_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/io/heatmap_writer.py` & `oaklib-0.6.5/src/oaklib/io/heatmap_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/io/html_writer.py` & `oaklib-0.6.5/src/oaklib/io/html_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/io/obograph_writer.py` & `oaklib-0.6.5/src/oaklib/io/obograph_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/io/rollup_report_writer.py` & `oaklib-0.6.5/src/oaklib/io/rollup_report_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/io/streaming_axiom_writer.py` & `oaklib-0.6.5/src/oaklib/io/streaming_axiom_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/io/streaming_csv_writer.py` & `oaklib-0.6.5/src/oaklib/io/streaming_csv_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/io/streaming_fhir_writer.py` & `oaklib-0.6.5/src/oaklib/io/streaming_fhir_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/io/streaming_info_writer.py` & `oaklib-0.6.5/src/oaklib/io/streaming_info_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/io/streaming_json_lines_writer.py` & `oaklib-0.6.5/src/oaklib/io/streaming_json_lines_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/io/streaming_json_writer.py` & `oaklib-0.6.5/src/oaklib/io/streaming_json_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/io/streaming_kgcl_writer.py` & `oaklib-0.6.5/src/oaklib/io/streaming_kgcl_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/io/streaming_markdown_writer.py` & `oaklib-0.6.5/src/oaklib/io/streaming_markdown_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/io/streaming_nl_writer.py` & `oaklib-0.6.5/src/oaklib/io/streaming_nl_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/io/streaming_obo_json_writer.py` & `oaklib-0.6.5/src/oaklib/io/streaming_obo_json_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/io/streaming_obo_writer.py` & `oaklib-0.6.5/src/oaklib/io/streaming_obo_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/io/streaming_owl_functional_writer.py` & `oaklib-0.6.5/src/oaklib/io/streaming_owl_functional_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/io/streaming_rdf_writer.py` & `oaklib-0.6.5/src/oaklib/io/streaming_rdf_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/io/streaming_writer.py` & `oaklib-0.6.5/src/oaklib/io/streaming_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/io/streaming_yaml_writer.py` & `oaklib-0.6.5/src/oaklib/io/streaming_yaml_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/mappers/base_mapper.py` & `oaklib-0.6.5/src/oaklib/mappers/base_mapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/mappers/ontology_metadata_mapper.py` & `oaklib-0.6.5/src/oaklib/mappers/ontology_metadata_mapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/parsers/__init__.py` & `oaklib-0.6.5/src/oaklib/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/parsers/association_parser.py` & `oaklib-0.6.5/src/oaklib/parsers/association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/parsers/association_parser_factory.py` & `oaklib-0.6.5/src/oaklib/parsers/association_parser_factory.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/parsers/boomer_parser.py` & `oaklib-0.6.5/src/oaklib/parsers/boomer_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/parsers/gaf_association_parser.py` & `oaklib-0.6.5/src/oaklib/parsers/gaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/parsers/gencc_association_parser.py` & `oaklib-0.6.5/src/oaklib/parsers/gencc_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/parsers/hpoa_association_parser.py` & `oaklib-0.6.5/src/oaklib/parsers/hpoa_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/parsers/hpoa_g2d_association_parser.py` & `oaklib-0.6.5/src/oaklib/parsers/hpoa_g2d_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/parsers/hpoa_g2p_association_parser.py` & `oaklib-0.6.5/src/oaklib/parsers/hpoa_g2p_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/parsers/kgx_association_parser.py` & `oaklib-0.6.5/src/oaklib/parsers/kgx_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/parsers/mim2gene_association_parser.py` & `oaklib-0.6.5/src/oaklib/parsers/mim2gene_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/parsers/pairwise_association_parser.py` & `oaklib-0.6.5/src/oaklib/parsers/pairwise_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/parsers/parser_base.py` & `oaklib-0.6.5/src/oaklib/parsers/parser_base.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/parsers/phaf_association_parser.py` & `oaklib-0.6.5/src/oaklib/parsers/phaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/parsers/xaf_association_parser.py` & `oaklib-0.6.5/src/oaklib/parsers/xaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/resource.py` & `oaklib-0.6.5/src/oaklib/resource.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/selector.py` & `oaklib-0.6.5/src/oaklib/selector.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/transformers/chained_ontology_transformer.py` & `oaklib-0.6.5/src/oaklib/transformers/chained_ontology_transformer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/transformers/edge_filter_transformer.py` & `oaklib-0.6.5/src/oaklib/transformers/edge_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/transformers/graph_transformer.py` & `oaklib-0.6.5/src/oaklib/transformers/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/transformers/node_filter_transformer.py` & `oaklib-0.6.5/src/oaklib/transformers/node_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/transformers/sep_transformer.py` & `oaklib-0.6.5/src/oaklib/transformers/sep_transformer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/transformers/transformers_factory.py` & `oaklib-0.6.5/src/oaklib/transformers/transformers_factory.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/apikey_manager.py` & `oaklib-0.6.5/src/oaklib/utilities/apikey_manager.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/associations/association_differ.py` & `oaklib-0.6.5/src/oaklib/utilities/associations/association_differ.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/associations/association_index.py` & `oaklib-0.6.5/src/oaklib/utilities/associations/association_index.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/axioms/disjointness_axiom_analyzer.py` & `oaklib-0.6.5/src/oaklib/utilities/axioms/disjointness_axiom_analyzer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/axioms/logical_definition_analyzer.py` & `oaklib-0.6.5/src/oaklib/utilities/axioms/logical_definition_analyzer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/axioms/logical_definition_summarizer.py` & `oaklib-0.6.5/src/oaklib/utilities/axioms/logical_definition_summarizer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/axioms/logical_definition_utilities.py` & `oaklib-0.6.5/src/oaklib/utilities/axioms/logical_definition_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/basic_utils.py` & `oaklib-0.6.5/src/oaklib/utilities/basic_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/format_utilities.py` & `oaklib-0.6.5/src/oaklib/utilities/format_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/graph/networkx_bridge.py` & `oaklib-0.6.5/src/oaklib/utilities/graph/networkx_bridge.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/graph/relationship_walker.py` & `oaklib-0.6.5/src/oaklib/utilities/graph/relationship_walker.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/identifier_utils.py` & `oaklib-0.6.5/src/oaklib/utilities/identifier_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/iterator_utils.py` & `oaklib-0.6.5/src/oaklib/utilities/iterator_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/keyval_cache.py` & `oaklib-0.6.5/src/oaklib/utilities/keyval_cache.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/kgcl_utilities.py` & `oaklib-0.6.5/src/oaklib/utilities/kgcl_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/label_utilities.py` & `oaklib-0.6.5/src/oaklib/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/lexical/lexical_indexer.py` & `oaklib-0.6.5/src/oaklib/utilities/lexical/lexical_indexer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/lexical/patternizer.py` & `oaklib-0.6.5/src/oaklib/utilities/lexical/patternizer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/lexical/synonymizer.py` & `oaklib-0.6.5/src/oaklib/utilities/lexical/synonymizer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/mapping/boomer_utils.py` & `oaklib-0.6.5/src/oaklib/utilities/mapping/boomer_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/mapping/cross_ontology_diffs.py` & `oaklib-0.6.5/src/oaklib/utilities/mapping/cross_ontology_diffs.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/mapping/mapping_propagator.py` & `oaklib-0.6.5/src/oaklib/utilities/mapping/mapping_propagator.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/mapping/mapping_validation.py` & `oaklib-0.6.5/src/oaklib/utilities/mapping/mapping_validation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/mapping/sssom_utils.py` & `oaklib-0.6.5/src/oaklib/utilities/mapping/sssom_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/ner_utilities.py` & `oaklib-0.6.5/src/oaklib/utilities/ner_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/nlp/natual_language_generation.py` & `oaklib-0.6.5/src/oaklib/utilities/nlp/natual_language_generation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/obograph_utils.py` & `oaklib-0.6.5/src/oaklib/utilities/obograph_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/ontology_builder.py` & `oaklib-0.6.5/src/oaklib/utilities/ontology_builder.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/publication_utils/doi_wrapper.py` & `oaklib-0.6.5/src/oaklib/utilities/publication_utils/doi_wrapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/publication_utils/pubdb_wrapper.py` & `oaklib-0.6.5/src/oaklib/utilities/publication_utils/pubdb_wrapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/publication_utils/pubmed_wrapper.py` & `oaklib-0.6.5/src/oaklib/utilities/publication_utils/pubmed_wrapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/reasoning/relation_graph.py` & `oaklib-0.6.5/src/oaklib/utilities/reasoning/relation_graph.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/semsim/similarity_utils.py` & `oaklib-0.6.5/src/oaklib/utilities/semsim/similarity_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/stats/hypergeometric.py` & `oaklib-0.6.5/src/oaklib/utilities/stats/hypergeometric.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/subsets/slimmer_utils.py` & `oaklib-0.6.5/src/oaklib/utilities/subsets/slimmer_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/subsets/subset_analysis.py` & `oaklib-0.6.5/src/oaklib/utilities/subsets/subset_analysis.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/subsets/value_set_expander.py` & `oaklib-0.6.5/src/oaklib/utilities/subsets/value_set_expander.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/table_filler.py` & `oaklib-0.6.5/src/oaklib/utilities/table_filler.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/taxon/taxon_constraint_utils.py` & `oaklib-0.6.5/src/oaklib/utilities/taxon/taxon_constraint_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/validation/definition_ontology_rule.py` & `oaklib-0.6.5/src/oaklib/utilities/validation/definition_ontology_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/validation/disjointness_rule.py` & `oaklib-0.6.5/src/oaklib/utilities/validation/disjointness_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/validation/lint_utils.py` & `oaklib-0.6.5/src/oaklib/utilities/validation/lint_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/validation/ontology_rule.py` & `oaklib-0.6.5/src/oaklib/utilities/validation/ontology_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/validation/rule_runner.py` & `oaklib-0.6.5/src/oaklib/utilities/validation/rule_runner.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/src/oaklib/utilities/writers/change_handler.py` & `oaklib-0.6.5/src/oaklib/utilities/writers/change_handler.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.4/PKG-INFO` & `oaklib-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oaklib
-Version: 0.6.4
+Version: 0.6.5
 Summary: Ontology Access Kit: Python library for common ontology operations over a variety of backends
 Author: cmungall
 Author-email: cjm@berkeleybop.org
 Requires-Python: >=3.9,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -19,14 +19,15 @@
 Requires-Dist: SQLAlchemy (>=1.4.32)
 Requires-Dist: aiohttp ; extra == "llm"
 Requires-Dist: airium (>=0.2.5)
 Requires-Dist: appdirs (>=1.4.4)
 Requires-Dist: class-resolver (>=0.4.2)
 Requires-Dist: click
 Requires-Dist: curies (>=0.6.6)
+Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: eutils (>=0.6.0)
 Requires-Dist: funowl (>=0.2.0)
 Requires-Dist: gilda (>=1.0.0) ; extra == "gilda"
 Requires-Dist: html2text ; extra == "llm"
 Requires-Dist: jsonlines (>=4.0.0,<5.0.0)
 Requires-Dist: kgcl-rdflib (==0.5.0)
 Requires-Dist: kgcl-schema (>=0.6.8,<0.7.0)
```

