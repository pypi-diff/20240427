# Comparing `tmp/pillow_jxl_plugin-1.2.3.tar.gz` & `tmp/pillow_jxl_plugin-1.2.4.tar.gz`

## Comparing `pillow_jxl_plugin-1.2.3.tar` & `pillow_jxl_plugin-1.2.4.tar`

### file list

```diff
@@ -1,63 +1,66 @@
--rw-r--r--   0     1001      127     1506 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/Cargo.toml
--rw-r--r--   0     1001      127    35148 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/COPYING
--rw-r--r--   0     1001      127      698 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/LICENSE
--rw-r--r--   0     1001      127     3767 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/README.md
--rw-r--r--   0     1001      127     1439 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/benches/decode.rs
--rw-r--r--   0     1001      127     1829 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/benches/encode.rs
--rw-r--r--   0     1001      127     3667 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/common.rs
--rw-r--r--   0     1001      127     3211 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/decode/result.rs
--rw-r--r--   0     1001      127    17932 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/decode.rs
--rw-r--r--   0     1001      127    22931 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/encode.rs
--rw-r--r--   0     1001      127     4368 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/errors.rs
--rw-r--r--   0     1001      127     7720 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/image.rs
--rw-r--r--   0     1001      127     5835 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/lib.rs
--rw-r--r--   0     1001      127     4491 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/memory.rs
--rw-r--r--   0     1001      127     3298 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/parallel/resizable_runner.rs
--rw-r--r--   0     1001      127     3130 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/parallel/threads_runner.rs
--rw-r--r--   0     1001      127     3332 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/parallel.rs
--rw-r--r--   0     1001      127     4162 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/tests/decode.rs
--rw-r--r--   0     1001      127     5918 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/tests/encode.rs
--rw-r--r--   0     1001      127      480 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/tests.rs
--rw-r--r--   0     1001      127     1536 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/utils.rs
--rw-r--r--   0     1001      127     3767 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/README.md
--rw-r--r--   0     1001      127       78 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/Cargo.toml
--rw-r--r--   0     1001      127      968 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/Cargo.toml
--rw-r--r--   0     1001      127    35148 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/COPYING
--rw-r--r--   0     1001      127      697 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/LICENSE
--rw-r--r--   0     1001      127      618 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/README.md
--rw-r--r--   0     1001      127     1138 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/build.rs
--rw-r--r--   0     1001      127     2292 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/cms.rs
--rw-r--r--   0     1001      127     2884 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/codestream_header.rs
--rw-r--r--   0     1001      127     1259 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/color_encoding.rs
--rw-r--r--   0     1001      127     9423 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/decode.rs
--rw-r--r--   0     1001      127    10492 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/encode.rs
--rw-r--r--   0     1001      127    14713 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/lib.rs
--rw-r--r--   0     1001      127      371 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/memory_manager.rs
--rw-r--r--   0     1001      127      551 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/parallel_runner.rs
--rw-r--r--   0     1001      127     1529 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/resizable_parallel_runner.rs
--rw-r--r--   0     1001      127      981 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/stats.rs
--rw-r--r--   0     1001      127     1379 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/thread_parallel_runner.rs
--rw-r--r--   0     1001      127     1821 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/types.rs
--rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 pillow_jxl_plugin-1.2.3/Cargo.toml
--rw-r--r--   0     1001      127      451 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/.github/dependabot.yml
--rw-r--r--   0     1001      127     6270 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/.github/workflows/release.yml
--rw-r--r--   0     1001      127     1877 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/.github/workflows/test.yml
--rw-r--r--   0     1001      127      725 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/.gitignore
--rw-r--r--   0     1001      127      108 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/.gitmodules
--rw-r--r--   0     1001      127     1065 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/LICENSE
--rw-r--r--   0     1001      127     1931 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/README.md
--rw-r--r--   0     1001      127     1862 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/build.rs
--rw-r--r--   0     1001      127     4296 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/pillow_jxl/JpegXLImagePlugin.py
--rw-r--r--   0     1001      127      165 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/pillow_jxl/__init__.py
--rw-r--r--   0     1001      127     1182 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/pillow_jxl/__init__.pyi
--rw-r--r--   0     1001      127        0 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/pillow_jxl/py.typed
--rw-r--r--   0     1001      127        7 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/requirements-dev.txt
--rw-r--r--   0     1001      127     2818 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/src/decode.rs
--rw-r--r--   0     1001      127     4356 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/src/encode.rs
--rw-r--r--   0     1001      127      298 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/src/lib.rs
--rw-r--r--   0     1001      127   106457 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/test/images/icc_profile/62AHB.jpg
--rw-r--r--   0     1001      127    80683 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/test/images/icc_profile/62AHB.jxl
--rw-r--r--   0     1001      127      395 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/test/test_plugin.py
--rw-r--r--   0     1001      127    12051 2024-04-15 05:31:30.000000 pillow_jxl_plugin-1.2.3/Cargo.lock
--rw-r--r--   0     1001      127      426 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     2336 1970-01-01 00:00:00.000000 pillow_jxl_plugin-1.2.3/PKG-INFO
+-rw-r--r--   0     1001      127      968 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/Cargo.toml
+-rw-r--r--   0     1001      127    35148 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/COPYING
+-rw-r--r--   0     1001      127      697 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/LICENSE
+-rw-r--r--   0     1001      127      618 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/README.md
+-rw-r--r--   0     1001      127     1138 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/build.rs
+-rw-r--r--   0     1001      127     2292 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/src/cms.rs
+-rw-r--r--   0     1001      127     2884 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/src/codestream_header.rs
+-rw-r--r--   0     1001      127     1259 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/src/color_encoding.rs
+-rw-r--r--   0     1001      127     9423 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/src/decode.rs
+-rw-r--r--   0     1001      127    10492 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/src/encode.rs
+-rw-r--r--   0     1001      127    14713 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/src/lib.rs
+-rw-r--r--   0     1001      127      371 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/src/memory_manager.rs
+-rw-r--r--   0     1001      127      551 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/src/parallel_runner.rs
+-rw-r--r--   0     1001      127     1529 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/src/resizable_parallel_runner.rs
+-rw-r--r--   0     1001      127      981 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/src/stats.rs
+-rw-r--r--   0     1001      127     1379 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/src/thread_parallel_runner.rs
+-rw-r--r--   0     1001      127     1821 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/src/types.rs
+-rw-r--r--   0     1001      127       78 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/Cargo.toml
+-rw-r--r--   0     1001      127     1506 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/Cargo.toml
+-rw-r--r--   0     1001      127    35148 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/COPYING
+-rw-r--r--   0     1001      127      698 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/LICENSE
+-rw-r--r--   0     1001      127     3767 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/README.md
+-rw-r--r--   0     1001      127     1439 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/benches/decode.rs
+-rw-r--r--   0     1001      127     1829 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/benches/encode.rs
+-rw-r--r--   0     1001      127     3667 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/src/common.rs
+-rw-r--r--   0     1001      127     3211 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/src/decode/result.rs
+-rw-r--r--   0     1001      127    18925 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/src/decode.rs
+-rw-r--r--   0     1001      127    22931 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/src/encode.rs
+-rw-r--r--   0     1001      127     4368 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/src/errors.rs
+-rw-r--r--   0     1001      127     7720 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/src/image.rs
+-rw-r--r--   0     1001      127     5835 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/src/lib.rs
+-rw-r--r--   0     1001      127     4491 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/src/memory.rs
+-rw-r--r--   0     1001      127     3298 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/src/parallel/resizable_runner.rs
+-rw-r--r--   0     1001      127     3130 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/src/parallel/threads_runner.rs
+-rw-r--r--   0     1001      127     3332 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/src/parallel.rs
+-rw-r--r--   0     1001      127     4162 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/src/tests/decode.rs
+-rw-r--r--   0     1001      127     5918 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/src/tests/encode.rs
+-rw-r--r--   0     1001      127      480 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/src/tests.rs
+-rw-r--r--   0     1001      127     1536 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/src/utils.rs
+-rw-r--r--   0     1001      127     3767 2024-04-27 16:50:20.000000 pillow_jxl_plugin-1.2.4/jpegxl-rs/README.md
+-rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 pillow_jxl_plugin-1.2.4/Cargo.toml
+-rw-r--r--   0     1001      127      451 2024-04-27 16:50:19.000000 pillow_jxl_plugin-1.2.4/.github/dependabot.yml
+-rw-r--r--   0     1001      127     6501 2024-04-27 16:50:19.000000 pillow_jxl_plugin-1.2.4/.github/workflows/release.yml
+-rw-r--r--   0     1001      127     1918 2024-04-27 16:50:19.000000 pillow_jxl_plugin-1.2.4/.github/workflows/test.yml
+-rw-r--r--   0     1001      127      725 2024-04-27 16:50:19.000000 pillow_jxl_plugin-1.2.4/.gitignore
+-rw-r--r--   0     1001      127      108 2024-04-27 16:50:19.000000 pillow_jxl_plugin-1.2.4/.gitmodules
+-rw-r--r--   0     1001      127     1065 2024-04-27 16:50:19.000000 pillow_jxl_plugin-1.2.4/LICENSE
+-rw-r--r--   0     1001      127     1931 2024-04-27 16:50:19.000000 pillow_jxl_plugin-1.2.4/README.md
+-rw-r--r--   0     1001      127     1862 2024-04-27 16:50:19.000000 pillow_jxl_plugin-1.2.4/build.rs
+-rw-r--r--   0     1001      127     4420 2024-04-27 16:50:19.000000 pillow_jxl_plugin-1.2.4/pillow_jxl/JpegXLImagePlugin.py
+-rw-r--r--   0     1001      127      165 2024-04-27 16:50:19.000000 pillow_jxl_plugin-1.2.4/pillow_jxl/__init__.py
+-rw-r--r--   0     1001      127     1182 2024-04-27 16:50:19.000000 pillow_jxl_plugin-1.2.4/pillow_jxl/__init__.pyi
+-rw-r--r--   0     1001      127        0 2024-04-27 16:50:19.000000 pillow_jxl_plugin-1.2.4/pillow_jxl/py.typed
+-rw-r--r--   0     1001      127        7 2024-04-27 16:50:19.000000 pillow_jxl_plugin-1.2.4/requirements-dev.txt
+-rw-r--r--   0     1001      127     2829 2024-04-27 16:50:19.000000 pillow_jxl_plugin-1.2.4/src/decode.rs
+-rw-r--r--   0     1001      127     4356 2024-04-27 16:50:19.000000 pillow_jxl_plugin-1.2.4/src/encode.rs
+-rw-r--r--   0     1001      127      298 2024-04-27 16:50:19.000000 pillow_jxl_plugin-1.2.4/src/lib.rs
+-rw-r--r--   0     1001      127   106457 2024-04-27 16:50:19.000000 pillow_jxl_plugin-1.2.4/test/images/icc_profile/62AHB.jpg
+-rw-r--r--   0     1001      127    80683 2024-04-27 16:50:19.000000 pillow_jxl_plugin-1.2.4/test/images/icc_profile/62AHB.jxl
+-rw-r--r--   0     1001      127     1779 2024-04-27 16:50:19.000000 pillow_jxl_plugin-1.2.4/test/images/sample.jpg
+-rw-r--r--   0     1001      127     3815 2024-04-27 16:50:19.000000 pillow_jxl_plugin-1.2.4/test/images/sample.jxl
+-rw-r--r--   0     1001      127     4579 2024-04-27 16:50:19.000000 pillow_jxl_plugin-1.2.4/test/images/sample.png
+-rw-r--r--   0     1001      127     1358 2024-04-27 16:50:19.000000 pillow_jxl_plugin-1.2.4/test/test_plugin.py
+-rw-r--r--   0     1001      127    12282 2024-04-27 16:50:43.000000 pillow_jxl_plugin-1.2.4/Cargo.lock
+-rw-r--r--   0     1001      127      426 2024-04-27 16:50:19.000000 pillow_jxl_plugin-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2336 1970-01-01 00:00:00.000000 pillow_jxl_plugin-1.2.4/PKG-INFO
```

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/Cargo.toml` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/Cargo.toml`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/COPYING` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/COPYING`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/LICENSE` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/LICENSE`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/README.md` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/README.md`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/benches/decode.rs` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/benches/decode.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/benches/encode.rs` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/benches/encode.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/common.rs` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/src/common.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/decode/result.rs` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/src/decode/result.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/decode.rs` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/src/decode.rs`

 * *Files 2% similar despite different names*

```diff
@@ -489,14 +489,44 @@
             if jpeg_buf.is_empty() {
                 Data::Pixels(Pixels::new(buffer, unsafe { &pixel_format.assume_init() }))
             } else {
                 Data::Jpeg(jpeg_buf)
             },
         ))
     }
+
+    /// Reconstruct JPEG data. Fallback to pixels in a specific pixel type if JPEG reconstruction fails
+    ///
+    /// # Note
+    /// You can reconstruct JPEG data or get pixels in one go
+    ///
+    /// # Errors
+    /// Return a [`DecodeError`] when internal decoder fails
+    pub fn reconstruct_with<T: PixelType>(&self, data: &[u8]) -> Result<(Metadata, Data), DecodeError> {
+        let mut buffer = vec![];
+        let mut pixel_format = MaybeUninit::uninit();
+        let mut jpeg_buf = vec![];
+        let metadata = self.decode_internal(
+            data,
+            Some(T::pixel_type()),
+            self.icc_profile,
+            Some(&mut jpeg_buf),
+            pixel_format.as_mut_ptr(),
+            &mut buffer,
+        )?;
+
+        Ok((
+            metadata,
+            if jpeg_buf.is_empty() {
+                Data::Pixels(Pixels::new(buffer, unsafe { &pixel_format.assume_init() }))
+            } else {
+                Data::Jpeg(jpeg_buf)
+            },
+        ))
+    }
 }
 
 impl<'prl, 'mm> Drop for JxlDecoder<'prl, 'mm> {
     fn drop(&mut self) {
         unsafe { JxlDecoderDestroy(self.dec) };
     }
 }
```

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/encode.rs` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/src/encode.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/errors.rs` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/src/errors.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/image.rs` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/src/image.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/lib.rs` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/memory.rs` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/src/memory.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/parallel/resizable_runner.rs` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/src/parallel/resizable_runner.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/parallel/threads_runner.rs` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/src/parallel/threads_runner.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/parallel.rs` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/src/parallel.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/tests/decode.rs` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/src/tests/decode.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/tests/encode.rs` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/src/tests/encode.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/utils.rs` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/src/utils.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/README.md` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/README.md`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/Cargo.toml` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/Cargo.toml`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/COPYING` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-rs/COPYING`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/LICENSE` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/LICENSE`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/README.md` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/README.md`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/build.rs` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/build.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/cms.rs` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/src/cms.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/codestream_header.rs` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/src/codestream_header.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/color_encoding.rs` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/src/color_encoding.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/decode.rs` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/src/decode.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/encode.rs` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/src/encode.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/lib.rs` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/parallel_runner.rs` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/src/parallel_runner.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/resizable_parallel_runner.rs` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/src/resizable_parallel_runner.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/stats.rs` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/src/stats.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/thread_parallel_runner.rs` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/src/thread_parallel_runner.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/types.rs` & `pillow_jxl_plugin-1.2.4/jpegxl-rs/jpegxl-sys/src/types.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/Cargo.toml` & `pillow_jxl_plugin-1.2.4/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pillow-jxl-plugin"
-version = "1.2.3"
+version = "1.2.4"
 edition = "2021"
 build = "build.rs"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pillow_jxl"
 crate-type = ["cdylib"]
```

### Comparing `pillow_jxl_plugin-1.2.3/.github/workflows/release.yml` & `pillow_jxl_plugin-1.2.4/.github/workflows/release.yml`

 * *Files 4% similar despite different names*

```diff
@@ -126,24 +126,31 @@
       - uses: actions/checkout@v4
         with:
           submodules: recursive
 
       - uses: actions/setup-python@v5
         with:
           architecture: ${{ matrix.target }}
+      
+      - name: Check dependencys
+        run: |
+          brew install jpeg-xl
+          ls /opt/homebrew/Cellar/jpeg-xl/
+          ls /opt/homebrew/Cellar/brotli/
+          ls /opt/homebrew/Cellar/highway/
 
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         env: 
           RUST_BACKTRACE: 1
           MACOSX_DEPLOYMENT_TARGET: 12.7
           # from homebrew
-          DEP_JXL_LIB: /usr/local/Cellar/jpeg-xl/0.10.2/lib
-          DEP_BROTLI_LIB: /usr/local/Cellar/brotli/1.1.0/lib
-          DEP_HWY_LIB: /usr/local/Cellar/highway/1.1.0/lib
+          DEP_JXL_LIB: /opt/homebrew/Cellar/jpeg-xl/0.10.2/lib
+          DEP_BROTLI_LIB: /opt/homebrew/Cellar/brotli/1.1.0/lib
+          DEP_HWY_LIB: /opt/homebrew/Cellar/highway/1.1.0/lib
         with:
           target: ${{ matrix.target }}
           args: --release --out dist --find-interpreter --features dynamic
           sccache: 'true'
 
       - name: Upload wheels
         uses: actions/upload-artifact@v4
@@ -182,15 +189,15 @@
       - uses: actions/download-artifact@v4
         with:
           pattern: wheels-*
       - name: upload to github release
         uses: softprops/action-gh-release@v2
         with:
           files: |
-            *.whl
+            wheels-*/*.whl
           prerelease: ${{ contains(github.ref, 'alpha') || contains(github.ref, 'beta') || contains(github.ref, 'dev') }}
       - name: Publish to TestPyPI
         if: ${{ contains(github.ref, 'alpha') || contains(github.ref, 'beta') || contains(github.ref, 'dev') }}
         uses: PyO3/maturin-action@v1
         env:
           MATURIN_PYPI_TOKEN: ${{ secrets.TESTPYPI_API_TOKEN }}
           MATURIN_REPOSITORY_URL: https://test.pypi.org/legacy/
```

### Comparing `pillow_jxl_plugin-1.2.3/.github/workflows/test.yml` & `pillow_jxl_plugin-1.2.4/.github/workflows/test.yml`

 * *Files 23% similar despite different names*

```diff
@@ -36,29 +36,30 @@
         run: rustup show
 
       - name: Cache Rust
         uses: Swatinem/rust-cache@v2
 
       - name: Install Plugin
         run: |
-          export DEP_JXL_LIB=/usr/local/Cellar/jpeg-xl/0.10.2/lib
-          export DEP_BROTLI_LIB=/usr/local/Cellar/brotli/1.1.0/lib
-          export DEP_HWY_LIB=/usr/local/Cellar/highway/1.1.0/lib
+          brew install jpeg-xl
+          export DEP_JXL_LIB=/opt/homebrew/Cellar/jpeg-xl/0.10.2/lib
+          export DEP_BROTLI_LIB=/opt/homebrew/Cellar/brotli/1.1.0/lib
+          export DEP_HWY_LIB=/opt/homebrew/Cellar/highway/1.1.0/lib
           source venv/bin/activate
           pip install maturin
           maturin develop --features dynamic
     
       - name: Test with pytest
         run: |
           source venv/bin/activate
           pip install -r requirements-dev.txt
           pytest test/ --junitxml=junit/test-results-${{ matrix.python-version }}.xml
 
       - name: Upload pytest test results
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
           name: pytest-results-${{ matrix.python-version }}
           path: junit/test-results-${{ matrix.python-version }}.xml
         # Use always() to always run this step to publish test results when there are test failures
         if: ${{ always() }}
```

### Comparing `pillow_jxl_plugin-1.2.3/.gitignore` & `pillow_jxl_plugin-1.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/LICENSE` & `pillow_jxl_plugin-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/README.md` & `pillow_jxl_plugin-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/build.rs` & `pillow_jxl_plugin-1.2.4/build.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/pillow_jxl/JpegXLImagePlugin.py` & `pillow_jxl_plugin-1.2.4/pillow_jxl/JpegXLImagePlugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,40 +102,40 @@
     # default quality is 90
     lossless = info.get("lossless", False)
     quality = 0 if lossless else _quality_to_frame_distance(info.get("quality", 90))
 
     decoding_speed = info.get("decoding_speed", 0)
     effort = info.get("effort", 7)
     use_container = info.get("use_container", True)
+    use_original_profile = info.get("use_original_profile", True)
 
     enc = Encoder(
         mode=im.mode,
         lossless=lossless,
         quality=quality,
         decoding_speed=decoding_speed,
         effort=effort,
         use_container=use_container,
+        use_original_profile=use_original_profile,
     )
     # FIXME (Isotr0py): im.filename maybe None if parse stream
     # TODO (Isotr0py): This part should be refactored in the near future
     if im.format == "JPEG" and im.filename:
         with open(im.filename, "rb") as f:
             data = enc(f.read(), im.width, im.height, jpeg_encode=True)
     else:
         exif = info.get("exif", im.getexif().tobytes())
         if exif and exif.startswith(b"Exif\x00\x00"):
             exif = exif[6:]
         metadata = {
-            "exif": exif,
+            "exif": exif if exif is not None else b"",
             "jumb": info.get("jumb", b""),
             "xmp": info.get("xmp", b""),
         }
-        data = enc(
-            im.tobytes(), im.width, im.height, jpeg_encode=False, **metadata
-        )
+        data = enc(im.tobytes(), im.width, im.height, jpeg_encode=False, **metadata)
     fp.write(data)
 
 
 Image.register_open(JXLImageFile.format, JXLImageFile, _accept)
 Image.register_save(JXLImageFile.format, _save)
 Image.register_extension(JXLImageFile.format, ".jxl")
 Image.register_mime(JXLImageFile.format, "image/jxl")
```

### Comparing `pillow_jxl_plugin-1.2.3/pillow_jxl/__init__.pyi` & `pillow_jxl_plugin-1.2.4/pillow_jxl/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/src/decode.rs` & `pillow_jxl_plugin-1.2.4/src/decode.rs`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
                     .icc_profile(true)
                     .parallel_runner(&parallel_runner)
                     .build()
                     .unwrap()
             }
             false => decoder_builder().icc_profile(true).build().unwrap(),
         };
-        let (info, img) = decoder.reconstruct(&data).unwrap();
+        let (info, img) = decoder.reconstruct_with::<u8>(&data).unwrap();
         let (jpeg, img) = match img {
             Data::Jpeg(x) => (true, x),
             Data::Pixels(Pixels::Uint8(x)) => (false, x),
             _ => panic!("Unsupported dtype for decoding"),
         };
         let icc_profile: Vec<u8> = match &info.icc_profile {
             Some(x) => x.to_vec(),
```

### Comparing `pillow_jxl_plugin-1.2.3/src/encode.rs` & `pillow_jxl_plugin-1.2.4/src/encode.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/test/images/icc_profile/62AHB.jpg` & `pillow_jxl_plugin-1.2.4/test/images/icc_profile/62AHB.jpg`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/test/images/icc_profile/62AHB.jxl` & `pillow_jxl_plugin-1.2.4/test/images/icc_profile/62AHB.jxl`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.3/Cargo.lock` & `pillow_jxl_plugin-1.2.4/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 name = "autocfg"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "bitflags"
-version = "1.3.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
 name = "cc"
-version = "1.0.94"
+version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17f6e324229dc011159fcc089755d1e2e216a90d43a7dea6853ca740b84f35e7"
+checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -177,17 +177,17 @@
 name = "libc"
 version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "memoffset"
@@ -202,38 +202,38 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
 
 [[package]]
 name = "pillow-jxl-plugin"
-version = "1.2.3"
+version = "1.2.4"
 dependencies = [
  "jpegxl-rs",
  "pyo3",
 ]
 
 [[package]]
 name = "pkg-config"
@@ -245,26 +245,26 @@
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.80"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a56dea16b0a29e94408b9aa5e2940a4eedbd128a1ba20e8f7ae60fd3d465af0e"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -272,49 +272,49 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
  "syn",
 ]
@@ -326,17 +326,17 @@
 checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
@@ -353,43 +353,43 @@
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
 name = "syn"
-version = "2.0.59"
+version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4a6531ffc7b071655e4ce2e04bd464c4830bb585a61cabb96cf808f05172615a"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "thiserror"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
+checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
+checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -402,61 +402,68 @@
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "windows-targets"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
+ "windows_i686_gnullvm",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.48.5"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
```

### Comparing `pillow_jxl_plugin-1.2.3/PKG-INFO` & `pillow_jxl_plugin-1.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pillow-jxl-plugin
-Version: 1.2.3
+Version: 1.2.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: packaging
 Requires-Dist: pillow
 License-File: LICENSE
 Requires-Python: >=3.8
```

