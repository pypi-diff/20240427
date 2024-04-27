# Comparing `tmp/felupe-8.4.0.tar.gz` & `tmp/felupe-8.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "felupe-8.4.0.tar", last modified: Fri Apr 12 12:09:25 2024, max compression
+gzip compressed data, was "felupe-8.5.0.tar", last modified: Sat Apr 27 14:14:00 2024, max compression
```

## Comparing `felupe-8.4.0.tar` & `felupe-8.5.0.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.886152 felupe-8.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35081 2024-04-12 12:09:18.000000 felupe-8.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    55811 2024-04-12 12:09:25.886152 felupe-8.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12855 2024-04-12 12:09:18.000000 felupe-8.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-12 12:09:18.000000 felupe-8.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 12:09:25.886152 felupe-8.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.858152 felupe-8.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.858152 felupe-8.4.0/src/felupe/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.862152 felupe-8.4.0/src/felupe/assembly/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/assembly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/assembly/_axi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/assembly/_cartesian.py
--rw-r--r--   0 runner    (1001) docker     (127)     9937 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/assembly/_integral.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.862152 felupe-8.4.0/src/felupe/assembly/expression/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/assembly/expression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/assembly/expression/_basis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/assembly/expression/_bilinear.py
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/assembly/expression/_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/assembly/expression/_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/assembly/expression/_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/assembly/expression/_mixed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.866152 felupe-8.4.0/src/felupe/constitution/
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/constitution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/constitution/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/constitution/_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)    24929 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/constitution/_mixed.py
--rw-r--r--   0 runner    (1001) docker     (127)    17741 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/constitution/_models_hyperelasticity.py
--rw-r--r--   0 runner    (1001) docker     (127)    16167 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/constitution/_models_hyperelasticity_ad.py
--rw-r--r--   0 runner    (1001) docker     (127)    18221 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/constitution/_models_linear_elasticity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/constitution/_models_linear_elasticity_large_strain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/constitution/_models_pseudo_elasticity.py
--rw-r--r--   0 runner    (1001) docker     (127)    17580 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/constitution/_user_materials.py
--rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/constitution/_user_materials_hyperelastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/constitution/_user_materials_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    18040 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/constitution/_view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.866152 felupe-8.4.0/src/felupe/dof/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/dof/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8920 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/dof/_boundary.py
--rw-r--r--   0 runner    (1001) docker     (127)    20346 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/dof/_loadcase.py
--rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/dof/_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.866152 felupe-8.4.0/src/felupe/element/
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/element/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/element/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    18387 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/element/_hexahedron.py
--rw-r--r--   0 runner    (1001) docker     (127)    11420 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/element/_lagrange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/element/_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/element/_quad.py
--rw-r--r--   0 runner    (1001) docker     (127)     7853 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/element/_tetra.py
--rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/element/_triangle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.870152 felupe-8.4.0/src/felupe/field/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/field/_axi.py
--rw-r--r--   0 runner    (1001) docker     (127)    12182 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/field/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11297 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/field/_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/field/_dual.py
--rw-r--r--   0 runner    (1001) docker     (127)     5861 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/field/_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/field/_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/field/_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/field/_planestrain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.870152 felupe-8.4.0/src/felupe/math/
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/math/_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/math/_math.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/math/_solve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/math/_spatial.py
--rw-r--r--   0 runner    (1001) docker     (127)    45047 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/math/_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.874152 felupe-8.4.0/src/felupe/mechanics/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mechanics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8496 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mechanics/_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mechanics/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mechanics/_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    12227 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mechanics/_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mechanics/_multipoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mechanics/_pointload.py
--rw-r--r--   0 runner    (1001) docker     (127)    11473 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mechanics/_solidbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mechanics/_solidbody_gravity.py
--rw-r--r--   0 runner    (1001) docker     (127)    18763 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mechanics/_solidbody_incompressible.py
--rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mechanics/_solidbody_pressure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mechanics/_step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.874152 felupe-8.4.0/src/felupe/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mesh/_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    17192 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mesh/_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mesh/_discrete_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mesh/_dual.py
--rw-r--r--   0 runner    (1001) docker     (127)    15620 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mesh/_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mesh/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mesh/_line_rectangle_cube.py
--rw-r--r--   0 runner    (1001) docker     (127)    48808 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mesh/_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mesh/_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    32323 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/mesh/_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.878152 felupe-8.4.0/src/felupe/quadrature/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/quadrature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/quadrature/_gausslegendre.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/quadrature/_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/quadrature/_sphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/quadrature/_tetra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/quadrature/_triangle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.878152 felupe-8.4.0/src/felupe/region/
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/region/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14750 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/region/_boundary.py
--rw-r--r--   0 runner    (1001) docker     (127)    10703 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/region/_region.py
--rw-r--r--   0 runner    (1001) docker     (127)    19319 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/region/_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.878152 felupe-8.4.0/src/felupe/solve/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/solve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/solve/_solve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.878152 felupe-8.4.0/src/felupe/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/tools/_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13311 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/tools/_newton.py
--rw-r--r--   0 runner    (1001) docker     (127)    20261 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/tools/_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/tools/_post.py
--rw-r--r--   0 runner    (1001) docker     (127)    14006 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/tools/_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/tools/_save.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-12 12:09:18.000000 felupe-8.4.0/src/felupe/tools/_solve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.882152 felupe-8.4.0/src/felupe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    55811 2024-04-12 12:09:25.000000 felupe-8.4.0/src/felupe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-12 12:09:25.000000 felupe-8.4.0/src/felupe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:09:25.000000 felupe-8.4.0/src/felupe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-12 12:09:25.000000 felupe-8.4.0/src/felupe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 12:09:25.000000 felupe-8.4.0/src/felupe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:09:25.882152 felupe-8.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_basis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_bilinearform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_composite.py
--rw-r--r--   0 runner    (1001) docker     (127)    15877 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_constitution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_constitution_newton.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_dof.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     8348 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_math.py
--rw-r--r--   0 runner    (1001) docker     (127)    15767 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_mechanics.py
--rw-r--r--   0 runner    (1001) docker     (127)    15972 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_mpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_planestrain.py
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_quadrature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_readme.py
--rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_solve.py
--rw-r--r--   0 runner    (1001) docker     (127)    16175 2024-04-12 12:09:18.000000 felupe-8.4.0/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.133736 felupe-8.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35081 2024-04-27 14:13:54.000000 felupe-8.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    55533 2024-04-27 14:14:00.133736 felupe-8.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12577 2024-04-27 14:13:54.000000 felupe-8.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-27 14:13:54.000000 felupe-8.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 14:14:00.133736 felupe-8.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.105736 felupe-8.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.109736 felupe-8.5.0/src/felupe/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.109736 felupe-8.5.0/src/felupe/assembly/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/assembly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/assembly/_axi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/assembly/_cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9954 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/assembly/_integral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.113736 felupe-8.5.0/src/felupe/assembly/expression/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/assembly/expression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/assembly/expression/_basis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/assembly/expression/_bilinear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5846 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/assembly/expression/_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/assembly/expression/_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/assembly/expression/_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/assembly/expression/_mixed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.113736 felupe-8.5.0/src/felupe/constitution/
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/constitution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13345 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/constitution/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/constitution/_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24929 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/constitution/_mixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18171 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/constitution/_models_hyperelasticity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19611 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/constitution/_models_hyperelasticity_ad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18945 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/constitution/_models_linear_elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/constitution/_models_linear_elasticity_large_strain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/constitution/_models_pseudo_elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17580 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/constitution/_user_materials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12840 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/constitution/_user_materials_hyperelastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/constitution/_user_materials_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19014 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/constitution/_view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.117736 felupe-8.5.0/src/felupe/dof/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/dof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/dof/_boundary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21950 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/dof/_loadcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/dof/_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.117736 felupe-8.5.0/src/felupe/element/
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/element/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/element/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18359 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/element/_hexahedron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11406 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/element/_lagrange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/element/_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/element/_quad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/element/_tetra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/element/_triangle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.117736 felupe-8.5.0/src/felupe/field/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/field/_axi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12182 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/field/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11297 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/field/_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/field/_dual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5861 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/field/_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/field/_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/field/_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/field/_planestrain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.121736 felupe-8.5.0/src/felupe/math/
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/math/_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/math/_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/math/_solve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/math/_spatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45045 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/math/_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.121736 felupe-8.5.0/src/felupe/mechanics/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mechanics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mechanics/_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mechanics/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mechanics/_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12323 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mechanics/_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mechanics/_multipoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mechanics/_pointload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mechanics/_solidbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mechanics/_solidbody_gravity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18871 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mechanics/_solidbody_incompressible.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mechanics/_solidbody_pressure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mechanics/_step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.125736 felupe-8.5.0/src/felupe/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mesh/_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17231 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mesh/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mesh/_discrete_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mesh/_dual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15599 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mesh/_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mesh/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mesh/_line_rectangle_cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48571 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mesh/_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mesh/_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32125 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/mesh/_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.125736 felupe-8.5.0/src/felupe/quadrature/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/quadrature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7205 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/quadrature/_gausslegendre.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/quadrature/_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/quadrature/_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/quadrature/_tetra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/quadrature/_triangle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.125736 felupe-8.5.0/src/felupe/region/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/region/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14780 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/region/_boundary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10703 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/region/_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19319 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/region/_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.125736 felupe-8.5.0/src/felupe/solve/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/solve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/solve/_solve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.129736 felupe-8.5.0/src/felupe/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/tools/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13687 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/tools/_newton.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20261 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/tools/_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/tools/_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14006 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/tools/_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/tools/_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-27 14:13:54.000000 felupe-8.5.0/src/felupe/tools/_solve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.133736 felupe-8.5.0/src/felupe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    55533 2024-04-27 14:14:00.000000 felupe-8.5.0/src/felupe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-27 14:14:00.000000 felupe-8.5.0/src/felupe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 14:14:00.000000 felupe-8.5.0/src/felupe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-27 14:14:00.000000 felupe-8.5.0/src/felupe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-27 14:14:00.000000 felupe-8.5.0/src/felupe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:00.133736 felupe-8.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_basis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_bilinearform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16942 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_constitution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_constitution_newton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_dof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8348 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15767 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_mechanics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15972 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_mpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_planestrain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_quadrature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_solve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16175 2024-04-27 14:13:54.000000 felupe-8.5.0/tests/test_tools.py
```

### Comparing `felupe-8.4.0/LICENSE` & `felupe-8.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/PKG-INFO` & `felupe-8.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: felupe
-Version: 8.4.0
+Version: 8.5.0
 Summary: Finite Element Analysis
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -733,15 +733,15 @@
 Requires-Dist: felupe[io,parallel,plot,progress,view]; extra == "all"
 
 <p align="center">
   <a href="https://felupe.readthedocs.io/en/latest/?badge=latest"><img src="https://user-images.githubusercontent.com/5793153/235789118-eb03eb25-2556-401d-8a0f-580f37e72f8d.png" height="80px"/></a>
   <p align="center"><i>Finite element analysis for continuum mechanics of solid bodies.</i></p>
 </p>
 
-[![FElupe](https://img.shields.io/badge/%F0%9F%94%8D-FElupe-white)](https://felupe.readthedocs.io) [![PyPI version shields.io](https://img.shields.io/pypi/v/felupe.svg)](https://pypi.python.org/pypi/felupe/) [![Documentation Status](https://readthedocs.org/projects/felupe/badge/?version=latest)](https://felupe.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/felupe/branch/main/graph/badge.svg?token=J2QP6Y6LVH)](https://codecov.io/gh/adtzlr/felupe) [![DOI](https://zenodo.org/badge/360657894.svg)](https://zenodo.org/badge/latestdoi/360657894) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black) ![PyPI - Downloads](https://img.shields.io/pypi/dm/felupe) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/adtzlr/felupe-web/main?labpath=notebooks/binder/01_Getting-Started.ipynb) [![lite-badge](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://adtzlr.github.io/felupe-web/lab?path=01_Getting-Started.ipynb) <a target="_blank" href="https://colab.research.google.com/github/adtzlr/felupe-web/blob/main/notebooks/colab/01_Getting-Started.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
+[![FElupe](https://img.shields.io/badge/%F0%9F%94%8D-FElupe-white)](https://felupe.readthedocs.io) [![PyPI version shields.io](https://img.shields.io/pypi/v/felupe.svg)](https://pypi.python.org/pypi/felupe/) [![Documentation Status](https://readthedocs.org/projects/felupe/badge/?version=latest)](https://felupe.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![codecov](https://codecov.io/gh/adtzlr/felupe/branch/main/graph/badge.svg?token=J2QP6Y6LVH)](https://codecov.io/gh/adtzlr/felupe) [![DOI](https://zenodo.org/badge/360657894.svg)](https://zenodo.org/badge/latestdoi/360657894) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black) ![PyPI - Downloads](https://img.shields.io/pypi/dm/felupe) [![lite-badge](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://adtzlr.github.io/felupe-web/lab?path=01_Getting-Started.ipynb) <a target="_blank" href="https://colab.research.google.com/github/adtzlr/felupe-web/blob/main/notebooks/colab/01_Getting-Started.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
 
 FElupe is a Python 3.8+ 🐍 finite element analysis package 📦 focussing on the formulation and numerical solution of nonlinear problems in continuum mechanics 🔧 of solid bodies 🚂. Its name is a combination of FE (finite element) and the german word *Lupe* 🔍 (magnifying glass) as a synonym for getting an insight 📖 how a finite element analysis code 🧮 looks like under the hood 🕳️.
 
 <p align="center">
   <a href="https://felupe.readthedocs.io/en/latest/examples/ex01_beam.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex01_beam_thumb.png" height="160px"/></a> <a href="https://felupe.readthedocs.io/en/latest/examples/ex02_plate-with-hole.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex02_plate-with-hole_thumb.png" height="160px"/></a> <a 
   href="https://felupe.readthedocs.io/en/latest/examples/ex03_plasticity.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex03_plasticity_thumb.png" height="160px"/></a> <a 
   href="https://felupe.readthedocs.io/en/latest/examples/ex04_balloon.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex04_balloon_thumb.png" height="160px"/></a> <a
```

### Comparing `felupe-8.4.0/README.md` & `felupe-8.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <p align="center">
   <a href="https://felupe.readthedocs.io/en/latest/?badge=latest"><img src="https://user-images.githubusercontent.com/5793153/235789118-eb03eb25-2556-401d-8a0f-580f37e72f8d.png" height="80px"/></a>
   <p align="center"><i>Finite element analysis for continuum mechanics of solid bodies.</i></p>
 </p>
 
-[![FElupe](https://img.shields.io/badge/%F0%9F%94%8D-FElupe-white)](https://felupe.readthedocs.io) [![PyPI version shields.io](https://img.shields.io/pypi/v/felupe.svg)](https://pypi.python.org/pypi/felupe/) [![Documentation Status](https://readthedocs.org/projects/felupe/badge/?version=latest)](https://felupe.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/felupe/branch/main/graph/badge.svg?token=J2QP6Y6LVH)](https://codecov.io/gh/adtzlr/felupe) [![DOI](https://zenodo.org/badge/360657894.svg)](https://zenodo.org/badge/latestdoi/360657894) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black) ![PyPI - Downloads](https://img.shields.io/pypi/dm/felupe) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/adtzlr/felupe-web/main?labpath=notebooks/binder/01_Getting-Started.ipynb) [![lite-badge](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://adtzlr.github.io/felupe-web/lab?path=01_Getting-Started.ipynb) <a target="_blank" href="https://colab.research.google.com/github/adtzlr/felupe-web/blob/main/notebooks/colab/01_Getting-Started.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
+[![FElupe](https://img.shields.io/badge/%F0%9F%94%8D-FElupe-white)](https://felupe.readthedocs.io) [![PyPI version shields.io](https://img.shields.io/pypi/v/felupe.svg)](https://pypi.python.org/pypi/felupe/) [![Documentation Status](https://readthedocs.org/projects/felupe/badge/?version=latest)](https://felupe.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![codecov](https://codecov.io/gh/adtzlr/felupe/branch/main/graph/badge.svg?token=J2QP6Y6LVH)](https://codecov.io/gh/adtzlr/felupe) [![DOI](https://zenodo.org/badge/360657894.svg)](https://zenodo.org/badge/latestdoi/360657894) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black) ![PyPI - Downloads](https://img.shields.io/pypi/dm/felupe) [![lite-badge](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://adtzlr.github.io/felupe-web/lab?path=01_Getting-Started.ipynb) <a target="_blank" href="https://colab.research.google.com/github/adtzlr/felupe-web/blob/main/notebooks/colab/01_Getting-Started.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
 
 FElupe is a Python 3.8+ 🐍 finite element analysis package 📦 focussing on the formulation and numerical solution of nonlinear problems in continuum mechanics 🔧 of solid bodies 🚂. Its name is a combination of FE (finite element) and the german word *Lupe* 🔍 (magnifying glass) as a synonym for getting an insight 📖 how a finite element analysis code 🧮 looks like under the hood 🕳️.
 
 <p align="center">
   <a href="https://felupe.readthedocs.io/en/latest/examples/ex01_beam.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex01_beam_thumb.png" height="160px"/></a> <a href="https://felupe.readthedocs.io/en/latest/examples/ex02_plate-with-hole.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex02_plate-with-hole_thumb.png" height="160px"/></a> <a 
   href="https://felupe.readthedocs.io/en/latest/examples/ex03_plasticity.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex03_plasticity_thumb.png" height="160px"/></a> <a 
   href="https://felupe.readthedocs.io/en/latest/examples/ex04_balloon.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex04_balloon_thumb.png" height="160px"/></a> <a
```

#### html2text {}

```diff
@@ -3,23 +3,19 @@
        Finite element analysis for continuum mechanics of solid bodies.
 [![FElupe](https://img.shields.io/badge/%F0%9F%94%8D-FElupe-white)](https://
 felupe.readthedocs.io) [![PyPI version shields.io](https://img.shields.io/pypi/
 v/felupe.svg)](https://pypi.python.org/pypi/felupe/) [![Documentation Status]
 (https://readthedocs.org/projects/felupe/badge/?version=latest)](https://
 felupe.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://
 img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-
-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/
-Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov]
-(https://codecov.io/gh/adtzlr/felupe/branch/main/graph/
+3.0) [![codecov](https://codecov.io/gh/adtzlr/felupe/branch/main/graph/
 badge.svg?token=J2QP6Y6LVH)](https://codecov.io/gh/adtzlr/felupe) [![DOI]
 (https://zenodo.org/badge/360657894.svg)](https://zenodo.org/badge/latestdoi/
 360657894) ![Codestyle black](https://img.shields.io/badge/code%20style-black-
-black) ![PyPI - Downloads](https://img.shields.io/pypi/dm/felupe) [![Binder]
-(https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/adtzlr/
-felupe-web/main?labpath=notebooks/binder/01_Getting-Started.ipynb) [![lite-
+black) ![PyPI - Downloads](https://img.shields.io/pypi/dm/felupe) [![lite-
 badge](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://
 adtzlr.github.io/felupe-web/lab?path=01_Getting-Started.ipynb) _[_O_p_e_n_ _I_n
 _C_o_l_a_b_]FElupe is a Python 3.8+ ð finite element analysis package ð¦
 focussing on the formulation and numerical solution of nonlinear problems in
 continuum mechanics ð§ of solid bodies ð. Its name is a combination of FE
 (finite element) and the german word *Lupe* ð (magnifying glass) as a
 synonym for getting an insight ð how a finite element analysis code ð§®
```

### Comparing `felupe-8.4.0/pyproject.toml` & `felupe-8.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/__init__.py` & `felupe-8.5.0/src/felupe/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/assembly/_axi.py` & `felupe-8.5.0/src/felupe/assembly/_axi.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/assembly/_cartesian.py` & `felupe-8.5.0/src/felupe/assembly/_cartesian.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/assembly/_integral.py` & `felupe-8.5.0/src/felupe/assembly/_integral.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     Examples
     --------
     The stiffness matrix for a linear-elastic solid body on a cube out of hexahedrons
     is assembled as follows. First, the mesh, the region and the field objects are
     created.
 
     >>> import felupe as fem
-
+    >>>
     >>> mesh = fem.Cube(n=11)
     >>> region = fem.RegionHexahedron(mesh)
     >>> displacement = fem.Field(region, dim=3)
     >>> field = fem.FieldContainer([displacement])
 
     The (constant) fourth-order elasticity tensor for linear-elasticity is created with
     two trailing axes, one for each quadrature point and one for each cell. Due to the
@@ -125,15 +125,15 @@
         \frac{\boldsymbol{\partial \sigma}}{\partial \boldsymbol{\varepsilon}} =
         2 \mu \ \boldsymbol{I} \odot \boldsymbol{I} + \gamma \ \boldsymbol{I} \otimes
         \boldsymbol{I}
 
 
     >>> import numpy as np
     >>> from felupe.math import cdya, dya
-
+    >>>
     >>> mu, lmbda = 1.0, 2.0
     >>> I = np.eye(3).reshape(3, 3, 1, 1)
     >>> dSdE = 2 * mu * cdya(I, I) + lmbda * dya(I, I)
     >>> dSdE.shape
     (3, 3, 3, 3, 1, 1)
 
     The integral form object provides methods for cell-wise stiffness matrices via its
@@ -165,15 +165,15 @@
         \hat{K}_{aibk(c)} = \left( \frac{\partial h_a}{\partial x_J} \right)_{(qc)}
             \left( \frac{\partial \sigma_{ij}}{\partial \varepsilon_{kl}} \right)_{(qc)}
             \left( \frac{\partial h_b}{\partial x_L} \right)_{(qc)} ~ dv_{(qc)}
 
 
     >>> form = fem.IntegralForm([dSdE], v=field, dV=region.dV, u=field)
     >>> values = form.integrate(parallel=False)
-    >>> values.shape
+    >>> values[0].shape
     (8, 3, 8, 3, 1000)
 
     The cell-wise stiffness matrices are re-used to assemble the sparse system stiffness
     matrix. The parallel keyword argument enables a threaded assembly.
 
     ..  math::
```

### Comparing `felupe-8.4.0/src/felupe/assembly/expression/_basis.py` & `felupe-8.5.0/src/felupe/assembly/expression/_basis.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/assembly/expression/_bilinear.py` & `felupe-8.5.0/src/felupe/assembly/expression/_bilinear.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/assembly/expression/_decorator.py` & `felupe-8.5.0/src/felupe/assembly/expression/_decorator.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,23 +67,26 @@
     `scikit-fem <https://github.com/kinnala/scikit-fem>`_ offers. The
     :func:`felupe.Form` decorator handles a field container. The form class is similar,
     but not identical in its usage compared to :class:`felupe.IntegralForm`. It requires
     a callable function (with optional arguments and keyword arguments) instead of a
     pre-computed array to be passed. The bilinear form of linear elasticity serves as a
     reference example for the demonstration on how to use this feature of FElupe. The
     stiffness matrix is assembled for a unit cube out of hexahedrons.
-
-    >>> import felupe as fem
-    >>> 
-    >>> mesh = fem.Cube(n=11)
-    >>> region = fem.RegionHexahedron(mesh)
-    >>> displacement = fem.Field(region, dim=3)
-    >>> field = fem.FieldContainer([displacement])
-    >>> 
-    >>> boundaries, loadcase = fem.dof.uniaxial(field, move=0.5, clamped=True)
+    
+    ..  pyvista-plot::
+        :context:
+
+        >>> import felupe as fem
+        >>> 
+        >>> mesh = fem.Cube(n=6)
+        >>> region = fem.RegionHexahedron(mesh)
+        >>> displacement = fem.Field(region, dim=3)
+        >>> field = fem.FieldContainer([displacement])
+        >>> 
+        >>> boundaries, loadcase = fem.dof.uniaxial(field, move=0.5, clamped=True)
 
     The bilinear form of linear elasticity is defined as
 
     ..  math::
 
         a(v, u) = \int_\Omega 2 \mu \
             \delta\boldsymbol{\varepsilon} : \boldsymbol{\varepsilon} +
@@ -103,38 +106,39 @@
     of field (gradients) ``(v, u)`` followed by arguments and keyword arguments.
     Optionally, the integration/assembly may be performed in parallel (threaded).
     Please note that this is only faster for relatively large systems. The weak-form
     function is decorated by :func:`felupe.Form` where the appropriate fields are linked
     to ``v`` and ``u`` along with the gradient flags for both fields. Arguments as well
     as keyword arguments of the weak-form may be defined inside the decorator or as part
     of the assembly arguments.
-
-    >>> from felupe.math import ddot, trace, sym, grad
-    >>> 
-    >>> @fem.Form(
-    >>>     v=field, u=field, kwargs={"μ": 1.0, "λ": 2.0}
-    >>> )
-    >>> def bilinearform():
-    >>>     "A container for a bilinear form."
-    >>>
-    >>>     def linear_elasticity(v, u, μ, λ):
-    >>>         "Linear elasticity."
-    >>>
-    >>>         δε, ε = sym(grad(v)), sym(grad(u))
-    >>>         return 2 * μ * ddot(δε, ε) + λ * trace(δε) * trace(ε)
-    >>>
-    >>>     return [linear_elasticity,]
-    >>> 
-    >>> stiffness_matrix = bilinearform.assemble(v=field, u=field, parallel=False)
-    >>> 
-    >>> system = fem.solve.partition(
-    >>>     field, stiffness_matrix, dof1=loadcase["dof1"], dof0=loadcase["dof0"]
-    >>> )
-    >>> field += fem.solve.solve(*system, ext0=loadcase["ext0"])
-    >>> field.plot("Principal Values of Logarithmic Strain").show()
+    
+    ..  pyvista-plot::
+        :context:
+            
+        >>> from felupe.math import ddot, trace, sym, grad
+        >>> 
+        >>> @fem.Form(v=field, u=field, kwargs={"μ": 1.0, "λ": 2.0})
+        ... def bilinearform():
+        ...     "A container for a bilinear form."
+        ...
+        ...     def linear_elasticity(v, u, μ, λ):
+        ...         "Linear elasticity."
+        ...
+        ...         δε, ε = sym(grad(v)), sym(grad(u))
+        ...         return 2 * μ * ddot(δε, ε) + λ * trace(δε) * trace(ε)
+        ...
+        ...     return [linear_elasticity,]
+        >>> 
+        >>> stiffness_matrix = bilinearform.assemble(v=field, u=field, parallel=False)
+        >>> 
+        >>> system = fem.solve.partition(
+        ...     field, stiffness_matrix, dof1=loadcase["dof1"], dof0=loadcase["dof0"]
+        ... )
+        >>> field += fem.solve.solve(*system, ext0=loadcase["ext0"])
+        >>> field.plot("Principal Values of Logarithmic Strain").show()
 
     """
 
     def form(weakform):
         return FormExpression(
             weakform=weakform,
             v=v,
```

### Comparing `felupe-8.4.0/src/felupe/assembly/expression/_expression.py` & `felupe-8.5.0/src/felupe/assembly/expression/_expression.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/assembly/expression/_linear.py` & `felupe-8.5.0/src/felupe/assembly/expression/_linear.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/assembly/expression/_mixed.py` & `felupe-8.5.0/src/felupe/assembly/expression/_mixed.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/constitution/__init__.py` & `felupe-8.5.0/src/felupe/constitution/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/constitution/_kinematics.py` & `felupe-8.5.0/src/felupe/constitution/_kinematics.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/constitution/_mixed.py` & `felupe-8.5.0/src/felupe/constitution/_mixed.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/constitution/_models_hyperelasticity.py` & `felupe-8.5.0/src/felupe/constitution/_models_hyperelasticity.py`

 * *Files 5% similar despite different names*

```diff
@@ -171,21 +171,32 @@
 
        \mathbb{A}_{U} &= K J \left( (2J - 1) \boldsymbol{F}^{-T} \otimes
        \boldsymbol{F}^{-T} - (J - 1) \boldsymbol{F}^{-T} \overset{il}{\otimes}
        \boldsymbol{F}^{-T} \right)
 
     Examples
     --------
-    >>> import felupe as fem
-    >>>
-    >>> umat = fem.NeoHooke(mu=1.0, bulk=2.0)
-    >>> ax = umat.plot()
+    ..  pyvista-plot::
+        :context:
 
-    ..  image:: images/umat_neohooke_nearlyincompressible.png
-        :width: 400px
+        >>> import felupe as fem
+        >>>
+        >>> umat = fem.NeoHooke(mu=1.0, bulk=2.0)
+        >>> ax = umat.plot()
+
+    ..  pyvista-plot::
+        :include-source: False
+        :context:
+        :force_static:
+
+        >>> import pyvista as pv
+        >>>
+        >>> fig = ax.get_figure()
+        >>> chart = pv.ChartMPL(fig)
+        >>> chart.show()
 
     """
 
     def __init__(self, mu=None, bulk=None, parallel=False):
         self.parallel = parallel
 
         self.mu = mu
@@ -418,21 +429,32 @@
        \mathbb{A} &= \mu \boldsymbol{I} \overset{ik}{\otimes} \boldsymbol{I}
            + \left(\mu - \lambda \ln(J) \right)
                \boldsymbol{F}^{-T} \overset{il}{\otimes} \boldsymbol{F}^{-T}
            + \lambda \boldsymbol{F}^{-T} {\otimes} \boldsymbol{F}^{-T}
 
     Examples
     --------
-    >>> import felupe as fem
-    >>>
-    >>> umat = fem.NeoHookeCompressible(mu=1.0, lmbda=2.0)
-    >>> ax = umat.plot()
+    ..  pyvista-plot::
+        :context:
 
-    ..  image:: images/umat_neohooke_compressible.png
-        :width: 400px
+        >>> import felupe as fem
+        >>>
+        >>> umat = fem.NeoHookeCompressible(mu=1.0, lmbda=2.0)
+        >>> ax = umat.plot()
+
+    ..  pyvista-plot::
+        :include-source: False
+        :context:
+        :force_static:
+
+        >>> import pyvista as pv
+        >>>
+        >>> fig = ax.get_figure()
+        >>> chart = pv.ChartMPL(fig)
+        >>> chart.show()
 
     """
 
     def __init__(self, mu=None, lmbda=None, parallel=False):
         self.parallel = parallel
 
         self.mu = mu
```

### Comparing `felupe-8.4.0/src/felupe/constitution/_models_linear_elasticity.py` & `felupe-8.5.0/src/felupe/constitution/_models_linear_elasticity.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,26 @@
 import numpy as np
 
 from ..math import cdya, dya, identity, trace, transpose
 from ._base import ConstitutiveMaterial
 
 
 def lame_converter(E, nu):
-    """Convert material parameters to first and second Lamé - constants.
+    r"""Convert the pair of given material parameters Young's modulus :math:`E` and
+    Poisson ratio :math:`\nu` to first and second Lamé - constants :math:`\lambda` and
+    :math:`\mu`.
+
+    Notes
+    -----
+
+    ..  math::
+
+        \lambda &= \frac{E \nu}{(1 + \nu) (1 - 2 \nu)}
+
+        \mu &= \frac{E}{2 (1 + \nu)}
 
     Parameters
     ----------
     E : float
         Young's modulus.
     nu : float
         Poisson ratio.
@@ -89,21 +100,32 @@
 
         \boldsymbol{\varepsilon} = \frac{1}{2} \left( \frac{\partial \boldsymbol{u}}
         {\partial \boldsymbol{X}} + \left( \frac{\partial \boldsymbol{u}}
         {\partial \boldsymbol{X}} \right)^T \right)
     
     Examples
     --------
-    >>> import felupe as fem
-    >>> 
-    >>> umat = fem.LinearElastic(E=1, nu=0.3)
-    >>> ax = umat.plot()
-
-    ..  image:: images/umat_linearelastic.png
-        :width: 400px
+    ..  pyvista-plot::
+        :context:
+        
+        >>> import felupe as fem
+        >>> 
+        >>> umat = fem.LinearElastic(E=1, nu=0.3)
+        >>> ax = umat.plot()
+    
+    ..  pyvista-plot::
+        :include-source: False
+        :context:
+        :force_static:
+
+        >>> import pyvista as pv
+        >>>
+        >>> fig = ax.get_figure()
+        >>> chart = pv.ChartMPL(fig)
+        >>> chart.show()
 
     """
 
     def __init__(self, E=None, nu=None):
         self.E = E
         self.nu = nu
 
@@ -239,21 +261,32 @@
 
         \boldsymbol{\varepsilon} = \frac{1}{2} \left( \frac{\partial \boldsymbol{u}}
         {\partial \boldsymbol{X}} + \left( \frac{\partial \boldsymbol{u}}
         {\partial \boldsymbol{X}} \right)^T \right)
 
     Examples
     --------
-    >>> import felupe as fem
-    >>> 
-    >>> umat = fem.constitution.LinearElasticTensorNotation(E=1, nu=0.3)
-    >>> ax = umat.plot()
-
-    ..  image:: images/umat_linearelastic.png
-        :width: 400px
+    ..  pyvista-plot::
+        :context:
+        
+        >>> import felupe as fem
+        >>> 
+        >>> umat = fem.constitution.LinearElasticTensorNotation(E=1, nu=0.3)
+        >>> ax = umat.plot()
+    
+    ..  pyvista-plot::
+        :include-source: False
+        :context:
+        :force_static:
+
+        >>> import pyvista as pv
+        >>>
+        >>> fig = ax.get_figure()
+        >>> chart = pv.ChartMPL(fig)
+        >>> chart.show()
 
     """
 
     def __init__(self, E=None, nu=None, parallel=False):
         self.parallel = parallel
 
         self.E = E
```

### Comparing `felupe-8.4.0/src/felupe/constitution/_models_linear_elasticity_large_strain.py` & `felupe-8.5.0/src/felupe/constitution/_models_linear_elasticity_large_strain.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from ._base import ConstitutiveMaterial
 from ._models_hyperelasticity import NeoHookeCompressible
 from ._models_linear_elasticity import lame_converter
 
 
 class LinearElasticLargeStrain(ConstitutiveMaterial):
     r"""Linear-elastic material formulation suitable for large-rotation analyses based
-    on the nearly-incompressible Neo-Hookean material formulation.
+    on the compressible Neo-Hookean material formulation.
 
     Parameters
     ----------
     E : float
         Young's modulus.
     nu : float
         Poisson ratio.
@@ -37,21 +37,32 @@
     See Also
     --------
     NeoHookeCompressible: Compressible isotropic hyperelastic Neo-Hooke material
         formulation.
 
     Examples
     --------
-    >>> import felupe as fem
-    >>>
-    >>> umat = fem.LinearElasticLargeStrain(E=1.0, nu=0.3)
-    >>> ax = umat.plot()
+    ..  pyvista-plot::
+        :context:
 
-    ..  image:: images/umat_linearelasticlargestrain.png
-        :width: 400px
+        >>> import felupe as fem
+        >>>
+        >>> umat = fem.LinearElasticLargeStrain(E=1.0, nu=0.3)
+        >>> ax = umat.plot()
+
+    ..  pyvista-plot::
+        :include-source: False
+        :context:
+        :force_static:
+
+        >>> import pyvista as pv
+        >>>
+        >>> fig = ax.get_figure()
+        >>> chart = pv.ChartMPL(fig)
+        >>> chart.show()
 
     """
 
     def __init__(self, E=None, nu=None, parallel=False):
         self.E = E
         self.nu = nu
```

### Comparing `felupe-8.4.0/src/felupe/constitution/_models_pseudo_elasticity.py` & `felupe-8.5.0/src/felupe/constitution/_models_pseudo_elasticity.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,28 +52,39 @@
 
         \mathbb{A} &= \frac{\partial^2 \psi}{\partial \boldsymbol{F} \partial
         \boldsymbol{F}} + \frac{\partial \eta}{\partial \psi} \frac{\partial \psi}
         {\partial \boldsymbol{F}} \otimes \frac{\partial \psi}{\partial \boldsymbol{F}}
 
     Examples
     --------
-    >>> import felupe as fem
-    >>>
-    >>> neo_hooke = fem.NeoHooke(mu=1.0)
-    >>> umat = fem.OgdenRoxburgh(material=neo_hooke, r=3.0, m=1.0, beta=0.0)
-    >>>
-    >>> ax = umat.plot(
-    >>>     ux=fem.math.linsteps([1, 1.5, 1, 2, 1, 2.5, 1], num=15),
-    >>>     ps=None,
-    >>>     bx=None,
-    >>>     incompressible=True,
-    >>> )
+    ..  pyvista-plot::
+        :context:
 
-    .. image:: images/umat.png
-       :width: 400px
+        >>> import felupe as fem
+        >>>
+        >>> neo_hooke = fem.NeoHooke(mu=1.0)
+        >>> umat = fem.OgdenRoxburgh(material=neo_hooke, r=3.0, m=1.0, beta=0.0)
+        >>>
+        >>> ax = umat.plot(
+        ...     ux=fem.math.linsteps([1, 1.5, 1, 2, 1, 2.5, 1], num=15),
+        ...     ps=None,
+        ...     bx=None,
+        ...     incompressible=True,
+        ... )
+
+    ..  pyvista-plot::
+        :include-source: False
+        :context:
+        :force_static:
+
+        >>> import pyvista as pv
+        >>>
+        >>> fig = ax.get_figure()
+        >>> chart = pv.ChartMPL(fig)
+        >>> chart.show()
 
     """
 
     def __init__(self, material, r, m, beta):
         # isotropic hyperelastic material formulation
         self.material = self.fun = material
```

### Comparing `felupe-8.4.0/src/felupe/constitution/_user_materials.py` & `felupe-8.5.0/src/felupe/constitution/_user_materials.py`

 * *Files 4% similar despite different names*

```diff
@@ -224,40 +224,40 @@
            + \left(\mu - \lambda \ln(J) \right)
                \boldsymbol{F}^{-T} \overset{il}{\otimes} \boldsymbol{F}^{-T}
            + \lambda \boldsymbol{F}^{-T} {\otimes} \boldsymbol{F}^{-T}
     
     >>> import numpy as np
     >>> import felupe as fem
     >>> from felupe.math import (
-    >>>     cdya_ik,
-    >>>     cdya_il,
-    >>>     det,
-    >>>     dya,
-    >>>     identity,
-    >>>     inv,
-    >>>     transpose
-    >>> )
+    ...     cdya_ik,
+    ...     cdya_il,
+    ...     det,
+    ...     dya,
+    ...     identity,
+    ...     inv,
+    ...     transpose
+    ... )
     
     >>> def stress(x, mu, lmbda):
-    >>>     F, statevars = x[0], x[-1]
-    >>>     J = det(F)
-    >>>     lnJ = np.log(J)
-    >>>     iFT = transpose(inv(F, J))
-    >>>     dWdF = mu * (F - iFT) + lmbda * lnJ * iFT
-    >>>     return [dWdF, statevars]
+    ...     F, statevars = x[0], x[-1]
+    ...     J = det(F)
+    ...     lnJ = np.log(J)
+    ...     iFT = transpose(inv(F, J))
+    ...     dWdF = mu * (F - iFT) + lmbda * lnJ * iFT
+    ...     return [dWdF, statevars]
     
     >>> def elasticity(x, mu, lmbda):
-    >>>     F = x[0]
-    >>>     J = det(F)
-    >>>     iFT = transpose(inv(F, J))
-    >>>     eye = identity(F)
-    >>>     return [
-    >>>         mu * cdya_ik(eye, eye) + lmbda * dya(iFT, iFT) +
-    >>>         (mu - lmbda * np.log(J)) * cdya_il(iFT, iFT)
-    >>>     ]
+    ...     F = x[0]
+    ...     J = det(F)
+    ...     iFT = transpose(inv(F, J))
+    ...     eye = identity(F)
+    ...     return [
+    ...         mu * cdya_ik(eye, eye) + lmbda * dya(iFT, iFT) +
+    ...         (mu - lmbda * np.log(J)) * cdya_il(iFT, iFT)
+    ...     ]
     
     >>> umat = fem.Material(stress, elasticity, mu=1.0, lmbda=2.0)
     
     The material formulation is tested in a minimal example of non-homogeneous uniaxial
     tension.
 
     >>> mesh = fem.Cube(n=6)
```

### Comparing `felupe-8.4.0/src/felupe/constitution/_user_materials_hyperelastic.py` & `felupe-8.5.0/src/felupe/constitution/_user_materials_hyperelastic.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,26 +106,37 @@
         See the `documentation of tensortrax <https://github.com/adtzlr/tensortrax>`_
         for further details.
 
     Examples
     --------
     View force-stretch curves on elementary incompressible deformations.
 
-    >>> import felupe as fem
-    >>> import tensortrax.math as tm
-    >>>
-    >>> def neo_hooke(C, mu):
-    >>>     "Strain energy function of the Neo-Hookean material formulation."
-    >>>     return mu / 2 * (tm.linalg.det(C) ** (-1/3) * tm.trace(C) - 3)
-    >>>
-    >>> umat = fem.Hyperelastic(neo_hooke, mu=1)
-    >>> ax = umat.plot(incompressible=True)
+    ..  pyvista-plot::
+        :context:
 
-    ..  image:: images/umat_neo_hooke.png
-        :width: 400px
+        >>> import felupe as fem
+        >>> import tensortrax.math as tm
+        >>>
+        >>> def neo_hooke(C, mu):
+        ...     "Strain energy function of the Neo-Hookean material formulation."
+        ...     return mu / 2 * (tm.linalg.det(C) ** (-1/3) * tm.trace(C) - 3)
+        >>>
+        >>> umat = fem.Hyperelastic(neo_hooke, mu=1)
+        >>> ax = umat.plot(incompressible=True)
+
+    ..  pyvista-plot::
+        :include-source: False
+        :context:
+        :force_static:
+
+        >>> import pyvista as pv
+        >>>
+        >>> fig = ax.get_figure()
+        >>> chart = pv.ChartMPL(fig)
+        >>> chart.show()
 
     See Also
     --------
     saint_venant_kirchhoff : Strain energy function of the Saint
         Venant-Kirchhoff material formulation.
     neo_hooke : Strain energy function of the Neo-Hookean material formulation.
     mooney_rivlin : Strain energy function of the Mooney-Rivlin material formulation.
@@ -146,19 +157,23 @@
             self.fun = tr.take(fun, item=0)
             self.fun_statevars = tr.take(fun, item=1)
         else:
             self.fun = fun
 
         self.parallel = parallel
 
+        keyword_args = kwargs
+        if hasattr(fun, "kwargs"):
+            keyword_args = {**fun.kwargs, **keyword_args}
+
         super().__init__(
             stress=self._stress,
             elasticity=self._elasticity,
             nstatevars=nstatevars,
-            **kwargs,
+            **keyword_args,
         )
 
     def _stress(self, x, **kwargs):
         F = np.ascontiguousarray(x[0])
 
         if self.nstatevars > 0:
             statevars = (x[1],)
@@ -281,27 +296,38 @@
 
     ..  note::
         See the `documentation of tensortrax <https://github.com/adtzlr/tensortrax>`_
         for further details.
 
     Examples
     --------
-    >>> import felupe as fem
-    >>> import tensortrax.math as tm
-    >>>
-    >>> def neo_hooke(F, mu):
-    >>>     C = tm.dot(tm.transpose(F), F)
-    >>>     S = mu * tm.special.dev(tm.linalg.det(C)**(-1/3) * C) @ tm.linalg.inv(C)
-    >>>     return F @ S
-    >>>
-    >>> umat = fem.MaterialAD(neo_hooke, mu=1)
-    >>> ax = umat.plot(incompressible=True)
+    ..  pyvista-plot::
+        :context:
 
-    ..  image:: images/umat_materialad_neohooke.png
-        :width: 400px
+        >>> import felupe as fem
+        >>> import tensortrax.math as tm
+        >>>
+        >>> def neo_hooke(F, mu):
+        ...     C = tm.dot(tm.transpose(F), F)
+        ...     S = mu * tm.special.dev(tm.linalg.det(C)**(-1/3) * C) @ tm.linalg.inv(C)
+        ...     return F @ S
+        >>>
+        >>> umat = fem.MaterialAD(neo_hooke, mu=1)
+        >>> ax = umat.plot(incompressible=True)
+
+    ..  pyvista-plot::
+        :include-source: False
+        :context:
+        :force_static:
+
+        >>> import pyvista as pv
+        >>>
+        >>> fig = ax.get_figure()
+        >>> chart = pv.ChartMPL(fig)
+        >>> chart.show()
 
     """
 
     def __init__(self, fun, nstatevars=0, parallel=False, **kwargs):
         if nstatevars > 0:
             # split the original function into two sub-functions
             self.fun = tr.take(fun, item=0)
```

### Comparing `felupe-8.4.0/src/felupe/constitution/_user_materials_models.py` & `felupe-8.5.0/src/felupe/constitution/_user_materials_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,17 +66,32 @@
                 2 \mu \ \boldsymbol{1} \odot \boldsymbol{1}
 
             \boldsymbol{\sigma} &= \boldsymbol{\sigma}_n
                 + \mathbb{C} : \Delta\boldsymbol{\varepsilon}
 
     Examples
     --------
-    >>> import felupe as fem
-    >>>
-    >>> umat = fem.MaterialStrain(material=fem.linear_elastic, λ=2.0, μ=1.0)
+    ..  pyvista-plot::
+        :context:
+
+        >>> import felupe as fem
+        >>>
+        >>> umat = fem.MaterialStrain(material=fem.linear_elastic, λ=2.0, μ=1.0)
+        >>> ax = umat.plot()
+
+    ..  pyvista-plot::
+        :include-source: False
+        :context:
+        :force_static:
+
+        >>> import pyvista as pv
+        >>>
+        >>> fig = ax.get_figure()
+        >>> chart = pv.ChartMPL(fig)
+        >>> chart.show()
 
     See Also
     --------
     MaterialStrain : A strain-based user-defined material definition with a given
         function for the stress tensor and the (fourth-order) elasticity tensor.
 
     """
@@ -192,25 +207,39 @@
                     2 \mu \left( \boldsymbol{1} \odot \boldsymbol{1}
                      - \frac{1}{3} \boldsymbol{1} \otimes \boldsymbol{1}
                     - n \otimes n \right)
                 \right]
 
     Examples
     --------
-    >>> import felupe as fem
-    >>>
-    >>> umat = fem.MaterialStrain(
-    >>>     material=fem.linear_elastic_plastic_isotropic_hardening,
-    >>>     λ=2.0,
-    >>>     μ=1.0,
-    >>>     σy=1.0,
-    >>>     K=0.1,
-    >>>     dim=3,
-    >>>     statevars=(1, (3, 3)),
-    >>> )
+    ..  pyvista-plot::
+        :context:
+
+        >>> import felupe as fem
+        >>>
+        >>> umat = fem.MaterialStrain(
+        ...     material=fem.linear_elastic_plastic_isotropic_hardening,
+        ...     λ=2.0,
+        ...     μ=1.0,
+        ...     σy=1.0,
+        ...     K=0.1,
+        ...     dim=3,
+        ...     statevars=(1, (3, 3)),
+        ... )
+
+    ..  pyvista-plot::
+        :include-source: False
+        :context:
+        :force_static:
+
+        >>> import pyvista as pv
+        >>>
+        >>> fig = ax.get_figure()
+        >>> chart = pv.ChartMPL(fig)
+        >>> chart.show()
 
     See Also
     --------
     MaterialStrain : A strain-based user-defined material definition with a given
         function for the stress tensor and the (fourth-order) elasticity tensor.
 
     """
```

### Comparing `felupe-8.4.0/src/felupe/constitution/_view.py` & `felupe-8.5.0/src/felupe/constitution/_view.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,17 +88,23 @@
                 if callable(fun):
                     label = [name.title() for name in fun.__name__.split("_")]
                 title += " (" + " ".join(label) + ")"
             fig.suptitle(title)
 
         if show_kwargs:
             if hasattr(self.umat, "kwargs"):
-                parameters = ", ".join(
-                    [f"{key}={value}" for key, value in self.umat.kwargs.items()]
-                )
+                p = []
+                for key, value in self.umat.kwargs.items():
+                    if hasattr(value, "__len__"):
+                        val = "[" + " ".join([f"{v:.3g}" for v in value]) + "]"
+                    else:
+                        val = f"{value:.3g}"
+                    p.append(f"{key}={val}")
+                parameters = ", ".join(p)
+
                 ax.set_title(parameters, fontdict=dict(fontsize="small"), wrap=True)
 
         return ax
 
 
 class ViewMaterial(PlotMaterial):
     """Create views on normal force per undeformed area vs. stretch curves for the
@@ -122,27 +128,38 @@
         ``linsteps([1.0, 1.75], num=15)```.
     statevars : ndarray or None, optional
         Array with state variables (default is None). If None, the state variables are
         assumed to be initially zero.
 
     Examples
     --------
-    >>> import felupe as fem
-    >>>
-    >>> umat = fem.OgdenRoxburgh(fem.NeoHooke(mu=1, bulk=2), r=3, m=1, beta=0)
-    >>> view = fem.ViewMaterial(
-    >>>     umat,
-    >>>     ux=fem.math.linsteps([1, 1.5, 1, 2, 1, 2.5, 1], num=15),
-    >>>     ps=None,
-    >>>     bx=None,
-    >>> )
-    >>> ax = view.plot(show_title=True, show_kwargs=True)
+    ..  pyvista-plot::
+        :context:
 
-    .. image:: images/umat.png
-       :width: 400px
+        >>> import felupe as fem
+        >>>
+        >>> umat = fem.OgdenRoxburgh(fem.NeoHooke(mu=1, bulk=2), r=3, m=1, beta=0)
+        >>> view = fem.ViewMaterial(
+        ...     umat,
+        ...     ux=fem.math.linsteps([1, 1.5, 1, 2, 1, 2.5, 1], num=15),
+        ...     ps=None,
+        ...     bx=None,
+        ... )
+        >>> ax = view.plot(show_title=True, show_kwargs=True)
+
+    ..  pyvista-plot::
+        :include-source: False
+        :context:
+        :force_static:
+
+        >>> import pyvista as pv
+        >>>
+        >>> fig = ax.get_figure()
+        >>> chart = pv.ChartMPL(fig)
+        >>> chart.show()
 
     """
 
     def __init__(
         self,
         umat,
         ux=linsteps([0.7, 2.5], num=36),
@@ -362,34 +379,56 @@
         ``linsteps([1, 1.75], num=15)``.
     statevars : ndarray or None, optional
         Array with state variables (default is None). If None, the state variables are
         assumed to be initially zero.
 
     Examples
     --------
-    >>> import felupe as fem
-    >>>
-    >>> umat = fem.Hyperelastic(fem.extended_tube, Gc=0.2, Ge=0.2, beta=0.2, delta=0.1)
-    >>> preview = fem.ViewMaterialIncompressible(umat)
-    >>> ax = preview.plot(show_title=True, show_kwargs=True)
-
-    .. image:: images/preview_hyperelastic.png
-       :width: 400px
-
-    >>> umat = fem.OgdenRoxburgh(fem.NeoHooke(mu=1), r=3, m=1, beta=0)
-    >>> view = fem.ViewMaterialIncompressible(
-    >>>     umat,
-    >>>     ux=fem.math.linsteps([1, 1.5, 1, 2, 1, 2.5, 1], num=15),
-    >>>     ps=None,
-    >>>     bx=None,
-    >>> )
-    >>> ax = view.plot(show_title=True, show_kwargs=True)
+    ..  pyvista-plot::
+        :context:
 
-    .. image:: images/umat_incompressible.png
-       :width: 400px
+        >>> import felupe as fem
+        >>>
+        >>> umat = fem.Hyperelastic(fem.extended_tube, Gc=0.2, Ge=0.2, beta=0.2, delta=0.1)
+        >>> preview = fem.ViewMaterialIncompressible(umat)
+        >>> ax = preview.plot(show_title=True, show_kwargs=True)
+
+    ..  pyvista-plot::
+        :include-source: False
+        :context:
+        :force_static:
+
+        >>> import pyvista as pv
+        >>>
+        >>> fig = ax.get_figure()
+        >>> chart = pv.ChartMPL(fig)
+        >>> chart.show()
+
+    ..  pyvista-plot::
+        :context:
+
+        >>> umat = fem.OgdenRoxburgh(fem.NeoHooke(mu=1), r=3, m=1, beta=0)
+        >>> view = fem.ViewMaterialIncompressible(
+        ...     umat,
+        ...     ux=fem.math.linsteps([1, 1.5, 1, 2, 1, 2.5, 1], num=15),
+        ...     ps=None,
+        ...     bx=None,
+        ... )
+        >>> ax = view.plot(show_title=True, show_kwargs=True)
+
+    ..  pyvista-plot::
+        :include-source: False
+        :context:
+        :force_static:
+
+        >>> import pyvista as pv
+        >>>
+        >>> fig = ax.get_figure()
+        >>> chart = pv.ChartMPL(fig)
+        >>> chart.show()
 
     """
 
     def __init__(
         self,
         umat,
         ux=linsteps([0.7, 2.5], num=36),
```

### Comparing `felupe-8.4.0/src/felupe/dof/_loadcase.py` & `felupe-8.5.0/src/felupe/dof/_loadcase.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,33 +62,33 @@
 
     Examples
     --------
     The x-symmetry boundary for a symmetry on the x-axis contains all points at the
     given x-coordinate. The degrees of freedom are prescribed except for the symmetry
     x-axis.
 
-    >>> import numpy as np
-    >>> import felupe as fem
+    ..  pyvista-plot::
 
-    >>> mesh = fem.Circle(radius=1, n=6, sections=[0, 270])
-    >>> x, y = mesh.points.T
-    >>> region = fem.RegionQuad(mesh)
-    >>> displacement = fem.FieldPlaneStrain(region, dim=2)
-
-    >>> boundaries = fem.dof.symmetry(displacement, axes=(True, False), x=0.0)
-
-    >>> plotter = mesh.plot(off_screen=True)
-    >>> plotter.add_points(
-    >>>     np.pad(mesh.points[boundaries["symx"].points], ((0, 0), (0, 1))),
-    >>>     point_size=20,
-    >>>     color="red",
-    >>> )
-    >>> img = plotter.screenshot("boundary_symx.png", transparent_background=True)
-
-    ..  image:: images/boundary_symx.png
+        >>> import numpy as np
+        >>> import felupe as fem
+        >>>
+        >>> mesh = fem.Circle(radius=1, n=6, sections=[0, 270])
+        >>> x, y = mesh.points.T
+        >>> region = fem.RegionQuad(mesh)
+        >>> displacement = fem.FieldPlaneStrain(region, dim=2)
+        >>>
+        >>> boundaries = fem.dof.symmetry(displacement, axes=(True, False), x=0.0)
+        >>>
+        >>> plotter = mesh.plot()
+        >>> actor = plotter.add_points(
+        ...     np.pad(mesh.points[boundaries["symx"].points], ((0, 0), (0, 1))),
+        ...     point_size=20,
+        ...     color="red",
+        ... )
+        >>> plotter.show()
 
     See Also
     --------
     felupe.Boundary : A collection of prescribed degrees of freedom.
     """
 
     # convert axes to array and slice by mesh dimension
@@ -161,34 +161,37 @@
         degrees of freedom.
 
     Examples
     --------
     A quarter of a solid hyperelastic cube is subjected to uniaxial displacement-
     controlled compression on a rigid end face.
 
-    >>> import felupe as fem
-
-    >>> region = fem.RegionHexahedron(fem.Cube(a=(0, 0, 0), b=(2, 3, 1), n=(11, 16, 6)))
-    >>> field = fem.FieldContainer([fem.Field(region, dim=3)])
+    ..  pyvista-plot::
+        :context:
 
-    >>> boundaries = fem.dof.uniaxial(field, axis=2, clamped=True)[0]
+        >>> import felupe as fem
+        >>>
+        >>> region = fem.RegionHexahedron(fem.Cube(a=(0, 0, 0), b=(2, 3, 1), n=(6, 11, 5)))
+        >>> field = fem.FieldContainer([fem.Field(region, dim=3)])
+        >>>
+        >>> boundaries = fem.dof.uniaxial(field, axis=2, clamped=True)[0]
 
     The longitudinal displacement is applied incrementally.
 
-    >>> solid = fem.SolidBodyNearlyIncompressible(fem.NeoHooke(mu=1), field, bulk=5000)
-    >>> step = fem.Step(
-    >>>     items=[solid],
-    >>>     ramp={boundaries["move"]: fem.math.linsteps([0, -0.3], num=5)},
-    >>>     boundaries=boundaries
-    >>> )
-
-    >>> fem.Job(steps=[step]).evaluate()
-    >>> img = field.screenshot("Principal Values of Logarithmic Strain")
+    ..  pyvista-plot::
+        :context:
 
-    ..  image:: images/loadcase_ux.png
+        >>> solid = fem.SolidBodyNearlyIncompressible(fem.NeoHooke(mu=1), field, bulk=5000)
+        >>> step = fem.Step(
+        ...     items=[solid],
+        ...     ramp={boundaries["move"]: fem.math.linsteps([0, -0.3], num=5)},
+        ...     boundaries=boundaries
+        ... )
+        >>> job = fem.Job(steps=[step]).evaluate()
+        >>> field.plot("Principal Values of Logarithmic Strain").show()
 
     See Also
     --------
     felupe.Boundary : A collection of prescribed degrees of freedom.
     felupe.dof.partition : Partition degrees of freedom into prescribed and active dof.
     felupe.dof.apply : Apply prescribed values for a list of boundaries.
     felupe.dof.symmetry : Return a dict of boundaries for the symmetry axes.
@@ -291,69 +294,99 @@
         Instead, use a shape where the clamped end faces do not share mesh-points.
 
     Examples
     --------
     A cross-like planar specimen of a hyperelastic solid is subjected to biaxial
     displacement-controlled tension on rigid end faces.
 
-    >>> import numpy as np
-    >>> import felupe as fem
-
-    >>> mesh = fem.Rectangle(a=(0, 0), b=(1, 1), n=(21, 21))
-    >>> x, y = mesh.points.T
-    >>> points = np.arange(mesh.npoints)[np.logical_or.reduce([x <= 0.6, y <= 0.6])]
-    >>> mesh.update(cells=mesh.cells[np.all(np.isin(mesh.cells, points), axis=1)])
-
-    >>> region = fem.RegionQuad(mesh)
-    >>> field = fem.FieldContainer([fem.FieldPlaneStrain(region, dim=2)])
+    ..  pyvista-plot::
+        :context:
 
-    >>> boundaries = fem.dof.biaxial(field, clampes=(True, True))[0]
+        >>> import numpy as np
+        >>> import felupe as fem
+        >>>
+        >>> mesh = fem.Rectangle(a=(0, 0), b=(1, 1), n=(21, 21))
+        >>> x, y = mesh.points.T
+        >>> points = np.arange(mesh.npoints)[np.logical_or.reduce([x <= 0.6, y <= 0.6])]
+        >>> mesh.update(cells=mesh.cells[np.all(np.isin(mesh.cells, points), axis=1)])
+        >>>
+        >>> region = fem.RegionQuad(mesh)
+        >>> field = fem.FieldContainer([fem.FieldPlaneStrain(region, dim=2)])
+        >>>
+        >>> boundaries = fem.dof.biaxial(field, clampes=(True, True))[0]
 
     The longitudinal displacements are applied incrementally.
 
-    >>> solid = fem.SolidBodyNearlyIncompressible(fem.NeoHooke(mu=1), field, bulk=5000)
-    >>> step = fem.Step(
-    >>>     items=[solid],
-    >>>     ramp={
-    >>>         boundaries["move-right-0"]: fem.math.linsteps([0, 0.1], num=5),
-    >>>         boundaries["move-right-1"]: fem.math.linsteps([0, 0.1], num=5),
-    >>>     },
-    >>>     boundaries=boundaries
-    >>> )
+    ..  pyvista-plot::
+        :context:
 
-    >>> fem.Job(steps=[step]).evaluate()
-    >>> img = field.screenshot("Principal Values of Logarithmic Strain")
-
-    ..  image:: images/loadcase_bx.png
+        >>> solid = fem.SolidBodyNearlyIncompressible(fem.NeoHooke(mu=1), field, bulk=5000)
+        >>> step = fem.Step(
+        ...     items=[solid],
+        ...     ramp={
+        ...         boundaries["move-right-0"]: fem.math.linsteps([0, 0.1], num=5),
+        ...         boundaries["move-right-1"]: fem.math.linsteps([0, 0.1], num=5),
+        ...     },
+        ...     boundaries=boundaries
+        ... )
+        >>> job = fem.Job(steps=[step]).evaluate()
+        >>> field.plot("Principal Values of Logarithmic Strain").show()
 
     Repeating the above example with ``fem.dof.biaxial(field, clampes=(False, False)``
     results in a different deformation at the end faces.
 
-    ..  image:: images/loadcase_bx_free.png
+    ..  pyvista-plot::
+
+        >>> import numpy as np
+        >>> import felupe as fem
+        >>>
+        >>> mesh = fem.Rectangle(a=(0, 0), b=(1, 1), n=(21, 21))
+        >>> x, y = mesh.points.T
+        >>> points = np.arange(mesh.npoints)[np.logical_or.reduce([x <= 0.6, y <= 0.6])]
+        >>> mesh.update(cells=mesh.cells[np.all(np.isin(mesh.cells, points), axis=1)])
+        >>>
+        >>> region = fem.RegionQuad(mesh)
+        >>> field = fem.FieldContainer([fem.FieldPlaneStrain(region, dim=2)])
+        >>>
+        >>> boundaries = fem.dof.biaxial(field, clampes=(False, False))[0]
+        >>>
+        >>> solid = fem.SolidBodyNearlyIncompressible(fem.NeoHooke(mu=1), field, bulk=5000)
+        >>> step = fem.Step(
+        ...     items=[solid],
+        ...     ramp={
+        ...         boundaries["move-right-0"]: fem.math.linsteps([0, 0.1], num=5),
+        ...         boundaries["move-right-1"]: fem.math.linsteps([0, 0.1], num=5),
+        ...     },
+        ...     boundaries=boundaries
+        ... )
+        >>> job = fem.Job(steps=[step]).evaluate()
+        >>> field.plot("Principal Values of Logarithmic Strain").show()
 
     The biaxial load case may also invoke a planar loading, where one of the
     longitudinal axes is fixed with no displacements at the end plates. The clampling
     must at least be deactivated on the fixed longitudinal axis.
 
-    >>> mesh = fem.Cube(n=2)
-    >>> region = fem.RegionHexahedron(mesh)
-    >>> field = fem.FieldContainer([fem.Field(region, dim=3)])
-    >>> boundaries = fem.dof.biaxial(
-    >>>     field, clampes=(True, False), moves=(0, 0), sym=False, axes=(0, 1)
-    >>> )[0]
-    >>> solid = fem.SolidBodyNearlyIncompressible(fem.NeoHooke(mu=1), field, bulk=5000)
-    >>> step = fem.Step(
-    >>>     items=[solid],
-    >>>     ramp={boundaries["move-right-0"]: fem.math.linsteps([0, 0.3], num=5),},
-    >>>     boundaries=boundaries
-    >>> )
-    >>> fem.Job(steps=[step]).evaluate()
-    >>> img = field.screenshot("Principal Values of Logarithmic Strain")
+    ..  pyvista-plot::
 
-    ..  image:: images/loadcase_ps.png
+        >>> import felupe as fem
+        >>>
+        >>> mesh = fem.Cube(n=5)
+        >>> region = fem.RegionHexahedron(mesh)
+        >>> field = fem.FieldContainer([fem.Field(region, dim=3)])
+        >>> boundaries = fem.dof.biaxial(
+        ...     field, clampes=(True, False), moves=(0, 0), sym=False, axes=(0, 1)
+        ... )[0]
+        >>> solid = fem.SolidBodyNearlyIncompressible(fem.NeoHooke(mu=1), field, bulk=5000)
+        >>> step = fem.Step(
+        ...     items=[solid],
+        ...     ramp={boundaries["move-right-0"]: fem.math.linsteps([0, 0.3], num=5),},
+        ...     boundaries=boundaries
+        ... )
+        >>> job = fem.Job(steps=[step]).evaluate()
+        >>> field.plot("Principal Values of Logarithmic Strain").show()
 
     See Also
     --------
     felupe.Boundary : A collection of prescribed degrees of freedom.
     felupe.dof.partition : Partition degrees of freedom into prescribed and active dof.
     felupe.dof.apply : Apply prescribed values for a list of boundaries.
     felupe.dof.symmetry : Return a dict of boundaries for the symmetry axes.
@@ -462,37 +495,43 @@
         degrees of freedom.
 
     Examples
     --------
     A rectangular planar specimen of a hyperelastic solid is subjected to a
     displacement-controlled combined shear-compression loading on rigid end faces.
 
-    >>> import felupe as fem
+    ..  pyvista-plot::
+        :context:
 
-    >>> mesh = fem.Rectangle(a=(0, 0), b=(4, 1), n=(41, 11))
-    >>> region = fem.RegionQuad(mesh)
-    >>> field = fem.FieldContainer([fem.FieldPlaneStrain(region, dim=2)])
+        >>> import felupe as fem
+        >>>
+        >>> mesh = fem.Rectangle(a=(0, 0), b=(4, 1), n=(41, 11))
+        >>> region = fem.RegionQuad(mesh)
+        >>> field = fem.FieldContainer([fem.FieldPlaneStrain(region, dim=2)])
 
     The top edge is moved by ``-0.1`` to add a 10% constant compressive loading.
 
-    >>> boundaries = fem.dof.shear(field, moves=(0, 0, -0.1))[0]
+    ..  pyvista-plot::
+        :context:
 
-    The shear displacement is applied incrementally.
+        >>> boundaries = fem.dof.shear(field, moves=(0, 0, -0.1))[0]
 
-    >>> solid = fem.SolidBodyNearlyIncompressible(fem.NeoHooke(mu=1), field, bulk=5000)
-    >>> step = fem.Step(
-    >>>     items=[solid],
-    >>>     ramp={boundaries["move"]: fem.math.linsteps([0, 1], num=5)},
-    >>>     boundaries=boundaries
-    >>> )
+    The shear displacement is applied incrementally.
 
-    >>> fem.Job(steps=[step]).evaluate()
-    >>> img = field.screenshot("Principal Values of Logarithmic Strain")
+    ..  pyvista-plot::
+        :context:
 
-    ..  image:: images/loadcase_shear.png
+        >>> solid = fem.SolidBodyNearlyIncompressible(fem.NeoHooke(mu=1), field, bulk=5000)
+        >>> step = fem.Step(
+        ...     items=[solid],
+        ...     ramp={boundaries["move"]: fem.math.linsteps([0, 1], num=5)},
+        ...     boundaries=boundaries
+        ... )
+        >>> job = fem.Job(steps=[step]).evaluate()
+        >>> field.plot("Principal Values of Logarithmic Strain").show()
 
     See Also
     --------
     felupe.Boundary : A collection of prescribed degrees of freedom.
     felupe.dof.partition : Partition degrees of freedom into prescribed and active dof.
     felupe.dof.apply : Apply prescribed values for a list of boundaries.
     felupe.dof.symmetry : Return a dict of boundaries for the symmetry axes.
```

### Comparing `felupe-8.4.0/src/felupe/dof/_tools.py` & `felupe-8.5.0/src/felupe/dof/_tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,42 +79,44 @@
         1d-array of int with all prescribed degress of freedom.
     dof1 : ndarray
         1d-array of int with all active degrees of freedom.
 
     Examples
     --------
 
-    >>> import felupe as fem
+    ..  pyvista-plot::
+        :context:
 
-    >>> mesh = fem.Rectangle(a=(0, 0), b=(1, 1), n=(3, 3))
-    >>> region = fem.RegionQuad(mesh)
-    >>> displacement = fem.FieldPlaneStrain(region, dim=2)
-    >>> field = fem.FieldContainer([displacement])
+        >>> import felupe as fem
+        >>>
+        >>> mesh = fem.Rectangle(a=(0, 0), b=(1, 1), n=(3, 3))
+        >>> region = fem.RegionQuad(mesh)
+        >>> displacement = fem.FieldPlaneStrain(region, dim=2)
+        >>> field = fem.FieldContainer([displacement])
 
     A plot shows the point-ids along with the associated degrees of freedom.
 
-    >>> plotter = mesh.plot(off_screen=True)
-    >>> plotter.add_point_labels(
-    >>>     points=np.pad(mesh.points, ((0, 0), (0, 1))),
-    >>>     labels=[
-    >>>         f"Point {i}: DOF {a}, {b}"
-    >>>         for i, (a, b) in enumerate(displacement.indices.dof)
-    >>>     ],
-    >>> )
-    >>> img = plotter.screenshot("dof_partition.png", transparent_background=True)
+    ..  pyvista-plot::
+        :context:
 
-    ..  image:: images/dof_partition.png
+        >>> plotter = mesh.plot()
+        >>> actor = plotter.add_point_labels(
+        ...     points=np.pad(mesh.points, ((0, 0), (0, 1))),
+        ...     labels=[
+        ...         f"Point {i}: DOF {a}, {b}"
+        ...         for i, (a, b) in enumerate(displacement.indices.dof)
+        ...     ],
+        ... )
+        >>> plotter.show()
 
     >>> boundaries = dict(
-    >>>     left=fem.Boundary(displacement, fx=0, value=0.2),
-    >>>     right=fem.Boundary(displacement, fx=1),
-    >>> )
-
+    ...     left=fem.Boundary(displacement, fx=0, value=0.2),
+    ...     right=fem.Boundary(displacement, fx=1),
+    ... )
     >>> dof0, dof1 = fem.dof.partition(field, boundaries)
-
     >>> dof0
     array([ 0,  1,  4,  5,  6,  7, 10, 11, 12, 13, 16, 17])
 
     >>> dof1
     array([ 2,  3,  8,  9, 14, 15])
 
     See Also
@@ -173,25 +175,25 @@
         Field values at mesh-points for all (default) or only the prescribed components
         of the ``field`` based on ``dof0``.
 
     Examples
     --------
 
     >>> import felupe as fem
-
+    >>>
     >>> mesh = fem.Rectangle(a=(0, 0), b=(1, 1), n=(3, 3))
     >>> region = fem.RegionQuad(mesh)
     >>> displacement = fem.FieldPlaneStrain(region, dim=2)
     >>> field = fem.FieldContainer([displacement])
-
+    >>>
     >>> boundaries = dict(
-    >>>     left=fem.Boundary(displacement, fx=0, value=0.2),
-    >>>     right=fem.Boundary(displacement, fx=1),
-    >>> )
-
+    ...     left=fem.Boundary(displacement, fx=0, value=0.2),
+    ...     right=fem.Boundary(displacement, fx=1),
+    ... )
+    >>>
     >>> dof0, dof1 = fem.dof.partition(field, boundaries)
     >>> ext0 = fem.dof.apply(field, boundaries, dof0=dof0)
 
     >>> dof0
     array([ 0,  1,  4,  5,  6,  7, 10, 11, 12, 13, 16, 17])
 
     >>> dof1
@@ -200,16 +202,16 @@
     >>> ext0
     array([0.2, 0.2, 0. , 0. , 0.2, 0.2, 0. , 0. , 0.2, 0.2, 0. , 0. ])
 
     ``dof0=None`` is required (default) if the prescribed displacement array should be
     returned for all degrees of freedom.
 
     >>> fem.dof.apply(field, boundaries).reshape(
-    >>>     displacement.values.shape
-    >>> )
+    ...     displacement.values.shape
+    ... )
     array([[0.2, 0.2],
            [0. , 0. ],
            [0. , 0. ],
            [0.2, 0.2],
            [0. , 0. ],
            [0. , 0. ],
            [0.2, 0.2],
```

### Comparing `felupe-8.4.0/src/felupe/element/__init__.py` & `felupe-8.5.0/src/felupe/element/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/element/_base.py` & `felupe-8.5.0/src/felupe/element/_base.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/element/_hexahedron.py` & `felupe-8.5.0/src/felupe/element/_hexahedron.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     .. math::
 
        h(r,s,t) = 1
 
     Examples
     --------
     .. pyvista-plot::
-       :include-source: True
+       :force_static:
 
        >>> import felupe as fem
        >>>
        >>> element = fem.ConstantHexahedron()
        >>> element.plot().show()
 
     References
@@ -103,15 +103,15 @@
                (1+r) (1+s) (1+t) \\
                (1-r) (1+s) (1+t)
            \end{bmatrix}
 
     Examples
     --------
     .. pyvista-plot::
-       :include-source: True
+       :force_static:
 
        >>> import felupe as fem
        >>>
        >>> element = fem.Hexahedron()
        >>> element.plot().show()
 
     References
@@ -191,15 +191,15 @@
 
     The shape functions :math:`\boldsymbol{h}` are given in terms of the coordinates
     :math:`(r,s,t)`..
 
     Examples
     --------
     .. pyvista-plot::
-       :include-source: True
+       :force_static:
 
        >>> import felupe as fem
        >>>
        >>> element = fem.QuadraticHexahedron()
        >>> element.plot().show()
 
     References
@@ -430,15 +430,15 @@
 
     The shape functions :math:`\boldsymbol{h}` are given in terms of the coordinates
     :math:`(r,s,t)`.
 
     Examples
     --------
     .. pyvista-plot::
-       :include-source: True
+       :force_static:
 
        >>> import felupe as fem
        >>>
        >>> element = fem.TriQuadraticHexahedron()
        >>> element.plot().show()
 
     References
```

### Comparing `felupe-8.4.0/src/felupe/element/_lagrange.py` & `felupe-8.5.0/src/felupe/element/_lagrange.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,23 +234,23 @@
 
         \boldsymbol{H}_{3D}(r,s,t) &= \boldsymbol{h}(r) \otimes \boldsymbol{h}(s)
             \otimes \boldsymbol{h}(t)
 
     Examples
     --------
     .. pyvista-plot::
-       :include-source: True
+       :force_static:
 
        >>> import felupe as fem
        >>>
        >>> element = fem.ArbitraryOrderLagrangeElement(order=4, dim=2)
        >>> element.plot().show()
 
     .. pyvista-plot::
-       :include-source: True
+       :force_static:
 
        >>> import felupe as fem
        >>>
        >>> element = fem.ArbitraryOrderLagrangeElement(order=3, dim=3)
        >>> element.plot().show()
     """
```

### Comparing `felupe-8.4.0/src/felupe/element/_line.py` & `felupe-8.5.0/src/felupe/element/_line.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/element/_quad.py` & `felupe-8.5.0/src/felupe/element/_quad.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     .. math::
 
        h(r,s) = 1
 
     Examples
     --------
     .. pyvista-plot::
-       :include-source: True
+       :force_static:
 
        >>> import felupe as fem
        >>>
        >>> element = fem.ConstantQuad()
        >>> element.plot().show()
 
     References
@@ -84,15 +84,15 @@
                (1+r) (1+s) \\
                (1-r) (1+s)
            \end{bmatrix}
 
     Examples
     --------
     .. pyvista-plot::
-       :include-source: True
+       :force_static:
 
        >>> import felupe as fem
        >>>
        >>> element = fem.Quad()
        >>> element.plot().show()
 
     References
@@ -150,15 +150,15 @@
 
     The shape functions :math:`\boldsymbol{h}` are given in terms of the coordinates
     :math:`(r,s)`.
 
     Examples
     --------
     .. pyvista-plot::
-       :include-source: True
+       :force_static:
 
        >>> import felupe as fem
        >>>
        >>> element = fem.QuadraticQuad()
        >>> element.plot().show()
 
     References
@@ -229,15 +229,15 @@
 
     The shape functions :math:`\boldsymbol{h}` are given in terms of the coordinates
     :math:`(r,s)`.
 
     Examples
     --------
     .. pyvista-plot::
-       :include-source: True
+       :force_static:
 
        >>> import felupe as fem
        >>>
        >>> element = fem.BiQuadraticQuad()
        >>> element.plot().show()
 
     References
```

### Comparing `felupe-8.4.0/src/felupe/element/_tetra.py` & `felupe-8.5.0/src/felupe/element/_tetra.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                s \\
                t
            \end{bmatrix}
 
     Examples
     --------
     .. pyvista-plot::
-       :include-source: True
+       :force_static:
 
        >>> import felupe as fem
        >>>
        >>> element = fem.Tetra()
        >>> element.plot().show()
 
     References
@@ -95,15 +95,15 @@
                t \\
                r s t (1-r-s-t)
            \end{bmatrix}
 
     Examples
     --------
     .. pyvista-plot::
-       :include-source: True
+       :force_static:
 
        >>> import felupe as fem
        >>>
        >>> element = fem.TetraMINI()
        >>> element.plot().show()
 
     References
@@ -188,15 +188,15 @@
        t_3 &= s
 
        t_4 &= t
 
     Examples
     --------
     .. pyvista-plot::
-       :include-source: True
+       :force_static:
 
        >>> import felupe as fem
        >>>
        >>> element = fem.QuadraticTetra()
        >>> element.plot().show()
 
     References
```

### Comparing `felupe-8.4.0/src/felupe/element/_triangle.py` & `felupe-8.5.0/src/felupe/element/_triangle.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                r \\
                s
            \end{bmatrix}
 
     Examples
     --------
     .. pyvista-plot::
-       :include-source: True
+       :force_static:
 
        >>> import felupe as fem
        >>>
        >>> element = fem.Triangle()
        >>> element.plot().show()
 
     References
@@ -92,15 +92,15 @@
                s \\
                r s (1-r-s)
            \end{bmatrix}
 
     Examples
     --------
     .. pyvista-plot::
-       :include-source: True
+       :force_static:
 
        >>> import felupe as fem
        >>>
        >>> element = fem.TriangleMINI()
        >>> element.plot().show()
 
     References
@@ -161,15 +161,15 @@
                4 r s \\
                4 s (1-r-s)
            \end{bmatrix}
 
     Examples
     --------
     .. pyvista-plot::
-       :include-source: True
+       :force_static:
 
        >>> import felupe as fem
        >>>
        >>> element = fem.QuadraticTriangle()
        >>> element.plot().show()
 
     References
```

### Comparing `felupe-8.4.0/src/felupe/field/_axi.py` & `felupe-8.5.0/src/felupe/field/_axi.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/field/_base.py` & `felupe-8.5.0/src/felupe/field/_base.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/field/_container.py` & `felupe-8.5.0/src/felupe/field/_container.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         Field: 1
 
     >>> volume_ratio = fem.Field(region_dual)
     >>> field & volume_ratio  # displacement & pressure & volume_ratio
     <felupe FieldContainer object>
       Number of fields: 3
       Dimension of fields:
-        Field: 2
+        Field: 3
         Field: 1
         Field: 1
 
     See Also
     --------
     felupe.Field : Field on points of a :class:`~felupe.Region` with dimension ``dim``
         and initial point ``values``.
```

### Comparing `felupe-8.4.0/src/felupe/field/_dual.py` & `felupe-8.5.0/src/felupe/field/_dual.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/field/_evaluate.py` & `felupe-8.5.0/src/felupe/field/_evaluate.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/field/_fields.py` & `felupe-8.5.0/src/felupe/field/_fields.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/field/_indices.py` & `felupe-8.5.0/src/felupe/field/_indices.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/field/_planestrain.py` & `felupe-8.5.0/src/felupe/field/_planestrain.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/math/__init__.py` & `felupe-8.5.0/src/felupe/math/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/math/_field.py` & `felupe-8.5.0/src/felupe/math/_field.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/math/_math.py` & `felupe-8.5.0/src/felupe/math/_math.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/math/_solve.py` & `felupe-8.5.0/src/felupe/math/_solve.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/math/_spatial.py` & `felupe-8.5.0/src/felupe/math/_spatial.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/math/_tensor.py` & `felupe-8.5.0/src/felupe/math/_tensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,25 +77,25 @@
     --------
     >>> import felupe as fem
     >>> import numpy as np
     >>> 
     >>> A = np.random.rand(3, 2, 8, 20)
     >>> I = fem.math.identity(A)
     >>> I.shape
-    (3, 3, 1, 1)
+    (3, 2, 1, 1)
     
     With given dimension of the matrix axes the shape of the output is different.
     
     >>> fem.math.identity(A, dim=2).shape
     (2, 2, 1, 1)
     
     Note how the number of batch axes change if a ``shape`` is given.
     
     >>> fem.math.identity(A, shape=(4, 7, 3)).shape
-    (3, 3, 1, 1, 1)
+    (3, 2, 1, 1, 1)
     
     See Also
     --------
     numpy.eye : Return a 2-D array with ones on the diagonal and zeros elsewhere.
     """
 
     M = None
@@ -448,15 +448,15 @@
     Examples
     --------
     >>> import felupe as fem
     >>> import numpy as np
     >>>
     >>> A = fem.math.transpose(np.arange(9, dtype=float).reshape(1, 3, 3).T) / 10
     >>> A += np.eye(3).reshape(3, 3, 1)
-    >>> A[..., 0]
+
     >>> A.shape
     (3, 3, 1)
 
     >>> A[..., 0]
     array([[1. , 0.1, 0.2],
            [0.3, 1.4, 0.5],
            [0.6, 0.7, 1.8]])
@@ -774,17 +774,18 @@
     array([1.69      , 2.57066372])
 
     The associated eigenvectors are extracted. The first column is the eigenvector,
     associated to the greated eigenvalue, for the first right Cauchy-Green deformation
     tensor and the second column for the second right Cauchy-Green deformation tensor.
 
     >>> v[:, 0]
-    array([[ 4.92775421e-17,  0.00000000e+00],
-           [-1.00000000e+00,  1.65906569e-02],
-           [ 1.11022302e-16,  9.99862366e-01]])
+    array([[-4.61810381e-01,  0.00000000e+00],
+           [ 1.11022302e-16, -9.99862366e-01],
+           [ 8.86978676e-01,  1.65906569e-02]])
+
 
     See Also
     --------
     felupe.math.eig : Compute the eigenvalues and right eigenvectors of a square array.
     numpy.linalg.eig : Compute the eigenvalues and right eigenvectors of a square array.
     numpy.linalg.eigh : Return the eigenvalues and eigenvectors of a complex Hermitian
         (conjugate symmetric) or a real symmetric matrix.
@@ -857,15 +858,14 @@
 
     Examples
     --------
     >>> import felupe as fem
     >>> import numpy as np
     >>>
     >>> A = fem.math.transpose(np.arange(9, dtype=float).reshape(1, 3, 3).T)
-    >>> A[..., 0]
     >>> A.shape
     (3, 3, 1)
 
     >>> A[..., 0]
     array([[0., 1., 2.],
            [3., 4., 5.],
            [6., 7., 8.]])
@@ -1119,16 +1119,18 @@
     >>> import numpy as np
     >>>
     >>> a = np.arange(30, dtype=float).reshape(3, 2, 5)
     >>> b = np.arange(80, 20, -2, dtype=float).reshape(5, 2, 3).T
     >>> fem.math.cross(a, b)
     array([[[-800., -682., -564., -446., -328.],
             [-750., -632., -514., -396., -278.]],
+    <BLANKLINE>
            [[1600., 1364., 1128.,  892.,  656.],
             [1500., 1264., 1028.,  792.,  556.]],
+    <BLANKLINE>
            [[-800., -682., -564., -446., -328.],
             [-750., -632., -514., -396., -278.]]])
 
     See Also
     --------
     numpy.cross : Return the cross product of two (arrays of) vectors.
     """
```

### Comparing `felupe-8.4.0/src/felupe/mechanics/__init__.py` & `felupe-8.5.0/src/felupe/mechanics/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/mechanics/_curve.py` & `felupe-8.5.0/src/felupe/mechanics/_curve.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,39 +43,40 @@
         container of the completed substep is available as ``substep.x``. Default
         is ``callback=lambda stepnumber, substepnumber, substep, **kwargs: None``.
     **kwargs : dict, optional
         Optional keyword-arguments for the ``callback`` function.
 
     Examples
     --------
-    >>> import felupe as fem
-    >>>
-    >>> mesh = fem.Cube(n=6)
-    >>> region = fem.RegionHexahedron(mesh)
-    >>> field = fem.FieldContainer([fem.Field(region, dim=3)])
-    >>>
-    >>> boundaries = dict()
-    >>> boundaries["fixed"] = fem.Boundary(field[0], fx=0, skip=(False, False, False))
-    >>> boundaries["clamped"] = fem.Boundary(field[0], fx=1, skip=(True, False, False))
-    >>> boundaries["move"] = fem.Boundary(field[0], fx=1, skip=(False, True, True))
-    >>>
-    >>> umat = fem.NeoHooke(mu=1, bulk=2)
-    >>> solid = fem.SolidBody(umat, field)
-    >>>
-    >>> move = fem.math.linsteps([0, 1], num=5)
-    >>> step = fem.Step(items=[solid], ramp={boundaries["move"]: move}, boundaries=boundaries)
-    >>>
-    >>> job = fem.CharacteristicCurve(steps=[step], boundary=boundaries["move"])
-    >>> job.evaluate()
-    >>> fig, ax = job.plot(
-    >>>    xlabel=r"Displacement $u_1$ in mm $\rightarrow$",
-    >>>    ylabel=r"Normal Force in $F_1$ in N $\rightarrow$",
-    >>>    marker="o",
-    >>> )
-    >>> ax2 = solid.imshow("Principal Values of Cauchy Stress")
+    ..  pyvista-plot::
+
+        >>> import felupe as fem
+        >>>
+        >>> mesh = fem.Cube(n=6)
+        >>> region = fem.RegionHexahedron(mesh)
+        >>> field = fem.FieldContainer([fem.Field(region, dim=3)])
+        >>>
+        >>> boundaries = dict()
+        >>> boundaries["fixed"] = fem.Boundary(field[0], fx=0, skip=(False, False, False))
+        >>> boundaries["clamped"] = fem.Boundary(field[0], fx=1, skip=(True, False, False))
+        >>> boundaries["move"] = fem.Boundary(field[0], fx=1, skip=(False, True, True))
+        >>>
+        >>> umat = fem.NeoHooke(mu=1, bulk=2)
+        >>> solid = fem.SolidBody(umat, field)
+        >>>
+        >>> move = fem.math.linsteps([0, 1], num=5)
+        >>> step = fem.Step(items=[solid], ramp={boundaries["move"]: move}, boundaries=boundaries)
+        >>>
+        >>> job = fem.CharacteristicCurve(steps=[step], boundary=boundaries["move"]).evaluate()
+        >>> fig, ax = job.plot(
+        ...    xlabel=r"Displacement $u_1$ in mm $\rightarrow$",
+        ...    ylabel=r"Normal Force in $F_1$ in N $\rightarrow$",
+        ...    marker="o",
+        ... )
+        >>> solid.plot("Principal Values of Cauchy Stress").show()
 
     See Also
     --------
     Step : A Step with multiple substeps, subsequently depending on the solution
         of the previous substep.
     Job : A job with a list of steps and a method to evaluate them.
     tools.NewtonResult : A data class which represents the result found by
```

### Comparing `felupe-8.4.0/src/felupe/mechanics/_helpers.py` & `felupe-8.5.0/src/felupe/mechanics/_helpers.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/mechanics/_item.py` & `felupe-8.5.0/src/felupe/mechanics/_item.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,23 +47,23 @@
     >>>
     >>> mesh = fem.Cube(n=11)
     >>> region = fem.RegionHexahedron(mesh)
     >>> field = fem.FieldContainer([fem.Field(region, dim=3)])
     >>> boundaries, loadcase = fem.dof.uniaxial(field, clamped=True)
     >>>
     >>> @fem.Form(v=field, u=field)
-    >>> def bilinearform():
-    >>>     def a(v, u, μ=1.0, λ=2.0):
-    >>>         δε, ε = sym(grad(v)), sym(grad(u))
-    >>>         return 2 * μ * ddot(δε, ε) + λ * trace(δε) * trace(ε)
-    >>>     return [a]
+    ... def bilinearform():
+    ...     def a(v, u, μ=1.0, λ=2.0):
+    ...         δε, ε = sym(grad(v)), sym(grad(u))
+    ...         return 2 * μ * ddot(δε, ε) + λ * trace(δε) * trace(ε)
+    ...     return [a]
     >>>
     >>> item = fem.FormItem(bilinearform, linearform=None, sym=True)
     >>> step = fem.Step(items=[item], boundaries=boundaries)
-    >>> fem.Job(steps=[step]).evaluate()
+    >>> job = fem.Job(steps=[step]).evaluate()
 
     See Also
     --------
     felupe.Form : A function decorator for a linear- or bilinear-form object.
     felupe.Step : A Step with multiple substeps.
 
     """
```

### Comparing `felupe-8.4.0/src/felupe/mechanics/_job.py` & `felupe-8.5.0/src/felupe/mechanics/_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,32 +81,34 @@
         List with norms of the objective function for each completed substep of each
         step. See also class:`~felupe.tools.NewtonResult`.
     kwargs : dict
         Optional keyword-arguments for the ``callback`` function.
 
     Examples
     --------
-    >>> import felupe as fem
-    >>>
-    >>> mesh = fem.Cube(n=6)
-    >>> region = fem.RegionHexahedron(mesh)
-    >>> field = fem.FieldContainer([fem.Field(region, dim=3)])
-    >>>
-    >>> boundaries = fem.dof.symmetry(field[0])
-    >>> boundaries["clamped"] = fem.Boundary(field[0], fx=1, skip=(True, False, False))
-    >>> boundaries["move"] = fem.Boundary(field[0], fx=1, skip=(False, True, True))
-    >>>
-    >>> umat = fem.NeoHooke(mu=1, bulk=2)
-    >>> solid = fem.SolidBody(umat, field)
-    >>>
-    >>> move = fem.math.linsteps([0, 1], num=5)
-    >>> step = fem.Step(items=[solid], ramp={boundaries["move"]: move}, boundaries=boundaries)
-    >>>
-    >>> job = fem.Job(steps=[step]).evaluate()
-    >>> ax = solid.imshow("Principal Values of Cauchy Stress")
+    ..  pyvista-plot::
+
+        >>> import felupe as fem
+        >>>
+        >>> mesh = fem.Cube(n=6)
+        >>> region = fem.RegionHexahedron(mesh)
+        >>> field = fem.FieldContainer([fem.Field(region, dim=3)])
+        >>>
+        >>> boundaries = fem.dof.symmetry(field[0])
+        >>> boundaries["clamped"] = fem.Boundary(field[0], fx=1, skip=(True, False, False))
+        >>> boundaries["move"] = fem.Boundary(field[0], fx=1, skip=(False, True, True))
+        >>>
+        >>> umat = fem.NeoHooke(mu=1, bulk=2)
+        >>> solid = fem.SolidBody(umat, field)
+        >>>
+        >>> move = fem.math.linsteps([0, 1], num=5)
+        >>> step = fem.Step(items=[solid], ramp={boundaries["move"]: move}, boundaries=boundaries)
+        >>>
+        >>> job = fem.Job(steps=[step]).evaluate()
+        >>> solid.plot("Principal Values of Cauchy Stress").show()
 
     See Also
     --------
     Step : A Step with multiple substeps, subsequently depending on the solution
         of the previous substep.
     CharacteristicCurve : A job with a list of steps and a method to evaluate them.
         Force-displacement curve data is tracked during evaluation for a given
```

### Comparing `felupe-8.4.0/src/felupe/mechanics/_multipoint.py` & `felupe-8.5.0/src/felupe/mechanics/_multipoint.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/mechanics/_pointload.py` & `felupe-8.5.0/src/felupe/mechanics/_pointload.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/mechanics/_solidbody.py` & `felupe-8.5.0/src/felupe/mechanics/_solidbody.py`

 * *Files 3% similar despite different names*

```diff
@@ -177,33 +177,35 @@
 
     ..  note::
         This class also supports ``umat`` with mixed-field formulations like
         :class:`~felupe.NearlyIncompressible` or :class:`~felupe.ThreeFieldVariation`.
 
     Examples
     --------
-    >>> import felupe as fem
-    >>>
-    >>> mesh = fem.Cube(n=6)
-    >>> region = fem.RegionHexahedron(mesh)
-    >>> field = fem.FieldContainer([fem.Field(region, dim=3)])
-    >>> boundaries, loadcase = fem.dof.uniaxial(field, clamped=True)
-    >>>
-    >>> umat = fem.NeoHooke(mu=1, bulk=2)
-    >>> solid = fem.SolidBody(umat, field)
-    >>>
-    >>> table = fem.math.linsteps([0, 1], num=5)
-    >>> step = fem.Step(
-    >>>     items=[solid],
-    >>>     ramp={boundaries["move"]: table},
-    >>>     boundaries=boundaries,
-    >>> )
-    >>>
-    >>> job = fem.Job(steps=[step]).evaluate()
-    >>> ax = solid.imshow("Principal Values of Cauchy Stress")
+    ..  pyvista-plot::
+
+        >>> import felupe as fem
+        >>>
+        >>> mesh = fem.Cube(n=6)
+        >>> region = fem.RegionHexahedron(mesh)
+        >>> field = fem.FieldContainer([fem.Field(region, dim=3)])
+        >>> boundaries, loadcase = fem.dof.uniaxial(field, clamped=True)
+        >>>
+        >>> umat = fem.NeoHooke(mu=1, bulk=2)
+        >>> solid = fem.SolidBody(umat, field)
+        >>>
+        >>> table = fem.math.linsteps([0, 1], num=5)
+        >>> step = fem.Step(
+        ...     items=[solid],
+        ...     ramp={boundaries["move"]: table},
+        ...     boundaries=boundaries,
+        ... )
+        >>>
+        >>> job = fem.Job(steps=[step]).evaluate()
+        >>> solid.plot("Principal Values of Cauchy Stress").show()
 
     See Also
     --------
     felupe.SolidBodyNearlyIncompressible : A (nearly) incompressible solid body with
         methods for the assembly of sparse vectors/matrices.
     """
```

### Comparing `felupe-8.4.0/src/felupe/mechanics/_solidbody_gravity.py` & `felupe-8.5.0/src/felupe/mechanics/_solidbody_gravity.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,34 +42,36 @@
     ..  math::
 
         \delta W_{ext} = \int_V
             \delta \boldsymbol{u} \cdot \rho \boldsymbol{g} \ dV
 
     Examples
     --------
-    >>> import felupe as fem
-    >>>
-    >>> mesh = fem.Cube(n=6)
-    >>> region = fem.RegionHexahedron(mesh)
-    >>> field = fem.FieldContainer([fem.Field(region, dim=3)])
-    >>> boundaries = fem.dof.symmetry(field[0])
-    >>>
-    >>> umat = fem.NeoHooke(mu=1, bulk=2)
-    >>> solid = fem.SolidBody(umat, field)
-    >>> gravity = fem.SolidBodyGravity(field, density=1.0)
-    >>>
-    >>> table = fem.math.linsteps([0, 1], num=5, axis=0, axes=3)
-    >>> step = fem.Step(
-    >>>     items=[solid, gravity],
-    >>>     ramp={gravity: 2 * table},
-    >>>     boundaries=boundaries,
-    >>> )
-    >>>
-    >>> job = fem.Job(steps=[step]).evaluate()
-    >>> ax = solid.imshow("Principal Values of Cauchy Stress")
+    ..  pyvista-plot::
+
+        >>> import felupe as fem
+        >>>
+        >>> mesh = fem.Cube(n=6)
+        >>> region = fem.RegionHexahedron(mesh)
+        >>> field = fem.FieldContainer([fem.Field(region, dim=3)])
+        >>> boundaries = fem.dof.symmetry(field[0])
+        >>>
+        >>> umat = fem.NeoHooke(mu=1, bulk=2)
+        >>> solid = fem.SolidBody(umat, field)
+        >>> gravity = fem.SolidBodyGravity(field, density=1.0)
+        >>>
+        >>> table = fem.math.linsteps([0, 1], num=5, axis=0, axes=3)
+        >>> step = fem.Step(
+        ...     items=[solid, gravity],
+        ...     ramp={gravity: 2 * table},
+        ...     boundaries=boundaries,
+        ... )
+        >>>
+        >>> job = fem.Job(steps=[step]).evaluate()
+        >>> solid.plot("Principal Values of Cauchy Stress").show()
 
     """
 
     def __init__(self, field, gravity=None, density=1.0):
         self.field = field
         self.results = Results(stress=False, elasticity=False)
         self.assemble = Assemble(vector=self._vector, matrix=self._matrix)
```

### Comparing `felupe-8.4.0/src/felupe/mechanics/_solidbody_incompressible.py` & `felupe-8.5.0/src/felupe/mechanics/_solidbody_incompressible.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,33 +266,35 @@
         :label: nearlyinc-deformed-volume
         
         v = \int_V J\ dV
 
 
     Examples
     --------
-    >>> import felupe as fem
-    >>>
-    >>> mesh = fem.Cube(n=6)
-    >>> region = fem.RegionHexahedron(mesh)
-    >>> field = fem.FieldContainer([fem.Field(region, dim=3)])
-    >>> boundaries, loadcase = fem.dof.uniaxial(field, clamped=True)
-    >>>
-    >>> umat = fem.NeoHooke(mu=1)
-    >>> solid = fem.SolidBodyNearlyIncompressible(umat, field, bulk=5000)
-    >>>
-    >>> table = fem.math.linsteps([0, 1], num=5)
-    >>> step = fem.Step(
-    >>>     items=[solid],
-    >>>     ramp={boundaries["move"]: table},
-    >>>     boundaries=boundaries,
-    >>> )
-    >>>
-    >>> job = fem.Job(steps=[step]).evaluate()
-    >>> ax = solid.imshow("Principal Values of Cauchy Stress")
+    ..  pyvista-plot::
+        
+        >>> import felupe as fem
+        >>>
+        >>> mesh = fem.Cube(n=6)
+        >>> region = fem.RegionHexahedron(mesh)
+        >>> field = fem.FieldContainer([fem.Field(region, dim=3)])
+        >>> boundaries, loadcase = fem.dof.uniaxial(field, clamped=True)
+        >>>
+        >>> umat = fem.NeoHooke(mu=1)
+        >>> solid = fem.SolidBodyNearlyIncompressible(umat, field, bulk=5000)
+        >>>
+        >>> table = fem.math.linsteps([0, 1], num=5)
+        >>> step = fem.Step(
+        ...     items=[solid],
+        ...     ramp={boundaries["move"]: table},
+        ...     boundaries=boundaries,
+        ... )
+        >>>
+        >>> job = fem.Job(steps=[step]).evaluate()
+        >>> solid.plot("Principal Values of Cauchy Stress").show()
     
     References
     ----------
     ..  [1] J. Bonet, A. J. Gil, and R. D. Wood, "Nonlinear Solid Mechanics for Finite
         Element Analysis: Statics". Cambridge University Press, Jun. 05, 2016. 
         doi: 10.1017/cbo9781316336144.
```

### Comparing `felupe-8.4.0/src/felupe/mechanics/_solidbody_pressure.py` & `felupe-8.5.0/src/felupe/mechanics/_solidbody_pressure.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,39 +37,43 @@
     ..  math::
 
         \delta W_{ext} = \int_{\partial V}
             \delta \boldsymbol{u} \cdot p J \boldsymbol{F}^{-T} \ d\boldsymbol{A}
 
     Examples
     --------
-    >>> import felupe as fem
-    >>>
-    >>> mesh = fem.Rectangle(n=6)
-    >>> region = fem.RegionQuad(mesh)
-    >>> field = fem.FieldContainer([fem.FieldAxisymmetric(region, dim=2)])
-    >>> boundaries = fem.dof.symmetry(field[0])
-    >>> umat = fem.NeoHooke(mu=1, bulk=2)
-    >>> solid = fem.SolidBody(umat, field)
-    >>>
-    >>> region_pressure = fem.RegionQuadBoundary(
-    >>>     mesh=mesh,
-    >>>     only_surface=True,  # select only faces on the outline
-    >>>     mask=mesh.points[:, 0] == 1,  # select a subset of faces on the surface
-    >>>     ensure_3d=True,  # requires True for axisymmetric/plane strain, otherwise False
-    >>> )
-    >>> field_boundary = fem.FieldContainer([fem.FieldAxisymmetric(region_pressure, dim=2)])
-    >>> pressure = fem.SolidBodyPressure(field=field_boundary)
-    >>>
-    >>> table = fem.math.linsteps([0, 1], num=5)
-    >>> step = fem.Step(
-    >>>     items=[solid, pressure], ramp={pressure: 1 * table}, boundaries=boundaries
-    >>> )
-    >>>
-    >>> job = fem.Job(steps=[step]).evaluate()
-    >>> ax = solid.imshow("Principal Values of Cauchy Stress", component=2)
+    ..  pyvista-plot::
+
+        >>> import felupe as fem
+        >>>
+        >>> mesh = fem.Rectangle(n=6)
+        >>> region = fem.RegionQuad(mesh)
+        >>> field = fem.FieldContainer([fem.FieldAxisymmetric(region, dim=2)])
+        >>> boundaries = fem.dof.symmetry(field[0])
+        >>> umat = fem.NeoHooke(mu=1, bulk=2)
+        >>> solid = fem.SolidBody(umat, field)
+        >>>
+        >>> region_pressure = fem.RegionQuadBoundary(
+        ...     mesh=mesh,
+        ...     only_surface=True,  # select only faces on the outline
+        ...     mask=mesh.points[:, 0] == 1,  # select a subset of faces on the surface
+        ...     ensure_3d=True,  # requires True for axisymmetric/plane strain, otherwise False
+        ... )
+        >>> field_boundary = fem.FieldContainer([fem.FieldAxisymmetric(region_pressure, dim=2)])
+        >>> pressure = fem.SolidBodyPressure(field=field_boundary)
+        >>>
+        >>> table = fem.math.linsteps([0, 1], num=5)
+        >>> step = fem.Step(
+        ...     items=[solid, pressure], ramp={pressure: 1 * table}, boundaries=boundaries
+        ... )
+        >>>
+        >>> job = fem.Job(steps=[step]).evaluate()
+        >>> solid.plot(
+        ...     "Principal Values of Cauchy Stress", component=2, clim=[-1.01, -0.99]
+        ... ).show()
     """
 
     def __init__(self, field, pressure=None):
         self.field = field
         self._normals = self.field.region.normals
 
         self.results = Results()
```

### Comparing `felupe-8.4.0/src/felupe/mechanics/_step.py` & `felupe-8.5.0/src/felupe/mechanics/_step.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,32 +34,34 @@
         A dict with :class:`~felupe.Boundary` or ``item``-keys which holds the array of
         values to ramp (default is None). If None, only one substep is evaluated.
     boundaries : dict of Boundary, optional
         A dict with :class:`~felupe.Boundary` conditions (default is None).
 
     Examples
     --------
-    >>> import felupe as fem
-    >>>
-    >>> mesh = fem.Cube(n=6)
-    >>> region = fem.RegionHexahedron(mesh)
-    >>> field = fem.FieldContainer([fem.Field(region, dim=3)])
-    >>>
-    >>> boundaries = fem.dof.symmetry(field[0])
-    >>> boundaries["clamped"] = fem.Boundary(field[0], fx=1, skip=(True, False, False))
-    >>> boundaries["move"] = fem.Boundary(field[0], fx=1, skip=(False, True, True))
-    >>>
-    >>> umat = fem.NeoHooke(mu=1, bulk=2)
-    >>> solid = fem.SolidBody(umat, field)
-    >>>
-    >>> move = fem.math.linsteps([0, 1], num=5)
-    >>> step = fem.Step(items=[solid], ramp={boundaries["move"]: move}, boundaries=boundaries)
-    >>>
-    >>> job = fem.Job(steps=[step]).evaluate()
-    >>> ax = solid.imshow("Principal Values of Cauchy Stress")
+    ..  pyvista-plot::
+
+        >>> import felupe as fem
+        >>>
+        >>> mesh = fem.Cube(n=6)
+        >>> region = fem.RegionHexahedron(mesh)
+        >>> field = fem.FieldContainer([fem.Field(region, dim=3)])
+        >>>
+        >>> boundaries = fem.dof.symmetry(field[0])
+        >>> boundaries["clamped"] = fem.Boundary(field[0], fx=1, skip=(True, False, False))
+        >>> boundaries["move"] = fem.Boundary(field[0], fx=1, skip=(False, True, True))
+        >>>
+        >>> umat = fem.NeoHooke(mu=1, bulk=2)
+        >>> solid = fem.SolidBody(umat, field)
+        >>>
+        >>> move = fem.math.linsteps([0, 1], num=5)
+        >>> step = fem.Step(items=[solid], ramp={boundaries["move"]: move}, boundaries=boundaries)
+        >>>
+        >>> job = fem.Job(steps=[step]).evaluate()
+        >>> ax = solid.plot("Principal Values of Cauchy Stress").show()
     """
 
     def __init__(self, items, ramp=None, boundaries=None):
         self.items = items
 
         if ramp is None:
             self.ramp = {}
```

### Comparing `felupe-8.4.0/src/felupe/mesh/__init__.py` & `felupe-8.5.0/src/felupe/mesh/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/mesh/_container.py` & `felupe-8.5.0/src/felupe/mesh/_container.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
            >>> container = fem.MeshContainer([rect1, rect2])
            >>> mesh = container.stack()
            >>>
            >>> mesh.plot().show()
 
         >>> mesh
         <felupe Mesh object>
-          Number of points: 121
+          Number of points: 242
           Number of cells:
             quad: 90
 
         See Also
         --------
         felupe.mesh.stack : Stack cell-blocks from meshes with identical points-array
             and cell-types.
```

### Comparing `felupe-8.4.0/src/felupe/mesh/_convert.py` & `felupe-8.5.0/src/felupe/mesh/_convert.py`

 * *Files 3% similar despite different names*

```diff
@@ -343,15 +343,16 @@
 
        >>> import felupe as fem
        >>>
        >>> mesh = fem.Rectangle(n=6)
        >>> mesh_with_midpoints_edges = fem.mesh.add_midpoints_edges(mesh)
        >>>
        >>> plotter = mesh_with_midpoints_edges.plot(
-       >>>     plotter=mesh.plot(), style="points", color="black")
+       ...     plotter=mesh.plot(), style="points", color="black"
+       ... )
        >>> plotter.show()
 
     >>> mesh_with_midpoints_edges
     <felupe Mesh object>
       Number of points: 96
       Number of cells:
         quad8: 25
@@ -420,24 +421,25 @@
     .. pyvista-plot::
        :include-source: True
 
        >>> import felupe as fem
        >>>
        >>> mesh = fem.Rectangle(n=6)
        >>> mesh_with_midpoints_faces = fem.mesh.add_midpoints_faces(
-       >>>     mesh, cell_type_new="quad"
-       >>> )
+       ...     mesh, cell_type_new="quad"
+       ... )
        >>>
        >>> plotter = mesh_with_midpoints_faces.plot(
-       >>>     plotter=mesh.plot(), style="points", color="black"
-       >>> ).show()
+       ...     plotter=mesh.plot(), style="points", color="black"
+       ... )
+       >>> plotter.show()
 
     >>> mesh_with_midpoints_faces
     <felupe Mesh object>
-      Number of points: 36
+      Number of points: 61
       Number of cells:
         quad: 25
 
     See Also
     --------
     felupe.Mesh.add_midpoints_faces : Add midpoints on faces for given points and cells
         and update cell_type accordingly.
@@ -504,19 +506,19 @@
     .. pyvista-plot::
        :include-source: True
 
        >>> import felupe as fem
        >>>
        >>> mesh = fem.Cube(n=6)
        >>> mesh_with_midpoints_volumes = fem.mesh.add_midpoints_volumes(
-       >>>     mesh, cell_type_new="hexahedron9"
-       >>> )
+       ...     mesh, cell_type_new="hexahedron9"
+       ... )
        >>>
        >>> plotter = mesh.plot(opacity=0.5)
-       >>> plotter.add_points(mesh_with_midpoints_volumes.points, color="black")
+       >>> actor = plotter.add_points(mesh_with_midpoints_volumes.points, color="black")
        >>> plotter.show()
 
     >>> mesh_with_midpoints_volumes
     <felupe Mesh object>
       Number of points: 341
       Number of cells:
         hexahedron9: 125
```

### Comparing `felupe-8.4.0/src/felupe/mesh/_discrete_geometry.py` & `felupe-8.5.0/src/felupe/mesh/_discrete_geometry.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/mesh/_dual.py` & `felupe-8.5.0/src/felupe/mesh/_dual.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,16 +77,16 @@
     >>> import felupe as fem
     >>>
     >>> mesh = fem.Rectangle(n=5).add_midpoints_edges()
     >>> region = fem.RegionQuadraticQuad(mesh=mesh)
     >>>
     >>> mesh_dual = fem.mesh.dual(mesh, points_per_cell=1, disconnect=False)
     >>> region_dual = fem.RegionConstantQuad(
-    >>>     mesh_dual, quadrature=region.quadrature, grad=False
-    >>> )
+    ...     mesh_dual, quadrature=region.quadrature, grad=False
+    ... )
     >>>
     >>> displacement = fem.FieldPlaneStrain(region, dim=2)
     >>> pressure = fem.Field(region_dual)
     >>> field = fem.FieldContainer([displacement, pressure])
 
     See Also
     --------
```

### Comparing `felupe-8.4.0/src/felupe/mesh/_geometry.py` & `felupe-8.5.0/src/felupe/mesh/_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,20 +40,18 @@
     >>> mesh
     <felupe Mesh object>
       Number of points: 1
       Number of cells:
         vertex: 1
 
     >>> mesh.points
-    array([-2.1])
+    array([[-2.1]])
 
     >>> mesh.cells
     array([[0]])
-
-    >>> mesh.imshow()
     """
 
     def __init__(self, a=0.0):
         self.a = a
 
         points = np.array([a]).reshape(1, -1)
         cells = np.array([[0]])
```

### Comparing `felupe-8.4.0/src/felupe/mesh/_helpers.py` & `felupe-8.5.0/src/felupe/mesh/_helpers.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/mesh/_line_rectangle_cube.py` & `felupe-8.5.0/src/felupe/mesh/_line_rectangle_cube.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/mesh/_mesh.py` & `felupe-8.5.0/src/felupe/mesh/_mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,16 +93,16 @@
     .. pyvista-plot::
        :include-source: True
 
        >>> import numpy as np
        >>> import felupe as fem
        >>>
        >>> points = np.array(
-       >>>     [[0.0, 0.0], [0.5, 0.1], [1.0, 0.2], [0.0, 1.0], [0.5, 0.9], [1.0, 0.8]]
-       >>> )
+       ...     [[0.0, 0.0], [0.5, 0.1], [1.0, 0.2], [0.0, 1.0], [0.5, 0.9], [1.0, 0.8]]
+       ... )
        >>> cells = np.array([[0, 1, 4, 3], [1, 2, 5, 4]])
        >>> mesh = fem.Mesh(points, cells, cell_type="quad")
        >>>
        >>> mesh.plot().show()
 
 
     See Also
@@ -365,15 +365,15 @@
         >>> import numpy as np
         >>> import felupe as fem
         >>>
         >>> mesh = fem.Cube(n=11)
         >>> mesh.update(points=np.vstack([mesh.points, mesh.points]))
         >>> point_ids = mesh.get_point_ids([0, 1, 1])
         >>> point_ids
-        array([1320, 2651], dtype=int64)
+        array([1320, 2651])
 
         >>> mesh.points[point_ids]
         array([[0., 1., 1.],
                [0., 1., 1.]])
 
         """
         return np.argwhere(mode(fun(self.points, value, **kwargs), axis=1))[:, 0]
@@ -395,19 +395,19 @@
         --------
         >>> import numpy as np
         >>> import felupe as fem
         >>>
         >>> mesh = fem.Cube(n=11)
         >>> point_ids = mesh.get_point_ids([0, 1, 1])
         >>> point_ids
-        array([1320], dtype=int64)
+        array([1320])
 
         >>> cell_ids = mesh.get_cell_ids(point_ids)
         >>> cell_ids
-        array([990], dtype=int64)
+        array([990])
 
         """
         return np.argwhere(np.isin(self.cells, point_ids).any(axis=1))[:, 0]
 
     def get_cell_ids_neighbours(self, cell_ids):
         """Return cell ids which share points with given cell ids.
 
@@ -425,24 +425,25 @@
         --------
         >>> import numpy as np
         >>> import felupe as fem
         >>>
         >>> mesh = fem.Cube(n=11)
         >>> point_ids = mesh.get_point_ids([0, 1, 1])
         >>> point_ids
-        array([1320], dtype=int64)
+        array([1320])
 
         >>> cell_ids = mesh.get_cell_ids(point_ids)
         >>> cell_ids
-        array([990], dtype=int64)
+        array([990])
 
         Find the cell ids which share at least one point with the given cell id(s).
 
         >>> cell_ids_neighbours = mesh.get_cell_ids_neighbours(cell_ids)
-        array([880, 881, 890, 891, 980, 981, 990, 991], dtype=int64)
+        >>> cell_ids_neighbours
+        array([880, 881, 890, 891, 980, 981, 990, 991])
 
         """
         return self.get_cell_ids(self.cells[cell_ids])
 
     def get_point_ids_shared(self, cell_ids_neighbours):
         """Return shared point ids for given cell ids.
 
@@ -460,24 +461,25 @@
         --------
         >>> import numpy as np
         >>> import felupe as fem
         >>>
         >>> mesh = fem.Cube(n=11)
         >>> point_ids = mesh.get_point_ids([0, 1, 1])
         >>> point_ids
-        array([1320], dtype=int64)
+        array([1320])
 
         >>> cell_ids = mesh.get_cell_ids(point_ids)
         >>> cell_ids
-        array([990], dtype=int64)
+        array([990])
 
         Find the cell ids which share at least one point with the given cell id(s).
 
         >>> cell_ids_neighbours = mesh.get_cell_ids_neighbours(cell_ids)
-        array([880, 881, 890, 891, 980, 981, 990, 991], dtype=int64)
+        >>> cell_ids_neighbours
+        array([880, 881, 890, 891, 980, 981, 990, 991])
 
         Find the shared point ids for the list of cell ids.
 
         >>> point_ids_shared = mesh.get_point_ids_shared(cell_ids_neighbours)
         >>> point_ids_shared
         array([1189])
 
@@ -499,15 +501,15 @@
         --------
         >>> import numpy as np
         >>> import felupe as fem
         >>>
         >>> mesh = fem.Cube(n=11)
         >>> point_ids_corners = mesh.get_point_ids_corners()
         >>> point_ids_corners
-        array([   0, 1210,   10, 1220,  110, 1320,  120, 1330], dtype=int64)
+        array([   0, 1210,   10, 1220,  110, 1320,  120, 1330])
 
         """
 
         xmin = np.min(self.points, axis=0)
         xmax = np.max(self.points, axis=0)
         points = np.vstack(
             [x.ravel() for x in np.meshgrid(*np.vstack([xmin, xmax]).T)]
@@ -537,26 +539,28 @@
         3. Get the shared point of the cell and its neighbours.
         4. Get pair-wise shared points which are located on an edge.
         5. Replace the shared points with the corner point.
         6. Delete the cell attached to the corner point.
 
         Examples
         --------
-        >>> import numpy as np
-        >>> import felupe as fem
-        >>>
-        >>> mesh = fem.Rectangle(b=(3, 1), n=(16, 6))
+        ..  pyvista-plot::
+            :context:
 
-        ..  image:: images/mesh_corners_before.png
-            :width: 400px
+            >>> import numpy as np
+            >>> import felupe as fem
+            >>>
+            >>> mesh = fem.Rectangle(b=(3, 1), n=(16, 6))
+            >>> mesh.plot().show()
 
-        >>> mesh = mesh.modify_corners()  # inplace
+        ..  pyvista-plot::
+            :context:
 
-        ..  image:: images/mesh_corners_after.png
-            :width: 400px
+            >>> mesh = mesh.modify_corners()  # inplace
+            >>> mesh.plot().show()
 
         """
 
         if self.cell_type not in ["quad", "hexahedron"]:
             message = [
                 "Cell type not supported.",
                 "Must be either 'quad' or 'hexahedron'",
@@ -649,16 +653,16 @@
         >>> import felupe as fem
         >>>
         >>> mesh = fem.Rectangle(n=5).add_midpoints_edges()
         >>> region = fem.RegionQuadraticQuad(mesh=mesh)
         >>>
         >>> mesh_dual = mesh.dual(points_per_cell=1, disconnect=False)
         >>> region_dual = fem.RegionConstantQuad(
-        >>>     mesh_dual, quadrature=region.quadrature, grad=False
-        >>> )
+        ...     mesh_dual, quadrature=region.quadrature, grad=False
+        ... )
         >>>
         >>> displacement = fem.FieldPlaneStrain(region, dim=2)
         >>> pressure = fem.Field(region_dual)
         >>> field = fem.FieldContainer([displacement, pressure])
 
         See Also
         --------
@@ -1025,16 +1029,16 @@
         .. pyvista-plot::
            :include-source: True
 
            >>> import felupe as fem
            >>>
            >>> inner = fem.mesh.revolve(fem.Point(1)).expand(z=0.4).translate(0.2, axis=2)
            >>> outer = fem.mesh.revolve(fem.Point(2), phi=160).rotate(
-           >>>     axis=2, angle_deg=20
-           >>> ).expand(z=1.2)
+           ...     axis=2, angle_deg=20
+           ... ).expand(z=1.2)
            >>> mesh = inner.fill_between(outer, n=6)
            >>>
            >>> mesh.plot().show()
 
         See Also
         --------
         felupe.mesh.fill_between : Fill a 2d-Quad Mesh between two 1d-Line Meshes, embedded
@@ -1066,18 +1070,14 @@
 
         >>> import numpy as np
         >>> import felupe as fem
         >>>
         >>> mesh = fem.Rectangle(n=3)
         >>> mesh.update(points=mesh.points * np.array([[-1, 1]]))
         >>> region = fem.RegionQuad(mesh)
-        UserWarning: Negative volumes for cells
-         [0 1 2 3]
-        Try ``mesh.flip(np.any(region.dV < 0, axis=0))`` and re-create the region.
-          warnings.warn(message_negative_volumes)
 
         The sum of the differential volumes :math:`V = \sum_c \sum_q dV_{qc}` is evaluated
         to -1.0.
 
         >>> region.dV.sum()
         -1.0
 
@@ -1172,19 +1172,19 @@
 
         Examples
         --------
         >>> import felupe as fem
         >>>
         >>> mesh = fem.Circle(n=6)
         >>> mesh.points.min(axis=0), mesh.points.max(axis=0)
-        (array([0., 0., 0.]), array([1., 1., 1.]))
+        (array([-1., -1.]), array([1., 1.]))
 
         >>> translated = mesh.translate(0.3, axis=1)
         >>> translated.points.min(axis=0), translated.points.max(axis=0)
-        (array([0. , 0.3, 0. ]), array([1. , 1.3, 1. ]))
+        (array([-1. , -0.7]), array([1. , 1.3]))
 
         See Also
         --------
         felupe.mesh.translate : Translate (move) a Mesh along a given axis.
         """
 
         return as_mesh(translate(self, move=move, axis=axis))
@@ -1429,16 +1429,16 @@
 
            >>> import felupe as fem
            >>>
            >>> mesh = fem.Rectangle(n=6)
            >>> mesh_with_midpoints_edges = mesh.add_midpoints_edges()
            >>>
            >>> mesh_with_midpoints_edges.plot(
-           >>>     plotter=mesh.plot(), style="points", color="black"
-           >>> ).show()
+           ...     plotter=mesh.plot(), style="points", color="black"
+           ... ).show()
 
         >>> mesh_with_midpoints_edges
         <felupe Mesh object>
           Number of points: 96
           Number of cells:
             quad8: 25
 
@@ -1472,20 +1472,20 @@
 
            >>> import felupe as fem
            >>>
            >>> mesh = fem.Rectangle(n=6)
            >>> mesh_with_midpoints_faces = mesh.add_midpoints_faces(cell_type="quad")
            >>>
            >>> mesh_with_midpoints_faces.plot(
-           >>>     plotter=mesh.plot(), style="points", color="black"
-           >>> ).show()
+           ...     plotter=mesh.plot(), style="points", color="black"
+           ... ).show()
 
         >>> mesh_with_midpoints_faces
         <felupe Mesh object>
-          Number of points: 36
+          Number of points: 61
           Number of cells:
             quad: 25
 
         See Also
         --------
         felupe.mesh.add_midpoints_faces : Add midpoints on faces for given points and
             cells and update cell_type accordingly.
@@ -1512,19 +1512,19 @@
         .. pyvista-plot::
            :include-source: True
 
            >>> import felupe as fem
            >>>
            >>> mesh = fem.Cube(n=6)
            >>> mesh_with_midpoints_volumes = fem.mesh.add_midpoints_volumes(
-           >>>     mesh, cell_type_new="hexahedron9"
-           >>> )
+           ...     mesh, cell_type_new="hexahedron9"
+           ... )
            >>>
            >>> plotter = mesh.plot(opacity=0.5)
-           >>> plotter.add_points(mesh_with_midpoints_volumes.points, color="black")
+           >>> actor = plotter.add_points(mesh_with_midpoints_volumes.points, color="black")
            >>> plotter.show()
 
         >>> mesh_with_midpoints_volumes
         <felupe Mesh object>
           Number of points: 341
           Number of cells:
             hexahedron9: 125
```

### Comparing `felupe-8.4.0/src/felupe/mesh/_read.py` & `felupe-8.5.0/src/felupe/mesh/_read.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/mesh/_tools.py` & `felupe-8.5.0/src/felupe/mesh/_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,16 +166,16 @@
     .. pyvista-plot::
        :include-source: True
 
        >>> import felupe as fem
        >>>
        >>> inner = fem.mesh.revolve(fem.Point(1)).expand(z=0.4).translate(0.2, axis=2)
        >>> outer = fem.mesh.revolve(fem.Point(2), phi=160).rotate(
-       >>>     axis=2, angle_deg=20
-       >>> ).expand(z=1.2)
+       ...     axis=2, angle_deg=20
+       ... ).expand(z=1.2)
        >>> mesh = fem.mesh.fill_between(inner, outer, n=6)
        >>>
        >>> mesh.plot().show()
 
     See Also
     --------
     felupe.Mesh.fill_between : Fill a 2d-Quad Mesh between two 1d-Line Meshes, embedded
@@ -644,19 +644,19 @@
 
     Examples
     --------
     >>> import felupe as fem
     >>>
     >>> mesh = fem.Circle(n=6)
     >>> mesh.points.min(axis=0), mesh.points.max(axis=0)
-    (array([0., 0., 0.]), array([1., 1., 1.]))
+    (array([-1., -1.]), array([1., 1.]))
 
     >>> translated = fem.mesh.translate(mesh, 0.3, axis=1)
     >>> translated.points.min(axis=0), translated.points.max(axis=0)
-    (array([0. , 0.3, 0. ]), array([1. , 1.3, 1. ]))
+    (array([-1. , -0.7]), array([1. , 1.3]))
 
     See Also
     --------
     felupe.Mesh.translate : Translate (move) a Mesh along a given axis.
     """
 
     points_new = np.array(points)
@@ -698,18 +698,14 @@
 
     >>> import numpy as np
     >>> import felupe as fem
     >>>
     >>> mesh = fem.Rectangle(n=3)
     >>> mesh.update(points=mesh.points * np.array([[-1, 1]]))
     >>> region = fem.RegionQuad(mesh)
-    UserWarning: Negative volumes for cells
-     [0 1 2 3]
-    Try ``mesh.flip(np.any(region.dV < 0, axis=0))`` and re-create the region.
-      warnings.warn(message_negative_volumes)
 
     The sum of the differential volumes :math:`V = \sum_c \sum_q dV_{qc}` is evaluated
     to -1.0.
 
     >>> region.dV.sum()
     -1.0
```

### Comparing `felupe-8.4.0/src/felupe/quadrature/_gausslegendre.py` & `felupe-8.5.0/src/felupe/quadrature/_gausslegendre.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,60 +50,60 @@
         \int_{-1}^1 f(x) dx \approx \sum f(x_q) w_q
 
     with quadrature points :math:`x_q` and corresponding weights :math:`w_q`.
 
     Examples
     --------
     .. pyvista-plot::
-       :include-source: True
+       :force_static:
 
        >>> import felupe as fem
        >>>
        >>> element = fem.Line()
        >>> quadrature = fem.GaussLegendre(order=2, dim=1)
        >>> quadrature.plot(
-       >>>     plotter=element.plot(add_point_labels=False, show_points=False),
-       >>>     weighted=True,
-       >>> ).show()
+       ...     plotter=element.plot(add_point_labels=False, show_points=False),
+       ...     weighted=True,
+       ... ).show()
 
     .. pyvista-plot::
-       :include-source: True
+       :force_static:
 
        >>> import felupe as fem
        >>>
        >>> element = fem.QuadraticQuad()
        >>> quadrature = fem.GaussLegendre(order=2, dim=2)
        >>> quadrature.plot(
-       >>>     plotter=element.plot(add_point_labels=False, show_points=False),
-       >>>     weighted=True,
-       >>> ).show()
+       ...     plotter=element.plot(add_point_labels=False, show_points=False),
+       ...     weighted=True,
+       ... ).show()
 
     .. pyvista-plot::
-       :include-source: True
+       :force_static:
 
        >>> import felupe as fem
        >>>
        >>> element = fem.QuadraticHexahedron()
        >>> quadrature = fem.GaussLegendre(order=2, dim=3)
        >>> quadrature.plot(
-       >>>     plotter=element.plot(add_point_labels=False, show_points=False),
-       >>>     weighted=True,
-       >>> ).show()
+       ...     plotter=element.plot(add_point_labels=False, show_points=False),
+       ...     weighted=True,
+       ... ).show()
 
     .. pyvista-plot::
-       :include-source: True
+       :force_static:
 
        >>> import felupe as fem
        >>>
        >>> element = fem.ArbitraryOrderLagrangeElement(order=5, dim=2)
        >>> quadrature = fem.GaussLegendre(order=5, dim=2)
        >>> quadrature.plot(
-       >>>     plotter=element.plot(add_point_labels=False, show_points=False),
-       >>>     weighted=True,
-       >>> ).show()
+       ...     plotter=element.plot(add_point_labels=False, show_points=False),
+       ...     weighted=True,
+       ... ).show()
     """
 
     def __init__(self, order: int, dim: int, permute: bool = True):
         if dim not in [1, 2, 3]:
             raise ValueError("Wrong dimension.")
 
         x, w = np.polynomial.legendre.leggauss(1 + order)
@@ -186,41 +186,41 @@
        :include-source: True
 
        >>> import felupe as fem
        >>>
        >>> element = fem.QuadraticQuad()
        >>> quadrature = fem.GaussLegendreBoundary(order=2, dim=2)
        >>> quadrature.plot(
-       >>>     plotter=element.plot(add_point_labels=False, show_points=False),
-       >>>     weighted=True,
-       >>> ).show()
+       ...     plotter=element.plot(add_point_labels=False, show_points=False),
+       ...     weighted=True,
+       ... ).show()
 
     .. pyvista-plot::
        :include-source: True
 
        >>> import felupe as fem
        >>>
        >>> element = fem.QuadraticHexahedron()
        >>> quadrature = fem.GaussLegendreBoundary(order=2, dim=3)
        >>> quadrature.plot(
-       >>>     plotter=element.plot(add_point_labels=False, show_points=False),
-       >>>     weighted=True,
-       >>> ).show()
+       ...     plotter=element.plot(add_point_labels=False, show_points=False),
+       ...     weighted=True,
+       ... ).show()
 
     .. pyvista-plot::
        :include-source: True
 
        >>> import felupe as fem
        >>>
        >>> element = fem.ArbitraryOrderLagrangeElement(order=5, dim=3)
        >>> quadrature = fem.GaussLegendreBoundary(order=5, dim=3)
        >>> quadrature.plot(
-       >>>     plotter=element.plot(add_point_labels=False, show_points=False),
-       >>>     weighted=True,
-       >>> ).show()
+       ...     plotter=element.plot(add_point_labels=False, show_points=False),
+       ...     weighted=True,
+       ... ).show()
 
     """
 
     def __init__(self, order: int, dim: int, permute: bool = True):
         super().__init__(order=order, dim=dim - 1, permute=permute)
 
         # reset dimension
```

### Comparing `felupe-8.4.0/src/felupe/quadrature/_scheme.py` & `felupe-8.5.0/src/felupe/quadrature/_scheme.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/quadrature/_sphere.py` & `felupe-8.5.0/src/felupe/quadrature/_sphere.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,16 +14,18 @@
 
 You should have received a copy of the GNU General Public License
 along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
+from ._scheme import Scheme
 
-class BazantOh:
+
+class BazantOh(Scheme):
     r"""Quadrature scheme for a numeric integration of the surface of a unit sphere
     [1]_.
 
     Parameters
     ----------
     n : int, optional
         The number of quadrature points (default is 21).
@@ -36,31 +38,42 @@
 
         \int_{\partial V} f(x) dA \approx \sum f(x_q) w_q
 
     with quadrature points :math:`x_q` and corresponding weights :math:`w_q`.
 
     Examples
     --------
-    >>> import felupe as fem
-    >>>
-    >>> quadrature = fem.BazantOh(n=21)
+
+    .. pyvista-plot::
+       :force_static:
+
+       >>> import felupe as fem
+       >>> import pyvista as pv
+       >>>
+       >>> quadrature = fem.BazantOh(n=21)
+       >>>
+       >>> plotter = quadrature.plot(weighted=True)
+       >>> sphere = pv.Sphere(radius=1).clip(normal="z", invert=False)
+       >>> actor = plotter.add_mesh(sphere, opacity=0.3, color="white")
+       >>> plotter.show()
 
     References
     ----------
     .. [1] Bazant, Z. P., & Oh, B. H. (1986). Efficient Numerical Integration on
        the Surface of a Sphere. ZAMM ‐ Journal of Applied Mathematics and
        Mechanics / Zeitschrift für Angewandte Mathematik und Mechanik, 66(1),
        37-49. https://doi.org/10.1002/zamm.19860660108
     """
 
     def __init__(self, n: int = 21):
         schemes = {
             21: self._scheme_21,
         }
-        self.points, self.weights = schemes[n]()
+        points, weights = schemes[n]()
+        super().__init__(points=points, weights=weights)
 
     def _scheme_21(self):
         "2x21-point scheme (degree 9, orthogonal symmetries)."
 
         a = np.sqrt(2) / 2
         b = 0.836095596749
         c = 0.387907304067
```

### Comparing `felupe-8.4.0/src/felupe/quadrature/_tetra.py` & `felupe-8.5.0/src/felupe/quadrature/_tetra.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,49 +42,49 @@
         \int_V f(x) dV \approx \sum f(x_q) w_q
 
     with quadrature points :math:`x_q` and corresponding weights :math:`w_q` [1]_.
 
     Examples
     --------
     .. pyvista-plot::
-       :include-source: True
+       :force_static:
 
        >>> import felupe as fem
        >>>
        >>> element = fem.Tetra()
        >>> quadrature = fem.TetrahedronQuadrature(order=1)
        >>> quadrature.plot(
-       >>>     plotter=element.plot(add_point_labels=False, show_points=False),
-       >>>     weighted=True,
-       >>> ).show()
+       ...     plotter=element.plot(add_point_labels=False, show_points=False),
+       ...     weighted=True,
+       ... ).show()
 
 
     .. pyvista-plot::
-       :include-source: True
+       :force_static:
 
        >>> import felupe as fem
        >>>
        >>> element = fem.QuadraticTetra()
        >>> quadrature = fem.TetrahedronQuadrature(order=2)
        >>> quadrature.plot(
-       >>>     plotter=element.plot(add_point_labels=False, show_points=False),
-       >>>     weighted=True,
-       >>> ).show()
+       ...     plotter=element.plot(add_point_labels=False, show_points=False),
+       ...     weighted=True,
+       ... ).show()
 
     .. pyvista-plot::
-       :include-source: True
+       :force_static:
 
        >>> import felupe as fem
        >>>
        >>> element = fem.QuadraticTetra()
        >>> quadrature = fem.TetrahedronQuadrature(order=5)
        >>> quadrature.plot(
-       >>>     plotter=element.plot(add_point_labels=False, show_points=False),
-       >>>     weighted=True,
-       >>> ).show()
+       ...     plotter=element.plot(add_point_labels=False, show_points=False),
+       ...     weighted=True,
+       ... ).show()
 
     References
     ----------
     .. [1] O. C. Zienkiewicz, R. L. Taylor and J. Z. Zhu, The Finite Element Method: Its
        Basis and Fundamentals, 7th ed., Elsevier, 2013.
     """
```

### Comparing `felupe-8.4.0/src/felupe/quadrature/_triangle.py` & `felupe-8.5.0/src/felupe/quadrature/_triangle.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,49 +42,49 @@
         \int_A f(x) dA \approx \sum f(x_q) w_q
 
     with quadrature points :math:`x_q` and corresponding weights :math:`w_q` [1]_ [2]_.
 
     Examples
     --------
     .. pyvista-plot::
-       :include-source: True
+       :force_static:
 
        >>> import felupe as fem
        >>>
        >>> element = fem.Triangle()
        >>> quadrature = fem.TriangleQuadrature(order=1)
        >>> quadrature.plot(
-       >>>     plotter=element.plot(add_point_labels=False, show_points=False),
-       >>>     weighted=True,
-       >>> ).show()
+       ...     plotter=element.plot(add_point_labels=False, show_points=False),
+       ...     weighted=True,
+       ... ).show()
 
 
     .. pyvista-plot::
-       :include-source: True
+       :force_static:
 
        >>> import felupe as fem
        >>>
        >>> element = fem.QuadraticTriangle()
        >>> quadrature = fem.TriangleQuadrature(order=2)
        >>> quadrature.plot(
-       >>>     plotter=element.plot(add_point_labels=False, show_points=False),
-       >>>     weighted=True,
-       >>> ).show()
+       ...     plotter=element.plot(add_point_labels=False, show_points=False),
+       ...     weighted=True,
+       ... ).show()
 
     .. pyvista-plot::
-       :include-source: True
+       :force_static:
 
        >>> import felupe as fem
        >>>
        >>> element = fem.QuadraticTriangle()
        >>> quadrature = fem.TriangleQuadrature(order=5)
        >>> quadrature.plot(
-       >>>     plotter=element.plot(add_point_labels=False, show_points=False),
-       >>>     weighted=True,
-       >>> ).show()
+       ...     plotter=element.plot(add_point_labels=False, show_points=False),
+       ...     weighted=True,
+       ... ).show()
 
     References
     ----------
     .. [1] K. J. Bathe, Finite element procedures, 2nd ed. K. J. Bathe, Watertown, MA,
        2014.
     .. [2] O. C. Zienkiewicz, R. L. Taylor and J. Z. Zhu, The Finite Element Method: Its
        Basis and Fundamentals, 7th ed., Elsevier, 2013.
```

### Comparing `felupe-8.4.0/src/felupe/region/__init__.py` & `felupe-8.5.0/src/felupe/region/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/region/_boundary.py` & `felupe-8.5.0/src/felupe/region/_boundary.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,15 +334,15 @@
     geometric gradient :math:`\partial X_I / \partial r_J` and the weights `w` of the
     quadrature points. The differential area vectors array is of shape
     ``(nquadraturepoints, ndim, nboundarycells)``.
 
     >>> region.dA
     array([[[ 0.  , -0.5 ,  0.  ,  0.5 ,  0.  ,  0.  ],
             [ 0.  , -0.5 ,  0.  ,  0.5 ,  0.  ,  0.  ]],
-
+    <BLANKLINE>
            [[-0.25, -0.  , -0.25, -0.  ,  0.25,  0.25],
             [-0.25, -0.  , -0.25, -0.  ,  0.25,  0.25]]])
 
     In a boundary region, the numeric differential volumes are the magnitudes of the
     differential area vectors. For a quad mesh, the boundary cell volumes are the edge
     lengths.
 
@@ -351,15 +351,15 @@
 
     Unit normal vectors are obtained by the ratio of the differential area vectors and
     the differential volumes.
 
     >>> region.dA / region.dV  ## this is equal to ``region.normals``
     array([[[ 0., -1.,  0.,  1.,  0.,  0.],
             [ 0., -1.,  0.,  1.,  0.,  0.]],
-
+    <BLANKLINE>
            [[-1., -0., -1., -0.,  1.,  1.],
             [-1., -0., -1., -0.,  1.,  1.]]])
 
     The partial derivative of the first element shape function w.r.t. the undeformed
     coordinates evaluated at the second integration point of the last element of the
     region:
```

### Comparing `felupe-8.4.0/src/felupe/region/_region.py` & `felupe-8.5.0/src/felupe/region/_region.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/region/_templates.py` & `felupe-8.5.0/src/felupe/region/_templates.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/solve/_solve.py` & `felupe-8.5.0/src/felupe/solve/_solve.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/tools/__init__.py` & `felupe-8.5.0/src/felupe/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/tools/_misc.py` & `felupe-8.5.0/src/felupe/tools/_misc.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/tools/_newton.py` & `felupe-8.5.0/src/felupe/tools/_newton.py`

 * *Files 6% similar despite different names*

```diff
@@ -324,15 +324,28 @@
     --------
     >>> import felupe as fem
 
     >>> region = fem.RegionHexahedron(fem.Cube(n=6))
     >>> field = fem.FieldContainer([fem.Field(region, dim=3)])
     >>> boundaries, loadcase = fem.dof.uniaxial(field, move=0.2, clamped=True)
     >>> solid = fem.SolidBody(umat=fem.NeoHooke(mu=1.0, bulk=2.0), field=field)
-    >>> res = fem.newtonrhapson(items=[solid], **loadcase)
+    >>> res = fem.newtonrhapson(items=[solid], **loadcase)  # doctest: +ELLIPSIS
+    <BLANKLINE>
+    Newton-Rhapson solver
+    =====================
+    <BLANKLINE>
+    | # | norm(fun) |  norm(dx) |
+    |---|-----------|-----------|
+    | 1 | 7.553e-02 | 1.898e+00 |
+    | 2 | 1.310e-03 | 5.091e-02 |
+    | 3 | 3.086e-07 | 6.698e-04 |
+    | 4 | 2.255e-14 | 1.527e-07 |
+    <BLANKLINE>
+    Converged in 4 iterations ...
+    <BLANKLINE>
 
     Newton's method had success
 
     >>> res.success
     True
 
     and 4 iterations were needed to converge within the specified tolerance.
@@ -340,15 +353,15 @@
     >>> res.iterations
     4
 
     The norm of the objective function for all active degrees of freedom is lower than
     3e-15.
 
     >>> np.linalg.norm(res.fun[loadcase["dof1"]])
-    2.7482611016095555e-15
+    2.7384964752762237e-15
 
     """
     if verbose is None:
         FELUPE_VERBOSE = os.environ.get("FELUPE_VERBOSE")
         if FELUPE_VERBOSE is None:
             verbose = True
         else:
```

### Comparing `felupe-8.4.0/src/felupe/tools/_plot.py` & `felupe-8.5.0/src/felupe/tools/_plot.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/tools/_post.py` & `felupe-8.5.0/src/felupe/tools/_post.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/tools/_project.py` & `felupe-8.5.0/src/felupe/tools/_project.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe/tools/_save.py` & `felupe-8.5.0/src/felupe/tools/_save.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,16 +60,15 @@
     >>> field = fem.FieldContainer([fem.Field(region, dim=3)])
     >>>
     >>> boundaries, loadcase = fem.dof.uniaxial(field, clamped=True, move=0.3)
     >>>
     >>> umat = fem.NeoHooke(mu=1)
     >>> solid = fem.SolidBodyNearlyIncompressible(umat, field, bulk=5000)
     >>> step = fem.Step(items=[solid], boundaries=boundaries)
-    >>> job = fem.CharacteristicCurve(steps=[step], boundary=boundaries["move"])
-    >>> job.evaluate()
+    >>> job = fem.CharacteristicCurve(steps=[step], boundary=boundaries["move"]).evaluate()
 
     >>> fem.save(region, field, forces=job.res.fun, gradient=solid.results.stress)
 
     """
 
     u = field.fields[0]
     mesh = region.mesh
```

### Comparing `felupe-8.4.0/src/felupe/tools/_solve.py` & `felupe-8.5.0/src/felupe/tools/_solve.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/src/felupe.egg-info/PKG-INFO` & `felupe-8.5.0/src/felupe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: felupe
-Version: 8.4.0
+Version: 8.5.0
 Summary: Finite Element Analysis
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -733,15 +733,15 @@
 Requires-Dist: felupe[io,parallel,plot,progress,view]; extra == "all"
 
 <p align="center">
   <a href="https://felupe.readthedocs.io/en/latest/?badge=latest"><img src="https://user-images.githubusercontent.com/5793153/235789118-eb03eb25-2556-401d-8a0f-580f37e72f8d.png" height="80px"/></a>
   <p align="center"><i>Finite element analysis for continuum mechanics of solid bodies.</i></p>
 </p>
 
-[![FElupe](https://img.shields.io/badge/%F0%9F%94%8D-FElupe-white)](https://felupe.readthedocs.io) [![PyPI version shields.io](https://img.shields.io/pypi/v/felupe.svg)](https://pypi.python.org/pypi/felupe/) [![Documentation Status](https://readthedocs.org/projects/felupe/badge/?version=latest)](https://felupe.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/felupe/branch/main/graph/badge.svg?token=J2QP6Y6LVH)](https://codecov.io/gh/adtzlr/felupe) [![DOI](https://zenodo.org/badge/360657894.svg)](https://zenodo.org/badge/latestdoi/360657894) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black) ![PyPI - Downloads](https://img.shields.io/pypi/dm/felupe) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/adtzlr/felupe-web/main?labpath=notebooks/binder/01_Getting-Started.ipynb) [![lite-badge](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://adtzlr.github.io/felupe-web/lab?path=01_Getting-Started.ipynb) <a target="_blank" href="https://colab.research.google.com/github/adtzlr/felupe-web/blob/main/notebooks/colab/01_Getting-Started.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
+[![FElupe](https://img.shields.io/badge/%F0%9F%94%8D-FElupe-white)](https://felupe.readthedocs.io) [![PyPI version shields.io](https://img.shields.io/pypi/v/felupe.svg)](https://pypi.python.org/pypi/felupe/) [![Documentation Status](https://readthedocs.org/projects/felupe/badge/?version=latest)](https://felupe.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![codecov](https://codecov.io/gh/adtzlr/felupe/branch/main/graph/badge.svg?token=J2QP6Y6LVH)](https://codecov.io/gh/adtzlr/felupe) [![DOI](https://zenodo.org/badge/360657894.svg)](https://zenodo.org/badge/latestdoi/360657894) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black) ![PyPI - Downloads](https://img.shields.io/pypi/dm/felupe) [![lite-badge](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://adtzlr.github.io/felupe-web/lab?path=01_Getting-Started.ipynb) <a target="_blank" href="https://colab.research.google.com/github/adtzlr/felupe-web/blob/main/notebooks/colab/01_Getting-Started.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
 
 FElupe is a Python 3.8+ 🐍 finite element analysis package 📦 focussing on the formulation and numerical solution of nonlinear problems in continuum mechanics 🔧 of solid bodies 🚂. Its name is a combination of FE (finite element) and the german word *Lupe* 🔍 (magnifying glass) as a synonym for getting an insight 📖 how a finite element analysis code 🧮 looks like under the hood 🕳️.
 
 <p align="center">
   <a href="https://felupe.readthedocs.io/en/latest/examples/ex01_beam.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex01_beam_thumb.png" height="160px"/></a> <a href="https://felupe.readthedocs.io/en/latest/examples/ex02_plate-with-hole.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex02_plate-with-hole_thumb.png" height="160px"/></a> <a 
   href="https://felupe.readthedocs.io/en/latest/examples/ex03_plasticity.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex03_plasticity_thumb.png" height="160px"/></a> <a 
   href="https://felupe.readthedocs.io/en/latest/examples/ex04_balloon.html"><img src="https://felupe.readthedocs.io/en/latest/_images/sphx_glr_ex04_balloon_thumb.png" height="160px"/></a> <a
```

### Comparing `felupe-8.4.0/src/felupe.egg-info/SOURCES.txt` & `felupe-8.5.0/src/felupe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/tests/test_basis.py` & `felupe-8.5.0/tests/test_basis.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/tests/test_bilinearform.py` & `felupe-8.5.0/tests/test_bilinearform.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/tests/test_composite.py` & `felupe-8.5.0/tests/test_composite.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/tests/test_constitution.py` & `felupe-8.5.0/tests/test_constitution.py`

 * *Files 6% similar despite different names*

```diff
@@ -293,15 +293,15 @@
 
     linear_elastic = fem.Material(stress, elasticity, mu=1, lmbda=2)
 
     s, statevars_new = linear_elastic.gradient([F, None])
     dsde = linear_elastic.hessian([F, None])
 
 
-def test_umat_hyperelastic(savefig=False):
+def test_umat_hyperelastic():
     r, x = pre(sym=False, add_identity=True)
     F = x[0]
 
     import matplotlib.pyplot as plt
     import tensortrax.math as tm
 
     def neo_hooke(C, mu=1):
@@ -332,21 +332,16 @@
         ),
     ]:
         umat = fem.Hyperelastic(model, **kwargs)
 
         s, statevars_new = umat.gradient([F, None])
         dsde = umat.hessian([F, None])
 
-        if savefig:
-            ax = umat.screenshot(
-                filename=f"../docs/felupe/images/umat_{umat.fun.__name__}.png",
-                incompressible=incompressible,
-            )
-
     for incompressible in [False, True]:
+        ax = umat.plot(incompressible=incompressible)
         ax = umat.screenshot(incompressible=incompressible)
 
 
 def test_umat_hyperelastic2():
     r, x = pre(sym=False, add_identity=True, add_random=True)
     F = x[0]
 
@@ -371,15 +366,15 @@
     s2, statevars_new = umat.gradient([F, None])
     dsde2 = umat.hessian([F, None])
 
     assert np.allclose(s, s2)
     assert np.allclose(dsde, dsde2)
 
 
-def test_umat_viscoelastic(savefig=False):
+def test_umat_viscoelastic():
     r, x = pre(sym=False, add_identity=True, add_random=True)
     F = x[0]
 
     import tensortrax.math as tm
 
     def viscoelastic(C, Cin, mu, eta, dtime):
         "Finite strain viscoelastic material formulation."
@@ -398,22 +393,20 @@
     statevars = np.zeros((6, *F.shape[-2:]))
     s, statevars_new = umat.gradient([F, statevars])
     dsde = umat.hessian([F, statevars])
 
     umat = fem.Hyperelastic(
         fem.constitution.finite_strain_viscoelastic, nstatevars=6, **kwargs
     )
-    if savefig:
-        ax = umat.screenshot(
-            filename="../docs/felupe/images/umat_finite_strain_viscoelastic.png",
-            ux=fem.math.linsteps([1, 1.5, 1, 2, 1, 2.5, 1], num=15),
-            ps=None,
-            bx=None,
-            incompressible=True,
-        )
+    umat.plot(
+        ux=fem.math.linsteps([1, 1.5, 1, 2, 1, 2.5, 1], num=15),
+        ps=None,
+        bx=None,
+        incompressible=True,
+    )
 
     s2, statevars_new = umat.gradient([F, statevars])
     dsde2 = umat.hessian([F, statevars])
 
     assert np.allclose(s, s2)
     assert np.allclose(dsde, dsde2)
 
@@ -509,22 +502,71 @@
 
     ax = umat.plot()
 
     dWdF, statevars_new = umat.gradient([F, None])
     (d2WdFdF,) = umat.hessian([F, None])
 
 
+def test_optimize():
+    stretches, stresses = (
+        np.array(
+            [
+                [1.000, 0.00],
+                [1.020, 0.26],
+                [1.125, 1.37],
+                [1.240, 2.30],
+                [1.390, 3.23],
+                [1.585, 4.16],
+                [1.900, 5.10],
+                [2.180, 6.00],
+                [2.420, 6.90],
+                [3.020, 8.80],
+                [3.570, 10.7],
+                [4.030, 12.5],
+                [4.760, 16.2],
+                [5.360, 19.9],
+                [5.750, 23.6],
+                [6.150, 27.4],
+                [6.400, 31.0],
+                [6.600, 34.8],
+                [6.850, 38.5],
+                [7.050, 42.1],
+                [7.150, 45.8],
+                [7.250, 49.6],
+                [7.400, 53.3],
+                [7.500, 57.0],
+                [7.600, 64.4],
+            ]
+        )
+        * np.array([1.0, 0.0980665])
+    ).T
+
+    for model in [
+        fem.neo_hooke,
+        fem.ogden,
+        fem.third_order_deformation,
+        fem.extended_tube,
+    ]:
+        umat = fem.Hyperelastic(model)
+        umat_new, res = umat.optimize(ux=[stretches, stresses], incompressible=True)
+
+        ux = np.linspace(stretches.min(), stretches.max(), num=200)
+        ax = umat_new.plot(incompressible=True, ux=ux, bx=None, ps=None)
+        ax.plot(stretches, stresses, "C0x")
+
+
 if __name__ == "__main__":
     test_nh()
     test_linear()
     test_linear_planestress()
     test_linear_planestrain()
     test_kinematics()
     test_umat()
-    test_umat_hyperelastic(savefig=True)
+    test_umat_hyperelastic()
     test_umat_hyperelastic2()
-    test_umat_viscoelastic(savefig=True)
+    test_umat_viscoelastic()
     test_umat_viscoelastic2()
     test_umat_strain()
     test_umat_strain_plasticity()
     test_elpliso()
     test_composite()
+    test_optimize()
```

### Comparing `felupe-8.4.0/tests/test_constitution_newton.py` & `felupe-8.5.0/tests/test_constitution_newton.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/tests/test_dof.py` & `felupe-8.5.0/tests/test_dof.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/tests/test_element.py` & `felupe-8.5.0/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/tests/test_field.py` & `felupe-8.5.0/tests/test_field.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/tests/test_form.py` & `felupe-8.5.0/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/tests/test_job.py` & `felupe-8.5.0/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/tests/test_math.py` & `felupe-8.5.0/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/tests/test_mechanics.py` & `felupe-8.5.0/tests/test_mechanics.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/tests/test_mesh.py` & `felupe-8.5.0/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/tests/test_mpc.py` & `felupe-8.5.0/tests/test_mpc.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/tests/test_planestrain.py` & `felupe-8.5.0/tests/test_planestrain.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/tests/test_plot.py` & `felupe-8.5.0/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/tests/test_quadrature.py` & `felupe-8.5.0/tests/test_quadrature.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/tests/test_readme.py` & `felupe-8.5.0/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/tests/test_region.py` & `felupe-8.5.0/tests/test_region.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/tests/test_solve.py` & `felupe-8.5.0/tests/test_solve.py`

 * *Files identical despite different names*

### Comparing `felupe-8.4.0/tests/test_tools.py` & `felupe-8.5.0/tests/test_tools.py`

 * *Files identical despite different names*

