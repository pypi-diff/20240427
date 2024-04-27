# Comparing `tmp/sim_rl-0.1.1.tar.gz` & `tmp/sim_rl-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sim_rl-0.1.1.tar", max compression
+gzip compressed data, was "sim_rl-0.1.2.tar", max compression
```

## Comparing `sim_rl-0.1.1.tar` & `sim_rl-0.1.2.tar`

### file list

```diff
@@ -1,139 +1,139 @@
--rw-r--r--   0        0        0      677 2024-04-27 12:30:21.128796 sim_rl-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    14269 2024-04-27 12:31:19.211387 sim_rl-0.1.1/README.md
--rw-r--r--   0        0        0     1467 2024-04-27 11:42:55.671351 sim_rl-0.1.1/sim_rl/.gitlab-ci.yml
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.672858 sim_rl-0.1.1/sim_rl/__init__.py
--rw-r--r--   0        0        0        6 2024-04-27 11:42:55.675004 sim_rl-0.1.1/sim_rl/agents/__init__.py
--rw-r--r--   0        0        0      161 2024-04-27 11:42:55.676011 sim_rl-0.1.1/sim_rl/agents/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3003 2024-04-27 11:42:55.677012 sim_rl-0.1.1/sim_rl/agents/buffer.py
--rw-r--r--   0        0        0    18118 2024-04-27 11:42:55.677012 sim_rl-0.1.1/sim_rl/agents/ddpg_agent.py
--rw-r--r--   0        0        0     9927 2024-04-27 11:42:55.678375 sim_rl-0.1.1/sim_rl/agents/model.py
--rw-r--r--   0        0        0   282094 2024-04-27 11:42:55.681384 sim_rl-0.1.1/sim_rl/agents/trained_agent.pt
--rw-r--r--   0        0        0   624642 2024-04-27 11:42:55.685384 sim_rl-0.1.1/sim_rl/agents/trained_ddpg_agent.pt
--rw-r--r--   0        0        0     1384 2024-04-27 11:42:55.686564 sim_rl-0.1.1/sim_rl/debug.py
--rw-r--r--   0        0        0       62 2024-04-27 12:07:17.748752 sim_rl-0.1.1/sim_rl/dist/sim_rl-0.1.0.tar.gz
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.687574 sim_rl-0.1.1/sim_rl/evaluation/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.688573 sim_rl-0.1.1/sim_rl/evaluation/convergence_evaluation/__init__.py
--rw-r--r--   0        0        0    12173 2024-04-27 11:42:55.689573 sim_rl-0.1.1/sim_rl/evaluation/convergence_evaluation/convergence_evaluation.py
--rw-r--r--   0        0        0   558104 2024-04-27 11:42:55.693572 sim_rl-0.1.1/sim_rl/evaluation/convergence_evaluation/reward_plot.png
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.694572 sim_rl-0.1.1/sim_rl/evaluation/decision_evaluation/__init__.py
--rw-r--r--   0        0        0     9735 2024-04-27 11:42:55.695572 sim_rl-0.1.1/sim_rl/evaluation/decision_evaluation/decision_evaluation.py
--rw-r--r--   0        0        0    29925 2024-04-27 11:42:55.697015 sim_rl-0.1.1/sim_rl/evaluation/decision_evaluation/output_plots/Transition_Proba_BeforeAfter_Blockage.png
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.698038 sim_rl-0.1.1/sim_rl/evaluation/noise_evaluation/__init__.py
--rw-r--r--   0        0        0     6478 2024-04-27 11:42:55.699055 sim_rl-0.1.1/sim_rl/evaluation/noise_evaluation/noise_evaluation.py
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.700040 sim_rl-0.1.1/sim_rl/evaluation/robustness_evaluation/__init__.py
--rw-r--r--   0        0        0     5068 2024-04-27 11:42:55.701036 sim_rl-0.1.1/sim_rl/evaluation/robustness_evaluation/robustness_evaluation.py
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.702037 sim_rl-0.1.1/sim_rl/evaluation/startup_evaluation/.gitkeep
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.703037 sim_rl-0.1.1/sim_rl/evaluation/startup_evaluation/__init__.py
--rw-r--r--   0        0        0    48479 2024-04-27 11:42:55.704037 sim_rl-0.1.1/sim_rl/evaluation/startup_evaluation/reward_plot.png
--rw-r--r--   0        0        0    49799 2024-04-27 11:42:55.705037 sim_rl-0.1.1/sim_rl/evaluation/startup_evaluation/reward_plot_0.png
--rw-r--r--   0        0        0    54169 2024-04-27 11:42:55.706037 sim_rl-0.1.1/sim_rl/evaluation/startup_evaluation/reward_plot_1.png
--rw-r--r--   0        0        0    38931 2024-04-27 11:42:55.707038 sim_rl-0.1.1/sim_rl/evaluation/startup_evaluation/reward_plot_2.png
--rw-r--r--   0        0        0    39307 2024-04-27 11:42:55.708042 sim_rl-0.1.1/sim_rl/evaluation/startup_evaluation/reward_plot_3.png
--rw-r--r--   0        0        0    10907 2024-04-27 11:42:55.709654 sim_rl-0.1.1/sim_rl/evaluation/startup_evaluation/startup_evaluation.py
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.709654 sim_rl-0.1.1/sim_rl/foundations/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.710662 sim_rl-0.1.1/sim_rl/foundations/breakdown_exploration/__init__.py
--rw-r--r--   0        0        0    33462 2024-04-27 11:42:55.711724 sim_rl-0.1.1/sim_rl/foundations/breakdown_exploration/__pycache__/state_exploration.cpython-311.pyc
--rw-r--r--   0        0        0    14679 2024-04-27 11:42:55.712736 sim_rl-0.1.1/sim_rl/foundations/breakdown_exploration/breakdown_exploration.py
--rw-r--r--   0        0        0      869 2024-04-27 11:42:55.714919 sim_rl-0.1.1/sim_rl/foundations/breakdown_exploration/output_data/all_breakdown_cases.json
--rw-r--r--   0        0        0       26 2024-04-27 11:42:55.715927 sim_rl-0.1.1/sim_rl/foundations/breakdown_exploration/output_data/coverage_metric/coverage.json
--rw-r--r--   0        0        0      205 2024-04-27 11:42:55.716928 sim_rl-0.1.1/sim_rl/foundations/breakdown_exploration/output_data/key_states/key_states.json
--rw-r--r--   0        0        0    17946 2024-04-27 11:42:55.717927 sim_rl-0.1.1/sim_rl/foundations/breakdown_exploration/output_data/key_states/rewards.png
--rw-r--r--   0        0        0       64 2024-04-27 11:42:55.718928 sim_rl-0.1.1/sim_rl/foundations/breakdown_exploration/output_data/peripheral_states/peripheral_states.json
--rw-r--r--   0        0        0    22059 2024-04-27 11:42:55.719926 sim_rl-0.1.1/sim_rl/foundations/breakdown_exploration/output_data/peripheral_states/visits.png
--rw-r--r--   0        0        0    46849 2024-04-27 11:42:55.720926 sim_rl-0.1.1/sim_rl/foundations/core_functions.py
--rw-r--r--   0        0        0    11311 2024-04-27 11:42:55.721927 sim_rl-0.1.1/sim_rl/foundations/core_plotting.py
--rw-r--r--   0        0        0    12662 2024-04-27 11:42:55.722926 sim_rl-0.1.1/sim_rl/foundations/output_csv/action_dict.csv
--rw-r--r--   0        0        0     1951 2024-04-27 11:42:55.723926 sim_rl-0.1.1/sim_rl/foundations/output_csv/actor_loss.csv
--rw-r--r--   0        0        0     1948 2024-04-27 11:42:55.725927 sim_rl-0.1.1/sim_rl/foundations/output_csv/critic_loss.csv
--rw-r--r--   0        0        0    19169 2024-04-27 11:42:55.726927 sim_rl-0.1.1/sim_rl/foundations/output_csv/next_state_model_loss.csv
--rw-r--r--   0        0        0     1073 2024-04-27 11:42:55.727926 sim_rl-0.1.1/sim_rl/foundations/output_csv/reward_dict.json
--rw-r--r--   0        0        0    20252 2024-04-27 11:42:55.727926 sim_rl-0.1.1/sim_rl/foundations/output_csv/reward_model_loss.csv
--rw-r--r--   0        0        0     1005 2024-04-27 11:42:55.728926 sim_rl-0.1.1/sim_rl/foundations/output_csv/transition_proba.csv
--rw-r--r--   0        0        0     2088 2024-04-27 11:42:55.729926 sim_rl-0.1.1/sim_rl/main.py
--rw-r--r--   0        0        0       77 2024-04-27 11:42:55.671351 sim_rl-0.1.1/sim_rl/Makefile
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.733136 sim_rl-0.1.1/sim_rl/queue_env/__init__.py
--rw-r--r--   0        0        0    12532 2024-04-27 11:42:55.734146 sim_rl-0.1.1/sim_rl/queue_env/queue_base_functions.py
--rw-r--r--   0        0        0      664 2024-04-27 11:42:55.735144 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/.github/workflows/auto-tagging.yml
--rw-r--r--   0        0        0     1679 2024-04-27 11:42:55.736269 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0      815 2024-04-27 11:42:55.737339 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/.gitignore
--rw-r--r--   0        0        0      649 2024-04-27 11:42:55.737339 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/.readthedocs.yml
--rw-r--r--   0        0        0     6292 2024-04-27 11:42:55.738409 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/CHANGELOG.md
--rw-r--r--   0        0        0      372 2024-04-27 11:42:55.739417 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/CITATION.cff
--rw-r--r--   0        0        0     2649 2024-04-27 11:42:55.742416 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/cliff.toml
--rw-r--r--   0        0        0   125538 2024-04-27 11:42:55.744416 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/_static/bootstrap-lumen.min.css
--rw-r--r--   0        0        0     3089 2024-04-27 11:42:55.745416 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/_static/copybutton.js
--rw-r--r--   0        0        0     1324 2024-04-27 11:42:55.746416 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/_static/customized_alabaster.css
--rw-r--r--   0        0        0    89478 2024-04-27 11:42:55.747746 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/_static/jquery.min.js
--rw-r--r--   0        0        0    11713 2024-04-27 11:42:55.748757 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/_static/qt_sphinx13.css
--rw-r--r--   0        0        0      157 2024-04-27 11:42:55.749759 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/_templates/layout.html
--rw-r--r--   0        0        0      593 2024-04-27 11:42:55.749759 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/_templates/opensearch.xml
--rw-r--r--   0        0        0     2163 2024-04-27 11:42:55.751041 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/_templates/search.html
--rw-r--r--   0        0        0      887 2024-04-27 11:42:55.752048 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/_templates/searchbox.html
--rw-r--r--   0        0        0     1234 2024-04-27 11:42:55.753050 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/_templates/searchresults.html
--rw-r--r--   0        0        0    11845 2024-04-27 11:42:55.754047 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/_themes/qt_sphinx13/layout.html
--rw-r--r--   0        0        0       81 2024-04-27 11:42:55.755049 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/_themes/qt_sphinx13/theme.conf
--rw-r--r--   0        0        0     8874 2024-04-27 11:42:55.756048 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/conf.py
--rw-r--r--   0        0        0    88538 2024-04-27 11:42:55.757048 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/current_state.png
--rw-r--r--   0        0        0   112321 2024-04-27 11:42:55.759055 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/current_state1.png
--rw-r--r--   0        0        0    87573 2024-04-27 11:42:55.760056 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/edge_type_2-1.png
--rw-r--r--   0        0        0    62803 2024-04-27 11:42:55.761054 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/edge_type_2.png
--rw-r--r--   0        0        0    69615 2024-04-27 11:42:55.763054 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/fig.png
--rw-r--r--   0        0        0      687 2024-04-27 11:42:55.763054 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/graph.rst
--rw-r--r--   0        0        0     1243 2024-04-27 11:42:55.764054 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/index.rst
--rw-r--r--   0        0        0      810 2024-04-27 11:42:55.765054 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/installation.rst
--rwxr-xr-x   0        0        0     6717 2024-04-27 11:42:55.765054 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/make.bat
--rw-r--r--   0        0        0     6961 2024-04-27 11:42:55.743416 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/Makefile
--rw-r--r--   0        0        0      270 2024-04-27 11:42:55.766429 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/modules.rst
--rw-r--r--   0        0        0    55346 2024-04-27 11:42:55.767965 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/my_network.png
--rw-r--r--   0        0        0    44926 2024-04-27 11:42:55.768972 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/my_network1.png
--rw-r--r--   0        0        0     1103 2024-04-27 11:42:55.768972 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/network.rst
--rw-r--r--   0        0        0    10454 2024-04-27 11:42:55.769972 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/overview.rst
--rw-r--r--   0        0        0     1169 2024-04-27 11:42:55.770971 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/queues.rst
--rw-r--r--   0        0        0       83 2024-04-27 11:42:55.770971 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/requirements.txt
--rw-r--r--   0        0        0    18131 2024-04-27 11:42:55.772477 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/sim.png
--rw-r--r--   0        0        0    38707 2024-04-27 11:42:55.773485 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/sim1.png
--rw-r--r--   0        0        0    13470 2024-04-27 11:42:55.773485 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/store.png
--rw-r--r--   0        0        0    26680 2024-04-27 11:42:55.775484 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/store1.png
--rw-r--r--   0        0        0     2656 2024-04-27 11:42:55.776484 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/examples/example_grocery_store.py
--rw-r--r--   0        0        0     1106 2024-04-27 11:42:55.740418 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/LICENSE.txt
--rw-r--r--   0        0        0      428 2024-04-27 11:42:55.741417 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/MANIFEST.in
--rw-r--r--   0        0        0   120400 2024-04-27 11:42:55.778484 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/poetry.lock
--rw-r--r--   0        0        0     2745 2024-04-27 11:42:55.779484 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/pyproject.toml
--rw-r--r--   0        0        0      635 2024-04-27 11:42:55.779484 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/__init__.py
--rw-r--r--   0        0        0     1072 2024-04-27 11:42:55.781484 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/graph/__init__.py
--rw-r--r--   0        0        0      948 2024-04-27 11:42:55.782484 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/graph/_pairwise.pyx
--rw-r--r--   0        0        0     2735 2024-04-27 11:42:55.782484 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_functions.py
--rw-r--r--   0        0        0    15023 2024-04-27 11:42:55.783484 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_generation.py
--rw-r--r--   0        0        0     5891 2024-04-27 11:42:55.784485 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_preparation.py
--rw-r--r--   0        0        0    17236 2024-04-27 11:42:55.785484 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_wrapper.py
--rw-r--r--   0        0        0      803 2024-04-27 11:42:55.786484 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/network/__init__.py
--rw-r--r--   0        0        0   954119 2024-04-27 11:42:55.790484 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/network/priority_queue.c
--rw-r--r--   0        0        0     5510 2024-04-27 11:42:55.792486 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/network/priority_queue.pyx
--rw-r--r--   0        0        0    75433 2024-04-27 11:42:55.793484 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/network/queue_network.py
--rw-r--r--   0        0        0      762 2024-04-27 11:42:55.794484 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/queues/__init__.py
--rw-r--r--   0        0        0     6627 2024-04-27 11:42:55.795484 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/queues/agents.py
--rw-r--r--   0        0        0   842825 2024-04-27 11:42:55.799488 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/queues/choice.c
--rw-r--r--   0        0        0      782 2024-04-27 11:42:55.800484 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/queues/choice.pyx
--rw-r--r--   0        0        0    14354 2024-04-27 11:42:55.800484 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/queues/queue_extentions.py
--rw-r--r--   0        0        0    36417 2024-04-27 11:42:55.802024 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/queues/queue_servers.py
--rw-r--r--   0        0        0     2817 2024-04-27 11:42:55.803042 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/union_find.py
--rw-r--r--   0        0        0     3711 2024-04-27 11:42:55.741417 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/README.rst
--rw-r--r--   0        0        0      359 2024-04-27 11:42:55.804076 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/setup.py
--rw-r--r--   0        0        0    44062 2024-04-27 11:42:55.805768 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/tests/img/test-mpl-1.x.png
--rw-r--r--   0        0        0    65478 2024-04-27 11:42:55.806775 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/tests/img/test-mpl-2.x.png
--rw-r--r--   0        0        0     3963 2024-04-27 11:42:55.807776 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/tests/test_graph_generation.py
--rw-r--r--   0        0        0    18195 2024-04-27 11:42:55.807776 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/tests/test_network.py
--rw-r--r--   0        0        0     2568 2024-04-27 11:42:55.809272 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/tests/test_qndigraph.py
--rw-r--r--   0        0        0    12268 2024-04-27 11:42:55.810280 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/tests/test_queue_server.py
--rw-r--r--   0        0        0     6394 2024-04-27 11:42:55.811282 sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/tests/test_statistical_properties.py
--rw-r--r--   0        0        0     5661 2024-04-27 11:42:55.812279 sim_rl-0.1.1/sim_rl/queue_env/queueing_network.py
--rw-r--r--   0        0        0       77 2024-04-27 11:42:55.813279 sim_rl-0.1.1/sim_rl/requirements.txt
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.814279 sim_rl-0.1.1/sim_rl/rl_env/__init__.py
--rw-r--r--   0        0        0    16574 2024-04-27 11:42:55.814279 sim_rl-0.1.1/sim_rl/rl_env/RL_Environment.py
--rw-r--r--   0        0        0        0 2024-04-27 11:42:55.835064 sim_rl-0.1.1/sim_rl/tuning/__init__.py
--rw-r--r--   0        0        0     9149 2024-04-27 11:42:55.836058 sim_rl-0.1.1/sim_rl/tuning/ray_tuning.py
--rw-r--r--   0        0        0     8381 2024-04-27 11:42:55.837057 sim_rl-0.1.1/sim_rl/tuning/wandb_tuning.py
--rw-r--r--   0        0        0      894 2024-04-27 11:42:55.838059 sim_rl-0.1.1/sim_rl/user_config/configuration.yml
--rw-r--r--   0        0        0      923 2024-04-27 11:42:55.839058 sim_rl-0.1.1/sim_rl/user_config/eval_hyperparams.yml
--rw-r--r--   0        0        0      482 2024-04-27 11:42:55.840057 sim_rl-0.1.1/sim_rl/user_config/tuning_hyperparams.yml
--rw-r--r--   0        0        0    14567 1970-01-01 00:00:00.000000 sim_rl-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      677 2024-04-27 14:03:11.167080 sim_rl-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    14709 2024-04-27 14:02:49.017380 sim_rl-0.1.2/README.md
+-rw-r--r--   0        0        0     1467 2024-04-27 11:42:55.671351 sim_rl-0.1.2/sim_rl/.gitlab-ci.yml
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.672858 sim_rl-0.1.2/sim_rl/__init__.py
+-rw-r--r--   0        0        0        6 2024-04-27 11:42:55.675004 sim_rl-0.1.2/sim_rl/agents/__init__.py
+-rw-r--r--   0        0        0      161 2024-04-27 11:42:55.676011 sim_rl-0.1.2/sim_rl/agents/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3003 2024-04-27 11:42:55.677012 sim_rl-0.1.2/sim_rl/agents/buffer.py
+-rw-r--r--   0        0        0    18118 2024-04-27 11:42:55.677012 sim_rl-0.1.2/sim_rl/agents/ddpg_agent.py
+-rw-r--r--   0        0        0     9927 2024-04-27 11:42:55.678375 sim_rl-0.1.2/sim_rl/agents/model.py
+-rw-r--r--   0        0        0   282094 2024-04-27 11:42:55.681384 sim_rl-0.1.2/sim_rl/agents/trained_agent.pt
+-rw-r--r--   0        0        0   624642 2024-04-27 11:42:55.685384 sim_rl-0.1.2/sim_rl/agents/trained_ddpg_agent.pt
+-rw-r--r--   0        0        0     1384 2024-04-27 11:42:55.686564 sim_rl-0.1.2/sim_rl/debug.py
+-rw-r--r--   0        0        0       62 2024-04-27 12:07:17.748752 sim_rl-0.1.2/sim_rl/dist/sim_rl-0.1.0.tar.gz
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.687574 sim_rl-0.1.2/sim_rl/evaluation/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.688573 sim_rl-0.1.2/sim_rl/evaluation/convergence_evaluation/__init__.py
+-rw-r--r--   0        0        0    12173 2024-04-27 11:42:55.689573 sim_rl-0.1.2/sim_rl/evaluation/convergence_evaluation/convergence_evaluation.py
+-rw-r--r--   0        0        0   558104 2024-04-27 11:42:55.693572 sim_rl-0.1.2/sim_rl/evaluation/convergence_evaluation/reward_plot.png
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.694572 sim_rl-0.1.2/sim_rl/evaluation/decision_evaluation/__init__.py
+-rw-r--r--   0        0        0     9735 2024-04-27 11:42:55.695572 sim_rl-0.1.2/sim_rl/evaluation/decision_evaluation/decision_evaluation.py
+-rw-r--r--   0        0        0    29925 2024-04-27 11:42:55.697015 sim_rl-0.1.2/sim_rl/evaluation/decision_evaluation/output_plots/Transition_Proba_BeforeAfter_Blockage.png
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.698038 sim_rl-0.1.2/sim_rl/evaluation/noise_evaluation/__init__.py
+-rw-r--r--   0        0        0     6478 2024-04-27 11:42:55.699055 sim_rl-0.1.2/sim_rl/evaluation/noise_evaluation/noise_evaluation.py
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.700040 sim_rl-0.1.2/sim_rl/evaluation/robustness_evaluation/__init__.py
+-rw-r--r--   0        0        0     5068 2024-04-27 11:42:55.701036 sim_rl-0.1.2/sim_rl/evaluation/robustness_evaluation/robustness_evaluation.py
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.702037 sim_rl-0.1.2/sim_rl/evaluation/startup_evaluation/.gitkeep
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.703037 sim_rl-0.1.2/sim_rl/evaluation/startup_evaluation/__init__.py
+-rw-r--r--   0        0        0    48479 2024-04-27 11:42:55.704037 sim_rl-0.1.2/sim_rl/evaluation/startup_evaluation/reward_plot.png
+-rw-r--r--   0        0        0    49799 2024-04-27 11:42:55.705037 sim_rl-0.1.2/sim_rl/evaluation/startup_evaluation/reward_plot_0.png
+-rw-r--r--   0        0        0    54169 2024-04-27 11:42:55.706037 sim_rl-0.1.2/sim_rl/evaluation/startup_evaluation/reward_plot_1.png
+-rw-r--r--   0        0        0    38931 2024-04-27 11:42:55.707038 sim_rl-0.1.2/sim_rl/evaluation/startup_evaluation/reward_plot_2.png
+-rw-r--r--   0        0        0    39307 2024-04-27 11:42:55.708042 sim_rl-0.1.2/sim_rl/evaluation/startup_evaluation/reward_plot_3.png
+-rw-r--r--   0        0        0    10907 2024-04-27 11:42:55.709654 sim_rl-0.1.2/sim_rl/evaluation/startup_evaluation/startup_evaluation.py
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.709654 sim_rl-0.1.2/sim_rl/foundations/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.710662 sim_rl-0.1.2/sim_rl/foundations/breakdown_exploration/__init__.py
+-rw-r--r--   0        0        0    33462 2024-04-27 11:42:55.711724 sim_rl-0.1.2/sim_rl/foundations/breakdown_exploration/__pycache__/state_exploration.cpython-311.pyc
+-rw-r--r--   0        0        0    14679 2024-04-27 11:42:55.712736 sim_rl-0.1.2/sim_rl/foundations/breakdown_exploration/breakdown_exploration.py
+-rw-r--r--   0        0        0      869 2024-04-27 11:42:55.714919 sim_rl-0.1.2/sim_rl/foundations/breakdown_exploration/output_data/all_breakdown_cases.json
+-rw-r--r--   0        0        0       26 2024-04-27 11:42:55.715927 sim_rl-0.1.2/sim_rl/foundations/breakdown_exploration/output_data/coverage_metric/coverage.json
+-rw-r--r--   0        0        0      205 2024-04-27 11:42:55.716928 sim_rl-0.1.2/sim_rl/foundations/breakdown_exploration/output_data/key_states/key_states.json
+-rw-r--r--   0        0        0    17946 2024-04-27 11:42:55.717927 sim_rl-0.1.2/sim_rl/foundations/breakdown_exploration/output_data/key_states/rewards.png
+-rw-r--r--   0        0        0       64 2024-04-27 11:42:55.718928 sim_rl-0.1.2/sim_rl/foundations/breakdown_exploration/output_data/peripheral_states/peripheral_states.json
+-rw-r--r--   0        0        0    22059 2024-04-27 11:42:55.719926 sim_rl-0.1.2/sim_rl/foundations/breakdown_exploration/output_data/peripheral_states/visits.png
+-rw-r--r--   0        0        0    46849 2024-04-27 11:42:55.720926 sim_rl-0.1.2/sim_rl/foundations/core_functions.py
+-rw-r--r--   0        0        0    11311 2024-04-27 11:42:55.721927 sim_rl-0.1.2/sim_rl/foundations/core_plotting.py
+-rw-r--r--   0        0        0    12662 2024-04-27 11:42:55.722926 sim_rl-0.1.2/sim_rl/foundations/output_csv/action_dict.csv
+-rw-r--r--   0        0        0     1951 2024-04-27 11:42:55.723926 sim_rl-0.1.2/sim_rl/foundations/output_csv/actor_loss.csv
+-rw-r--r--   0        0        0     1948 2024-04-27 11:42:55.725927 sim_rl-0.1.2/sim_rl/foundations/output_csv/critic_loss.csv
+-rw-r--r--   0        0        0    19169 2024-04-27 11:42:55.726927 sim_rl-0.1.2/sim_rl/foundations/output_csv/next_state_model_loss.csv
+-rw-r--r--   0        0        0     1073 2024-04-27 11:42:55.727926 sim_rl-0.1.2/sim_rl/foundations/output_csv/reward_dict.json
+-rw-r--r--   0        0        0    20252 2024-04-27 11:42:55.727926 sim_rl-0.1.2/sim_rl/foundations/output_csv/reward_model_loss.csv
+-rw-r--r--   0        0        0     1005 2024-04-27 11:42:55.728926 sim_rl-0.1.2/sim_rl/foundations/output_csv/transition_proba.csv
+-rw-r--r--   0        0        0     2088 2024-04-27 11:42:55.729926 sim_rl-0.1.2/sim_rl/main.py
+-rw-r--r--   0        0        0       77 2024-04-27 11:42:55.671351 sim_rl-0.1.2/sim_rl/Makefile
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.733136 sim_rl-0.1.2/sim_rl/queue_env/__init__.py
+-rw-r--r--   0        0        0    12532 2024-04-27 11:42:55.734146 sim_rl-0.1.2/sim_rl/queue_env/queue_base_functions.py
+-rw-r--r--   0        0        0      664 2024-04-27 11:42:55.735144 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/.github/workflows/auto-tagging.yml
+-rw-r--r--   0        0        0     1679 2024-04-27 11:42:55.736269 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0      815 2024-04-27 11:42:55.737339 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/.gitignore
+-rw-r--r--   0        0        0      649 2024-04-27 11:42:55.737339 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/.readthedocs.yml
+-rw-r--r--   0        0        0     6292 2024-04-27 11:42:55.738409 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/CHANGELOG.md
+-rw-r--r--   0        0        0      372 2024-04-27 11:42:55.739417 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/CITATION.cff
+-rw-r--r--   0        0        0     2649 2024-04-27 11:42:55.742416 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/cliff.toml
+-rw-r--r--   0        0        0   125538 2024-04-27 11:42:55.744416 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/_static/bootstrap-lumen.min.css
+-rw-r--r--   0        0        0     3089 2024-04-27 11:42:55.745416 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/_static/copybutton.js
+-rw-r--r--   0        0        0     1324 2024-04-27 11:42:55.746416 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/_static/customized_alabaster.css
+-rw-r--r--   0        0        0    89478 2024-04-27 11:42:55.747746 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/_static/jquery.min.js
+-rw-r--r--   0        0        0    11713 2024-04-27 11:42:55.748757 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/_static/qt_sphinx13.css
+-rw-r--r--   0        0        0      157 2024-04-27 11:42:55.749759 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/_templates/layout.html
+-rw-r--r--   0        0        0      593 2024-04-27 11:42:55.749759 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/_templates/opensearch.xml
+-rw-r--r--   0        0        0     2163 2024-04-27 11:42:55.751041 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/_templates/search.html
+-rw-r--r--   0        0        0      887 2024-04-27 11:42:55.752048 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/_templates/searchbox.html
+-rw-r--r--   0        0        0     1234 2024-04-27 11:42:55.753050 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/_templates/searchresults.html
+-rw-r--r--   0        0        0    11845 2024-04-27 11:42:55.754047 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/_themes/qt_sphinx13/layout.html
+-rw-r--r--   0        0        0       81 2024-04-27 11:42:55.755049 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/_themes/qt_sphinx13/theme.conf
+-rw-r--r--   0        0        0     8874 2024-04-27 11:42:55.756048 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/conf.py
+-rw-r--r--   0        0        0    88538 2024-04-27 11:42:55.757048 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/current_state.png
+-rw-r--r--   0        0        0   112321 2024-04-27 11:42:55.759055 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/current_state1.png
+-rw-r--r--   0        0        0    87573 2024-04-27 11:42:55.760056 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/edge_type_2-1.png
+-rw-r--r--   0        0        0    62803 2024-04-27 11:42:55.761054 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/edge_type_2.png
+-rw-r--r--   0        0        0    69615 2024-04-27 11:42:55.763054 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/fig.png
+-rw-r--r--   0        0        0      687 2024-04-27 11:42:55.763054 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/graph.rst
+-rw-r--r--   0        0        0     1243 2024-04-27 11:42:55.764054 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/index.rst
+-rw-r--r--   0        0        0      810 2024-04-27 11:42:55.765054 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/installation.rst
+-rwxr-xr-x   0        0        0     6717 2024-04-27 11:42:55.765054 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/make.bat
+-rw-r--r--   0        0        0     6961 2024-04-27 11:42:55.743416 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/Makefile
+-rw-r--r--   0        0        0      270 2024-04-27 11:42:55.766429 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/modules.rst
+-rw-r--r--   0        0        0    55346 2024-04-27 11:42:55.767965 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/my_network.png
+-rw-r--r--   0        0        0    44926 2024-04-27 11:42:55.768972 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/my_network1.png
+-rw-r--r--   0        0        0     1103 2024-04-27 11:42:55.768972 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/network.rst
+-rw-r--r--   0        0        0    10454 2024-04-27 11:42:55.769972 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/overview.rst
+-rw-r--r--   0        0        0     1169 2024-04-27 11:42:55.770971 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/queues.rst
+-rw-r--r--   0        0        0       83 2024-04-27 11:42:55.770971 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/requirements.txt
+-rw-r--r--   0        0        0    18131 2024-04-27 11:42:55.772477 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/sim.png
+-rw-r--r--   0        0        0    38707 2024-04-27 11:42:55.773485 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/sim1.png
+-rw-r--r--   0        0        0    13470 2024-04-27 11:42:55.773485 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/store.png
+-rw-r--r--   0        0        0    26680 2024-04-27 11:42:55.775484 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/store1.png
+-rw-r--r--   0        0        0     2656 2024-04-27 11:42:55.776484 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/examples/example_grocery_store.py
+-rw-r--r--   0        0        0     1106 2024-04-27 11:42:55.740418 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/LICENSE.txt
+-rw-r--r--   0        0        0      428 2024-04-27 11:42:55.741417 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/MANIFEST.in
+-rw-r--r--   0        0        0   120400 2024-04-27 11:42:55.778484 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/poetry.lock
+-rw-r--r--   0        0        0     2745 2024-04-27 11:42:55.779484 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/pyproject.toml
+-rw-r--r--   0        0        0      635 2024-04-27 11:42:55.779484 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/__init__.py
+-rw-r--r--   0        0        0     1072 2024-04-27 11:42:55.781484 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/graph/__init__.py
+-rw-r--r--   0        0        0      948 2024-04-27 11:42:55.782484 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/graph/_pairwise.pyx
+-rw-r--r--   0        0        0     2735 2024-04-27 11:42:55.782484 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_functions.py
+-rw-r--r--   0        0        0    15023 2024-04-27 11:42:55.783484 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_generation.py
+-rw-r--r--   0        0        0     5891 2024-04-27 11:42:55.784485 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_preparation.py
+-rw-r--r--   0        0        0    17236 2024-04-27 11:42:55.785484 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_wrapper.py
+-rw-r--r--   0        0        0      803 2024-04-27 11:42:55.786484 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/network/__init__.py
+-rw-r--r--   0        0        0   954119 2024-04-27 11:42:55.790484 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/network/priority_queue.c
+-rw-r--r--   0        0        0     5510 2024-04-27 11:42:55.792486 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/network/priority_queue.pyx
+-rw-r--r--   0        0        0    75433 2024-04-27 11:42:55.793484 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/network/queue_network.py
+-rw-r--r--   0        0        0      762 2024-04-27 11:42:55.794484 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/queues/__init__.py
+-rw-r--r--   0        0        0     6627 2024-04-27 11:42:55.795484 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/queues/agents.py
+-rw-r--r--   0        0        0   842825 2024-04-27 11:42:55.799488 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/queues/choice.c
+-rw-r--r--   0        0        0      782 2024-04-27 11:42:55.800484 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/queues/choice.pyx
+-rw-r--r--   0        0        0    14354 2024-04-27 11:42:55.800484 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/queues/queue_extentions.py
+-rw-r--r--   0        0        0    36417 2024-04-27 11:42:55.802024 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/queues/queue_servers.py
+-rw-r--r--   0        0        0     2817 2024-04-27 11:42:55.803042 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/union_find.py
+-rw-r--r--   0        0        0     3711 2024-04-27 11:42:55.741417 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/README.rst
+-rw-r--r--   0        0        0      359 2024-04-27 11:42:55.804076 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/setup.py
+-rw-r--r--   0        0        0    44062 2024-04-27 11:42:55.805768 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/tests/img/test-mpl-1.x.png
+-rw-r--r--   0        0        0    65478 2024-04-27 11:42:55.806775 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/tests/img/test-mpl-2.x.png
+-rw-r--r--   0        0        0     3963 2024-04-27 11:42:55.807776 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/tests/test_graph_generation.py
+-rw-r--r--   0        0        0    18195 2024-04-27 11:42:55.807776 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/tests/test_network.py
+-rw-r--r--   0        0        0     2568 2024-04-27 11:42:55.809272 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/tests/test_qndigraph.py
+-rw-r--r--   0        0        0    12268 2024-04-27 11:42:55.810280 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/tests/test_queue_server.py
+-rw-r--r--   0        0        0     6394 2024-04-27 11:42:55.811282 sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/tests/test_statistical_properties.py
+-rw-r--r--   0        0        0     5661 2024-04-27 11:42:55.812279 sim_rl-0.1.2/sim_rl/queue_env/queueing_network.py
+-rw-r--r--   0        0        0       77 2024-04-27 11:42:55.813279 sim_rl-0.1.2/sim_rl/requirements.txt
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.814279 sim_rl-0.1.2/sim_rl/rl_env/__init__.py
+-rw-r--r--   0        0        0    16574 2024-04-27 11:42:55.814279 sim_rl-0.1.2/sim_rl/rl_env/RL_Environment.py
+-rw-r--r--   0        0        0        0 2024-04-27 11:42:55.835064 sim_rl-0.1.2/sim_rl/tuning/__init__.py
+-rw-r--r--   0        0        0     9149 2024-04-27 11:42:55.836058 sim_rl-0.1.2/sim_rl/tuning/ray_tuning.py
+-rw-r--r--   0        0        0     8381 2024-04-27 11:42:55.837057 sim_rl-0.1.2/sim_rl/tuning/wandb_tuning.py
+-rw-r--r--   0        0        0      894 2024-04-27 11:42:55.838059 sim_rl-0.1.2/sim_rl/user_config/configuration.yml
+-rw-r--r--   0        0        0      923 2024-04-27 11:42:55.839058 sim_rl-0.1.2/sim_rl/user_config/eval_hyperparams.yml
+-rw-r--r--   0        0        0      482 2024-04-27 11:42:55.840057 sim_rl-0.1.2/sim_rl/user_config/tuning_hyperparams.yml
+-rw-r--r--   0        0        0    15003 1970-01-01 00:00:00.000000 sim_rl-0.1.2/PKG-INFO
```

### Comparing `sim_rl-0.1.1/pyproject.toml` & `sim_rl-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sim_rl"
-version = "0.1.1"
+version = "0.1.2"
 description = "Simulation Driven RL Package Utilized to Optimize Queueing Systems"
 authors = ["Fatima Alani, Jinyan Wang, Jevon Charles, Joshua Forday, Aaron Ong, Vinayak Modi <fatima.al-ani23@imperial.ac.uk>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.11"
 torch = "2.2.0"
```

### Comparing `sim_rl-0.1.1/README.md` & `sim_rl-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 - `queue_env`: Defines the simulated queueing environment, utilizing functionalities from the `queueing-tool` package.
 - `rl_env`: Hosts the RL environment, which is portable and compatible with different agent types.
 - `features`: Includes several utility features:
   - **Breakdown Exploration**: Explores key states versus peripheral states
   - **Blockage Demonstration**: Demonstrates how the agent responds to a server outage by adjusting routing probabilities.
   - **Confidence Evaluation**: Assesses the stability and reliability of the agent across different training setups
   - **Noise Evaluation**: Evaluate the effect of environmental noise on the performance of the agent
-  - **Startup Evaluation**: Identifies the burn-in period of the agent
+  - **Startup Behavior Visualization**: Identifies the burn-in period of the agent
+  - **Num Runs**: Manages the number of simulation runs for training and evaluation
   - **Robustness Evaluation**: Assess robustness of decisions across multiple trained agents
 
 ## Prerequisites
 
 Before running the simulations, ensure you have the following installed:
-- Python 3.8+
+- Python >=3.10 <3.11
 - PyTorch 1.7+
 - NumPy
 - Pandas
 - Matplotlib
 - queueing-tool
 - wandb
 - Ray
@@ -285,51 +286,51 @@
 
 ```bash
 python main.py --function tune --config_file user_config/configuration.yml --param_file user_config/eval_hyperparams.yml --data_file output_csv --image_file output_plots --plot_curves True --save_file True --tuner ray_tune
 ```
 
 ## Step 3: Explore Features
 
-### 1. **Explore Breakdown Scenarios**
+### 1. **Breakdown Evaluation**
 
 This feature allows the user to train the agent based on customed exploration preferences between key states and peripheral states using weight parameter `w1_key` and `w2_peripheral`. The purpose of this feature is to enable the agent to not only generate high rewards for key states but also visit all breadown scenarios sufficiently enough. 
 
-Set up the parameters in `user_config\features_params\bloackage_explore_params.yml`:
+Set up the parameters in `user_config\eval_hyperparams.yml`:
 
-- `w1_key`: Weight parameter to control favor exploring key states.
-- `w2_peripheral`: Weight parameter to control favor exploring peripheral states.
+- `w1`: Weight parameter to control favor exploring key states.
+- `w2`: Weight parameter to control favor exploring peripheral states.
 - `reset`: A bool value that controls whether to reset weight parameters during training.
 - `reset_frequency`: A value that defines the number of episodes frequency to reset the weight parameters.
 - `num_output`: A value that defines the number of top and least reward/visits states to plot in a histogram
 - `output_json`: A bool value that determines whether to output the json file of key states and peripheral states
 - `output_histogram`: A bool value that determines whether to output the histogram that shows the rewards and visits of the top and least states.
 - `output_coverage_metric`: A bool value that determines whether to output the current coverage metric.
 
 To run this feature, navigate to `/evaluation/breakdown_exploration` and run:
    ```bash
    python breakdown_exploration.py
    ```
 
-### 2. **Blockage Demonstrations**
+### 2. **Decision Evaluation**
 
 This feature allows the user to test a trained agent's performance on a simulated server blockage queueing environment by visualizing the changes in transition probabilities. The purpose of this feature is to show how effectice the tranied agent is acting on breakdown cases. 
 
 Set up the parameters in `user_config\features_params\blockage_demonstration_params.yml`:
 
-- `num_sim`: Defines the number of jobs to simulate for each time step during training.
+- `sim_jobs`: Defines the number of jobs to simulate for each time step during training.
 - `time_steps`: Defines the number of time steps to perform for each episode.
 - `queue_index`: Defines the queue index that record the metrics for.
 - `metric`: Defines the metric to be reported for the selected queue.
 
 To use this feature, navigate to `/evaluation/blockage_demonstration` and run:
    ```bash
    python demonstrations.py
    ```
 
-### 3. **Startup Behavior Identification**
+### 3. **Startup Evaluation**
 
 This feature allows the user to visualize when the burn-in periods end on the learning curve. 
 
 Set up the parameters in the script:
 
 - `window_size`: Specifies the number of data points used to compute the moving average of the rewards.
 - `threshold`: Defines the maximum acceptable absolute value of the derivative of the smoothed rewards below which a reward is considered stable. 
@@ -337,22 +338,23 @@
 - `episode`: Specify which episode's rewards to analyze from a dataset.
 
 To perform the feature, navigate to `/evaluation/startup_behavior` and run:
    ```bash
    python startup.py
    ```
 
-### 4. **Confidence Evaluation** (need clarification from Josh)
+### 4. **Convergence Evaluation** (need clarification from Josh)
 
 This feature allows the user train multiple versions of the agent for different numbers of training episodes and then evaluate the performance of each agent on the simulation environment.
 
 Set up the parameters in the script:
 
-- `num_episodes_list`: A list that contains different numbers of episodes to train the agents.
-- `timesteps`: A value that defines the number of timesteps to train the agent during each episode.
+- `window_size`: Specifies the number of data points used to compute the moving average of the rewards.
+- `threshold`: Defines the maximum acceptable absolute value of the derivative of the smoothed rewards below which a reward is considered stable. 
+- `consecutive_points`: The number of consecutive data points that must all be below the threshold for the rewards to be considered as having stabilized. 
 
 To run this feature, navigate to `/evaluation/confidence_evaluation` and run:
    ```bash
    python confidence.py
    ```
 
 ### 5. **Robustness Evaluation** (need clarification from Fatima)
@@ -377,14 +379,16 @@
 This feature allows the user to evaluate the effect of environmental noise on the performance of the agent. (how is env noise defined here?) 
 
 Set up the parameters in the script:
 
 - `frequency `: The likelihood or frequency at which noise is introduced to the system. It must be a value between 0 and 1. This parameter determines how often, proportionally, noise will be added during the simulation. 
 - `mean`: The mean of the normal distribution from which the noise values are sampled. This represents the average value of the noise that will be introduced.
 - `variance`: The variance of the normal distribution from which the noise values are sampled. This parameter indicates the spread or dispersion of the noise around the mean.
+- `timesteps`: Number of time steps to run during training
+- `temperature`: Parameter that constrols the exaggeration of the influence of action vector has on transition probability
 
 To run the feature, navigate to `/evaluation/noise_evaluation` and run:
    ```bash
    python noise_evaluation.py
    ```
 
 ## Contribution
```

### Comparing `sim_rl-0.1.1/sim_rl/.gitlab-ci.yml` & `sim_rl-0.1.2/sim_rl/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/agents/buffer.py` & `sim_rl-0.1.2/sim_rl/agents/buffer.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/agents/ddpg_agent.py` & `sim_rl-0.1.2/sim_rl/agents/ddpg_agent.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/agents/model.py` & `sim_rl-0.1.2/sim_rl/agents/model.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/agents/trained_agent.pt` & `sim_rl-0.1.2/sim_rl/agents/trained_agent.pt`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/agents/trained_ddpg_agent.pt` & `sim_rl-0.1.2/sim_rl/agents/trained_ddpg_agent.pt`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/debug.py` & `sim_rl-0.1.2/sim_rl/debug.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/evaluation/convergence_evaluation/convergence_evaluation.py` & `sim_rl-0.1.2/sim_rl/evaluation/convergence_evaluation/convergence_evaluation.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/evaluation/convergence_evaluation/reward_plot.png` & `sim_rl-0.1.2/sim_rl/evaluation/convergence_evaluation/reward_plot.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/evaluation/decision_evaluation/decision_evaluation.py` & `sim_rl-0.1.2/sim_rl/evaluation/decision_evaluation/decision_evaluation.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/evaluation/decision_evaluation/output_plots/Transition_Proba_BeforeAfter_Blockage.png` & `sim_rl-0.1.2/sim_rl/evaluation/decision_evaluation/output_plots/Transition_Proba_BeforeAfter_Blockage.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/evaluation/noise_evaluation/noise_evaluation.py` & `sim_rl-0.1.2/sim_rl/evaluation/noise_evaluation/noise_evaluation.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/evaluation/robustness_evaluation/robustness_evaluation.py` & `sim_rl-0.1.2/sim_rl/evaluation/robustness_evaluation/robustness_evaluation.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/evaluation/startup_evaluation/reward_plot.png` & `sim_rl-0.1.2/sim_rl/evaluation/startup_evaluation/reward_plot.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/evaluation/startup_evaluation/reward_plot_0.png` & `sim_rl-0.1.2/sim_rl/evaluation/startup_evaluation/reward_plot_0.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/evaluation/startup_evaluation/reward_plot_1.png` & `sim_rl-0.1.2/sim_rl/evaluation/startup_evaluation/reward_plot_1.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/evaluation/startup_evaluation/reward_plot_2.png` & `sim_rl-0.1.2/sim_rl/evaluation/startup_evaluation/reward_plot_2.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/evaluation/startup_evaluation/reward_plot_3.png` & `sim_rl-0.1.2/sim_rl/evaluation/startup_evaluation/reward_plot_3.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/evaluation/startup_evaluation/startup_evaluation.py` & `sim_rl-0.1.2/sim_rl/evaluation/startup_evaluation/startup_evaluation.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/foundations/breakdown_exploration/__pycache__/state_exploration.cpython-311.pyc` & `sim_rl-0.1.2/sim_rl/foundations/breakdown_exploration/__pycache__/state_exploration.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/foundations/breakdown_exploration/breakdown_exploration.py` & `sim_rl-0.1.2/sim_rl/foundations/breakdown_exploration/breakdown_exploration.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/foundations/breakdown_exploration/output_data/all_breakdown_cases.json` & `sim_rl-0.1.2/sim_rl/foundations/breakdown_exploration/output_data/all_breakdown_cases.json`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/foundations/breakdown_exploration/output_data/key_states/rewards.png` & `sim_rl-0.1.2/sim_rl/foundations/breakdown_exploration/output_data/key_states/rewards.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/foundations/breakdown_exploration/output_data/peripheral_states/visits.png` & `sim_rl-0.1.2/sim_rl/foundations/breakdown_exploration/output_data/peripheral_states/visits.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/foundations/core_functions.py` & `sim_rl-0.1.2/sim_rl/foundations/core_functions.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/foundations/core_plotting.py` & `sim_rl-0.1.2/sim_rl/foundations/core_plotting.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/foundations/output_csv/action_dict.csv` & `sim_rl-0.1.2/sim_rl/foundations/output_csv/action_dict.csv`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/foundations/output_csv/actor_loss.csv` & `sim_rl-0.1.2/sim_rl/foundations/output_csv/actor_loss.csv`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/foundations/output_csv/critic_loss.csv` & `sim_rl-0.1.2/sim_rl/foundations/output_csv/critic_loss.csv`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/foundations/output_csv/next_state_model_loss.csv` & `sim_rl-0.1.2/sim_rl/foundations/output_csv/next_state_model_loss.csv`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/foundations/output_csv/reward_dict.json` & `sim_rl-0.1.2/sim_rl/foundations/output_csv/reward_dict.json`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/foundations/output_csv/reward_model_loss.csv` & `sim_rl-0.1.2/sim_rl/foundations/output_csv/reward_model_loss.csv`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/foundations/output_csv/transition_proba.csv` & `sim_rl-0.1.2/sim_rl/foundations/output_csv/transition_proba.csv`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/main.py` & `sim_rl-0.1.2/sim_rl/main.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_base_functions.py` & `sim_rl-0.1.2/sim_rl/queue_env/queue_base_functions.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/.github/workflows/auto-tagging.yml` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/.github/workflows/auto-tagging.yml`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/.github/workflows/run-tests.yml` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/.gitignore` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/.gitignore`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/.readthedocs.yml` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/CHANGELOG.md` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/cliff.toml` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/cliff.toml`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/_static/bootstrap-lumen.min.css` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/_static/bootstrap-lumen.min.css`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/_static/copybutton.js` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/_static/customized_alabaster.css` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/_static/customized_alabaster.css`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/_static/jquery.min.js` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/_static/jquery.min.js`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/_static/qt_sphinx13.css` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/_static/qt_sphinx13.css`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/_templates/opensearch.xml` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/_templates/opensearch.xml`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/_templates/search.html` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/_templates/search.html`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/_templates/searchbox.html` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/_templates/searchbox.html`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/_templates/searchresults.html` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/_templates/searchresults.html`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/_themes/qt_sphinx13/layout.html` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/_themes/qt_sphinx13/layout.html`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/conf.py` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/current_state.png` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/current_state.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/current_state1.png` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/current_state1.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/edge_type_2-1.png` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/edge_type_2-1.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/edge_type_2.png` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/edge_type_2.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/fig.png` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/fig.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/graph.rst` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/graph.rst`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/index.rst` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/installation.rst` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/make.bat` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/Makefile` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/my_network.png` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/my_network.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/my_network1.png` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/my_network1.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/network.rst` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/network.rst`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/overview.rst` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/queues.rst` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/queues.rst`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/sim.png` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/sim.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/sim1.png` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/sim1.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/store.png` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/store.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/docs/store1.png` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/docs/store1.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/examples/example_grocery_store.py` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/examples/example_grocery_store.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/LICENSE.txt` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/poetry.lock` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/poetry.lock`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/pyproject.toml` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/__init__.py` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/__init__.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/graph/__init__.py` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/graph/_pairwise.pyx` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/graph/_pairwise.pyx`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_functions.py` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_functions.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_generation.py` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_generation.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_preparation.py` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_preparation.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_wrapper.py` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/graph/graph_wrapper.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/network/__init__.py` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/network/__init__.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/network/priority_queue.c` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/network/priority_queue.c`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/network/priority_queue.pyx` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/network/priority_queue.pyx`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/network/queue_network.py` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/network/queue_network.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/queues/__init__.py` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/queues/agents.py` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/queues/agents.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/queues/choice.c` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/queues/choice.c`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/queues/choice.pyx` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/queues/choice.pyx`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/queues/queue_extentions.py` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/queues/queue_extentions.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/queues/queue_servers.py` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/queues/queue_servers.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/queueing_tool/union_find.py` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/queueing_tool/union_find.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/README.rst` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/README.rst`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/tests/img/test-mpl-1.x.png` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/tests/img/test-mpl-1.x.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/tests/img/test-mpl-2.x.png` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/tests/img/test-mpl-2.x.png`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/tests/test_graph_generation.py` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/tests/test_graph_generation.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/tests/test_network.py` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/tests/test_qndigraph.py` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/tests/test_qndigraph.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/tests/test_queue_server.py` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/tests/test_queue_server.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queue_foundations/tests/test_statistical_properties.py` & `sim_rl-0.1.2/sim_rl/queue_env/queue_foundations/tests/test_statistical_properties.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/queue_env/queueing_network.py` & `sim_rl-0.1.2/sim_rl/queue_env/queueing_network.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/rl_env/RL_Environment.py` & `sim_rl-0.1.2/sim_rl/rl_env/RL_Environment.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/tuning/ray_tuning.py` & `sim_rl-0.1.2/sim_rl/tuning/ray_tuning.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/tuning/wandb_tuning.py` & `sim_rl-0.1.2/sim_rl/tuning/wandb_tuning.py`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/user_config/configuration.yml` & `sim_rl-0.1.2/sim_rl/user_config/configuration.yml`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/sim_rl/user_config/eval_hyperparams.yml` & `sim_rl-0.1.2/sim_rl/user_config/eval_hyperparams.yml`

 * *Files identical despite different names*

### Comparing `sim_rl-0.1.1/PKG-INFO` & `sim_rl-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sim_rl
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simulation Driven RL Package Utilized to Optimize Queueing Systems
 Author: Fatima Alani, Jinyan Wang, Jevon Charles, Joshua Forday, Aaron Ong, Vinayak Modi
 Author-email: fatima.al-ani23@imperial.ac.uk
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: PyYAML (==6.0.1)
@@ -28,21 +28,22 @@
 - `queue_env`: Defines the simulated queueing environment, utilizing functionalities from the `queueing-tool` package.
 - `rl_env`: Hosts the RL environment, which is portable and compatible with different agent types.
 - `features`: Includes several utility features:
   - **Breakdown Exploration**: Explores key states versus peripheral states
   - **Blockage Demonstration**: Demonstrates how the agent responds to a server outage by adjusting routing probabilities.
   - **Confidence Evaluation**: Assesses the stability and reliability of the agent across different training setups
   - **Noise Evaluation**: Evaluate the effect of environmental noise on the performance of the agent
-  - **Startup Evaluation**: Identifies the burn-in period of the agent
+  - **Startup Behavior Visualization**: Identifies the burn-in period of the agent
+  - **Num Runs**: Manages the number of simulation runs for training and evaluation
   - **Robustness Evaluation**: Assess robustness of decisions across multiple trained agents
 
 ## Prerequisites
 
 Before running the simulations, ensure you have the following installed:
-- Python 3.8+
+- Python >=3.10 <3.11
 - PyTorch 1.7+
 - NumPy
 - Pandas
 - Matplotlib
 - queueing-tool
 - wandb
 - Ray
@@ -304,51 +305,51 @@
 
 ```bash
 python main.py --function tune --config_file user_config/configuration.yml --param_file user_config/eval_hyperparams.yml --data_file output_csv --image_file output_plots --plot_curves True --save_file True --tuner ray_tune
 ```
 
 ## Step 3: Explore Features
 
-### 1. **Explore Breakdown Scenarios**
+### 1. **Breakdown Evaluation**
 
 This feature allows the user to train the agent based on customed exploration preferences between key states and peripheral states using weight parameter `w1_key` and `w2_peripheral`. The purpose of this feature is to enable the agent to not only generate high rewards for key states but also visit all breadown scenarios sufficiently enough. 
 
-Set up the parameters in `user_config\features_params\bloackage_explore_params.yml`:
+Set up the parameters in `user_config\eval_hyperparams.yml`:
 
-- `w1_key`: Weight parameter to control favor exploring key states.
-- `w2_peripheral`: Weight parameter to control favor exploring peripheral states.
+- `w1`: Weight parameter to control favor exploring key states.
+- `w2`: Weight parameter to control favor exploring peripheral states.
 - `reset`: A bool value that controls whether to reset weight parameters during training.
 - `reset_frequency`: A value that defines the number of episodes frequency to reset the weight parameters.
 - `num_output`: A value that defines the number of top and least reward/visits states to plot in a histogram
 - `output_json`: A bool value that determines whether to output the json file of key states and peripheral states
 - `output_histogram`: A bool value that determines whether to output the histogram that shows the rewards and visits of the top and least states.
 - `output_coverage_metric`: A bool value that determines whether to output the current coverage metric.
 
 To run this feature, navigate to `/evaluation/breakdown_exploration` and run:
    ```bash
    python breakdown_exploration.py
    ```
 
-### 2. **Blockage Demonstrations**
+### 2. **Decision Evaluation**
 
 This feature allows the user to test a trained agent's performance on a simulated server blockage queueing environment by visualizing the changes in transition probabilities. The purpose of this feature is to show how effectice the tranied agent is acting on breakdown cases. 
 
 Set up the parameters in `user_config\features_params\blockage_demonstration_params.yml`:
 
-- `num_sim`: Defines the number of jobs to simulate for each time step during training.
+- `sim_jobs`: Defines the number of jobs to simulate for each time step during training.
 - `time_steps`: Defines the number of time steps to perform for each episode.
 - `queue_index`: Defines the queue index that record the metrics for.
 - `metric`: Defines the metric to be reported for the selected queue.
 
 To use this feature, navigate to `/evaluation/blockage_demonstration` and run:
    ```bash
    python demonstrations.py
    ```
 
-### 3. **Startup Behavior Identification**
+### 3. **Startup Evaluation**
 
 This feature allows the user to visualize when the burn-in periods end on the learning curve. 
 
 Set up the parameters in the script:
 
 - `window_size`: Specifies the number of data points used to compute the moving average of the rewards.
 - `threshold`: Defines the maximum acceptable absolute value of the derivative of the smoothed rewards below which a reward is considered stable. 
@@ -356,22 +357,23 @@
 - `episode`: Specify which episode's rewards to analyze from a dataset.
 
 To perform the feature, navigate to `/evaluation/startup_behavior` and run:
    ```bash
    python startup.py
    ```
 
-### 4. **Confidence Evaluation** (need clarification from Josh)
+### 4. **Convergence Evaluation** (need clarification from Josh)
 
 This feature allows the user train multiple versions of the agent for different numbers of training episodes and then evaluate the performance of each agent on the simulation environment.
 
 Set up the parameters in the script:
 
-- `num_episodes_list`: A list that contains different numbers of episodes to train the agents.
-- `timesteps`: A value that defines the number of timesteps to train the agent during each episode.
+- `window_size`: Specifies the number of data points used to compute the moving average of the rewards.
+- `threshold`: Defines the maximum acceptable absolute value of the derivative of the smoothed rewards below which a reward is considered stable. 
+- `consecutive_points`: The number of consecutive data points that must all be below the threshold for the rewards to be considered as having stabilized. 
 
 To run this feature, navigate to `/evaluation/confidence_evaluation` and run:
    ```bash
    python confidence.py
    ```
 
 ### 5. **Robustness Evaluation** (need clarification from Fatima)
@@ -396,14 +398,16 @@
 This feature allows the user to evaluate the effect of environmental noise on the performance of the agent. (how is env noise defined here?) 
 
 Set up the parameters in the script:
 
 - `frequency `: The likelihood or frequency at which noise is introduced to the system. It must be a value between 0 and 1. This parameter determines how often, proportionally, noise will be added during the simulation. 
 - `mean`: The mean of the normal distribution from which the noise values are sampled. This represents the average value of the noise that will be introduced.
 - `variance`: The variance of the normal distribution from which the noise values are sampled. This parameter indicates the spread or dispersion of the noise around the mean.
+- `timesteps`: Number of time steps to run during training
+- `temperature`: Parameter that constrols the exaggeration of the influence of action vector has on transition probability
 
 To run the feature, navigate to `/evaluation/noise_evaluation` and run:
    ```bash
    python noise_evaluation.py
    ```
 
 ## Contribution
```
