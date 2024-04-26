# Comparing `tmp/mira_simpeg-0.19.0.dev8.tar.gz` & `tmp/mira_simpeg-1!0.19.0.8a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mira_simpeg-0.19.0.dev8.tar", max compression
+gzip compressed data, was "mira_simpeg-1!0.19.0.8a2.tar", max compression
```

## Comparing `mira_simpeg-0.19.0.dev8.tar` & `mira_simpeg-1!0.19.0.8a2.tar`

### file list

```diff
@@ -1,182 +1,183 @@
--rw-r--r--   0        0        0     1109 2024-01-11 21:39:39.291988 mira_simpeg-0.19.0.dev8/LICENSE
--rw-r--r--   0        0        0     2807 2024-04-25 18:57:44.664220 mira_simpeg-0.19.0.dev8/pyproject.toml
--rw-r--r--   0        0        0     6106 2024-01-11 21:39:39.291988 mira_simpeg-0.19.0.dev8/README.rst
--rw-r--r--   0        0        0     3458 2024-01-11 21:39:39.291988 mira_simpeg-0.19.0.dev8/SimPEG/__init__.py
--rw-r--r--   0        0        0      158 2023-10-05 16:26:57.174949 mira_simpeg-0.19.0.dev8/SimPEG/base/__init__.py
--rw-r--r--   0        0        0    17746 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/base/pde_simulation.py
--rw-r--r--   0        0        0      895 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/dask/__init__.py
--rw-r--r--   0        0        0     2856 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/dask/data_misfit.py
--rw-r--r--   0        0        0        0 2023-10-05 16:26:57.174949 mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/__init__.py
--rw-r--r--   0        0        0        0 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/frequency_domain/__init__.py
--rw-r--r--   0        0        0     7742 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/frequency_domain/simulation.py
--rw-r--r--   0        0        0        0 2023-10-05 16:26:57.174949 mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/static/__init__.py
--rw-r--r--   0        0        0        0 2023-10-05 16:26:57.174949 mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/static/induced_polarization/__init__.py
--rw-r--r--   0        0        0     4104 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/static/induced_polarization/simulation.py
--rw-r--r--   0        0        0     1869 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/static/induced_polarization/simulation_2d.py
--rw-r--r--   0        0        0        0 2023-10-05 16:26:57.174949 mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/static/resistivity/__init__.py
--rw-r--r--   0        0        0     5153 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/static/resistivity/simulation.py
--rw-r--r--   0        0        0     6529 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/static/resistivity/simulation_2d.py
--rw-r--r--   0        0        0        0 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/time_domain/__init__.py
--rw-r--r--   0        0        0    18322 2024-04-25 18:57:44.664220 mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/time_domain/simulation.py
--rw-r--r--   0        0        0     7379 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/dask/inverse_problem.py
--rw-r--r--   0        0        0     4523 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/dask/objective_function.py
--rw-r--r--   0        0        0        0 2023-10-05 16:26:57.174949 mira_simpeg-0.19.0.dev8/SimPEG/dask/potential_fields/__init__.py
--rw-r--r--   0        0        0     3907 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/dask/potential_fields/base.py
--rw-r--r--   0        0        0        0 2023-10-05 16:26:57.174949 mira_simpeg-0.19.0.dev8/SimPEG/dask/potential_fields/gravity/__init__.py
--rw-r--r--   0        0        0      660 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/dask/potential_fields/gravity/simulation.py
--rw-r--r--   0        0        0        0 2023-10-05 16:26:57.174949 mira_simpeg-0.19.0.dev8/SimPEG/dask/potential_fields/magnetics/__init__.py
--rw-r--r--   0        0        0     1041 2024-01-12 17:21:33.839439 mira_simpeg-0.19.0.dev8/SimPEG/dask/potential_fields/magnetics/simulation.py
--rw-r--r--   0        0        0     6763 2024-04-12 20:56:06.259702 mira_simpeg-0.19.0.dev8/SimPEG/dask/simulation.py
--rw-r--r--   0        0        0     3132 2024-04-25 18:57:44.664220 mira_simpeg-0.19.0.dev8/SimPEG/dask/utils.py
--rw-r--r--   0        0        0    14075 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/data.py
--rw-r--r--   0        0        0     7307 2024-01-12 17:21:33.856459 mira_simpeg-0.19.0.dev8/SimPEG/data_misfit.py
--rw-r--r--   0        0        0      917 2024-01-12 17:21:33.856459 mira_simpeg-0.19.0.dev8/SimPEG/directives/__init__.py
--rw-r--r--   0        0        0   109257 2024-04-25 16:00:58.227398 mira_simpeg-0.19.0.dev8/SimPEG/directives/directives.py
--rw-r--r--   0        0        0    19820 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/directives/pgi_directives.py
--rw-r--r--   0        0        0    13400 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/directives/sim_directives.py
--rw-r--r--   0        0        0     1133 2024-01-12 17:21:33.858767 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/__init__.py
--rw-r--r--   0        0        0      210 2023-10-05 16:26:57.190595 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/analytics/__init__.py
--rw-r--r--   0        0        0     7105 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/analytics/DC.py
--rw-r--r--   0        0        0     8525 2024-01-12 17:21:33.858767 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/analytics/FDEM.py
--rw-r--r--   0        0        0     5084 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/analytics/FDEMcasing.py
--rw-r--r--   0        0        0    11443 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/analytics/FDEMDipolarfields.py
--rw-r--r--   0        0        0     5853 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/analytics/NSEM.py
--rw-r--r--   0        0        0     5381 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/analytics/TDEM.py
--rw-r--r--   0        0        0     6977 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/base.py
--rw-r--r--   0        0        0    23172 2024-01-12 17:21:33.859755 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/base_1d.py
--rw-r--r--   0        0        0     2011 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/frequency_domain/__init__.py
--rw-r--r--   0        0        0    60417 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/frequency_domain/fields.py
--rw-r--r--   0        0        0    13112 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/frequency_domain/receivers.py
--rw-r--r--   0        0        0    27311 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/frequency_domain/simulation.py
--rw-r--r--   0        0        0    11528 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/frequency_domain/simulation_1d.py
--rw-r--r--   0        0        0    43188 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/frequency_domain/sources.py
--rw-r--r--   0        0        0     2795 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/frequency_domain/survey.py
--rw-r--r--   0        0        0     1755 2024-01-11 21:39:39.308580 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/__init__.py
--rw-r--r--   0        0        0    26411 2024-01-11 21:39:39.324633 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/fields.py
--rw-r--r--   0        0        0    22562 2024-01-12 17:21:33.860755 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/receivers.py
--rw-r--r--   0        0        0    27228 2024-01-11 21:39:39.324633 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/simulation.py
--rw-r--r--   0        0        0    12406 2024-01-12 17:21:33.860755 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/simulation_1d.py
--rw-r--r--   0        0        0     7644 2024-01-11 21:39:39.326827 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/sources.py
--rw-r--r--   0        0        0     8922 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/survey.py
--rw-r--r--   0        0        0      793 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/__init__.py
--rw-r--r--   0        0        0     5445 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/analytic_1d.py
--rw-r--r--   0        0        0    18826 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/data_utils.py
--rw-r--r--   0        0        0     5072 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/data_viewer.py
--rw-r--r--   0        0        0     7488 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/edi_files_utils.py
--rw-r--r--   0        0        0    22004 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/plot_data_types.py
--rw-r--r--   0        0        0    30007 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/plot_utils.py
--rw-r--r--   0        0        0     1338 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/solutions_1d.py
--rw-r--r--   0        0        0     7617 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/source_utils.py
--rw-r--r--   0        0        0    18430 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/test_utils.py
--rw-r--r--   0        0        0      129 2023-10-05 16:26:57.206219 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/__init__.py
--rw-r--r--   0        0        0     1212 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/induced_polarization/__init__.py
--rw-r--r--   0        0        0     2144 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/induced_polarization/run.py
--rw-r--r--   0        0        0     4194 2024-01-12 17:21:33.860755 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/induced_polarization/simulation.py
--rw-r--r--   0        0        0      637 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/induced_polarization/survey.py
--rw-r--r--   0        0        0     2050 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/__init__.py
--rw-r--r--   0        0        0     8282 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/fields.py
--rw-r--r--   0        0        0     8412 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/fields_2d.py
--rw-r--r--   0        0        0    41758 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/IODC.py
--rw-r--r--   0        0        0    16671 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/receivers.py
--rw-r--r--   0        0        0     2089 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/run.py
--rw-r--r--   0        0        0    22651 2024-01-12 17:21:33.861755 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/simulation.py
--rw-r--r--   0        0        0    11514 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/simulation_1d.py
--rw-r--r--   0        0        0    27954 2024-01-12 17:21:33.863160 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/simulation_2d.py
--rw-r--r--   0        0        0     7782 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/sources.py
--rw-r--r--   0        0        0    12123 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/survey.py
--rw-r--r--   0        0        0     4071 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/utils.py
--rw-r--r--   0        0        0     1656 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/__init__.py
--rw-r--r--   0        0        0     2105 2023-10-05 16:26:57.206219 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/data.py
--rw-r--r--   0        0        0    14850 2024-01-11 21:39:39.327521 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/receivers.py
--rw-r--r--   0        0        0     5028 2023-10-05 16:26:57.206219 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/run.py
--rw-r--r--   0        0        0    21261 2024-01-11 21:39:39.343188 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/simulation.py
--rw-r--r--   0        0        0     2962 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/simulation_2d.py
--rw-r--r--   0        0        0     8465 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/sources.py
--rw-r--r--   0        0        0     4149 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/survey.py
--rw-r--r--   0        0        0     1124 2024-01-12 17:21:33.863160 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spontaneous_potential/__init__.py
--rw-r--r--   0        0        0     6658 2024-01-12 17:21:33.864168 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spontaneous_potential/simulation.py
--rw-r--r--   0        0        0     1011 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spontaneous_potential/sources.py
--rw-r--r--   0        0        0     1950 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/utils/__init__.py
--rw-r--r--   0        0        0    66992 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/utils/static_utils.py
--rw-r--r--   0        0        0     2290 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/time_domain/__init__.py
--rw-r--r--   0        0        0    24117 2024-04-12 20:56:06.263737 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/time_domain/fields.py
--rw-r--r--   0        0        0    12502 2024-04-12 20:56:06.263737 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/time_domain/receivers.py
--rw-r--r--   0        0        0    39494 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/time_domain/simulation.py
--rw-r--r--   0        0        0    14465 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/time_domain/simulation_1d.py
--rw-r--r--   0        0        0    71847 2024-01-12 17:21:33.865252 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/time_domain/sources.py
--rw-r--r--   0        0        0     1070 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/time_domain/survey.py
--rw-r--r--   0        0        0      947 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/utils/__init__.py
--rw-r--r--   0        0        0    16473 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/utils/current_utils.py
--rw-r--r--   0        0        0     6593 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/utils/em1d_utils.py
--rw-r--r--   0        0        0     5831 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/utils/testing_utils.py
--rw-r--r--   0        0        0     3578 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/utils/waveform_utils.py
--rw-r--r--   0        0        0     1528 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/viscous_remanent_magnetization/__init__.py
--rw-r--r--   0        0        0     6800 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/viscous_remanent_magnetization/receivers.py
--rw-r--r--   0        0        0    39890 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/viscous_remanent_magnetization/simulation.py
--rw-r--r--   0        0        0    18560 2024-01-12 17:21:33.865252 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/viscous_remanent_magnetization/sources.py
--rw-r--r--   0        0        0     2338 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/viscous_remanent_magnetization/survey.py
--rw-r--r--   0        0        0    20152 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/viscous_remanent_magnetization/waveforms.py
--rw-r--r--   0        0        0    13959 2024-01-12 17:21:33.866228 mira_simpeg-0.19.0.dev8/SimPEG/fields.py
--rw-r--r--   0        0        0       24 2023-10-05 16:26:57.230943 mira_simpeg-0.19.0.dev8/SimPEG/flow/__init__.py
--rw-r--r--   0        0        0     1136 2024-01-11 21:39:39.343527 mira_simpeg-0.19.0.dev8/SimPEG/flow/richards/__init__.py
--rw-r--r--   0        0        0    33981 2024-01-11 21:39:39.360202 mira_simpeg-0.19.0.dev8/SimPEG/flow/richards/empirical.py
--rw-r--r--   0        0        0     3618 2024-01-11 21:39:39.360202 mira_simpeg-0.19.0.dev8/SimPEG/flow/richards/receivers.py
--rw-r--r--   0        0        0    13567 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/flow/richards/simulation.py
--rw-r--r--   0        0        0     2798 2024-01-12 17:21:33.866228 mira_simpeg-0.19.0.dev8/SimPEG/flow/richards/survey.py
--rw-r--r--   0        0        0    10625 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/inverse_problem.py
--rw-r--r--   0        0        0     3329 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/inversion.py
--rw-r--r--   0        0        0   213269 2024-01-12 17:21:33.867169 mira_simpeg-0.19.0.dev8/SimPEG/maps.py
--rw-r--r--   0        0        0     1527 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/meta/__init__.py
--rw-r--r--   0        0        0    16903 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/meta/simulation.py
--rw-r--r--   0        0        0     1218 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/models.py
--rw-r--r--   0        0        0    14724 2024-01-12 17:21:33.868175 mira_simpeg-0.19.0.dev8/SimPEG/objective_function.py
--rw-r--r--   0        0        0    39604 2024-01-12 17:21:33.869168 mira_simpeg-0.19.0.dev8/SimPEG/optimization.py
--rw-r--r--   0        0        0      589 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/__init__.py
--rw-r--r--   0        0        0    13464 2024-01-12 17:21:33.870181 mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/base.py
--rw-r--r--   0        0        0     1100 2024-01-12 17:21:33.870181 mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/gravity/__init__.py
--rw-r--r--   0        0        0     2272 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/gravity/analytics.py
--rw-r--r--   0        0        0     2271 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/gravity/receivers.py
--rw-r--r--   0        0        0     9057 2024-01-12 17:21:33.871168 mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/gravity/simulation.py
--rw-r--r--   0        0        0      407 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/gravity/sources.py
--rw-r--r--   0        0        0     4774 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/gravity/survey.py
--rw-r--r--   0        0        0     1174 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/magnetics/__init__.py
--rw-r--r--   0        0        0     9821 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/magnetics/analytics.py
--rw-r--r--   0        0        0     2228 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/magnetics/receivers.py
--rw-r--r--   0        0        0    31502 2024-01-12 17:21:33.871168 mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/magnetics/simulation.py
--rw-r--r--   0        0        0     3669 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/magnetics/sources.py
--rw-r--r--   0        0        0     2693 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/magnetics/survey.py
--rw-r--r--   0        0        0    15572 2024-01-12 17:21:33.872185 mira_simpeg-0.19.0.dev8/SimPEG/props.py
--rw-r--r--   0        0        0     8134 2024-01-12 17:21:33.872578 mira_simpeg-0.19.0.dev8/SimPEG/regularization/__init__.py
--rw-r--r--   0        0        0    43137 2024-02-06 18:21:38.636361 mira_simpeg-0.19.0.dev8/SimPEG/regularization/base.py
--rw-r--r--   0        0        0     3908 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/regularization/correspondence.py
--rw-r--r--   0        0        0     9843 2024-01-12 17:21:33.872578 mira_simpeg-0.19.0.dev8/SimPEG/regularization/cross_gradient.py
--rw-r--r--   0        0        0     5244 2024-01-11 21:39:39.360810 mira_simpeg-0.19.0.dev8/SimPEG/regularization/jtv.py
--rw-r--r--   0        0        0    32347 2024-01-12 17:21:33.872578 mira_simpeg-0.19.0.dev8/SimPEG/regularization/pgi.py
--rw-r--r--   0        0        0    16758 2024-02-06 18:21:38.637365 mira_simpeg-0.19.0.dev8/SimPEG/regularization/regularization_mesh.py
--rw-r--r--   0        0        0    10363 2024-02-06 18:21:38.638358 mira_simpeg-0.19.0.dev8/SimPEG/regularization/sparse.py
--rw-r--r--   0        0        0       39 2023-10-05 16:26:57.247510 mira_simpeg-0.19.0.dev8/SimPEG/seismic/__init__.py
--rw-r--r--   0        0        0      760 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev8/SimPEG/seismic/straight_ray_tomography/__init__.py
--rw-r--r--   0        0        0     3578 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev8/SimPEG/seismic/straight_ray_tomography/simulation.py
--rw-r--r--   0        0        0     1688 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev8/SimPEG/seismic/straight_ray_tomography/survey.py
--rw-r--r--   0        0        0    19552 2024-01-12 17:21:33.872578 mira_simpeg-0.19.0.dev8/SimPEG/simulation.py
--rw-r--r--   0        0        0    17616 2024-01-12 17:21:33.872578 mira_simpeg-0.19.0.dev8/SimPEG/survey.py
--rw-r--r--   0        0        0     6705 2024-01-12 17:21:33.872578 mira_simpeg-0.19.0.dev8/SimPEG/utils/__init__.py
--rw-r--r--   0        0        0    39084 2024-01-12 17:21:33.877582 mira_simpeg-0.19.0.dev8/SimPEG/utils/code_utils.py
--rw-r--r--   0        0        0      531 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev8/SimPEG/utils/coord_utils.py
--rw-r--r--   0        0        0     4104 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev8/SimPEG/utils/counter_utils.py
--rw-r--r--   0        0        0      687 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev8/SimPEG/utils/curv_utils.py
--rw-r--r--   0        0        0       98 2023-10-05 16:26:57.263144 mira_simpeg-0.19.0.dev8/SimPEG/utils/drivers/__init__.py
--rw-r--r--   0        0        0     8117 2024-01-12 17:21:33.877582 mira_simpeg-0.19.0.dev8/SimPEG/utils/drivers/gravity_driver.py
--rw-r--r--   0        0        0     9736 2024-01-12 17:21:33.877582 mira_simpeg-0.19.0.dev8/SimPEG/utils/drivers/magnetics_driver.py
--rw-r--r--   0        0        0      631 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev8/SimPEG/utils/io_utils/__init__.py
--rw-r--r--   0        0        0    36848 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev8/SimPEG/utils/io_utils/io_utils_electromagnetics.py
--rw-r--r--   0        0        0     4825 2024-01-12 17:21:33.877582 mira_simpeg-0.19.0.dev8/SimPEG/utils/io_utils/io_utils_general.py
--rw-r--r--   0        0        0    13183 2024-01-12 17:21:33.877582 mira_simpeg-0.19.0.dev8/SimPEG/utils/io_utils/io_utils_pf.py
--rw-r--r--   0        0        0    14546 2024-02-06 18:21:38.638358 mira_simpeg-0.19.0.dev8/SimPEG/utils/mat_utils.py
--rw-r--r--   0        0        0     3480 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev8/SimPEG/utils/mesh_utils.py
--rw-r--r--   0        0        0    16902 2024-01-12 17:21:33.877582 mira_simpeg-0.19.0.dev8/SimPEG/utils/model_builder.py
--rw-r--r--   0        0        0     7038 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev8/SimPEG/utils/model_utils.py
--rw-r--r--   0        0        0    67694 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev8/SimPEG/utils/pgi_utils.py
--rw-r--r--   0        0        0    12916 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev8/SimPEG/utils/plot_utils.py
--rw-r--r--   0        0        0    10049 2024-01-11 21:39:39.376935 mira_simpeg-0.19.0.dev8/SimPEG/utils/solver_utils.py
--rw-r--r--   0        0        0     8080 1970-01-01 00:00:00.000000 mira_simpeg-0.19.0.dev8/PKG-INFO
+-rw-r--r--   0        0        0     1357 2024-04-23 21:36:15.037227 mira_simpeg-1!0.19.0.8a2/AUTHORS.rst
+-rw-r--r--   0        0        0     1109 2024-04-23 21:36:15.038868 mira_simpeg-1!0.19.0.8a2/LICENSE
+-rw-r--r--   0        0        0     3000 2024-04-26 21:48:13.008514 mira_simpeg-1!0.19.0.8a2/pyproject.toml
+-rw-r--r--   0        0        0     6106 2024-04-23 21:36:15.039948 mira_simpeg-1!0.19.0.8a2/README.rst
+-rw-r--r--   0        0        0     3458 2024-04-26 21:24:55.674602 mira_simpeg-1!0.19.0.8a2/SimPEG/__init__.py
+-rw-r--r--   0        0        0      158 2024-04-23 21:36:15.041080 mira_simpeg-1!0.19.0.8a2/SimPEG/base/__init__.py
+-rw-r--r--   0        0        0    17746 2024-04-23 21:44:49.705229 mira_simpeg-1!0.19.0.8a2/SimPEG/base/pde_simulation.py
+-rw-r--r--   0        0        0      895 2024-04-23 21:44:49.705229 mira_simpeg-1!0.19.0.8a2/SimPEG/dask/__init__.py
+-rw-r--r--   0        0        0     2856 2024-04-23 21:44:49.706330 mira_simpeg-1!0.19.0.8a2/SimPEG/dask/data_misfit.py
+-rw-r--r--   0        0        0        0 2024-04-23 21:36:15.042141 mira_simpeg-1!0.19.0.8a2/SimPEG/dask/electromagnetics/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 21:44:49.706330 mira_simpeg-1!0.19.0.8a2/SimPEG/dask/electromagnetics/frequency_domain/__init__.py
+-rw-r--r--   0        0        0     7742 2024-04-23 21:44:49.707875 mira_simpeg-1!0.19.0.8a2/SimPEG/dask/electromagnetics/frequency_domain/simulation.py
+-rw-r--r--   0        0        0        0 2024-04-23 21:36:15.042141 mira_simpeg-1!0.19.0.8a2/SimPEG/dask/electromagnetics/static/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 21:36:15.042141 mira_simpeg-1!0.19.0.8a2/SimPEG/dask/electromagnetics/static/induced_polarization/__init__.py
+-rw-r--r--   0        0        0     4104 2024-04-23 21:44:49.708382 mira_simpeg-1!0.19.0.8a2/SimPEG/dask/electromagnetics/static/induced_polarization/simulation.py
+-rw-r--r--   0        0        0     1869 2024-04-23 21:44:49.708382 mira_simpeg-1!0.19.0.8a2/SimPEG/dask/electromagnetics/static/induced_polarization/simulation_2d.py
+-rw-r--r--   0        0        0        0 2024-04-23 21:36:15.043210 mira_simpeg-1!0.19.0.8a2/SimPEG/dask/electromagnetics/static/resistivity/__init__.py
+-rw-r--r--   0        0        0     5153 2024-04-23 21:44:49.709450 mira_simpeg-1!0.19.0.8a2/SimPEG/dask/electromagnetics/static/resistivity/simulation.py
+-rw-r--r--   0        0        0     6529 2024-04-23 21:44:49.710497 mira_simpeg-1!0.19.0.8a2/SimPEG/dask/electromagnetics/static/resistivity/simulation_2d.py
+-rw-r--r--   0        0        0        0 2024-04-23 21:44:49.710580 mira_simpeg-1!0.19.0.8a2/SimPEG/dask/electromagnetics/time_domain/__init__.py
+-rw-r--r--   0        0        0    18322 2024-04-26 06:15:50.840542 mira_simpeg-1!0.19.0.8a2/SimPEG/dask/electromagnetics/time_domain/simulation.py
+-rw-r--r--   0        0        0     7379 2024-04-23 21:44:49.711582 mira_simpeg-1!0.19.0.8a2/SimPEG/dask/inverse_problem.py
+-rw-r--r--   0        0        0     4523 2024-04-23 21:44:49.711582 mira_simpeg-1!0.19.0.8a2/SimPEG/dask/objective_function.py
+-rw-r--r--   0        0        0        0 2024-04-23 21:36:15.043210 mira_simpeg-1!0.19.0.8a2/SimPEG/dask/potential_fields/__init__.py
+-rw-r--r--   0        0        0     3907 2024-04-23 21:44:49.712635 mira_simpeg-1!0.19.0.8a2/SimPEG/dask/potential_fields/base.py
+-rw-r--r--   0        0        0        0 2024-04-23 21:36:15.044222 mira_simpeg-1!0.19.0.8a2/SimPEG/dask/potential_fields/gravity/__init__.py
+-rw-r--r--   0        0        0      660 2024-04-23 21:44:49.714319 mira_simpeg-1!0.19.0.8a2/SimPEG/dask/potential_fields/gravity/simulation.py
+-rw-r--r--   0        0        0        0 2024-04-23 21:36:15.045283 mira_simpeg-1!0.19.0.8a2/SimPEG/dask/potential_fields/magnetics/__init__.py
+-rw-r--r--   0        0        0     1041 2024-04-23 21:44:49.714825 mira_simpeg-1!0.19.0.8a2/SimPEG/dask/potential_fields/magnetics/simulation.py
+-rw-r--r--   0        0        0     6763 2024-04-23 21:44:49.715438 mira_simpeg-1!0.19.0.8a2/SimPEG/dask/simulation.py
+-rw-r--r--   0        0        0     3132 2024-04-26 06:15:50.842746 mira_simpeg-1!0.19.0.8a2/SimPEG/dask/utils.py
+-rw-r--r--   0        0        0    14075 2024-04-23 21:36:15.046407 mira_simpeg-1!0.19.0.8a2/SimPEG/data.py
+-rw-r--r--   0        0        0     7307 2024-04-23 21:44:49.717648 mira_simpeg-1!0.19.0.8a2/SimPEG/data_misfit.py
+-rw-r--r--   0        0        0      917 2024-04-23 21:44:49.717648 mira_simpeg-1!0.19.0.8a2/SimPEG/directives/__init__.py
+-rw-r--r--   0        0        0   109257 2024-04-23 21:44:49.719768 mira_simpeg-1!0.19.0.8a2/SimPEG/directives/directives.py
+-rw-r--r--   0        0        0    19820 2024-04-23 21:36:15.048409 mira_simpeg-1!0.19.0.8a2/SimPEG/directives/pgi_directives.py
+-rw-r--r--   0        0        0    13400 2024-04-23 21:36:15.049515 mira_simpeg-1!0.19.0.8a2/SimPEG/directives/sim_directives.py
+-rw-r--r--   0        0        0     1133 2024-04-23 21:44:49.719768 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/__init__.py
+-rw-r--r--   0        0        0      210 2024-04-23 21:36:15.052838 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/analytics/__init__.py
+-rw-r--r--   0        0        0     7105 2024-04-23 21:36:15.049515 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/analytics/DC.py
+-rw-r--r--   0        0        0     8525 2024-04-23 21:44:49.720911 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/analytics/FDEM.py
+-rw-r--r--   0        0        0     5084 2024-04-23 21:36:15.051718 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/analytics/FDEMcasing.py
+-rw-r--r--   0        0        0    11443 2024-04-23 21:36:15.050575 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/analytics/FDEMDipolarfields.py
+-rw-r--r--   0        0        0     5853 2024-04-23 21:36:15.051718 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/analytics/NSEM.py
+-rw-r--r--   0        0        0     5381 2024-04-23 21:36:15.052754 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/analytics/TDEM.py
+-rw-r--r--   0        0        0     6977 2024-04-23 21:36:15.052838 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/base.py
+-rw-r--r--   0        0        0    23172 2024-04-23 21:44:49.721994 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/base_1d.py
+-rw-r--r--   0        0        0     2011 2024-04-23 21:36:15.053892 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/frequency_domain/__init__.py
+-rw-r--r--   0        0        0    60417 2024-04-23 21:36:15.054895 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/frequency_domain/fields.py
+-rw-r--r--   0        0        0    13112 2024-04-23 21:36:15.054895 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/frequency_domain/receivers.py
+-rw-r--r--   0        0        0    27311 2024-04-23 21:36:15.056005 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/frequency_domain/simulation.py
+-rw-r--r--   0        0        0    11528 2024-04-23 21:36:15.057115 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/frequency_domain/simulation_1d.py
+-rw-r--r--   0        0        0    43188 2024-04-23 21:36:15.058229 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/frequency_domain/sources.py
+-rw-r--r--   0        0        0     2795 2024-04-23 21:36:15.058229 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/frequency_domain/survey.py
+-rw-r--r--   0        0        0     1755 2024-04-23 21:36:15.059314 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/__init__.py
+-rw-r--r--   0        0        0    26411 2024-04-23 21:36:15.059314 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/fields.py
+-rw-r--r--   0        0        0    22562 2024-04-23 21:44:49.721994 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/receivers.py
+-rw-r--r--   0        0        0    27228 2024-04-23 21:36:15.060316 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/simulation.py
+-rw-r--r--   0        0        0    12406 2024-04-23 21:44:49.723059 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/simulation_1d.py
+-rw-r--r--   0        0        0     7644 2024-04-23 21:36:15.061455 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/sources.py
+-rw-r--r--   0        0        0     8922 2024-04-23 21:36:15.061455 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/survey.py
+-rw-r--r--   0        0        0      793 2024-04-23 21:36:15.062549 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/utils/__init__.py
+-rw-r--r--   0        0        0     5445 2024-04-23 21:36:15.062549 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/utils/analytic_1d.py
+-rw-r--r--   0        0        0    18826 2024-04-23 21:36:15.063623 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/utils/data_utils.py
+-rw-r--r--   0        0        0     5072 2024-04-23 21:36:15.063623 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/utils/data_viewer.py
+-rw-r--r--   0        0        0     7488 2024-04-23 21:36:15.064765 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/utils/edi_files_utils.py
+-rw-r--r--   0        0        0    22004 2024-04-23 21:36:15.064765 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/utils/plot_data_types.py
+-rw-r--r--   0        0        0    30007 2024-04-23 21:36:15.065754 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/utils/plot_utils.py
+-rw-r--r--   0        0        0     1338 2024-04-23 21:36:15.066861 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/utils/solutions_1d.py
+-rw-r--r--   0        0        0     7617 2024-04-23 21:36:15.066861 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/utils/source_utils.py
+-rw-r--r--   0        0        0    18430 2024-04-23 21:36:15.067956 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/utils/test_utils.py
+-rw-r--r--   0        0        0      129 2024-04-23 21:36:15.067956 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/__init__.py
+-rw-r--r--   0        0        0     1212 2024-04-23 21:36:15.069041 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/induced_polarization/__init__.py
+-rw-r--r--   0        0        0     2144 2024-04-23 21:36:15.069041 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/induced_polarization/run.py
+-rw-r--r--   0        0        0     4194 2024-04-23 21:44:49.724179 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/induced_polarization/simulation.py
+-rw-r--r--   0        0        0      637 2024-04-23 21:36:15.070115 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/induced_polarization/survey.py
+-rw-r--r--   0        0        0     2050 2024-04-23 21:36:15.071217 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/resistivity/__init__.py
+-rw-r--r--   0        0        0     8282 2024-04-23 21:36:15.072281 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/resistivity/fields.py
+-rw-r--r--   0        0        0     8412 2024-04-23 21:36:15.072281 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/resistivity/fields_2d.py
+-rw-r--r--   0        0        0    41758 2024-04-23 21:36:15.071217 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/resistivity/IODC.py
+-rw-r--r--   0        0        0    16671 2024-04-23 21:36:15.073369 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/resistivity/receivers.py
+-rw-r--r--   0        0        0     2089 2024-04-23 21:36:15.073369 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/resistivity/run.py
+-rw-r--r--   0        0        0    22651 2024-04-23 21:44:49.724687 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/resistivity/simulation.py
+-rw-r--r--   0        0        0    11514 2024-04-23 21:36:15.074421 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/resistivity/simulation_1d.py
+-rw-r--r--   0        0        0    27954 2024-04-23 21:44:49.725753 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/resistivity/simulation_2d.py
+-rw-r--r--   0        0        0     7782 2024-04-23 21:36:15.075508 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/resistivity/sources.py
+-rw-r--r--   0        0        0    12123 2024-04-23 21:36:15.075508 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/resistivity/survey.py
+-rw-r--r--   0        0        0     4071 2024-04-23 21:36:15.076561 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/resistivity/utils.py
+-rw-r--r--   0        0        0     1656 2024-04-23 21:36:15.076561 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/spectral_induced_polarization/__init__.py
+-rw-r--r--   0        0        0     2105 2024-04-23 21:36:15.077663 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/spectral_induced_polarization/data.py
+-rw-r--r--   0        0        0    14850 2024-04-23 21:36:15.077663 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/spectral_induced_polarization/receivers.py
+-rw-r--r--   0        0        0     5028 2024-04-23 21:36:15.077663 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/spectral_induced_polarization/run.py
+-rw-r--r--   0        0        0    21261 2024-04-23 21:36:15.078662 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/spectral_induced_polarization/simulation.py
+-rw-r--r--   0        0        0     2962 2024-04-23 21:36:15.078662 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/spectral_induced_polarization/simulation_2d.py
+-rw-r--r--   0        0        0     8465 2024-04-23 21:36:15.079665 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/spectral_induced_polarization/sources.py
+-rw-r--r--   0        0        0     4149 2024-04-23 21:36:15.079753 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/spectral_induced_polarization/survey.py
+-rw-r--r--   0        0        0     1124 2024-04-23 21:44:49.726812 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/spontaneous_potential/__init__.py
+-rw-r--r--   0        0        0     6658 2024-04-23 21:44:49.726812 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/spontaneous_potential/simulation.py
+-rw-r--r--   0        0        0     1011 2024-04-23 21:36:15.080817 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/spontaneous_potential/sources.py
+-rw-r--r--   0        0        0     1950 2024-04-23 21:36:15.080817 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/utils/__init__.py
+-rw-r--r--   0        0        0    66992 2024-04-23 21:36:15.083042 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/utils/static_utils.py
+-rw-r--r--   0        0        0     2290 2024-04-23 21:36:15.084141 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/time_domain/__init__.py
+-rw-r--r--   0        0        0    24117 2024-04-23 21:44:49.727873 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/time_domain/fields.py
+-rw-r--r--   0        0        0    12502 2024-04-23 21:44:49.728990 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/time_domain/receivers.py
+-rw-r--r--   0        0        0    39494 2024-04-23 21:36:15.085209 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/time_domain/simulation.py
+-rw-r--r--   0        0        0    14465 2024-04-23 21:36:15.086334 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/time_domain/simulation_1d.py
+-rw-r--r--   0        0        0    71847 2024-04-23 21:44:49.730237 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/time_domain/sources.py
+-rw-r--r--   0        0        0     1070 2024-04-23 21:36:15.087424 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/time_domain/survey.py
+-rw-r--r--   0        0        0      947 2024-04-23 21:36:15.087424 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/utils/__init__.py
+-rw-r--r--   0        0        0    16473 2024-04-23 21:36:15.088491 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/utils/current_utils.py
+-rw-r--r--   0        0        0     6593 2024-04-23 21:36:15.088491 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/utils/em1d_utils.py
+-rw-r--r--   0        0        0     5831 2024-04-23 21:36:15.088491 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/utils/testing_utils.py
+-rw-r--r--   0        0        0     3578 2024-04-23 21:36:15.089533 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/utils/waveform_utils.py
+-rw-r--r--   0        0        0     1528 2024-04-23 21:36:15.089621 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/viscous_remanent_magnetization/__init__.py
+-rw-r--r--   0        0        0     6800 2024-04-23 21:36:15.089621 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/viscous_remanent_magnetization/receivers.py
+-rw-r--r--   0        0        0    39890 2024-04-23 21:36:15.090712 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/viscous_remanent_magnetization/simulation.py
+-rw-r--r--   0        0        0    18560 2024-04-23 21:44:49.731331 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/viscous_remanent_magnetization/sources.py
+-rw-r--r--   0        0        0     2338 2024-04-23 21:36:15.091810 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/viscous_remanent_magnetization/survey.py
+-rw-r--r--   0        0        0    20152 2024-04-23 21:36:15.091810 mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/viscous_remanent_magnetization/waveforms.py
+-rw-r--r--   0        0        0    13959 2024-04-23 21:44:49.731331 mira_simpeg-1!0.19.0.8a2/SimPEG/fields.py
+-rw-r--r--   0        0        0       24 2024-04-23 21:36:15.092892 mira_simpeg-1!0.19.0.8a2/SimPEG/flow/__init__.py
+-rw-r--r--   0        0        0     1136 2024-04-23 21:36:15.094094 mira_simpeg-1!0.19.0.8a2/SimPEG/flow/richards/__init__.py
+-rw-r--r--   0        0        0    33981 2024-04-23 21:36:15.094094 mira_simpeg-1!0.19.0.8a2/SimPEG/flow/richards/empirical.py
+-rw-r--r--   0        0        0     3618 2024-04-23 21:36:15.095187 mira_simpeg-1!0.19.0.8a2/SimPEG/flow/richards/receivers.py
+-rw-r--r--   0        0        0    13567 2024-04-23 21:36:15.095187 mira_simpeg-1!0.19.0.8a2/SimPEG/flow/richards/simulation.py
+-rw-r--r--   0        0        0     2798 2024-04-23 21:44:49.732393 mira_simpeg-1!0.19.0.8a2/SimPEG/flow/richards/survey.py
+-rw-r--r--   0        0        0    10625 2024-04-23 21:36:15.096365 mira_simpeg-1!0.19.0.8a2/SimPEG/inverse_problem.py
+-rw-r--r--   0        0        0     3329 2024-04-23 21:36:15.096365 mira_simpeg-1!0.19.0.8a2/SimPEG/inversion.py
+-rw-r--r--   0        0        0   213269 2024-04-23 21:44:49.734614 mira_simpeg-1!0.19.0.8a2/SimPEG/maps.py
+-rw-r--r--   0        0        0     1527 2024-04-23 21:36:15.099474 mira_simpeg-1!0.19.0.8a2/SimPEG/meta/__init__.py
+-rw-r--r--   0        0        0    16903 2024-04-23 21:36:15.099474 mira_simpeg-1!0.19.0.8a2/SimPEG/meta/simulation.py
+-rw-r--r--   0        0        0     1218 2024-04-23 21:36:15.099474 mira_simpeg-1!0.19.0.8a2/SimPEG/models.py
+-rw-r--r--   0        0        0    14724 2024-04-23 21:44:49.734614 mira_simpeg-1!0.19.0.8a2/SimPEG/objective_function.py
+-rw-r--r--   0        0        0    39604 2024-04-23 21:44:49.735673 mira_simpeg-1!0.19.0.8a2/SimPEG/optimization.py
+-rw-r--r--   0        0        0      589 2024-04-23 21:36:15.101974 mira_simpeg-1!0.19.0.8a2/SimPEG/potential_fields/__init__.py
+-rw-r--r--   0        0        0    13464 2024-04-23 21:44:49.736672 mira_simpeg-1!0.19.0.8a2/SimPEG/potential_fields/base.py
+-rw-r--r--   0        0        0     1100 2024-04-23 21:44:49.737762 mira_simpeg-1!0.19.0.8a2/SimPEG/potential_fields/gravity/__init__.py
+-rw-r--r--   0        0        0     2272 2024-04-23 21:36:15.103050 mira_simpeg-1!0.19.0.8a2/SimPEG/potential_fields/gravity/analytics.py
+-rw-r--r--   0        0        0     2271 2024-04-23 21:36:15.103050 mira_simpeg-1!0.19.0.8a2/SimPEG/potential_fields/gravity/receivers.py
+-rw-r--r--   0        0        0     9057 2024-04-23 21:44:49.737762 mira_simpeg-1!0.19.0.8a2/SimPEG/potential_fields/gravity/simulation.py
+-rw-r--r--   0        0        0      407 2024-04-23 21:36:15.104116 mira_simpeg-1!0.19.0.8a2/SimPEG/potential_fields/gravity/sources.py
+-rw-r--r--   0        0        0     4774 2024-04-23 21:36:15.104116 mira_simpeg-1!0.19.0.8a2/SimPEG/potential_fields/gravity/survey.py
+-rw-r--r--   0        0        0     1174 2024-04-23 21:36:15.105238 mira_simpeg-1!0.19.0.8a2/SimPEG/potential_fields/magnetics/__init__.py
+-rw-r--r--   0        0        0     9821 2024-04-23 21:36:15.105238 mira_simpeg-1!0.19.0.8a2/SimPEG/potential_fields/magnetics/analytics.py
+-rw-r--r--   0        0        0     2228 2024-04-23 21:36:15.106353 mira_simpeg-1!0.19.0.8a2/SimPEG/potential_fields/magnetics/receivers.py
+-rw-r--r--   0        0        0    31502 2024-04-23 21:44:49.738852 mira_simpeg-1!0.19.0.8a2/SimPEG/potential_fields/magnetics/simulation.py
+-rw-r--r--   0        0        0     3669 2024-04-23 21:36:15.107357 mira_simpeg-1!0.19.0.8a2/SimPEG/potential_fields/magnetics/sources.py
+-rw-r--r--   0        0        0     2693 2024-04-23 21:36:15.107357 mira_simpeg-1!0.19.0.8a2/SimPEG/potential_fields/magnetics/survey.py
+-rw-r--r--   0        0        0    15572 2024-04-23 21:44:49.738852 mira_simpeg-1!0.19.0.8a2/SimPEG/props.py
+-rw-r--r--   0        0        0     8134 2024-04-23 21:44:49.739851 mira_simpeg-1!0.19.0.8a2/SimPEG/regularization/__init__.py
+-rw-r--r--   0        0        0    43137 2024-04-23 21:44:49.740935 mira_simpeg-1!0.19.0.8a2/SimPEG/regularization/base.py
+-rw-r--r--   0        0        0     3908 2024-04-23 21:36:15.109568 mira_simpeg-1!0.19.0.8a2/SimPEG/regularization/correspondence.py
+-rw-r--r--   0        0        0     9843 2024-04-23 21:44:49.740935 mira_simpeg-1!0.19.0.8a2/SimPEG/regularization/cross_gradient.py
+-rw-r--r--   0        0        0     5244 2024-04-23 21:36:15.110567 mira_simpeg-1!0.19.0.8a2/SimPEG/regularization/jtv.py
+-rw-r--r--   0        0        0    32347 2024-04-23 21:44:49.742023 mira_simpeg-1!0.19.0.8a2/SimPEG/regularization/pgi.py
+-rw-r--r--   0        0        0    16758 2024-04-23 21:44:49.743023 mira_simpeg-1!0.19.0.8a2/SimPEG/regularization/regularization_mesh.py
+-rw-r--r--   0        0        0    10363 2024-04-23 21:44:49.744026 mira_simpeg-1!0.19.0.8a2/SimPEG/regularization/sparse.py
+-rw-r--r--   0        0        0       39 2024-04-23 21:36:15.112709 mira_simpeg-1!0.19.0.8a2/SimPEG/seismic/__init__.py
+-rw-r--r--   0        0        0      760 2024-04-23 21:36:15.112709 mira_simpeg-1!0.19.0.8a2/SimPEG/seismic/straight_ray_tomography/__init__.py
+-rw-r--r--   0        0        0     3578 2024-04-23 21:36:15.113787 mira_simpeg-1!0.19.0.8a2/SimPEG/seismic/straight_ray_tomography/simulation.py
+-rw-r--r--   0        0        0     1688 2024-04-23 21:36:15.113787 mira_simpeg-1!0.19.0.8a2/SimPEG/seismic/straight_ray_tomography/survey.py
+-rw-r--r--   0        0        0    19552 2024-04-23 21:44:49.744114 mira_simpeg-1!0.19.0.8a2/SimPEG/simulation.py
+-rw-r--r--   0        0        0    17616 2024-04-23 21:44:49.745235 mira_simpeg-1!0.19.0.8a2/SimPEG/survey.py
+-rw-r--r--   0        0        0     6705 2024-04-23 21:44:49.746464 mira_simpeg-1!0.19.0.8a2/SimPEG/utils/__init__.py
+-rw-r--r--   0        0        0    39084 2024-04-23 21:44:49.747464 mira_simpeg-1!0.19.0.8a2/SimPEG/utils/code_utils.py
+-rw-r--r--   0        0        0      531 2024-04-23 21:36:15.117440 mira_simpeg-1!0.19.0.8a2/SimPEG/utils/coord_utils.py
+-rw-r--r--   0        0        0     4104 2024-04-23 21:36:15.117440 mira_simpeg-1!0.19.0.8a2/SimPEG/utils/counter_utils.py
+-rw-r--r--   0        0        0      687 2024-04-23 21:36:15.117440 mira_simpeg-1!0.19.0.8a2/SimPEG/utils/curv_utils.py
+-rw-r--r--   0        0        0       98 2024-04-23 21:36:15.118440 mira_simpeg-1!0.19.0.8a2/SimPEG/utils/drivers/__init__.py
+-rw-r--r--   0        0        0     8117 2024-04-23 21:44:49.748551 mira_simpeg-1!0.19.0.8a2/SimPEG/utils/drivers/gravity_driver.py
+-rw-r--r--   0        0        0     9736 2024-04-23 21:44:49.748551 mira_simpeg-1!0.19.0.8a2/SimPEG/utils/drivers/magnetics_driver.py
+-rw-r--r--   0        0        0      631 2024-04-23 21:36:15.119520 mira_simpeg-1!0.19.0.8a2/SimPEG/utils/io_utils/__init__.py
+-rw-r--r--   0        0        0    36848 2024-04-23 21:36:15.120522 mira_simpeg-1!0.19.0.8a2/SimPEG/utils/io_utils/io_utils_electromagnetics.py
+-rw-r--r--   0        0        0     4825 2024-04-23 21:44:49.749552 mira_simpeg-1!0.19.0.8a2/SimPEG/utils/io_utils/io_utils_general.py
+-rw-r--r--   0        0        0    13183 2024-04-23 21:44:49.749552 mira_simpeg-1!0.19.0.8a2/SimPEG/utils/io_utils/io_utils_pf.py
+-rw-r--r--   0        0        0    14546 2024-04-23 21:44:49.750679 mira_simpeg-1!0.19.0.8a2/SimPEG/utils/mat_utils.py
+-rw-r--r--   0        0        0     3480 2024-04-23 21:36:15.121641 mira_simpeg-1!0.19.0.8a2/SimPEG/utils/mesh_utils.py
+-rw-r--r--   0        0        0    16902 2024-04-23 21:44:49.750679 mira_simpeg-1!0.19.0.8a2/SimPEG/utils/model_builder.py
+-rw-r--r--   0        0        0     7038 2024-04-23 21:36:15.122641 mira_simpeg-1!0.19.0.8a2/SimPEG/utils/model_utils.py
+-rw-r--r--   0        0        0    67694 2024-04-23 21:36:15.123707 mira_simpeg-1!0.19.0.8a2/SimPEG/utils/pgi_utils.py
+-rw-r--r--   0        0        0    12916 2024-04-23 21:36:15.123707 mira_simpeg-1!0.19.0.8a2/SimPEG/utils/plot_utils.py
+-rw-r--r--   0        0        0    10049 2024-04-23 21:36:15.124818 mira_simpeg-1!0.19.0.8a2/SimPEG/utils/solver_utils.py
+-rw-r--r--   0        0        0     8081 1970-01-01 00:00:00.000000 mira_simpeg-1!0.19.0.8a2/PKG-INFO
```

### Comparing `mira_simpeg-0.19.0.dev8/LICENSE` & `mira_simpeg-1!0.19.0.8a2/LICENSE`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/pyproject.toml` & `mira_simpeg-1!0.19.0.8a2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #SimPEG: Simulation and Parameter Estimation in Geophysics
 #
 #SimPEG is a python package for simulation and gradient based
 #parameter estimation in the context of geophysical applications.
 
 [tool.poetry]
 name = "Mira-SimPEG"
-version = "0.19.0.dev8"
+version = "1!0.19.0.8a2"
 license = "MIT"
 description = "Mira Geoscience fork of SimPEG: Simulation and Parameter Estimation in Geophysics"
 
 authors = ["Rowan Cockett <rowanc1@gmail.com>", "dominiquef@mirageoscience.com"]
 repository = "http://github.com/simpeg/simpeg"
 documentation = "https://docs.simpeg.xyz/"
 homepage = "http://simpeg.xyz/"
@@ -32,18 +32,27 @@
 
 packages = [
     { include = "SimPEG" },
 ]
 
 exclude = ["tests*", "examples*", "tutorials*"]
 
+include = [
+    "COPYING",
+    "COPYING.LESSER",
+    "LICENSE",
+    "README.rst",
+    "THIRD_PARTY_SOFTWARE.rst",
+]
+
 [tool.poetry.dependencies]
 discretize = ">=0.8.0"
 empymod = ">=2.0.0"
 geoh5py = {version = "*", allow-prereleases = true}
+#geoh5py = {url = "http://localhost:8888/geoh5py.tar.gz#sha256="}
 numpy = ">=1.20"
 pandas = "*"
 pymatsolver = ">=0.2"
 scikit-learn = ">=1.2"
 scipy = ">=1.8.0"
 
 dask = {version = "*", optional = true}
```

### Comparing `mira_simpeg-0.19.0.dev8/README.rst` & `mira_simpeg-1!0.19.0.8a2/README.rst`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/__init__.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/base/pde_simulation.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/base/pde_simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/dask/__init__.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/dask/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/dask/data_misfit.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/dask/data_misfit.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/frequency_domain/simulation.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/dask/electromagnetics/frequency_domain/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/static/induced_polarization/simulation.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/dask/electromagnetics/static/induced_polarization/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/static/induced_polarization/simulation_2d.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/dask/electromagnetics/static/induced_polarization/simulation_2d.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/static/resistivity/simulation.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/dask/electromagnetics/static/resistivity/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/static/resistivity/simulation_2d.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/dask/electromagnetics/static/resistivity/simulation_2d.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/dask/electromagnetics/time_domain/simulation.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/dask/electromagnetics/time_domain/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/dask/inverse_problem.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/dask/inverse_problem.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/dask/objective_function.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/dask/objective_function.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/dask/potential_fields/base.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/dask/potential_fields/base.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/dask/potential_fields/gravity/simulation.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/dask/potential_fields/gravity/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/dask/potential_fields/magnetics/simulation.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/dask/potential_fields/magnetics/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/dask/simulation.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/dask/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/dask/utils.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/dask/utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/data.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/data.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/data_misfit.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/data_misfit.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/directives/__init__.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/directives/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/directives/directives.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/directives/directives.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/directives/pgi_directives.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/directives/pgi_directives.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/directives/sim_directives.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/directives/sim_directives.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/__init__.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/analytics/DC.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/analytics/DC.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/analytics/FDEM.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/analytics/FDEM.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/analytics/FDEMcasing.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/analytics/FDEMcasing.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/analytics/FDEMDipolarfields.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/analytics/FDEMDipolarfields.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/analytics/NSEM.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/analytics/NSEM.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/analytics/TDEM.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/analytics/TDEM.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/base.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/base.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/base_1d.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/base_1d.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/frequency_domain/__init__.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/frequency_domain/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/frequency_domain/fields.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/frequency_domain/fields.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/frequency_domain/receivers.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/frequency_domain/receivers.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/frequency_domain/simulation.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/frequency_domain/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/frequency_domain/simulation_1d.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/frequency_domain/simulation_1d.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/frequency_domain/sources.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/frequency_domain/sources.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/frequency_domain/survey.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/frequency_domain/survey.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/__init__.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/fields.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/fields.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/receivers.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/receivers.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/simulation.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/simulation_1d.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/simulation_1d.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/sources.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/sources.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/survey.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/survey.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/__init__.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/analytic_1d.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/utils/analytic_1d.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/data_utils.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/data_viewer.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/utils/data_viewer.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/edi_files_utils.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/utils/edi_files_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/plot_data_types.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/utils/plot_data_types.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/plot_utils.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/solutions_1d.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/utils/solutions_1d.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/source_utils.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/utils/source_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/natural_source/utils/test_utils.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/natural_source/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/induced_polarization/__init__.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/induced_polarization/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/induced_polarization/run.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/induced_polarization/run.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/induced_polarization/simulation.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/induced_polarization/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/induced_polarization/survey.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/induced_polarization/survey.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/__init__.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/resistivity/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/fields.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/resistivity/fields.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/fields_2d.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/resistivity/fields_2d.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/IODC.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/resistivity/IODC.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/receivers.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/resistivity/receivers.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/run.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/resistivity/run.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/simulation.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/resistivity/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/simulation_1d.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/resistivity/simulation_1d.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/simulation_2d.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/resistivity/simulation_2d.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/sources.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/resistivity/sources.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/survey.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/resistivity/survey.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/resistivity/utils.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/resistivity/utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/__init__.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/spectral_induced_polarization/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/data.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/spectral_induced_polarization/data.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/receivers.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/spectral_induced_polarization/receivers.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/run.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/spectral_induced_polarization/run.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/simulation.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/spectral_induced_polarization/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/simulation_2d.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/spectral_induced_polarization/simulation_2d.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/sources.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/spectral_induced_polarization/sources.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spectral_induced_polarization/survey.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/spectral_induced_polarization/survey.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spontaneous_potential/__init__.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/spontaneous_potential/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spontaneous_potential/simulation.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/spontaneous_potential/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/spontaneous_potential/sources.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/spontaneous_potential/sources.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/utils/__init__.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/static/utils/static_utils.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/static/utils/static_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/time_domain/__init__.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/time_domain/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/time_domain/fields.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/time_domain/fields.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/time_domain/receivers.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/time_domain/receivers.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/time_domain/simulation.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/time_domain/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/time_domain/simulation_1d.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/time_domain/simulation_1d.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/time_domain/sources.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/time_domain/sources.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/time_domain/survey.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/time_domain/survey.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/utils/__init__.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/utils/current_utils.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/utils/current_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/utils/em1d_utils.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/utils/em1d_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/utils/testing_utils.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/utils/testing_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/utils/waveform_utils.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/utils/waveform_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/viscous_remanent_magnetization/__init__.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/viscous_remanent_magnetization/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/viscous_remanent_magnetization/receivers.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/viscous_remanent_magnetization/receivers.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/viscous_remanent_magnetization/simulation.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/viscous_remanent_magnetization/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/viscous_remanent_magnetization/sources.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/viscous_remanent_magnetization/sources.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/viscous_remanent_magnetization/survey.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/viscous_remanent_magnetization/survey.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/electromagnetics/viscous_remanent_magnetization/waveforms.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/electromagnetics/viscous_remanent_magnetization/waveforms.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/fields.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/fields.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/flow/richards/__init__.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/flow/richards/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/flow/richards/empirical.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/flow/richards/empirical.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/flow/richards/receivers.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/flow/richards/receivers.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/flow/richards/simulation.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/flow/richards/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/flow/richards/survey.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/flow/richards/survey.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/inverse_problem.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/inverse_problem.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/inversion.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/inversion.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/maps.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/maps.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/meta/__init__.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/meta/simulation.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/meta/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/models.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/models.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/objective_function.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/objective_function.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/optimization.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/optimization.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/__init__.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/potential_fields/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/base.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/potential_fields/base.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/gravity/__init__.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/potential_fields/gravity/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/gravity/analytics.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/potential_fields/gravity/analytics.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/gravity/receivers.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/potential_fields/gravity/receivers.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/gravity/simulation.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/potential_fields/gravity/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/gravity/survey.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/potential_fields/gravity/survey.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/magnetics/__init__.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/potential_fields/magnetics/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/magnetics/analytics.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/potential_fields/magnetics/analytics.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/magnetics/receivers.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/potential_fields/magnetics/receivers.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/magnetics/simulation.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/potential_fields/magnetics/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/magnetics/sources.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/potential_fields/magnetics/sources.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/potential_fields/magnetics/survey.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/potential_fields/magnetics/survey.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/props.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/props.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/regularization/__init__.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/regularization/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/regularization/base.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/regularization/base.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/regularization/correspondence.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/regularization/correspondence.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/regularization/cross_gradient.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/regularization/cross_gradient.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/regularization/jtv.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/regularization/jtv.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/regularization/pgi.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/regularization/pgi.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/regularization/regularization_mesh.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/regularization/regularization_mesh.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/regularization/sparse.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/regularization/sparse.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/seismic/straight_ray_tomography/__init__.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/seismic/straight_ray_tomography/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/seismic/straight_ray_tomography/simulation.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/seismic/straight_ray_tomography/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/seismic/straight_ray_tomography/survey.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/seismic/straight_ray_tomography/survey.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/simulation.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/simulation.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/survey.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/survey.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/utils/__init__.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/utils/code_utils.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/utils/code_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/utils/coord_utils.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/utils/coord_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/utils/counter_utils.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/utils/counter_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/utils/curv_utils.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/utils/curv_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/utils/drivers/gravity_driver.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/utils/drivers/gravity_driver.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/utils/drivers/magnetics_driver.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/utils/drivers/magnetics_driver.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/utils/io_utils/__init__.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/utils/io_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/utils/io_utils/io_utils_electromagnetics.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/utils/io_utils/io_utils_electromagnetics.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/utils/io_utils/io_utils_general.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/utils/io_utils/io_utils_general.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/utils/io_utils/io_utils_pf.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/utils/io_utils/io_utils_pf.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/utils/mat_utils.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/utils/mat_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/utils/mesh_utils.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/utils/mesh_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/utils/model_builder.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/utils/model_builder.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/utils/model_utils.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/utils/pgi_utils.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/utils/pgi_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/utils/plot_utils.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/SimPEG/utils/solver_utils.py` & `mira_simpeg-1!0.19.0.8a2/SimPEG/utils/solver_utils.py`

 * *Files identical despite different names*

### Comparing `mira_simpeg-0.19.0.dev8/PKG-INFO` & `mira_simpeg-1!0.19.0.8a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mira-SimPEG
-Version: 0.19.0.dev8
+Version: 1!0.19.0.8a2
 Summary: Mira Geoscience fork of SimPEG: Simulation and Parameter Estimation in Geophysics
 Home-page: http://simpeg.xyz/
 License: MIT
 Keywords: geophysics inverse problem
 Author: Rowan Cockett
 Author-email: rowanc1@gmail.com
 Classifier: Development Status :: 4 - Beta
```

