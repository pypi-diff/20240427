# Comparing `tmp/rapidgzip-0.8.1.tar.gz` & `tmp/rapidgzip-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidgzip-0.8.1.tar", last modified: Fri Aug  4 20:40:31 2023, max compression
+gzip compressed data, was "rapidgzip-0.9.0.tar", last modified: Wed Aug 30 20:03:54 2023, max compression
```

## Comparing `rapidgzip-0.8.1.tar` & `rapidgzip-0.9.0.tar`

### file list

```diff
@@ -1,153 +1,156 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:40:31.589851 rapidgzip-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11598 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/LICENSE-APACHE
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/LICENSE-MIT
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18221 2023-08-04 20:40:31.589851 rapidgzip-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16904 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:40:31.577851 rapidgzip-0.8.1/core/
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/AffinityHelpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/AlignedAllocator.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/AtomicMutex.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/BitManipulation.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    33408 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/BitReader.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11168 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/BitStringFinder.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    27049 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/BlockFetcher.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/BlockFinder.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/BlockFinderInterface.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/BlockMap.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/Cache.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/FasterVector.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    26576 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/FileUtils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/JoiningThread.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12027 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/ParallelBitStringFinder.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11696 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/Prefetcher.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/Statistics.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/StreamedResults.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/TestHelpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/ThreadPool.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/VectorView.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17649 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/common.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:40:31.577851 rapidgzip-0.8.1/core/filereader/
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/filereader/BufferView.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/filereader/Buffered.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/filereader/FileReader.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/filereader/Memory.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/filereader/Python.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12076 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/filereader/Shared.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/filereader/Standard.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7806 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/core/filereader/StreamAdapter.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:40:31.569851 rapidgzip-0.8.1/external/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:40:31.577851 rapidgzip-0.8.1/external/cxxopts/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-08-04 20:40:05.000000 rapidgzip-0.8.1/external/cxxopts/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:40:31.577851 rapidgzip-0.8.1/external/cxxopts/include/
--rw-r--r--   0 runner    (1001) docker     (123)    57765 2023-08-04 20:40:05.000000 rapidgzip-0.8.1/external/cxxopts/include/cxxopts.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:40:31.577851 rapidgzip-0.8.1/external/isa-l/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-08-04 20:40:06.000000 rapidgzip-0.8.1/external/isa-l/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:40:31.581851 rapidgzip-0.8.1/external/isa-l/igzip/
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-08-04 20:40:06.000000 rapidgzip-0.8.1/external/isa-l/igzip/huff_codes.h
--rw-r--r--   0 runner    (1001) docker     (123)   379753 2023-08-04 20:40:06.000000 rapidgzip-0.8.1/external/isa-l/igzip/hufftables_c.c
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-08-04 20:40:06.000000 rapidgzip-0.8.1/external/isa-l/igzip/igzip.c
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-08-04 20:40:06.000000 rapidgzip-0.8.1/external/isa-l/igzip/igzip_checksums.h
--rw-r--r--   0 runner    (1001) docker     (123)    22135 2023-08-04 20:40:06.000000 rapidgzip-0.8.1/external/isa-l/igzip/igzip_decode_block_stateless.asm
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-04 20:40:06.000000 rapidgzip-0.8.1/external/isa-l/igzip/igzip_decode_block_stateless_01.asm
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-04 20:40:06.000000 rapidgzip-0.8.1/external/isa-l/igzip/igzip_decode_block_stateless_04.asm
--rw-r--r--   0 runner    (1001) docker     (123)    75924 2023-08-04 20:40:06.000000 rapidgzip-0.8.1/external/isa-l/igzip/igzip_inflate.c
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-08-04 20:40:06.000000 rapidgzip-0.8.1/external/isa-l/igzip/igzip_inflate_multibinary.asm
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-08-04 20:40:06.000000 rapidgzip-0.8.1/external/isa-l/igzip/igzip_wrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-08-04 20:40:06.000000 rapidgzip-0.8.1/external/isa-l/igzip/inflate_data_structs.asm
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-08-04 20:40:06.000000 rapidgzip-0.8.1/external/isa-l/igzip/rfc1951_lookup.asm
--rw-r--r--   0 runner    (1001) docker     (123)   142279 2023-08-04 20:40:06.000000 rapidgzip-0.8.1/external/isa-l/igzip/static_inflate.h
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-08-04 20:40:06.000000 rapidgzip-0.8.1/external/isa-l/igzip/stdmac.asm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:40:31.581851 rapidgzip-0.8.1/external/isa-l/include/
--rw-r--r--   0 runner    (1001) docker     (123)    30750 2023-08-04 20:40:06.000000 rapidgzip-0.8.1/external/isa-l/include/igzip_lib.h
--rw-r--r--   0 runner    (1001) docker     (123)    11018 2023-08-04 20:40:06.000000 rapidgzip-0.8.1/external/isa-l/include/multibinary.asm
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-08-04 20:40:06.000000 rapidgzip-0.8.1/external/isa-l/include/reg_sizes.asm
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-08-04 20:40:06.000000 rapidgzip-0.8.1/external/isa-l/include/unaligned.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:40:31.581851 rapidgzip-0.8.1/external/rpmalloc/
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-08-04 20:40:07.000000 rapidgzip-0.8.1/external/rpmalloc/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:40:31.581851 rapidgzip-0.8.1/external/rpmalloc/rpmalloc/
--rw-r--r--   0 runner    (1001) docker     (123)   128343 2023-08-04 20:40:07.000000 rapidgzip-0.8.1/external/rpmalloc/rpmalloc/rpmalloc.c
--rw-r--r--   0 runner    (1001) docker     (123)    18023 2023-08-04 20:40:07.000000 rapidgzip-0.8.1/external/rpmalloc/rpmalloc/rpmalloc.h
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-08-04 20:40:07.000000 rapidgzip-0.8.1/external/rpmalloc/rpmalloc/rpnew.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:40:31.585851 rapidgzip-0.8.1/external/zlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-04 20:40:07.000000 rapidgzip-0.8.1/external/zlib/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-08-04 20:40:07.000000 rapidgzip-0.8.1/external/zlib/adler32.c
--rw-r--r--   0 runner    (1001) docker     (123)    32250 2023-08-04 20:40:07.000000 rapidgzip-0.8.1/external/zlib/crc32.c
--rw-r--r--   0 runner    (1001) docker     (123)   591749 2023-08-04 20:40:07.000000 rapidgzip-0.8.1/external/zlib/crc32.h
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-08-04 20:40:07.000000 rapidgzip-0.8.1/external/zlib/gzguts.h
--rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-08-04 20:40:07.000000 rapidgzip-0.8.1/external/zlib/inffast.c
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-08-04 20:40:07.000000 rapidgzip-0.8.1/external/zlib/inffast.h
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-08-04 20:40:07.000000 rapidgzip-0.8.1/external/zlib/inffixed.h
--rw-r--r--   0 runner    (1001) docker     (123)    56089 2023-08-04 20:40:07.000000 rapidgzip-0.8.1/external/zlib/inflate.c
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-08-04 20:40:07.000000 rapidgzip-0.8.1/external/zlib/inflate.h
--rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-08-04 20:40:07.000000 rapidgzip-0.8.1/external/zlib/inftrees.c
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-08-04 20:40:07.000000 rapidgzip-0.8.1/external/zlib/inftrees.h
--rw-r--r--   0 runner    (1001) docker     (123)    16625 2023-08-04 20:40:07.000000 rapidgzip-0.8.1/external/zlib/zconf.h
--rw-r--r--   0 runner    (1001) docker     (123)    97323 2023-08-04 20:40:07.000000 rapidgzip-0.8.1/external/zlib/zlib.h
--rw-r--r--   0 runner    (1001) docker     (123)     7340 2023-08-04 20:40:07.000000 rapidgzip-0.8.1/external/zlib/zutil.c
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-08-04 20:40:07.000000 rapidgzip-0.8.1/external/zlib/zutil.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:40:31.585851 rapidgzip-0.8.1/nasm_extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/nasm_extension/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/nasm_extension/nasmcompiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/nasm_extension/winnasmcompiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:40:31.585851 rapidgzip-0.8.1/rapidgzip/
--rw-r--r--   0 runner    (1001) docker     (123)    20122 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/ChunkData.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17733 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/DecodedData.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/DecodedDataView.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/Error.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16354 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/GzipAnalyzer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/GzipBlockFinder.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    50335 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/GzipChunkFetcher.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/GzipReader.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/IndexFileFormat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/MarkerReplacement.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    33820 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/ParallelGzipReader.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/WindowMap.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:40:31.589851 rapidgzip-0.8.1/rapidgzip/blockfinder/
--rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/blockfinder/Bgzf.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15833 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/blockfinder/DynamicHuffman.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/blockfinder/Interface.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/blockfinder/PigzNaive.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13579 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/blockfinder/PigzParallel.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/blockfinder/PigzStringView.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/blockfinder/Uncompressed.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:40:31.589851 rapidgzip-0.8.1/rapidgzip/blockfinder/precodecheck/
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/blockfinder/precodecheck/BruteForceLUT.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/blockfinder/precodecheck/SingleCompressedLUT.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    27915 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/blockfinder/precodecheck/SingleLUT.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/blockfinder/precodecheck/WalkTreeCompressedLUT.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13289 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/blockfinder/precodecheck/WalkTreeLUT.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/blockfinder/precodecheck/WithoutLUT.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/crc32.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/definitions.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    52978 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/deflate.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/gzip.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:40:31.589851 rapidgzip-0.8.1/rapidgzip/huffman/
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/huffman/HuffmanCodingBase.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/huffman/HuffmanCodingCheckOnly.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16449 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/huffman/HuffmanCodingDoubleLiteralCached.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/huffman/HuffmanCodingLinearSearch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/huffman/HuffmanCodingReversedBitsCached.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/huffman/HuffmanCodingReversedBitsCachedCompressed.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/huffman/HuffmanCodingReversedCodesPerLength.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/huffman/HuffmanCodingSymbolsPerLength.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9730 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/isal.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/precode.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/rapidgzip.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip/zlib.hpp
--rw-r--r--   0 runner    (1001) docker     (123)   715568 2023-08-04 20:40:31.000000 rapidgzip-0.8.1/rapidgzip.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:40:31.589851 rapidgzip-0.8.1/rapidgzip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18221 2023-08-04 20:40:31.000000 rapidgzip-0.8.1/rapidgzip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-08-04 20:40:31.000000 rapidgzip-0.8.1/rapidgzip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 20:40:31.000000 rapidgzip-0.8.1/rapidgzip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-04 20:40:31.000000 rapidgzip-0.8.1/rapidgzip.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-04 20:40:31.000000 rapidgzip-0.8.1/rapidgzip.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13340 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/rapidgzip.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-08-04 20:40:31.593851 rapidgzip-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:40:31.589851 rapidgzip-0.8.1/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/tools/licenses.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19294 2023-08-04 20:39:58.000000 rapidgzip-0.8.1/tools/rapidgzip.cpp
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 20:03:54.751693 rapidgzip-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (999)    13578 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (999)    11354 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/LICENSE-APACHE
+-rw-r--r--   0 runner    (1001) docker     (999)     1080 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/LICENSE-MIT
+-rw-r--r--   0 runner    (1001) docker     (999)     1246 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (999)    22075 2023-08-30 20:03:54.751693 rapidgzip-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)    20758 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 20:03:54.727691 rapidgzip-0.9.0/core/
+-rw-r--r--   0 runner    (1001) docker     (999)     3766 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/AffinityHelpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     2615 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/AlignedAllocator.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)      704 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/AtomicMutex.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     9335 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/BitManipulation.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)    33408 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/BitReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)    11168 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/BitStringFinder.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)    27301 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/BlockFetcher.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     6810 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/BlockFinder.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)      903 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/BlockFinderInterface.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)    10488 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/BlockMap.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     7698 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/Cache.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     2267 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/FasterVector.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)    26576 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/FileUtils.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     1665 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/JoiningThread.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)    12027 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/ParallelBitStringFinder.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)    11696 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/Prefetcher.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     9508 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/Statistics.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     4204 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/StreamedResults.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     2876 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/TestHelpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     7133 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/ThreadPool.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     7013 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/VectorView.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)    17649 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/common.hpp
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 20:03:54.731691 rapidgzip-0.9.0/core/filereader/
+-rw-r--r--   0 runner    (1001) docker     (999)     4000 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/filereader/BufferView.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     6740 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/filereader/Buffered.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     1524 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/filereader/FileReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     2641 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/filereader/Memory.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)    11527 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/filereader/Python.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)    12347 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/filereader/Shared.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     9215 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/filereader/Standard.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     7806 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/core/filereader/StreamAdapter.hpp
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 20:03:54.715690 rapidgzip-0.9.0/external/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 20:03:54.731691 rapidgzip-0.9.0/external/cxxopts/
+-rw-r--r--   0 runner    (1001) docker     (999)     1055 2023-08-30 20:03:24.000000 rapidgzip-0.9.0/external/cxxopts/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 20:03:54.731691 rapidgzip-0.9.0/external/cxxopts/include/
+-rw-r--r--   0 runner    (1001) docker     (999)    58694 2023-08-30 20:03:24.000000 rapidgzip-0.9.0/external/cxxopts/include/cxxopts.hpp
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 20:03:54.731691 rapidgzip-0.9.0/external/isa-l/
+-rw-r--r--   0 runner    (1001) docker     (999)     1559 2023-08-30 20:03:25.000000 rapidgzip-0.9.0/external/isa-l/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 20:03:54.735692 rapidgzip-0.9.0/external/isa-l/igzip/
+-rw-r--r--   0 runner    (1001) docker     (999)     3624 2023-08-30 20:03:25.000000 rapidgzip-0.9.0/external/isa-l/igzip/huff_codes.h
+-rw-r--r--   0 runner    (1001) docker     (999)   379753 2023-08-30 20:03:25.000000 rapidgzip-0.9.0/external/isa-l/igzip/hufftables_c.c
+-rw-r--r--   0 runner    (1001) docker     (999)     2103 2023-08-30 20:03:25.000000 rapidgzip-0.9.0/external/isa-l/igzip/igzip.c
+-rw-r--r--   0 runner    (1001) docker     (999)      308 2023-08-30 20:03:25.000000 rapidgzip-0.9.0/external/isa-l/igzip/igzip_checksums.h
+-rw-r--r--   0 runner    (1001) docker     (999)    22135 2023-08-30 20:03:25.000000 rapidgzip-0.9.0/external/isa-l/igzip/igzip_decode_block_stateless.asm
+-rw-r--r--   0 runner    (1001) docker     (999)       61 2023-08-30 20:03:25.000000 rapidgzip-0.9.0/external/isa-l/igzip/igzip_decode_block_stateless_01.asm
+-rw-r--r--   0 runner    (1001) docker     (999)       79 2023-08-30 20:03:25.000000 rapidgzip-0.9.0/external/isa-l/igzip/igzip_decode_block_stateless_04.asm
+-rw-r--r--   0 runner    (1001) docker     (999)    82716 2023-08-30 20:03:25.000000 rapidgzip-0.9.0/external/isa-l/igzip/igzip_inflate.c
+-rw-r--r--   0 runner    (1001) docker     (999)     2236 2023-08-30 20:03:25.000000 rapidgzip-0.9.0/external/isa-l/igzip/igzip_inflate_multibinary.asm
+-rw-r--r--   0 runner    (1001) docker     (999)     2194 2023-08-30 20:03:25.000000 rapidgzip-0.9.0/external/isa-l/igzip/igzip_wrapper.h
+-rw-r--r--   0 runner    (1001) docker     (999)     5879 2023-08-30 20:03:25.000000 rapidgzip-0.9.0/external/isa-l/igzip/inflate_data_structs.asm
+-rw-r--r--   0 runner    (1001) docker     (999)     5044 2023-08-30 20:03:25.000000 rapidgzip-0.9.0/external/isa-l/igzip/rfc1951_lookup.asm
+-rw-r--r--   0 runner    (1001) docker     (999)   142279 2023-08-30 20:03:25.000000 rapidgzip-0.9.0/external/isa-l/igzip/static_inflate.h
+-rw-r--r--   0 runner    (1001) docker     (999)    10063 2023-08-30 20:03:25.000000 rapidgzip-0.9.0/external/isa-l/igzip/stdmac.asm
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 20:03:54.735692 rapidgzip-0.9.0/external/isa-l/include/
+-rw-r--r--   0 runner    (1001) docker     (999)    33207 2023-08-30 20:03:25.000000 rapidgzip-0.9.0/external/isa-l/include/igzip_lib.h
+-rw-r--r--   0 runner    (1001) docker     (999)    11018 2023-08-30 20:03:25.000000 rapidgzip-0.9.0/external/isa-l/include/multibinary.asm
+-rw-r--r--   0 runner    (1001) docker     (999)     7766 2023-08-30 20:03:25.000000 rapidgzip-0.9.0/external/isa-l/include/reg_sizes.asm
+-rw-r--r--   0 runner    (1001) docker     (999)     5054 2023-08-30 20:03:25.000000 rapidgzip-0.9.0/external/isa-l/include/unaligned.h
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 20:03:54.735692 rapidgzip-0.9.0/external/rpmalloc/
+-rw-r--r--   0 runner    (1001) docker     (999)     2400 2023-08-30 20:03:26.000000 rapidgzip-0.9.0/external/rpmalloc/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 20:03:54.735692 rapidgzip-0.9.0/external/rpmalloc/rpmalloc/
+-rw-r--r--   0 runner    (1001) docker     (999)   128343 2023-08-30 20:03:26.000000 rapidgzip-0.9.0/external/rpmalloc/rpmalloc/rpmalloc.c
+-rw-r--r--   0 runner    (1001) docker     (999)    18023 2023-08-30 20:03:26.000000 rapidgzip-0.9.0/external/rpmalloc/rpmalloc/rpmalloc.h
+-rw-r--r--   0 runner    (1001) docker     (999)     2363 2023-08-30 20:03:26.000000 rapidgzip-0.9.0/external/rpmalloc/rpmalloc/rpnew.h
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 20:03:54.739692 rapidgzip-0.9.0/external/zlib/
+-rw-r--r--   0 runner    (1001) docker     (999)     1002 2023-08-30 20:03:28.000000 rapidgzip-0.9.0/external/zlib/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (999)     5204 2023-08-30 20:03:28.000000 rapidgzip-0.9.0/external/zlib/adler32.c
+-rw-r--r--   0 runner    (1001) docker     (999)    32250 2023-08-30 20:03:28.000000 rapidgzip-0.9.0/external/zlib/crc32.c
+-rw-r--r--   0 runner    (1001) docker     (999)   591749 2023-08-30 20:03:28.000000 rapidgzip-0.9.0/external/zlib/crc32.h
+-rw-r--r--   0 runner    (1001) docker     (999)     6843 2023-08-30 20:03:28.000000 rapidgzip-0.9.0/external/zlib/gzguts.h
+-rw-r--r--   0 runner    (1001) docker     (999)    12998 2023-08-30 20:03:28.000000 rapidgzip-0.9.0/external/zlib/inffast.c
+-rw-r--r--   0 runner    (1001) docker     (999)      427 2023-08-30 20:03:28.000000 rapidgzip-0.9.0/external/zlib/inffast.h
+-rw-r--r--   0 runner    (1001) docker     (999)     6332 2023-08-30 20:03:28.000000 rapidgzip-0.9.0/external/zlib/inffixed.h
+-rw-r--r--   0 runner    (1001) docker     (999)    56089 2023-08-30 20:03:28.000000 rapidgzip-0.9.0/external/zlib/inflate.c
+-rw-r--r--   0 runner    (1001) docker     (999)     6683 2023-08-30 20:03:28.000000 rapidgzip-0.9.0/external/zlib/inflate.h
+-rw-r--r--   0 runner    (1001) docker     (999)    12999 2023-08-30 20:03:28.000000 rapidgzip-0.9.0/external/zlib/inftrees.c
+-rw-r--r--   0 runner    (1001) docker     (999)     2927 2023-08-30 20:03:28.000000 rapidgzip-0.9.0/external/zlib/inftrees.h
+-rw-r--r--   0 runner    (1001) docker     (999)    16625 2023-08-30 20:03:28.000000 rapidgzip-0.9.0/external/zlib/zconf.h
+-rw-r--r--   0 runner    (1001) docker     (999)    97323 2023-08-30 20:03:28.000000 rapidgzip-0.9.0/external/zlib/zlib.h
+-rw-r--r--   0 runner    (1001) docker     (999)     7340 2023-08-30 20:03:28.000000 rapidgzip-0.9.0/external/zlib/zutil.c
+-rw-r--r--   0 runner    (1001) docker     (999)     7297 2023-08-30 20:03:28.000000 rapidgzip-0.9.0/external/zlib/zutil.h
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 20:03:54.739692 rapidgzip-0.9.0/nasm_extension/
+-rw-r--r--   0 runner    (1001) docker     (999)     1322 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/nasm_extension/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (999)     3246 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/nasm_extension/nasmcompiler.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3198 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/nasm_extension/winnasmcompiler.py
+-rw-r--r--   0 runner    (1001) docker     (999)      366 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 20:03:54.743692 rapidgzip-0.9.0/rapidgzip/
+-rw-r--r--   0 runner    (1001) docker     (999)    22171 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/ChunkData.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)    23402 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/DecodedData.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     1088 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/DecodedDataView.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     3622 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/Error.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)    25064 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/GzipAnalyzer.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)    10356 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/GzipBlockFinder.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)    63203 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/GzipChunkFetcher.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)    17150 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/GzipReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)    17959 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/IndexFileFormat.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     1618 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/MarkerReplacement.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)    36725 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/ParallelGzipReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     2212 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/RFCTables.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     1973 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/WindowMap.hpp
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 20:03:54.747693 rapidgzip-0.9.0/rapidgzip/blockfinder/
+-rw-r--r--   0 runner    (1001) docker     (999)     9227 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/blockfinder/Bgzf.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)    16391 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/blockfinder/DynamicHuffman.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)      218 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/blockfinder/Interface.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     7506 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/blockfinder/PigzNaive.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)    13579 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/blockfinder/PigzParallel.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     6340 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/blockfinder/PigzStringView.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     4349 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/blockfinder/Uncompressed.hpp
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 20:03:54.747693 rapidgzip-0.9.0/rapidgzip/blockfinder/precodecheck/
+-rw-r--r--   0 runner    (1001) docker     (999)     5052 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/blockfinder/precodecheck/BruteForceLUT.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     7559 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/blockfinder/precodecheck/SingleCompressedLUT.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)    27915 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/blockfinder/precodecheck/SingleLUT.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     6702 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/blockfinder/precodecheck/WalkTreeCompressedLUT.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)    13654 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/blockfinder/precodecheck/WalkTreeLUT.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     5716 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/blockfinder/precodecheck/WithoutLUT.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)    12043 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/crc32.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     3985 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/definitions.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)    57302 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/deflate.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     6977 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/gzip.hpp
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 20:03:54.747693 rapidgzip-0.9.0/rapidgzip/huffman/
+-rw-r--r--   0 runner    (1001) docker     (999)     8528 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/huffman/HuffmanCodingBase.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     1379 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/huffman/HuffmanCodingCheckOnly.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     4613 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/huffman/HuffmanCodingDistanceISAL.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)    16449 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/huffman/HuffmanCodingDoubleLiteralCached.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     5756 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/huffman/HuffmanCodingISAL.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)    10209 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/huffman/HuffmanCodingLinearSearch.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     5633 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/huffman/HuffmanCodingReversedBitsCached.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     7051 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/huffman/HuffmanCodingReversedBitsCachedCompressed.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     6004 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/huffman/HuffmanCodingReversedCodesPerLength.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     5913 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/huffman/HuffmanCodingSymbolsPerLength.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)    15082 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/isal.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)     6476 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/precode.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)      148 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/rapidgzip.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)    14187 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip/zlib.hpp
+-rw-r--r--   0 runner    (1001) docker     (999)   749606 2023-08-30 20:03:54.000000 rapidgzip-0.9.0/rapidgzip.cpp
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 20:03:54.743692 rapidgzip-0.9.0/rapidgzip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)    22075 2023-08-30 20:03:54.000000 rapidgzip-0.9.0/rapidgzip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     4096 2023-08-30 20:03:54.000000 rapidgzip-0.9.0/rapidgzip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-30 20:03:54.000000 rapidgzip-0.9.0/rapidgzip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       44 2023-08-30 20:03:54.000000 rapidgzip-0.9.0/rapidgzip.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       10 2023-08-30 20:03:54.000000 rapidgzip-0.9.0/rapidgzip.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)    13313 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip.pyx
+-rw-r--r--   0 runner    (1001) docker     (999)     6781 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/rapidgzip.svg
+-rw-r--r--   0 runner    (1001) docker     (999)     1278 2023-08-30 20:03:54.751693 rapidgzip-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)     9365 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 20:03:54.751693 rapidgzip-0.9.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (999)     6464 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/tools/licenses.cpp
+-rw-r--r--   0 runner    (1001) docker     (999)    18323 2023-08-30 20:03:19.000000 rapidgzip-0.9.0/tools/rapidgzip.cpp
```

### Comparing `rapidgzip-0.8.1/CHANGELOG.md` & `rapidgzip-0.9.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,50 @@
 
+# Version 0.9.0 built on 2023-08-30
+
+## Added
+
+ - Support BGZI with `--import-index`. These can be created with `bgzip --reindex`.
+ - Check against a wrong index being loaded.
+ - Improve error messages when zlib or ISA-l wrappers are used.
+ - New output with `--analyze`:
+   - Show information about extra bytes written by pgzf, MiGz, QATzip, pgzip/mgzip, bgzip, dictzip.
+   - Print stream size statistics.
+   - Print out the position after the block header, i.e., the begin of the Huffman data.
+ - New profiling output with `--verbose`:
+   - Decompression durations split by ISA-l, zlib, rapidgzip internal
+   - The number of block offsets found with a block finder, from which decoding failed inside a chunk
+
+## Performance
+
+ - Avoid allocations by replacing the markers in-place by reinterpreting the buffer: Silesia +11 %, FASTQ +36 %.
+ - Allocate fixed 128 KiB chunks instead of one allocation per deflate block: FASTQ +3 %.
+ - Use ISA-L, if available, with -P 1: +110%.
+ - Use ISA-L when a window has become resolve inside a chunk: Silesia +12%, Random Base64 +70%.
+ - Use ISA-l Huffman decoder for literal/length alphabet in internal decoder: +20-40%.
+
+## Fixes
+
+ - Only show informational message about internal chunk fetcher with `--verbose`.
+ - Smaller fixes in the inflate wrappers.
+ - Check against zero-length end-of-block symbol.
+ - Reintroduce the error detection for distance code counts equal to 31 or 32, which was removed in 0.5.0.
+
+## API
+
+ - Add stopping points to inflate wrappers.
+ - `SharedFileReader`: Decouple statistics recording from printing.
+ - Add `VectorView` constructor taking a start and end pointer.
+ - Remove unused `deflate::Block::window` method.
+ - Make `SHOW_PROFILE` a simple bool member instead of template parameter.
+ - Make `DecodedData::data` private and a vector of views to actual buffers.
+ - Add `BufferViewFileReader(void*, size_t)` overload
+ - Remove unused argument to `ParallelGzipReader::maxDecompressedChunkSize()` getter.
+
+
 # Version 0.8.1 built on 2023-08-04
 
 ## Fixes
 
  - The CRC32 checksum was not correctly read from the footer when ISA-l was used.
  - Limit the minimum chunk size to 8 KiB, especially forbid a chunk size of 0, which lead to an infinite loop.
```

### Comparing `rapidgzip-0.8.1/LICENSE-APACHE` & `rapidgzip-0.9.0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/LICENSE-MIT` & `rapidgzip-0.9.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/MANIFEST.in` & `rapidgzip-0.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/PKG-INFO` & `rapidgzip-0.9.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,17 @@
-Metadata-Version: 2.1
-Name: rapidgzip
-Version: 0.8.1
-Summary: Parallel random access to gzip files
-Home-page: https://github.com/mxmlnkn/rapidgzip
-Author: Maximilian Knespel
-Author-email: mxmlnkn@github.de
-License: MIT
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Development Status :: 3 - Alpha
-Classifier: Natural Language :: English
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: C++
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: System :: Archiving
-Classifier: Topic :: System :: Archiving :: Compression
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE-APACHE
-License-File: LICENSE-MIT
-
 <div align="center">
 
 ![](https://raw.githubusercontent.com/mxmlnkn/indexed_bzip2/master/python/rapidgzip/rapidgzip.svg)
 
 # Rapidgzip: Parallelized Decompression of Gzip Files with Support for Fast Random Access
 
 [![PyPI version](https://badge.fury.io/py/rapidgzip.svg)](https://badge.fury.io/py/rapidgzip)
 [![Python Version](https://img.shields.io/pypi/pyversions/rapidgzip)](https://pypi.org/project/rapidgzip/)
 [![PyPI Platforms](https://img.shields.io/badge/pypi-linux%20%7C%20macOS%20%7C%20Windows-brightgreen)](https://pypi.org/project/rapidgzip/)
-[![Downloads](https://pepy.tech/badge/pragzip/month)](https://pepy.tech/project/rapidgzip)
+[![Downloads](https://static.pepy.tech/badge/rapidgzip/month)](https://pepy.tech/project/rapidgzip)
 <br>
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](http://opensource.org/licenses/MIT)
 [![Build Status](https://github.com/mxmlnkn/indexed_bzip2/workflows/tests/badge.svg)](https://github.com/mxmlnkn/rapidgzip/actions)
 [![codecov](https://codecov.io/gh/mxmlnkn/indexed_bzip2/branch/master/graph/badge.svg?token=94ZD4UTZQW)](https://codecov.io/gh/mxmlnkn/rapidgzip)
 ![C++17](https://img.shields.io/badge/C++-17-blue.svg)
 [![Discord](https://img.shields.io/discord/783411320354766878?label=discord)](https://discord.gg/Wra6t6akh2)
 [![Telegram](https://img.shields.io/badge/Chat-Telegram-%2330A3E6)](https://t.me/joinchat/FUdXxkXIv6c4Ib8bgaSxNg)
@@ -64,89 +31,46 @@
 This repository was created for visibility reasons and in order to keep indexed_bzip2 and rapidgzip releases separate.
 It will be updated at least for each release.
 Issues regarding rapidgzip should be opened [here](https://github.com/mxmlnkn/rapidgzip/issues).
 
 
 # Table of Contents
 
-1. [Performance](#performance-comparison-with-gzip-module)
-   1. [Decompression with Existing Index](#decompression-with-existing-index)
-   2. [Decompression from Scratch](#decompression-from-scratch)
-2. [Installation](#installation)
+1. [Installation](#installation)
+2. [Performance](#performance)
+   1. [Scaling Benchmarks on 2xAMD EPYC CPU 7702 (2x64 cores)](#scaling-benchmarks-on-2xamd-epyc-cpu-7702-2x64-cores)
+      1. [Decompression of Silesia Corpus](#decompression-of-silesia-corpus)
+      2. [Decompression Gzip-Compressed Base64 Data](#decompression-gzip-compressed-base64-data)
+   2. [Scaling Benchmarks on Ryzen 3900X](#scaling-benchmarks-on-ryzen-3900x)
+      1. [Decompression with Existing Index](#decompression-with-existing-index)
+      2. [Decompression from Scratch](#decompression-from-scratch)
 3. [Usage](#usage)
    1. [Command Line Tool](#command-line-tool)
    2. [Python Library](#python-library)
    3. [Via Ratarmount](#via-ratarmount)
    4. [C++ Library](#c-library)
 4. [Citation](#citation)
 5. [About](#about)
 6. [Internal Architecture](#internal-architecture)
 7. [Tracing the Decoder](#tracing-the-decoder)
 
 
-# Performance
-
-These are simple timing tests for reading all the contents of a gzip file sequentially.
-
-Results are shown for an AMD Ryzen 3900X 12-core (24 virtual cores) processor and with `gzipFilePath="4GiB-base64.gz"`, which is a 4 GiB gzip compressed file with base64 random data.
-
-Be aware that the chunk size requested from the Python code does influence the performance heavily.
-This benchmarks use a chunk size of 512 KiB.
-
-## Decompression with Existing Index
-
-|                        | 4GiB-base64                  | 4GiB-base64     | | 20x-silesia                   | 20x-silesia
-|------------------------|------------------------------|-----------------|-|-------------------------------|---------
-| Uncompressed Size      | 4 GiB                        |                 | | 3.95 GiB                      |
-| Compressed Size        | 3.04 GiB                     |                 | | 1.27 GiB                      |
-| **Module**             | **Bandwidth <br/> / (MB/s)** | **Speedup**     | |  **Bandwidth <br/> / (MB/s)** | **Speedup**
-| gzip                   |  250                         |    1            | |   293                         |  1
-| rapidgzip (0  threads) | 5060                         | 19.5            | |  5580                         | 18.6
-| rapidgzip (1  threads) |  445                         |  1.7            | |   624                         |  2.1
-| rapidgzip (2  threads) |  895                         |  3.5            | |  1190                         |  4.0
-| rapidgzip (6  threads) | 2500                         |  9.6            | |  3330                         | 11.1
-| rapidgzip (12 threads) | 4390                         | 16.9            | |  5810                         | 19.4
-| rapidgzip (24 threads) | 5150                         | 19.9            | |  5960                         | 19.9
-| rapidgzip (32 threads) | 5000                         | 19.3            | |  5640                         | 18.8
-
-
-## Decompression from Scratch
-
-### Python
-
-|                        | 4GiB-base64                  | 4GiB-base64     | | 20x-silesia                   | 20x-silesia
-|------------------------|------------------------------|-----------------|-|-------------------------------|---------
-| Uncompressed Size      | 4 GiB                        |                 | | 3.95 GiB                      |
-| Compressed Size        | 3.04 GiB                     |                 | | 1.27 GiB                      |
-| **Module**             | **Bandwidth <br/> / (MB/s)** | **Speedup**     | |  **Bandwidth <br/> / (MB/s)** | **Speedup**
-| gzip                   |  250                         |    1            | |   293                         |  1
-| rapidgzip (0  threads) | 3290                         | 12.7            | |  1820                         |  6.1
-| rapidgzip (1  threads) |  222                         |  0.9            | |   238                         |  0.8
-| rapidgzip (2  threads) |  435                         |  1.7            | |   415                         |  1.4
-| rapidgzip (6  threads) | 1260                         |  4.9            | |  1140                         |  3.8
-| rapidgzip (12 threads) | 2310                         |  8.9            | |  1550                         |  5.2
-| rapidgzip (24 threads) | 3200                         | 12.4            | |  1890                         |  6.3
-| rapidgzip (32 threads) | 3210                         | 12.4            | |  2060                         |  6.9
-
-Note that rapidgzip is generally faster when given an index because it can delegate the decompression to zlib while it has to use its own gzip decompression engine when no index exists yet.
-
-Note that values deviate roughly by 10% and therefore are rounded.
-
-The code used for benchmarking can be found [here](results/benchmarkPythonModule.py).
-
-
 # Installation
 
 You can simply install it from PyPI:
 
 ```
 python3 -m pip install --upgrade pip  # Recommended for newer manylinux wheels
 python3 -m pip install rapidgzip
+rapidgzip --help
 ```
 
+<details>
+<summary>Advanced Installations</summary>
+
 The latest unreleased development version can be tested out with:
 
 ```bash
 python3 -m pip install --force-reinstall 'git+https://github.com/mxmlnkn/indexed_bzip2.git@master#egginfo=rapidgzip&subdirectory=python/rapidgzip'
 ```
 
 And to build locally, you can use `build` and install the wheel:
@@ -154,14 +78,106 @@
 ```bash
 cd python/rapidgzip
 rm -rf dist
 python3 -m build .
 python3 -m pip install --force-reinstall --user dist/*.whl
 ```
 
+</details>
+
+
+# Performance
+
+Following are benchmarks showing the decompression bandwidth over the number of used cores.
+
+There are two rapidgzip variants shown: `(index)` and `(no index)`.
+Rapidgzip is generally faster when given an index with `--import-index` because it can delegate the decompression to ISA-l or zlib while it has to use its own custom-written gzip decompression engine when no index exists yet.
+Furthermore, decompression can be parallelized more evenly and more effectively when an index exists because the serializing window propagation step is not necessary.
+
+The violin plots show 20 repeated measurements as a single "blob".
+Thin blobs signal very reproducible timings while thick blobs signal a large variance.
+
+
+## Scaling Benchmarks on 2xAMD EPYC CPU 7702 (2x64 cores)
+
+### Decompression of Silesia Corpus
+
+![](https://raw.githubusercontent.com/mxmlnkn/indexed_bzip2/master/results/benchmarks/rapidgzip-0.9.0-scaling-benchmarks-2023-08-30/plots/result-parallel-decompression-silesia-dev-null-bandwidths-number-of-threads.png)
+
+This benchmark uses the [Silesia corpus](https://sun.aei.polsl.pl//~sdeor/index.php?page=silesia) compressed as a .tar.gz file to show the decompression performance.
+However, the compressed dataset is only ~69 MB, which is not sufficiently large to show parallelization over 128 cores.
+That's why the TAR file is repeated as often as there are number of cores in the benchmark times 2 and then compressed into a single large gzip file, which is ~18 GB compressed and 54 GB uncompressed for 128 cores.
+
+Rapidgzip achieves up to 24 GB/s with an index and 12 GB/s without.
+
+Pugz is not shown as comparison because it is not able to decompress the Silesia dataset because it contains binary data, which it cannot handle.
+
+
+### Decompression of Gzip-Compressed Base64 Data
+
+![](https://raw.githubusercontent.com/mxmlnkn/indexed_bzip2/master/results/benchmarks/rapidgzip-0.9.0-scaling-benchmarks-2023-08-30/plots/result-parallel-decompression-base64-dev-null-bandwidths-number-of-threads.png)
+
+This benchmarks uses random data, that has been base64 encoded and then gzip-compressed.
+This is the next best case for rapidgzip after the trivial case of purely random data, which cannot be compressed and therefore can be decompressed with a simple memory copy.
+This next best case results in mostly Huffman-coding compressed data with only very few LZ77 back-references.
+Without LZ77 back-references, parallel decompression can be done more independently and therefore faster than in the case of many LZ77 back-references.
+
+
+### Decompression of Gzip-Compressed FASTQ Data
+
+![](https://raw.githubusercontent.com/mxmlnkn/indexed_bzip2/master/results/benchmarks/rapidgzip-0.9.0-scaling-benchmarks-2023-08-30/plots/result-parallel-decompression-fastq-dev-null-bandwidths-number-of-threads.png)
+
+This benchmarks uses gzip-compressed [FASTQ data](http://ftp.sra.ebi.ac.uk/vol1/fastq/SRR224/085/SRR22403185/SRR22403185_2.fastq.gz).
+That's why the TAR file is repeated as often as there are number of cores in the benchmark to hold the decompression times roughly constant in order to make the benchmark over this large a range feasible.
+This is almost the worst case for rapidgzip because it contains many LZ77 back-references over very long ranges.
+This means that a fallback to ISA-L is not possible and it means that the costly two-staged decoding has to be done for almost all the data.
+This is also the reason why if fails to scale above 64 cores, i.e, to teh second CPU socket.
+The first and second decompression stages are completely independently submitted to a thread pool, which on this NUMA architecture means, that data needs to be costly transferred from one processor socket to the other if the second step for a chunk is not done on the same processor as the first.
+This should be fixable by making the ThreadPool NUMA-aware.
+
+These three scaling plots were created with rapidgzip 0.9.0 while the ones in the [paper](<results/paper/Knespel, Brunst - 2023 - Rapidgzip - Parallel Decompression and Seeking in Gzip Files Using Cache Prefetching.pdf>) were created with 0.5.0.
+
+
+## Scaling Benchmarks on Ryzen 3900X
+
+These benchmarks on my local workstation with a Ryzen 3900X only has 12 cores (24 virtual cores) but the base frequency is much higher than the 2xAMD EPYC CPU 7702.
+
+### Decompression With Existing Index
+
+|                        | 4GiB-base64                  | 4GiB-base64     | | 20x-silesia                   | 20x-silesia
+|------------------------|------------------------------|-----------------|-|-------------------------------|---------
+| Uncompressed Size      | 4 GiB                        |                 | | 3.95 GiB                      |
+| Compressed Size        | 3.04 GiB                     |                 | | 1.27 GiB                      |
+| **Module**             | **Bandwidth <br/> / (MB/s)** | **Speedup**     | |  **Bandwidth <br/> / (MB/s)** | **Speedup**
+| gzip                   |  250                         |    1            | |   293                         |  1
+| rapidgzip (0  threads) | 5179                         | 20.6            | |  5640                         | 18.8
+| rapidgzip (1  threads) |  488                         |  1.9            | |   684                         |  2.3
+| rapidgzip (2  threads) |  902                         |  3.6            | |  1200                         |  4.0
+| rapidgzip (6  threads) | 2617                         | 10.4            | |  3250                         | 10.9
+| rapidgzip (12 threads) | 4463                         | 17.7            | |  5600                         | 18.7
+| rapidgzip (24 threads) | 5240                         | 20.8            | |  5750                         | 19.2
+| rapidgzip (32 threads) | 4929                         | 19.6            | |  5300                         | 17.7
+
+
+### Decompression From Scratch
+
+|                        | 4GiB-base64                  | 4GiB-base64     | | 20x-silesia                   | 20x-silesia
+|------------------------|------------------------------|-----------------|-|-------------------------------|---------
+| Uncompressed Size      | 4 GiB                        |                 | | 3.95 GiB                      |
+| Compressed Size        | 3.04 GiB                     |                 | | 1.27 GiB                      |
+| **Module**             | **Bandwidth <br/> / (MB/s)** | **Speedup**     | |  **Bandwidth <br/> / (MB/s)** | **Speedup**
+| gzip                   |  250                         |    1            | |   293                         |  1
+| rapidgzip (0  threads) | 5060                         | 20.1            | |  2070                         |  6.9
+| rapidgzip (1  threads) |  487                         |  1.9            | |  630                          |  2.1
+| rapidgzip (2  threads) |  839                         |  3.3            | |  694                          |  2.3
+| rapidgzip (6  threads) | 2365                         |  9.4            | |  1740                         |  5.8
+| rapidgzip (12 threads) | 4116                         | 16.4            | |  1900                         |  6.4
+| rapidgzip (24 threads) | 4974                         | 19.8            | |  2040                         |  6.8
+| rapidgzip (32 threads) | 4612                         | 18.3            | |  2580                         |  8.6
+
 
 # Usage
 
 ## Command Line Tool
 
 ```bash
 rapidgzip --help
@@ -258,50 +274,51 @@
 I currently did not yet test integrating it into other projects other than simply manually copying the source in `src/core`, `src/rapidgzip`, and if integrated zlib is desired also `src/external/zlib`.
 If you have suggestions and wishes like support with CMake or Conan, please open an issue.
 
 
 # Citation
 
 A paper describing the implementation details and showing the scaling behavior with up to 128 cores has been submitted to and [accepted](https://www.hpdc.org/2023/program/technical-sessions/) in [ACM HPDC'23](https://www.hpdc.org/2023/), The 32nd International Symposium on High-Performance Parallel and Distributed Computing.
-The author's version can be found [here](<results/paper/Knespel, Brunst - 2023 - Rapidgzip - Parallel Decompression and Seeking in Gzip Files Using Cache Prefetching.pdf>) and the accompanying presentation [here](results/Presentation-2023-06-22.pdf).
+The paper can be accessed [freely on ACM DL](https://doi.org/10.1145/3588195.3592992).
+The accompanying presentation can be found [here](results/Presentation-2023-06-22.pdf).
 
 If you use this software for your scientific publication, please cite it as:
 
 This is preliminiary. The final citation will become available end of June 2023.
 
 ```bibtex
 @inproceedings{rapidgzip,
     author    = {Knespel, Maximilian and Brunst, Holger},
     title     = {Rapidgzip: Parallel Decompression and Seeking in Gzip Files Using Cache Prefetching},
     year      = {2023},
-    % isbn    = {},  % To be released end of June
+    isbn      = {9798400701559},
     publisher = {Association for Computing Machinery},
     address   = {New York, NY, USA},
     url       = {https://doi.org/10.1145/3588195.3592992},
     doi       = {10.1145/3588195.3592992},
     abstract  = {Gzip is a file compression format, which is ubiquitously used. Although a multitude of gzip implementations exist, only pugz can fully utilize current multi-core processor architectures for decompression. Yet, pugz cannot decompress arbitrary gzip files. It requires the decompressed stream to only contain byte values 9–126. In this work, we present a generalization of the parallelization scheme used by pugz that can be reliably applied to arbitrary gzip-compressed data without compromising performance. We show that the requirements on the file contents posed by pugz can be dropped by implementing an architecture based on a cache and a parallelized prefetcher. This architecture can safely handle faulty decompression results, which can appear when threads start decompressing in the middle of a gzip file by using trial and error. Using 128 cores, our implementation reaches 8.7 GB/s decompression bandwidth for gzip-compressed base64-encoded data, a speedup of 55 over the single-threaded GNU gzip, and 5.6 GB/s for the Silesia corpus, a speedup of 33 over GNU gzip.},
     booktitle = {Proceedings of the 32nd International Symposium on High-Performance Parallel and Distributed Computing},
-    % pages   = {16–29},  % To be released end of June
+    pages     = {295–307},
     numpages  = {13},
-    keywords  = {Gzip, Decompression, Parallel Algorithm, Performance, Random Access},
+    keywords  = {gzip, decompression, parallel algorithm, performance, random access},
     location  = {Orlando, FL, USA},
     series    = {HPDC '23},
 }
 ```
 
 # About
 
 This tool originated as a backend for [ratarmount](https://github.com/mxmlnkn/ratarmount).
 After writing the bzip2 backend for [ratarmount](https://github.com/mxmlnkn/indexed_bzip2), my hesitation about reimplementing custom decoders for existing file formats has vastly diminished.
 And, while random access to gzip files did exist with [indexed_gzip](https://github.com/pauldmccarthy/indexed_gzip), it did not support parallel decompression neither for the index creation nor when the index already exists.
-The latter of which is trivial, when ignoring load balancing issues, but parallelizing even the idnex creation is vastly more complicated because decompressing data requires the previous 32 KiB of decompressed data to be known.
+The latter of which is trivial, when ignoring load balancing issues, but parallelizing even the index creation is vastly more complicated because decompressing data requires the previous 32 KiB of decompressed data to be known.
 
 After implementing a production-ready version by improving upon the algorithm used by [pugz](https://github.com/Piezoid/pugz), I submitted a [paper](Citation).
-The review process was double-blind and I was unsure whether pseudonymize Pragzip because it has already been uploaded to Github.
-In the end, I used Rapidgzip during the review process and because I was not sure, which form fields should be filled with the pseudonymized title, I simply stuck with it.
+The review process was double-blind and I was unsure whether to pseudonymize Pragzip because it has already been uploaded to Github.
+In the end, I used "rapidgzip" during the review process and because I was not sure, which form fields should be filled with the pseudonymized title, I simply stuck with it.
 Rapidgzip was chosen for similar reason to rapidgzip, namely the P and RA are acronyms for Parallel and Random Access.
 As rapgzip, did not stick, I used rapidgzip, which now also contains the foremost design goal in its name: being rapidly faster than single-threaded implementations.
 Furthermore, the additional ID could be interpreted to stand for Index and Decompression, making "rapid" a partial backronym.
 
 
 # Internal Architecture
```

### Comparing `rapidgzip-0.8.1/README.md` & `rapidgzip-0.9.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,50 @@
+Metadata-Version: 2.1
+Name: rapidgzip
+Version: 0.9.0
+Summary: Parallel random access to gzip files
+Home-page: https://github.com/mxmlnkn/rapidgzip
+Author: Maximilian Knespel
+Author-email: mxmlnkn@github.de
+License: MIT
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Development Status :: 3 - Alpha
+Classifier: Natural Language :: English
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: C++
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System :: Archiving
+Classifier: Topic :: System :: Archiving :: Compression
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE-APACHE
+License-File: LICENSE-MIT
+
 <div align="center">
 
 ![](https://raw.githubusercontent.com/mxmlnkn/indexed_bzip2/master/python/rapidgzip/rapidgzip.svg)
 
 # Rapidgzip: Parallelized Decompression of Gzip Files with Support for Fast Random Access
 
 [![PyPI version](https://badge.fury.io/py/rapidgzip.svg)](https://badge.fury.io/py/rapidgzip)
 [![Python Version](https://img.shields.io/pypi/pyversions/rapidgzip)](https://pypi.org/project/rapidgzip/)
 [![PyPI Platforms](https://img.shields.io/badge/pypi-linux%20%7C%20macOS%20%7C%20Windows-brightgreen)](https://pypi.org/project/rapidgzip/)
-[![Downloads](https://pepy.tech/badge/pragzip/month)](https://pepy.tech/project/rapidgzip)
+[![Downloads](https://static.pepy.tech/badge/rapidgzip/month)](https://pepy.tech/project/rapidgzip)
 <br>
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](http://opensource.org/licenses/MIT)
 [![Build Status](https://github.com/mxmlnkn/indexed_bzip2/workflows/tests/badge.svg)](https://github.com/mxmlnkn/rapidgzip/actions)
 [![codecov](https://codecov.io/gh/mxmlnkn/indexed_bzip2/branch/master/graph/badge.svg?token=94ZD4UTZQW)](https://codecov.io/gh/mxmlnkn/rapidgzip)
 ![C++17](https://img.shields.io/badge/C++-17-blue.svg)
 [![Discord](https://img.shields.io/discord/783411320354766878?label=discord)](https://discord.gg/Wra6t6akh2)
 [![Telegram](https://img.shields.io/badge/Chat-Telegram-%2330A3E6)](https://t.me/joinchat/FUdXxkXIv6c4Ib8bgaSxNg)
@@ -31,89 +64,46 @@
 This repository was created for visibility reasons and in order to keep indexed_bzip2 and rapidgzip releases separate.
 It will be updated at least for each release.
 Issues regarding rapidgzip should be opened [here](https://github.com/mxmlnkn/rapidgzip/issues).
 
 
 # Table of Contents
 
-1. [Performance](#performance-comparison-with-gzip-module)
-   1. [Decompression with Existing Index](#decompression-with-existing-index)
-   2. [Decompression from Scratch](#decompression-from-scratch)
-2. [Installation](#installation)
+1. [Installation](#installation)
+2. [Performance](#performance)
+   1. [Scaling Benchmarks on 2xAMD EPYC CPU 7702 (2x64 cores)](#scaling-benchmarks-on-2xamd-epyc-cpu-7702-2x64-cores)
+      1. [Decompression of Silesia Corpus](#decompression-of-silesia-corpus)
+      2. [Decompression Gzip-Compressed Base64 Data](#decompression-gzip-compressed-base64-data)
+   2. [Scaling Benchmarks on Ryzen 3900X](#scaling-benchmarks-on-ryzen-3900x)
+      1. [Decompression with Existing Index](#decompression-with-existing-index)
+      2. [Decompression from Scratch](#decompression-from-scratch)
 3. [Usage](#usage)
    1. [Command Line Tool](#command-line-tool)
    2. [Python Library](#python-library)
    3. [Via Ratarmount](#via-ratarmount)
    4. [C++ Library](#c-library)
 4. [Citation](#citation)
 5. [About](#about)
 6. [Internal Architecture](#internal-architecture)
 7. [Tracing the Decoder](#tracing-the-decoder)
 
 
-# Performance
-
-These are simple timing tests for reading all the contents of a gzip file sequentially.
-
-Results are shown for an AMD Ryzen 3900X 12-core (24 virtual cores) processor and with `gzipFilePath="4GiB-base64.gz"`, which is a 4 GiB gzip compressed file with base64 random data.
-
-Be aware that the chunk size requested from the Python code does influence the performance heavily.
-This benchmarks use a chunk size of 512 KiB.
-
-## Decompression with Existing Index
-
-|                        | 4GiB-base64                  | 4GiB-base64     | | 20x-silesia                   | 20x-silesia
-|------------------------|------------------------------|-----------------|-|-------------------------------|---------
-| Uncompressed Size      | 4 GiB                        |                 | | 3.95 GiB                      |
-| Compressed Size        | 3.04 GiB                     |                 | | 1.27 GiB                      |
-| **Module**             | **Bandwidth <br/> / (MB/s)** | **Speedup**     | |  **Bandwidth <br/> / (MB/s)** | **Speedup**
-| gzip                   |  250                         |    1            | |   293                         |  1
-| rapidgzip (0  threads) | 5060                         | 19.5            | |  5580                         | 18.6
-| rapidgzip (1  threads) |  445                         |  1.7            | |   624                         |  2.1
-| rapidgzip (2  threads) |  895                         |  3.5            | |  1190                         |  4.0
-| rapidgzip (6  threads) | 2500                         |  9.6            | |  3330                         | 11.1
-| rapidgzip (12 threads) | 4390                         | 16.9            | |  5810                         | 19.4
-| rapidgzip (24 threads) | 5150                         | 19.9            | |  5960                         | 19.9
-| rapidgzip (32 threads) | 5000                         | 19.3            | |  5640                         | 18.8
-
-
-## Decompression from Scratch
-
-### Python
-
-|                        | 4GiB-base64                  | 4GiB-base64     | | 20x-silesia                   | 20x-silesia
-|------------------------|------------------------------|-----------------|-|-------------------------------|---------
-| Uncompressed Size      | 4 GiB                        |                 | | 3.95 GiB                      |
-| Compressed Size        | 3.04 GiB                     |                 | | 1.27 GiB                      |
-| **Module**             | **Bandwidth <br/> / (MB/s)** | **Speedup**     | |  **Bandwidth <br/> / (MB/s)** | **Speedup**
-| gzip                   |  250                         |    1            | |   293                         |  1
-| rapidgzip (0  threads) | 3290                         | 12.7            | |  1820                         |  6.1
-| rapidgzip (1  threads) |  222                         |  0.9            | |   238                         |  0.8
-| rapidgzip (2  threads) |  435                         |  1.7            | |   415                         |  1.4
-| rapidgzip (6  threads) | 1260                         |  4.9            | |  1140                         |  3.8
-| rapidgzip (12 threads) | 2310                         |  8.9            | |  1550                         |  5.2
-| rapidgzip (24 threads) | 3200                         | 12.4            | |  1890                         |  6.3
-| rapidgzip (32 threads) | 3210                         | 12.4            | |  2060                         |  6.9
-
-Note that rapidgzip is generally faster when given an index because it can delegate the decompression to zlib while it has to use its own gzip decompression engine when no index exists yet.
-
-Note that values deviate roughly by 10% and therefore are rounded.
-
-The code used for benchmarking can be found [here](results/benchmarkPythonModule.py).
-
-
 # Installation
 
 You can simply install it from PyPI:
 
 ```
 python3 -m pip install --upgrade pip  # Recommended for newer manylinux wheels
 python3 -m pip install rapidgzip
+rapidgzip --help
 ```
 
+<details>
+<summary>Advanced Installations</summary>
+
 The latest unreleased development version can be tested out with:
 
 ```bash
 python3 -m pip install --force-reinstall 'git+https://github.com/mxmlnkn/indexed_bzip2.git@master#egginfo=rapidgzip&subdirectory=python/rapidgzip'
 ```
 
 And to build locally, you can use `build` and install the wheel:
@@ -121,14 +111,106 @@
 ```bash
 cd python/rapidgzip
 rm -rf dist
 python3 -m build .
 python3 -m pip install --force-reinstall --user dist/*.whl
 ```
 
+</details>
+
+
+# Performance
+
+Following are benchmarks showing the decompression bandwidth over the number of used cores.
+
+There are two rapidgzip variants shown: `(index)` and `(no index)`.
+Rapidgzip is generally faster when given an index with `--import-index` because it can delegate the decompression to ISA-l or zlib while it has to use its own custom-written gzip decompression engine when no index exists yet.
+Furthermore, decompression can be parallelized more evenly and more effectively when an index exists because the serializing window propagation step is not necessary.
+
+The violin plots show 20 repeated measurements as a single "blob".
+Thin blobs signal very reproducible timings while thick blobs signal a large variance.
+
+
+## Scaling Benchmarks on 2xAMD EPYC CPU 7702 (2x64 cores)
+
+### Decompression of Silesia Corpus
+
+![](https://raw.githubusercontent.com/mxmlnkn/indexed_bzip2/master/results/benchmarks/rapidgzip-0.9.0-scaling-benchmarks-2023-08-30/plots/result-parallel-decompression-silesia-dev-null-bandwidths-number-of-threads.png)
+
+This benchmark uses the [Silesia corpus](https://sun.aei.polsl.pl//~sdeor/index.php?page=silesia) compressed as a .tar.gz file to show the decompression performance.
+However, the compressed dataset is only ~69 MB, which is not sufficiently large to show parallelization over 128 cores.
+That's why the TAR file is repeated as often as there are number of cores in the benchmark times 2 and then compressed into a single large gzip file, which is ~18 GB compressed and 54 GB uncompressed for 128 cores.
+
+Rapidgzip achieves up to 24 GB/s with an index and 12 GB/s without.
+
+Pugz is not shown as comparison because it is not able to decompress the Silesia dataset because it contains binary data, which it cannot handle.
+
+
+### Decompression of Gzip-Compressed Base64 Data
+
+![](https://raw.githubusercontent.com/mxmlnkn/indexed_bzip2/master/results/benchmarks/rapidgzip-0.9.0-scaling-benchmarks-2023-08-30/plots/result-parallel-decompression-base64-dev-null-bandwidths-number-of-threads.png)
+
+This benchmarks uses random data, that has been base64 encoded and then gzip-compressed.
+This is the next best case for rapidgzip after the trivial case of purely random data, which cannot be compressed and therefore can be decompressed with a simple memory copy.
+This next best case results in mostly Huffman-coding compressed data with only very few LZ77 back-references.
+Without LZ77 back-references, parallel decompression can be done more independently and therefore faster than in the case of many LZ77 back-references.
+
+
+### Decompression of Gzip-Compressed FASTQ Data
+
+![](https://raw.githubusercontent.com/mxmlnkn/indexed_bzip2/master/results/benchmarks/rapidgzip-0.9.0-scaling-benchmarks-2023-08-30/plots/result-parallel-decompression-fastq-dev-null-bandwidths-number-of-threads.png)
+
+This benchmarks uses gzip-compressed [FASTQ data](http://ftp.sra.ebi.ac.uk/vol1/fastq/SRR224/085/SRR22403185/SRR22403185_2.fastq.gz).
+That's why the TAR file is repeated as often as there are number of cores in the benchmark to hold the decompression times roughly constant in order to make the benchmark over this large a range feasible.
+This is almost the worst case for rapidgzip because it contains many LZ77 back-references over very long ranges.
+This means that a fallback to ISA-L is not possible and it means that the costly two-staged decoding has to be done for almost all the data.
+This is also the reason why if fails to scale above 64 cores, i.e, to teh second CPU socket.
+The first and second decompression stages are completely independently submitted to a thread pool, which on this NUMA architecture means, that data needs to be costly transferred from one processor socket to the other if the second step for a chunk is not done on the same processor as the first.
+This should be fixable by making the ThreadPool NUMA-aware.
+
+These three scaling plots were created with rapidgzip 0.9.0 while the ones in the [paper](<results/paper/Knespel, Brunst - 2023 - Rapidgzip - Parallel Decompression and Seeking in Gzip Files Using Cache Prefetching.pdf>) were created with 0.5.0.
+
+
+## Scaling Benchmarks on Ryzen 3900X
+
+These benchmarks on my local workstation with a Ryzen 3900X only has 12 cores (24 virtual cores) but the base frequency is much higher than the 2xAMD EPYC CPU 7702.
+
+### Decompression With Existing Index
+
+|                        | 4GiB-base64                  | 4GiB-base64     | | 20x-silesia                   | 20x-silesia
+|------------------------|------------------------------|-----------------|-|-------------------------------|---------
+| Uncompressed Size      | 4 GiB                        |                 | | 3.95 GiB                      |
+| Compressed Size        | 3.04 GiB                     |                 | | 1.27 GiB                      |
+| **Module**             | **Bandwidth <br/> / (MB/s)** | **Speedup**     | |  **Bandwidth <br/> / (MB/s)** | **Speedup**
+| gzip                   |  250                         |    1            | |   293                         |  1
+| rapidgzip (0  threads) | 5179                         | 20.6            | |  5640                         | 18.8
+| rapidgzip (1  threads) |  488                         |  1.9            | |   684                         |  2.3
+| rapidgzip (2  threads) |  902                         |  3.6            | |  1200                         |  4.0
+| rapidgzip (6  threads) | 2617                         | 10.4            | |  3250                         | 10.9
+| rapidgzip (12 threads) | 4463                         | 17.7            | |  5600                         | 18.7
+| rapidgzip (24 threads) | 5240                         | 20.8            | |  5750                         | 19.2
+| rapidgzip (32 threads) | 4929                         | 19.6            | |  5300                         | 17.7
+
+
+### Decompression From Scratch
+
+|                        | 4GiB-base64                  | 4GiB-base64     | | 20x-silesia                   | 20x-silesia
+|------------------------|------------------------------|-----------------|-|-------------------------------|---------
+| Uncompressed Size      | 4 GiB                        |                 | | 3.95 GiB                      |
+| Compressed Size        | 3.04 GiB                     |                 | | 1.27 GiB                      |
+| **Module**             | **Bandwidth <br/> / (MB/s)** | **Speedup**     | |  **Bandwidth <br/> / (MB/s)** | **Speedup**
+| gzip                   |  250                         |    1            | |   293                         |  1
+| rapidgzip (0  threads) | 5060                         | 20.1            | |  2070                         |  6.9
+| rapidgzip (1  threads) |  487                         |  1.9            | |  630                          |  2.1
+| rapidgzip (2  threads) |  839                         |  3.3            | |  694                          |  2.3
+| rapidgzip (6  threads) | 2365                         |  9.4            | |  1740                         |  5.8
+| rapidgzip (12 threads) | 4116                         | 16.4            | |  1900                         |  6.4
+| rapidgzip (24 threads) | 4974                         | 19.8            | |  2040                         |  6.8
+| rapidgzip (32 threads) | 4612                         | 18.3            | |  2580                         |  8.6
+
 
 # Usage
 
 ## Command Line Tool
 
 ```bash
 rapidgzip --help
@@ -225,50 +307,51 @@
 I currently did not yet test integrating it into other projects other than simply manually copying the source in `src/core`, `src/rapidgzip`, and if integrated zlib is desired also `src/external/zlib`.
 If you have suggestions and wishes like support with CMake or Conan, please open an issue.
 
 
 # Citation
 
 A paper describing the implementation details and showing the scaling behavior with up to 128 cores has been submitted to and [accepted](https://www.hpdc.org/2023/program/technical-sessions/) in [ACM HPDC'23](https://www.hpdc.org/2023/), The 32nd International Symposium on High-Performance Parallel and Distributed Computing.
-The author's version can be found [here](<results/paper/Knespel, Brunst - 2023 - Rapidgzip - Parallel Decompression and Seeking in Gzip Files Using Cache Prefetching.pdf>) and the accompanying presentation [here](results/Presentation-2023-06-22.pdf).
+The paper can be accessed [freely on ACM DL](https://doi.org/10.1145/3588195.3592992).
+The accompanying presentation can be found [here](results/Presentation-2023-06-22.pdf).
 
 If you use this software for your scientific publication, please cite it as:
 
 This is preliminiary. The final citation will become available end of June 2023.
 
 ```bibtex
 @inproceedings{rapidgzip,
     author    = {Knespel, Maximilian and Brunst, Holger},
     title     = {Rapidgzip: Parallel Decompression and Seeking in Gzip Files Using Cache Prefetching},
     year      = {2023},
-    % isbn    = {},  % To be released end of June
+    isbn      = {9798400701559},
     publisher = {Association for Computing Machinery},
     address   = {New York, NY, USA},
     url       = {https://doi.org/10.1145/3588195.3592992},
     doi       = {10.1145/3588195.3592992},
     abstract  = {Gzip is a file compression format, which is ubiquitously used. Although a multitude of gzip implementations exist, only pugz can fully utilize current multi-core processor architectures for decompression. Yet, pugz cannot decompress arbitrary gzip files. It requires the decompressed stream to only contain byte values 9–126. In this work, we present a generalization of the parallelization scheme used by pugz that can be reliably applied to arbitrary gzip-compressed data without compromising performance. We show that the requirements on the file contents posed by pugz can be dropped by implementing an architecture based on a cache and a parallelized prefetcher. This architecture can safely handle faulty decompression results, which can appear when threads start decompressing in the middle of a gzip file by using trial and error. Using 128 cores, our implementation reaches 8.7 GB/s decompression bandwidth for gzip-compressed base64-encoded data, a speedup of 55 over the single-threaded GNU gzip, and 5.6 GB/s for the Silesia corpus, a speedup of 33 over GNU gzip.},
     booktitle = {Proceedings of the 32nd International Symposium on High-Performance Parallel and Distributed Computing},
-    % pages   = {16–29},  % To be released end of June
+    pages     = {295–307},
     numpages  = {13},
-    keywords  = {Gzip, Decompression, Parallel Algorithm, Performance, Random Access},
+    keywords  = {gzip, decompression, parallel algorithm, performance, random access},
     location  = {Orlando, FL, USA},
     series    = {HPDC '23},
 }
 ```
 
 # About
 
 This tool originated as a backend for [ratarmount](https://github.com/mxmlnkn/ratarmount).
 After writing the bzip2 backend for [ratarmount](https://github.com/mxmlnkn/indexed_bzip2), my hesitation about reimplementing custom decoders for existing file formats has vastly diminished.
 And, while random access to gzip files did exist with [indexed_gzip](https://github.com/pauldmccarthy/indexed_gzip), it did not support parallel decompression neither for the index creation nor when the index already exists.
-The latter of which is trivial, when ignoring load balancing issues, but parallelizing even the idnex creation is vastly more complicated because decompressing data requires the previous 32 KiB of decompressed data to be known.
+The latter of which is trivial, when ignoring load balancing issues, but parallelizing even the index creation is vastly more complicated because decompressing data requires the previous 32 KiB of decompressed data to be known.
 
 After implementing a production-ready version by improving upon the algorithm used by [pugz](https://github.com/Piezoid/pugz), I submitted a [paper](Citation).
-The review process was double-blind and I was unsure whether pseudonymize Pragzip because it has already been uploaded to Github.
-In the end, I used Rapidgzip during the review process and because I was not sure, which form fields should be filled with the pseudonymized title, I simply stuck with it.
+The review process was double-blind and I was unsure whether to pseudonymize Pragzip because it has already been uploaded to Github.
+In the end, I used "rapidgzip" during the review process and because I was not sure, which form fields should be filled with the pseudonymized title, I simply stuck with it.
 Rapidgzip was chosen for similar reason to rapidgzip, namely the P and RA are acronyms for Parallel and Random Access.
 As rapgzip, did not stick, I used rapidgzip, which now also contains the foremost design goal in its name: being rapidly faster than single-threaded implementations.
 Furthermore, the additional ID could be interpreted to stand for Index and Decompression, making "rapid" a partial backronym.
 
 
 # Internal Architecture
```

### Comparing `rapidgzip-0.8.1/core/AffinityHelpers.hpp` & `rapidgzip-0.9.0/core/AffinityHelpers.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/core/AlignedAllocator.hpp` & `rapidgzip-0.9.0/core/AlignedAllocator.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/core/AtomicMutex.hpp` & `rapidgzip-0.9.0/core/AtomicMutex.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/core/BitManipulation.hpp` & `rapidgzip-0.9.0/core/BitManipulation.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/core/BitReader.hpp` & `rapidgzip-0.9.0/core/BitReader.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/core/BitStringFinder.hpp` & `rapidgzip-0.9.0/core/BitStringFinder.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/core/BlockFetcher.hpp` & `rapidgzip-0.9.0/core/BlockFetcher.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -28,16 +28,15 @@
  * Manages block data access. Calls to members are not thread-safe!
  * Requested blocks are cached and accesses may trigger prefetches,
  * which will be fetched in parallel using a thread pool.
  */
 template<typename T_BlockFinder,
          typename T_BlockData,
          typename FetchingStrategy,
-         bool     ENABLE_STATISTICS = false,
-         bool     SHOW_PROFILE = false>
+         bool     ENABLE_STATISTICS = false>
 class BlockFetcher
 {
 public:
     using BlockFinder = T_BlockFinder;
     using BlockData = T_BlockData;
     using BlockCache = Cache</** block offset in bits */ size_t, std::shared_ptr<BlockData> >;
 
@@ -175,37 +174,47 @@
     BlockFetcher( std::shared_ptr<BlockFinder> blockFinder,
                   size_t                       parallelization ) :
         m_parallelization( parallelization == 0 ? std::max<size_t>( 1U, availableCores() ) : parallelization ),
         m_blockFinder( std::move( blockFinder ) ),
         m_cache( std::max( size_t( 16 ), m_parallelization ) ),
         m_prefetchCache( 2 * m_parallelization /* Only m_parallelization would lead to lot of cache pollution! */ ),
         m_failedPrefetchCache( m_prefetchCache.capacity() ),
-        m_threadPool( m_parallelization )
+        /* If parallelization is 1, then do not start any thread even if the main thread is not doing much work. */
+        m_threadPool( m_parallelization == 1 ? 0 : m_parallelization )
     {
         if ( !m_blockFinder ) {
             throw std::invalid_argument( "BlockFinder must be valid!" );
         }
 
-        if constexpr ( ENABLE_STATISTICS || SHOW_PROFILE ) {
+        if constexpr ( ENABLE_STATISTICS ) {
             m_statistics.parallelization = m_parallelization;
         }
     }
 
 public:
     virtual
     ~BlockFetcher()
     {
-        if constexpr ( SHOW_PROFILE ) {
+        if ( m_showProfileOnDestruction ) {
             /* Clear caches while updating the unused entries statistic. */
             m_cache.shrinkTo( 0 );
             m_prefetchCache.shrinkTo( 0 );
             std::cerr << ( ThreadSafeOutput() << "[BlockFetcher::~BlockFetcher]" << statistics().print() );
         }
     }
 
+    /**
+     * @note Only will work if ENABLE_STATISTICS is true.
+     */
+    void
+    setShowProfileOnDestruction( bool showProfileOnDestruction )
+    {
+        m_showProfileOnDestruction = showProfileOnDestruction;
+    }
+
     [[nodiscard]] bool
     test( const size_t blockOffset ) const
     {
         return ( m_prefetching.find( blockOffset ) != m_prefetching.end() )
                || m_cache.test( blockOffset )
                || m_prefetchCache.test( blockOffset );
     }
@@ -233,15 +242,15 @@
         auto resultFromCaches = getFromCaches( blockOffset );
         auto& cachedResult = resultFromCaches.first;
         auto& queuedResult = resultFromCaches.second;
 
         const auto validDataBlockIndex = dataBlockIndex ? *dataBlockIndex : m_blockFinder->find( blockOffset );
         const auto nextBlockOffset = m_blockFinder->get( validDataBlockIndex + 1 );
 
-        if constexpr ( ENABLE_STATISTICS || SHOW_PROFILE ) {
+        if constexpr ( ENABLE_STATISTICS ) {
             m_statistics.recordBlockIndexGet( validDataBlockIndex );
         }
 
         /* Start requested calculation if necessary. */
         if ( !cachedResult.has_value() && !queuedResult.valid() ) {
             queuedResult = submitOnDemandTask( blockOffset, nextBlockOffset );
         }
@@ -256,15 +265,15 @@
             };
 
         prefetchNewBlocks( getPartitionOffsetFromOffset, resultIsReady );
 
         /* Return result */
         if ( cachedResult.has_value() ) {
             assert( !queuedResult.valid() );
-            if constexpr ( ENABLE_STATISTICS || SHOW_PROFILE ) {
+            if constexpr ( ENABLE_STATISTICS ) {
                 std::scoped_lock lock( m_analyticsMutex );
                 m_statistics.getTotalTime += duration( tGetStart );
             }
             return *std::move( cachedResult );
         }
 
         [[maybe_unused]] const auto tFutureGetStart = now();
@@ -274,15 +283,15 @@
             prefetchNewBlocks( getPartitionOffsetFromOffset, resultIsReady );
         }
         auto result = std::make_shared<BlockData>( queuedResult.get() );
         [[maybe_unused]] const auto futureGetDuration = duration( tFutureGetStart );
 
         insertIntoCache( blockOffset, result );
 
-        if constexpr ( ENABLE_STATISTICS || SHOW_PROFILE ) {
+        if constexpr ( ENABLE_STATISTICS ) {
             std::scoped_lock lock( m_analyticsMutex );
             m_statistics.futureWaitTotalTime += futureGetDuration;
             m_statistics.getTotalTime += duration( tGetStart );
         }
 
         return result;
     }
@@ -370,15 +379,15 @@
         const auto match = m_prefetching.find( blockOffset );
 
         if ( match != m_prefetching.end() ) {
             resultFuture = std::move( match->second );
             m_prefetching.erase( match );
             assert( resultFuture.valid() );
 
-            if constexpr ( ENABLE_STATISTICS || SHOW_PROFILE ) {
+            if constexpr ( ENABLE_STATISTICS ) {
                 ++m_statistics.prefetchDirectHits;
             }
         }
 
         return resultFuture;
     }
 
@@ -479,15 +488,15 @@
                 std::tie( nextPrefetchBlockOffset, nextPrefetchGetReturnCode ) =
                     m_blockFinder->get( blockIndexToPrefetch + 1, stopPrefetching() ? 0 : 0.0001 );
             }
             while ( !prefetchBlockOffset && ( prefetchGetReturnCode != GetReturnCode::FAILURE )
                     && !nextPrefetchBlockOffset && ( nextPrefetchGetReturnCode != GetReturnCode::FAILURE )
                     && !stopPrefetching() );
 
-            if constexpr ( ENABLE_STATISTICS || SHOW_PROFILE ) {
+            if constexpr ( ENABLE_STATISTICS ) {
                 if ( !prefetchBlockOffset.has_value() ) {
                     m_statistics.waitOnBlockFinderCount++;
                 }
             }
 
             /* Do not prefetch already cached/prefetched blocks or block indexes which are not yet in the block map. */
             if ( !prefetchBlockOffset.has_value()
@@ -530,15 +539,15 @@
         }
     }
 
     [[nodiscard]] std::future<BlockData>
     submitOnDemandTask( const size_t                blockOffset,
                         const std::optional<size_t> nextBlockOffset )
     {
-        if constexpr ( ENABLE_STATISTICS || SHOW_PROFILE ) {
+        if constexpr ( ENABLE_STATISTICS ) {
             ++m_statistics.onDemandFetchCount;
         }
         auto resultFuture = m_threadPool.submit(
             [this, blockOffset, nextBlockOffset] ()
             {
                 return decodeAndMeasureBlock(
                     blockOffset, nextBlockOffset ? *nextBlockOffset : std::numeric_limits<size_t>::max() );
@@ -591,15 +600,15 @@
 private:
     [[nodiscard]] BlockData
     decodeAndMeasureBlock( size_t blockOffset,
                            size_t nextBlockOffset ) const
     {
         [[maybe_unused]] const auto tDecodeStart = now();
         auto blockData = decodeBlock( blockOffset, nextBlockOffset );
-        if constexpr ( ENABLE_STATISTICS || SHOW_PROFILE ) {
+        if constexpr ( ENABLE_STATISTICS ) {
             const auto tDecodeEnd = now();
 
             std::scoped_lock lock( this->m_analyticsMutex );
 
             const auto& minStartTime = this->m_statistics.decodeBlockStartTime;
             this->m_statistics.decodeBlockStartTime.emplace(
                 minStartTime ? std::min( *minStartTime, tDecodeStart ) : tDecodeStart );
@@ -621,14 +630,16 @@
     mutable double m_readBlockDataTotalTime{ 0 };
     mutable std::mutex m_analyticsMutex;
 
     const size_t m_parallelization;
 
     FetchingStrategy m_fetchingStrategy;
 
+    bool m_showProfileOnDestruction{ false };
+
 private:
     /**
      * The block finder is used to prefetch blocks among others.
      * But, in general, it only returns unconfirmed guesses for block offsets (at first)!
      * Confirmed block offsets are written to the BlockMap but adding that in here seems a bit overkill
      * and would need further logic to get the next blocks given a specific one.
      * Therefore, the idea is to update and confirm the blocks inside the block finder, which would invalidate
```

### Comparing `rapidgzip-0.8.1/core/BlockFinder.hpp` & `rapidgzip-0.9.0/core/BlockFinder.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/core/BlockFinderInterface.hpp` & `rapidgzip-0.9.0/core/BlockFinderInterface.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/core/BlockMap.hpp` & `rapidgzip-0.9.0/core/BlockMap.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/core/Cache.hpp` & `rapidgzip-0.9.0/core/Cache.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/core/FasterVector.hpp` & `rapidgzip-0.9.0/core/FasterVector.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/core/FileUtils.hpp` & `rapidgzip-0.9.0/core/FileUtils.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/core/JoiningThread.hpp` & `rapidgzip-0.9.0/core/JoiningThread.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/core/ParallelBitStringFinder.hpp` & `rapidgzip-0.9.0/core/ParallelBitStringFinder.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/core/Prefetcher.hpp` & `rapidgzip-0.9.0/core/Prefetcher.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/core/Statistics.hpp` & `rapidgzip-0.9.0/core/Statistics.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/core/StreamedResults.hpp` & `rapidgzip-0.9.0/core/StreamedResults.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/core/TestHelpers.hpp` & `rapidgzip-0.9.0/core/TestHelpers.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/core/ThreadPool.hpp` & `rapidgzip-0.9.0/core/ThreadPool.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -125,14 +125,18 @@
     template<class T_Functor>
     std::future<decltype( std::declval<T_Functor>()() )>
     submit( T_Functor task,
             int       priority = 0 )
     {
         std::lock_guard lock( m_mutex );
 
+        if ( m_threadCount == 0 ) {
+            return std::async( std::launch::deferred, std::move( task ) );
+        }
+
         /* Use a packaged task, which abstracts handling the return type and makes the task return void. */
         using ReturnType = decltype( std::declval<T_Functor>()() );
         std::packaged_task<ReturnType()> packagedTask{ std::move( task ) };
         auto resultFuture = packagedTask.get_future();
         m_tasks[priority].emplace_back( std::move( packagedTask ) );
 
         if ( ( m_threads.size() < m_threadCount ) && ( m_idleThreadCount == 0 ) ) {
```

### Comparing `rapidgzip-0.8.1/core/VectorView.hpp` & `rapidgzip-0.9.0/core/VectorView.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,21 @@
     constexpr
     VectorView( const T* data,
                 size_t   size ) noexcept :
         m_data( data ),
         m_size( size )
     {}
 
+    constexpr
+    VectorView( const T* data,
+                const T* dataEnd ) noexcept :
+        m_data( data ),
+        m_size( std::distance( data, dataEnd ) )
+    {}
+
     [[nodiscard]] constexpr T
     front() const noexcept
     {
         return *m_data;
     }
 
     [[nodiscard]] constexpr const T*
```

### Comparing `rapidgzip-0.8.1/core/common.hpp` & `rapidgzip-0.9.0/core/common.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/core/filereader/BufferView.hpp` & `rapidgzip-0.9.0/core/filereader/BufferView.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,21 @@
 
 
 class BufferViewFileReader :
     public FileReader
 {
 public:
     explicit
+    BufferViewFileReader( const void* const buffer,
+                          const size_t      size ) :
+        m_buffer( reinterpret_cast<const std::byte*>( buffer ) ),
+        m_size( size )
+    {}
+
+    explicit
     BufferViewFileReader( const std::vector<char>& buffer ) :
         m_buffer( reinterpret_cast<const std::byte*>( buffer.data() ) ),
         m_size( buffer.size() )
     {}
 
     explicit
     BufferViewFileReader( const std::vector<unsigned char>& buffer ) :
```

### Comparing `rapidgzip-0.8.1/core/filereader/Buffered.hpp` & `rapidgzip-0.9.0/core/filereader/Buffered.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/core/filereader/FileReader.hpp` & `rapidgzip-0.9.0/core/filereader/FileReader.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/core/filereader/Memory.hpp` & `rapidgzip-0.9.0/core/filereader/Memory.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/core/filereader/Python.hpp` & `rapidgzip-0.9.0/core/filereader/Python.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/core/filereader/Shared.hpp` & `rapidgzip-0.9.0/core/filereader/Shared.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     explicit
     SharedFileReader( UniqueFileReader file ) :
         SharedFileReader( file.release() )
     {}
 
     ~SharedFileReader()
     {
-        if ( m_statistics && m_statistics->enabled && ( m_statistics.use_count() == 1 ) ) {
+        if ( m_statistics && m_statistics->showProfileOnDestruction && ( m_statistics.use_count() == 1 ) ) {
             std::cerr << ( ThreadSafeOutput()
                 << "[SharedFileReader::~SharedFileReader]\n"
                 << "   seeks back    : (" << m_statistics->seekBack.formatAverageWithUncertainty( true )
                 << " ) B (" << m_statistics->seekBack.count << "calls )\n"
                 << "   seeks forward : (" << m_statistics->seekForward.formatAverageWithUncertainty( true )
                 << " ) B (" << m_statistics->seekForward.count << "calls )\n"
                 << "   reads         : (" << m_statistics->read.formatAverageWithUncertainty( true )
@@ -112,14 +112,22 @@
     setStatisticsEnabled( bool enabled )
     {
         if ( m_statistics ) {
             m_statistics->enabled = enabled;
         }
     }
 
+    void
+    setShowProfileOnDestruction( bool showProfileOnDestruction )
+    {
+        if ( m_statistics ) {
+            m_statistics->showProfileOnDestruction = showProfileOnDestruction;
+        }
+    }
+
 private:
     /**
      * Create a new shared file reader from an existing SharedFileReader by copying shared pointers.
      * The underlying file and mutex are held as a shared_ptr and therefore not copied itself!
      * Make it private because only @ref clone should call this. It cannot be defaulted because the FileReader
      * base class deleted its copy constructor.
      */
@@ -305,14 +313,15 @@
             ++m_statistics->locks;
         }
         return std::scoped_lock( *m_mutex );
     }
 
 private:
     struct AccessStatistics {
+        bool showProfileOnDestruction{ false };
         bool enabled{ false };
         uint64_t lastAccessOffset{ 0 };  // necessary for pread because tell() won't work
         Statistics<uint64_t> read;
         Statistics<uint64_t> seekBack;
         Statistics<uint64_t> seekForward;
         double readingTime{ 0 };
         std::atomic<uint64_t> locks{ 0 };
```

### Comparing `rapidgzip-0.8.1/core/filereader/Standard.hpp` & `rapidgzip-0.9.0/core/filereader/Standard.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/core/filereader/StreamAdapter.hpp` & `rapidgzip-0.9.0/core/filereader/StreamAdapter.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/cxxopts/LICENSE` & `rapidgzip-0.9.0/external/cxxopts/LICENSE`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/cxxopts/include/cxxopts.hpp` & `rapidgzip-0.9.0/external/cxxopts/include/cxxopts.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,22 @@
 #    include <optional>
 #    ifdef __cpp_lib_optional
 #      define CXXOPTS_HAS_OPTIONAL
 #    endif
 #  endif
 #endif
 
+#define CXXOPTS_FALLTHROUGH
+#ifdef __has_cpp_attribute
+  #if __has_cpp_attribute(fallthrough)
+    #undef CXXOPTS_FALLTHROUGH
+    #define CXXOPTS_FALLTHROUGH [[fallthrough]]
+  #endif
+#endif
+
 #if __cplusplus >= 201603L
 #define CXXOPTS_NODISCARD [[nodiscard]]
 #else
 #define CXXOPTS_NODISCARD
 #endif
 
 #ifndef CXXOPTS_VECTOR_DELIMITER
@@ -357,14 +365,17 @@
   virtual ~Value() = default;
 
   virtual
   std::shared_ptr<Value>
   clone() const = 0;
 
   virtual void
+  add(const std::string& text) const = 0;
+
+  virtual void
   parse(const std::string& text) const = 0;
 
   virtual void
   parse() const = 0;
 
   virtual bool
   has_default() const = 0;
@@ -1052,14 +1063,30 @@
   while(!in.eof() && std::getline(in, token, CXXOPTS_VECTOR_DELIMITER)) {
     T v;
     parse_value(token, v);
     value.emplace_back(std::move(v));
   }
 }
 
+template <typename T>
+void
+add_value(const std::string& text, T& value)
+{
+  parse_value(text, value);
+}
+
+template <typename T>
+void
+add_value(const std::string& text, std::vector<T>& value)
+{
+  T v;
+  add_value(text, v);
+  value.emplace_back(std::move(v));
+}
+
 #ifdef CXXOPTS_HAS_OPTIONAL
 template <typename T>
 void
 parse_value(const std::string& text, std::optional<T>& value)
 {
   T result;
   parse_value(text, result);
@@ -1126,14 +1153,20 @@
     m_default = rhs.m_default;
     m_implicit = rhs.m_implicit;
     m_default_value = rhs.m_default_value;
     m_implicit_value = rhs.m_implicit_value;
   }
 
   void
+  add(const std::string& text) const override
+  {
+    add_value(text, *m_store);
+  }
+
+  void
   parse(const std::string& text) const override
   {
     parse_value(text, *m_store);
   }
 
   bool
   is_container() const override
@@ -1411,14 +1444,27 @@
   std::vector<HelpOptionDetails> options{};
 };
 
 class OptionValue
 {
   public:
   void
+  add
+  (
+    const std::shared_ptr<const OptionDetails>& details,
+    const std::string& text
+  )
+  {
+    ensure_value(details);
+    ++m_count;
+    m_value->add(text);
+    m_long_names = &details->long_names();
+  }
+
+  void
   parse
   (
     const std::shared_ptr<const OptionDetails>& details,
     const std::string& text
   )
   {
     ensure_value(details);
@@ -1780,15 +1826,15 @@
     const char* const* argv,
     int& current,
     const std::shared_ptr<OptionDetails>& value,
     const std::string& name
   );
 
   void
-  add_to_option(OptionMap::const_iterator iter, const std::string& option, const std::string& arg);
+  add_to_option(const std::shared_ptr<OptionDetails>& value, const std::string& arg);
 
   void
   parse_option
   (
     const std::shared_ptr<OptionDetails>& value,
     const std::string& name,
     const std::string& arg = ""
@@ -2235,14 +2281,15 @@
       [&](const std::string& name) { return name.length() > 1; }
     );
   auto num_length_1_names = (option_names.end() - first_short_name_iter);
   switch(num_length_1_names) {
   case 1:
     short_name = *first_short_name_iter;
     option_names.erase(first_short_name_iter);
+    CXXOPTS_FALLTHROUGH;
   case 0:
     break;
   default:
     throw_or_mimic<exceptions::invalid_option_format>(opts);
   };
 
   m_options.add_option
@@ -2326,17 +2373,21 @@
       ++current;
     }
   }
 }
 
 inline
 void
-OptionParser::add_to_option(OptionMap::const_iterator iter, const std::string& option, const std::string& arg)
+OptionParser::add_to_option(const std::shared_ptr<OptionDetails>& value, const std::string& arg)
 {
-  parse_option(iter->second, option, arg);
+  auto hash = value->hash();
+  auto& result = m_parsed[hash];
+  result.add(value, arg);
+
+  m_sequential.emplace_back(value->essential_name(), arg);
 }
 
 inline
 bool
 OptionParser::consume_positional(const std::string& a, PositionalListIterator& next)
 {
   while (next != m_positional.end())
@@ -2345,22 +2396,22 @@
     if (iter != m_options.end())
     {
       if (!iter->second->value().is_container())
       {
         auto& result = m_parsed[iter->second->hash()];
         if (result.count() == 0)
         {
-          add_to_option(iter, *next, a);
+          add_to_option(iter->second, a);
           ++next;
           return true;
         }
         ++next;
         continue;
       }
-      add_to_option(iter, *next, a);
+      add_to_option(iter->second, a);
       return true;
     }
     throw_or_mimic<exceptions::no_such_option>(*next);
   }
 
   return false;
 }
```

### Comparing `rapidgzip-0.8.1/external/isa-l/LICENSE` & `rapidgzip-0.9.0/external/isa-l/LICENSE`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/isa-l/igzip/huff_codes.h` & `rapidgzip-0.9.0/external/isa-l/igzip/huff_codes.h`

 * *Files 16% similar despite different names*

```diff
@@ -94,39 +94,8 @@
 #define DEPTH_MASK 0x7F
 #define DEPTH_MASK_HI (DEPTH_MASK << DEPTH_SHIFT)
 #define DEPTH_1       (1 << DEPTH_SHIFT)
 #define HEAP_TREE_SIZE (3*MAX_HISTHEAP_SIZE + 1)
 #define HEAP_TREE_NODE_START (HEAP_TREE_SIZE-1)
 #define MAX_BL_CODE_LEN 7
 
-/**
- * @brief Structure used to store huffman codes
- */
-struct huff_code {
-	union {
-		struct {
-#if __BYTE_ORDER__ == __ORDER_LITTLE_ENDIAN__
-			uint32_t code_and_extra:24;
-			uint32_t length2:8;
-#else
-			uint32_t length2:8;
-			uint32_t code_and_extra:24;
-#endif
-		};
-
-		struct {
-#if __BYTE_ORDER__ == __ORDER_LITTLE_ENDIAN__
-			uint16_t code;
-			uint8_t extra_bit_count;
-			uint8_t length;
-#else
-			uint8_t length;
-			uint8_t extra_bit_count;
-			uint16_t code;
-#endif
-		};
-
-		uint32_t code_and_length;
-	};
-};
-
 #endif
```

### Comparing `rapidgzip-0.8.1/external/isa-l/igzip/hufftables_c.c` & `rapidgzip-0.9.0/external/isa-l/igzip/hufftables_c.c`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/isa-l/igzip/igzip.c` & `rapidgzip-0.9.0/external/isa-l/igzip/igzip.c`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/isa-l/igzip/igzip_decode_block_stateless.asm` & `rapidgzip-0.9.0/external/isa-l/igzip/igzip_decode_block_stateless.asm`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/isa-l/igzip/igzip_inflate.c` & `rapidgzip-0.9.0/external/isa-l/igzip/igzip_inflate.c`

 * *Files 5% similar despite different names*

```diff
@@ -263,16 +263,15 @@
 }
 
 static void inline write_huff_code(struct huff_code *huff_code, uint32_t code, uint32_t length)
 {
 	huff_code->code_and_length = code | length << 24;
 }
 
-static int inline set_codes(struct huff_code *huff_code_table, int table_length,
-			    uint16_t * count)
+int set_codes(struct huff_code * huff_code_table, int const table_length, uint16_t const * const count)
 {
 	uint32_t max, code, length;
 	uint32_t next_code[MAX_HUFF_TREE_DEPTH + 1];
 	int i;
 	struct huff_code *table_end = huff_code_table + table_length;
 
 	/* Setup for calculating huffman codes */
@@ -296,19 +295,19 @@
 
 		write_huff_code(huff_code_table, code, length);
 		next_code[length] += 1;
 	}
 	return 0;
 }
 
-static int inline set_and_expand_lit_len_huffcode(struct huff_code *lit_len_huff,
-						  uint32_t table_length,
-						  uint16_t * count,
-						  uint16_t * expand_count,
-						  uint32_t * code_list)
+int set_and_expand_lit_len_huffcode(struct huff_code const * const lit_len_huff,
+						  uint32_t const table_length,
+						  uint16_t * const count,
+						  uint16_t * const expand_count,
+						  uint32_t * const code_list)
 {
 	int len_sym, len_size, extra_count, extra;
 	uint32_t count_total, count_tmp;
 	uint32_t code, code_len, expand_len;
 	struct huff_code *expand_next = &lit_len_huff[ISAL_DEF_LIT_SYMBOLS];
 	struct huff_code tmp_table[LIT_LEN - ISAL_DEF_LIT_SYMBOLS];
 	uint32_t max;
@@ -406,18 +405,18 @@
 {
 	return (index != 513) ? index : 512;
 }
 
 /* Sets result to the inflate_huff_code corresponding to the huffcode defined by
  * the lengths in huff_code_table,where count is a histogram of the appearance
  * of each code length */
-static void make_inflate_huff_code_lit_len(struct inflate_huff_code_large *result,
-					   struct huff_code *huff_code_table,
-					   uint32_t table_length, uint16_t * count_total,
-					   uint32_t * code_list, uint32_t multisym)
+void make_inflate_huff_code_lit_len(struct inflate_huff_code_large * const result,
+					   struct huff_code * const huff_code_table,
+					   uint32_t const table_length, uint16_t const * const count_total,
+					   uint32_t * const code_list, uint32_t const multisym)
 {
 	int i, j;
 	uint16_t code = 0;
 	uint32_t *long_code_list;
 	uint32_t long_code_length = 0;
 	uint16_t temp_code_list[1 << (MAX_LIT_LEN_CODE_LEN - ISAL_DECODE_LONG_BITS)];
 	uint32_t temp_code_length;
@@ -625,18 +624,19 @@
 		}
 		result->short_code_lookup[first_bits] = long_code_lookup_length |
 		    (max_length << LARGE_SHORT_MAX_LEN_OFFSET) | LARGE_FLAG_BIT;
 		long_code_lookup_length += 1 << (max_length - ISAL_DECODE_LONG_BITS);
 	}
 }
 
-static void inline make_inflate_huff_code_dist(struct inflate_huff_code_small *result,
-					       struct huff_code *huff_code_table,
-					       uint32_t table_length, uint16_t * count,
-					       uint32_t max_symbol)
+void make_inflate_huff_code_dist(struct inflate_huff_code_small * const result,
+                                 struct huff_code * const huff_code_table,
+                                 uint32_t const table_length,
+                                 uint16_t const * const count,
+                                 uint32_t const max_symbol)
 {
 	int i, j, k;
 	uint32_t *long_code_list;
 	uint32_t long_code_length = 0;
 	uint16_t temp_code_list[1 << (15 - ISAL_DECODE_SHORT_BITS)];
 	uint32_t temp_code_length;
 	uint32_t long_code_lookup_length = 0;
@@ -1105,15 +1105,15 @@
 		inflate_in_load(state, 0);
 
 	next_bits = state->read_in & ((1 << ISAL_DECODE_SHORT_BITS) - 1);
 
 	/* next_sym is a possible symbol decoded from next_bits. If bit 15 is 0,
 	 * next_code is a symbol. Bits 9:0 represent the symbol, and bits 14:10
 	 * represent the length of that symbols huffman code. If next_sym is not
-	 * a symbol, it provides a hint of where the large symbols containin
+	 * a symbol, it provides a hint of where the large symbols containing
 	 * this code are located. Note the hint is at largest the location the
 	 * first actual symbol in the long code list.*/
 	next_sym = huff_code->short_code_lookup[next_bits];
 
 	if ((next_sym & SMALL_FLAG_BIT) == 0) {
 		/* Return symbol found if next_code is a complete huffman code
 		 * and shift in buffer over by the length of the next_code */
@@ -1228,14 +1228,15 @@
 	};
 
 	/* If you are given a whole header and it matches the pregen header */
 	if (state->avail_in > (hufftables_default.deflate_hdr_count + sizeof(uint64_t))
 	    && header_matches_pregen(state))
 		return setup_pregen_header(state);
 
+    /* All of these appear when decoding a .bgz file! */
 	if (state->bfinal && state->avail_in <= SINGLE_SYM_THRESH) {
 		multisym = SINGLE_SYM_FLAG;
 	} else if (state->bfinal && state->avail_in <= DOUBLE_SYM_THRESH) {
 		multisym = DOUBLE_SYM_FLAG;
 	}
 
 	memset(code_count, 0, sizeof(code_count));
@@ -1439,14 +1440,15 @@
 
 	/* btype and bfinal are defined in RFC 1951, bfinal represents whether
 	 * the current block is the end of block, and btype represents the
 	 * encoding method on the current block. */
 
 	state->bfinal = inflate_in_read_bits(state, 1);
 	btype = inflate_in_read_bits(state, 2);
+	state->btype = btype;
 
 	if (state->read_in_length < 0)
 		ret = ISAL_END_INPUT;
 
 	else if (btype == 0) {
 		inflate_in_load(state, 40);
 		bytes = state->read_in_length / 8;
@@ -1773,14 +1775,18 @@
 	state->write_overflow_len = 0;
 	state->copy_overflow_length = 0;
 	state->copy_overflow_distance = 0;
 	state->wrapper_flag = 0;
 	state->tmp_in_size = 0;
 	state->tmp_out_processed = 0;
 	state->tmp_out_valid = 0;
+	state->points_to_stop_at = ISAL_STOPPING_POINT_NONE;
+	state->stopped_at = ISAL_STOPPING_POINT_NONE;
+	state->tmp_out_stopped_at = ISAL_STOPPING_POINT_NONE;
+	state->btype = -1;
 }
 
 void isal_inflate_reset(struct inflate_state *state)
 {
 	state->read_in = 0;
 	state->read_in_length = 0;
 	state->total_out = 0;
@@ -1793,14 +1799,17 @@
 	state->write_overflow_len = 0;
 	state->copy_overflow_length = 0;
 	state->copy_overflow_distance = 0;
 	state->wrapper_flag = 0;
 	state->tmp_in_size = 0;
 	state->tmp_out_processed = 0;
 	state->tmp_out_valid = 0;
+	state->stopped_at = ISAL_STOPPING_POINT_NONE;
+	state->tmp_out_stopped_at = ISAL_STOPPING_POINT_NONE;
+	state->btype = -1;
 }
 
 static inline uint32_t fixed_size_read(struct inflate_state *state,
 				       uint8_t ** read_buf, int read_size)
 {
 	uint32_t tmp_in_size = state->tmp_in_size;
 
@@ -2273,34 +2282,70 @@
 
 	uint8_t *start_out = state->next_out;
 	uint32_t avail_out = state->avail_out;
 	uint32_t copy_size = 0;
 	int32_t shift_size = 0;
 	int ret = 0;
 
+	state->stopped_at = ISAL_STOPPING_POINT_NONE;
+
+    /* First, copy from the internal output buffer before setting stopped_at to the real stopping point. */
+	if (state->tmp_out_stopped_at != ISAL_STOPPING_POINT_NONE) {
+		/* Copy data from tmp_out buffer into out_buffer */
+		uint32_t copy_size = state->tmp_out_valid - state->tmp_out_processed;
+		if (copy_size > state->avail_out)
+			copy_size = state->avail_out;
+
+		memcpy(state->next_out,
+		       &state->tmp_out_buffer[state->tmp_out_processed], copy_size);
+
+		state->tmp_out_processed += copy_size;
+		state->avail_out -= copy_size;
+		state->next_out += copy_size;
+
+		state->total_out += copy_size;
+
+		if (state->tmp_out_valid == state->tmp_out_processed) {
+			state->stopped_at = state->tmp_out_stopped_at;
+			state->tmp_out_stopped_at = ISAL_STOPPING_POINT_NONE;
+		}
+		return ISAL_DECOMP_OK;
+	}
+
 	if (!state->wrapper_flag && state->crc_flag == IGZIP_GZIP) {
 		struct isal_gzip_header gz_hdr;
 		isal_gzip_header_init(&gz_hdr);
 		ret = isal_read_gzip_header(state, &gz_hdr);
 		if (ret < 0)
 			return ret;
 		else if (ret > 0)
 			return ISAL_DECOMP_OK;
+
+		if ((ret == 0) && (state->points_to_stop_at & ISAL_STOPPING_POINT_END_OF_STREAM_HEADER)) {
+			state->stopped_at = ISAL_STOPPING_POINT_END_OF_STREAM_HEADER;
+			return ISAL_DECOMP_OK;
+		}
+
 	} else if (!state->wrapper_flag && state->crc_flag == IGZIP_ZLIB) {
 		struct isal_zlib_header z_hdr = { 0 };
 		ret = isal_read_zlib_header(state, &z_hdr);
 		if (ret < 0)
 			return ret;
 		else if (ret > 0)
 			return ISAL_DECOMP_OK;
 
 		if (z_hdr.dict_flag) {
 			state->dict_id = z_hdr.dict_id;
 			return ISAL_NEED_DICT;
 		}
+
+		if ((ret == 0) && (state->points_to_stop_at & ISAL_STOPPING_POINT_END_OF_STREAM_HEADER)) {
+			state->stopped_at = ISAL_STOPPING_POINT_END_OF_STREAM_HEADER;
+			return ISAL_DECOMP_OK;
+		}
 	} else if (state->block_state == ISAL_CHECKSUM_CHECK) {
 		switch (state->crc_flag) {
 		case ISAL_ZLIB:
 		case ISAL_ZLIB_NO_HDR_VER:
 			ret = check_zlib_checksum(state);
 			break;
 		case ISAL_GZIP:
@@ -2308,14 +2353,31 @@
 			ret = check_gzip_checksum(state);
 			break;
 		}
 
 		return (ret > 0) ? ISAL_DECOMP_OK : ret;
 	}
 
+    /* This is used to implement the stopping point feature. In order to exist the complex loop,
+     * it simply saves off all input buffer values to feign having run out of input data.
+     * Before returning, the buffers are then restored. */
+	int read_buffer_has_been_saved = 0;
+	uint8_t *next_in = NULL;
+	uint64_t read_in = 0;
+	uint32_t avail_in = 0;
+	int32_t read_in_length = 0;
+	int16_t tmp_in_size = 0;
+	uint8_t tmp_in_buffer[ISAL_DEF_MAX_HDR_SIZE];
+
+    /* These are used to determine whether a call made progress to decide whether a stopping point
+     * request needs to be executed. */
+	int32_t old_read_in_length = 0;
+	uint32_t old_avail_in = 0;
+    int made_progress = 0;
+
 	if (state->block_state != ISAL_BLOCK_FINISH) {
 		state->total_out += state->tmp_out_valid - state->tmp_out_processed;
 		/* If space in tmp_out buffer, decompress into the tmp_out_buffer */
 		if (state->tmp_out_valid < 2 * ISAL_DEF_HIST_SIZE) {
 			/* Setup to start decoding into temp buffer */
 			state->next_out = &state->tmp_out_buffer[state->tmp_out_valid];
 			state->avail_out =
@@ -2325,31 +2387,68 @@
 			if ((int32_t) state->avail_out < 0)
 				state->avail_out = 0;
 
 			/* Decode into internal buffer until exit */
 			while (state->block_state != ISAL_BLOCK_INPUT_DONE) {
 				if (state->block_state == ISAL_BLOCK_NEW_HDR
 				    || state->block_state == ISAL_BLOCK_HDR) {
-					ret = read_header_stateful(state);
+					old_read_in_length = state->read_in_length;
+					old_avail_in = state->avail_in;
 
+					/* Will also return 0 if it hasn't read anything, it seems. */
+					ret = read_header_stateful(state);
+					made_progress = (old_read_in_length != state->read_in_length) || (old_avail_in != state->avail_in);
+					if (made_progress && (ret == 0)
+						&& (state->points_to_stop_at & ISAL_STOPPING_POINT_END_OF_BLOCK_HEADER)) {
+						state->stopped_at = ISAL_STOPPING_POINT_END_OF_BLOCK_HEADER;
+						break;
+					}
 					if (ret)
 						break;
 				}
 
+				old_read_in_length = state->read_in_length;
+				old_avail_in = state->avail_in;
+				int is_empty_literal_block = 0;
+
 				if (state->block_state == ISAL_BLOCK_TYPE0) {
+					is_empty_literal_block = state->type0_block_len == 0;
 					ret = decode_literal_block(state);
 				} else {
 					uint8_t *tmp = state->tmp_out_buffer;
 					ret = decode_huffman_code_block_stateless(state, tmp);
 				}
 
+				made_progress = is_empty_literal_block
+				                || (old_read_in_length != state->read_in_length)
+				                || (old_avail_in != state->avail_in);
+				if (made_progress && (ret == 0) && (state->points_to_stop_at & ISAL_STOPPING_POINT_END_OF_BLOCK)) {
+					state->stopped_at = ISAL_STOPPING_POINT_END_OF_BLOCK;
+					break;
+				}
+
 				if (ret)
 					break;
 			}
 
+			if (!read_buffer_has_been_saved && (state->stopped_at != ISAL_STOPPING_POINT_NONE)) {
+				read_buffer_has_been_saved = 1;
+
+				next_in        = state->next_in;
+				read_in        = state->read_in;
+				avail_in       = state->avail_in;
+				read_in_length = state->read_in_length;
+				tmp_in_size    = state->tmp_in_size;
+				memcpy(tmp_in_buffer, state->tmp_in_buffer, sizeof(tmp_in_buffer));
+
+				state->avail_in = 0;
+				state->read_in_length = 0;
+				state->tmp_in_size = 0;
+			}
+
 			/* Copy valid data from internal buffer into out_buffer */
 			if (state->write_overflow_len != 0) {
 				store_le_u32(state->next_out, state->write_overflow_lits);
 				state->next_out += state->write_overflow_len;
 				state->total_out += state->write_overflow_len;
 				state->write_overflow_lits = 0;
 				state->write_overflow_len = 0;
@@ -2386,37 +2485,90 @@
 
 		if (ret == ISAL_INVALID_LOOKBACK || ret == ISAL_INVALID_BLOCK
 		    || ret == ISAL_INVALID_SYMBOL) {
 			/* Set total_out to not count data in tmp_out_buffer */
 			state->total_out -= state->tmp_out_valid - state->tmp_out_processed;
 			if (state->crc_flag)
 				update_checksum(state, start_out, state->next_out - start_out);
-			return ret;
+			goto stop_inflate_and_return;
 		}
 
-		/* If all data from tmp_out buffer has been processed, start
-		 * decompressing into the out buffer */
-		if (state->tmp_out_processed == state->tmp_out_valid) {
+		/**
+		 * If all data from tmp_out buffer has been processed, start decompressing into the out buffer.
+		 * Check that the input has not been cleared because of a stopping point because for some reason,
+		 * this might lead to read_header_stateful being called with avail_in == 0, tmp_in_size == 0, and
+		 * readin_in_length == 0. And even so, it will overwrite bfinal and probably other members with bogus
+		 * values because it does not check for an empty input buffer for some reason.
+		 * @verbatim
+		 * [IsalInflateWrapper] call isal_inflate at offset: 5546687
+		 *   isal_inflate
+		 *     decode_huffman_code_block_stateless
+		 *     empty out inputs
+		 *     read_header_stateful 2 avail_in 0, read_in_length: 0, tmp_in_size: 0, final: 0
+		 *         returned with: avail_in 0, read_in_length: 0, tmp_in_size: 0, final: 1, ret: 1
+		 *     -> now at offset: 5551066
+		 * @endverbatim
+		 * As tested on random-dna.gz
+		 */
+		if ((state->tmp_out_processed == state->tmp_out_valid) && !read_buffer_has_been_saved) {
 			while (state->block_state != ISAL_BLOCK_INPUT_DONE) {
 				if (state->block_state == ISAL_BLOCK_NEW_HDR
 				    || state->block_state == ISAL_BLOCK_HDR) {
+					old_read_in_length = state->read_in_length;
+					old_avail_in = state->avail_in;
+
 					ret = read_header_stateful(state);
 					if (ret)
 						break;
+
+					made_progress = (old_read_in_length != state->read_in_length) || (old_avail_in != state->avail_in);
+					if (made_progress && (ret == 0)
+						&& (state->points_to_stop_at & ISAL_STOPPING_POINT_END_OF_BLOCK_HEADER)) {
+						state->stopped_at = ISAL_STOPPING_POINT_END_OF_BLOCK_HEADER;
+						break;
+					}
 				}
 
-				if (state->block_state == ISAL_BLOCK_TYPE0)
+				old_read_in_length = state->read_in_length;
+				old_avail_in = state->avail_in;
+				int is_empty_literal_block = 0;
+
+				if (state->block_state == ISAL_BLOCK_TYPE0) {
+					is_empty_literal_block = state->type0_block_len == 0;
 					ret = decode_literal_block(state);
-				else
-					ret =
-					    decode_huffman_code_block_stateless(state,
-										start_out);
+				} else {
+					ret = decode_huffman_code_block_stateless(state, start_out);
+				}
+
+				made_progress = is_empty_literal_block
+				                || (old_read_in_length != state->read_in_length)
+				                || (old_avail_in != state->avail_in);
+				if (made_progress && (ret == 0) && (state->points_to_stop_at & ISAL_STOPPING_POINT_END_OF_BLOCK)) {
+					state->stopped_at = ISAL_STOPPING_POINT_END_OF_BLOCK;
+					break;
+				}
+
 				if (ret)
 					break;
 			}
+
+			if (!read_buffer_has_been_saved && (state->stopped_at != ISAL_STOPPING_POINT_NONE)) {
+				read_buffer_has_been_saved = 1;
+
+				next_in        = state->next_in;
+				read_in        = state->read_in;
+				avail_in       = state->avail_in;
+				read_in_length = state->read_in_length;
+				tmp_in_size    = state->tmp_in_size;
+				memcpy(tmp_in_buffer, state->tmp_in_buffer, sizeof(tmp_in_buffer));
+
+				state->avail_in = 0;
+				state->read_in_length = 0;
+				state->tmp_in_size = 0;
+			}
 		}
 
 		if (state->crc_flag)
 			update_checksum(state, start_out, state->next_out - start_out);
 
 		if (state->block_state != ISAL_BLOCK_INPUT_DONE
 		    || state->copy_overflow_length + state->write_overflow_len +
@@ -2462,15 +2614,15 @@
 			state->copy_overflow_distance = 0;
 			state->copy_overflow_length = 0;
 		}
 
 		if (ret == ISAL_INVALID_LOOKBACK || ret == ISAL_INVALID_BLOCK
 		    || ret == ISAL_INVALID_SYMBOL) {
 			state->total_out -= state->tmp_out_valid - state->tmp_out_processed;
-			return ret;
+			goto stop_inflate_and_return;
 		}
 
 		if (state->block_state == ISAL_BLOCK_INPUT_DONE
 		    && state->tmp_out_valid == state->tmp_out_processed) {
 			state->block_state = ISAL_BLOCK_FINISH;
 
 			switch (state->crc_flag) {
@@ -2490,9 +2642,25 @@
 				break;
 			}
 		}
 
 		state->total_out -= state->tmp_out_valid - state->tmp_out_processed;
 	}
 
+stop_inflate_and_return:
+
+	if (read_buffer_has_been_saved) {
+		state->next_in        = next_in;
+		state->read_in        = read_in;
+		state->avail_in       = avail_in;
+		state->read_in_length = read_in_length;
+		state->tmp_in_size    = tmp_in_size;
+		memcpy(state->tmp_in_buffer, tmp_in_buffer, sizeof(tmp_in_buffer));
+	}
+
+	if ((state->stopped_at != ISAL_STOPPING_POINT_NONE) && (state->tmp_out_valid != state->tmp_out_processed)) {
+		state->tmp_out_stopped_at = state->stopped_at;
+		state->stopped_at = ISAL_STOPPING_POINT_NONE;
+	}
+
 	return (ret > 0) ? ISAL_DECOMP_OK : ret;
 }
```

### Comparing `rapidgzip-0.8.1/external/isa-l/igzip/igzip_inflate_multibinary.asm` & `rapidgzip-0.9.0/external/isa-l/igzip/igzip_inflate_multibinary.asm`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/isa-l/igzip/igzip_wrapper.h` & `rapidgzip-0.9.0/external/isa-l/igzip/igzip_wrapper.h`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/isa-l/igzip/inflate_data_structs.asm` & `rapidgzip-0.9.0/external/isa-l/igzip/inflate_data_structs.asm`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/isa-l/igzip/rfc1951_lookup.asm` & `rapidgzip-0.9.0/external/isa-l/igzip/rfc1951_lookup.asm`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/isa-l/igzip/static_inflate.h` & `rapidgzip-0.9.0/external/isa-l/igzip/static_inflate.h`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/isa-l/igzip/stdmac.asm` & `rapidgzip-0.9.0/external/isa-l/igzip/stdmac.asm`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/isa-l/include/igzip_lib.h` & `rapidgzip-0.9.0/external/isa-l/include/igzip_lib.h`

 * *Files 9% similar despite different names*

```diff
@@ -226,14 +226,25 @@
 	ISAL_GZIP_COMMENT,
 	ISAL_GZIP_HCRC,
 	ISAL_ZLIB_DICT,
 	ISAL_CHECKSUM_CHECK,
 };
 
 
+enum isal_stopping_point
+{
+    ISAL_STOPPING_POINT_NONE                 = 0,
+    ISAL_STOPPING_POINT_END_OF_STREAM_HEADER = 1U << 0U,
+    ISAL_STOPPING_POINT_END_OF_STREAM        = 1U << 1U,  // after gzip footer has been read
+    ISAL_STOPPING_POINT_END_OF_BLOCK_HEADER  = 1U << 2U,
+    ISAL_STOPPING_POINT_END_OF_BLOCK         = 1U << 3U,
+    ISAL_STOPPING_POINT_ALL                  = 0xFFFFFFFFU,
+};
+
+
 /* Inflate Flags */
 #define ISAL_DEFLATE	0	/* Default */
 #define ISAL_GZIP	1
 #define ISAL_GZIP_NO_HDR	2
 #define ISAL_ZLIB	3
 #define ISAL_ZLIB_NO_HDR	4
 #define ISAL_ZLIB_NO_HDR_VER	5
@@ -507,14 +518,20 @@
 	int32_t copy_overflow_distance;	//!< Lookback distance when outbuffer overflow occurred
 	int16_t wrapper_flag;
 	int16_t tmp_in_size;	//!< Number of bytes in tmp_in_buffer
 	int32_t tmp_out_valid;	//!< Number of bytes in tmp_out_buffer
 	int32_t tmp_out_processed;	//!< Number of bytes processed in tmp_out_buffer
 	uint8_t tmp_in_buffer[ISAL_DEF_MAX_HDR_SIZE];	//!< Temporary buffer containing data from the input stream
 	uint8_t tmp_out_buffer[2 * ISAL_DEF_HIST_SIZE + ISAL_LOOK_AHEAD]; 	//!< Temporary buffer containing data from the output stream
+
+	enum isal_stopping_point points_to_stop_at;
+	enum isal_stopping_point stopped_at;
+	enum isal_stopping_point tmp_out_stopped_at;
+	/* Only has a meaningful value when stopped_at == ISAL_STOPPING_POINT_END_OF_BLOCK_HEADER. */
+	uint8_t btype;
 };
 
 /******************************************************************************/
 /* Compression functions */
 /******************************************************************************/
 /**
  * @brief Set gzip header default values
@@ -679,11 +696,75 @@
  * @param buf: buffer to calculate checksum on
  * @param len: buffer length in bytes
  *
  * @returns 32-bit Adler-32 checksum
  */
 uint32_t isal_adler32(uint32_t init, const unsigned char *buf, uint64_t len);
 
+
+
+/**
+ * @brief Structure used to store huffman codes
+ */
+struct huff_code {
+	union {
+		struct {
+#if __BYTE_ORDER__ == __ORDER_LITTLE_ENDIAN__
+			uint32_t code_and_extra:24;
+			uint32_t length2:8;
+#else
+			uint32_t length2:8;
+			uint32_t code_and_extra:24;
+#endif
+		};
+
+		struct {
+#if __BYTE_ORDER__ == __ORDER_LITTLE_ENDIAN__
+			uint16_t code;
+			uint8_t extra_bit_count;
+			uint8_t length;
+#else
+			uint8_t length;
+			uint8_t extra_bit_count;
+			uint16_t code;
+#endif
+		};
+
+		uint32_t code_and_length;
+	};
+};
+
+
+/**
+ * @param[in,out] lit_len_huff Array of huff_code. huff_code::length is used to initialize
+ *                huff_code::code and huff_code::extra_bits.
+ * @param[in] table_length
+ * @param[in,out] count
+ * @param[in,out] expand_count
+ * @param[out] code_list
+ * @return ISAL_DECOMP_OK or ISAL_INVALID_BLOCK.
+ */
+int set_and_expand_lit_len_huffcode(struct huff_code const * const lit_len_huff,
+						  uint32_t const table_length,
+						  uint16_t * const count,
+						  uint16_t * const expand_count,
+						  uint32_t * const code_list);
+
+/**
+ * @param table_length unused
+ */
+void make_inflate_huff_code_lit_len(struct inflate_huff_code_large * const result,
+					   struct huff_code * const huff_code_table,
+					   uint32_t const table_length, uint16_t const * const count_total,
+					   uint32_t * const code_list, uint32_t const multisym);
+
+int set_codes(struct huff_code * huff_code_table, int const table_length, uint16_t const * const count);
+
+void make_inflate_huff_code_dist(struct inflate_huff_code_small * const result,
+                                 struct huff_code * const huff_code_table,
+                                 uint32_t const table_length,
+                                 uint16_t const * const count,
+                                 uint32_t const max_symbol);
 #ifdef __cplusplus
 }
 #endif
 #endif	/* ifndef _IGZIP_H */
```

### Comparing `rapidgzip-0.8.1/external/isa-l/include/multibinary.asm` & `rapidgzip-0.9.0/external/isa-l/include/multibinary.asm`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/isa-l/include/reg_sizes.asm` & `rapidgzip-0.9.0/external/isa-l/include/reg_sizes.asm`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/isa-l/include/unaligned.h` & `rapidgzip-0.9.0/external/isa-l/include/unaligned.h`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/rpmalloc/LICENSE` & `rapidgzip-0.9.0/external/rpmalloc/LICENSE`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/rpmalloc/rpmalloc/rpmalloc.c` & `rapidgzip-0.9.0/external/rpmalloc/rpmalloc/rpmalloc.c`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/rpmalloc/rpmalloc/rpmalloc.h` & `rapidgzip-0.9.0/external/rpmalloc/rpmalloc/rpmalloc.h`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/rpmalloc/rpmalloc/rpnew.h` & `rapidgzip-0.9.0/external/rpmalloc/rpmalloc/rpnew.h`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/zlib/LICENSE` & `rapidgzip-0.9.0/external/zlib/LICENSE`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/zlib/adler32.c` & `rapidgzip-0.9.0/external/zlib/adler32.c`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/zlib/crc32.c` & `rapidgzip-0.9.0/external/zlib/crc32.c`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/zlib/crc32.h` & `rapidgzip-0.9.0/external/zlib/crc32.h`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/zlib/gzguts.h` & `rapidgzip-0.9.0/external/zlib/gzguts.h`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/zlib/inffast.c` & `rapidgzip-0.9.0/external/zlib/inffast.c`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/zlib/inffixed.h` & `rapidgzip-0.9.0/external/zlib/inffixed.h`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/zlib/inflate.c` & `rapidgzip-0.9.0/external/zlib/inflate.c`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/zlib/inflate.h` & `rapidgzip-0.9.0/external/zlib/inflate.h`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/zlib/inftrees.c` & `rapidgzip-0.9.0/external/zlib/inftrees.c`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/zlib/inftrees.h` & `rapidgzip-0.9.0/external/zlib/inftrees.h`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/zlib/zconf.h` & `rapidgzip-0.9.0/external/zlib/zconf.h`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/zlib/zlib.h` & `rapidgzip-0.9.0/external/zlib/zlib.h`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/zlib/zutil.c` & `rapidgzip-0.9.0/external/zlib/zutil.c`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/external/zlib/zutil.h` & `rapidgzip-0.9.0/external/zlib/zutil.h`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/nasm_extension/LICENSE` & `rapidgzip-0.9.0/nasm_extension/LICENSE`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/nasm_extension/nasmcompiler.py` & `rapidgzip-0.9.0/nasm_extension/nasmcompiler.py`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/nasm_extension/winnasmcompiler.py` & `rapidgzip-0.9.0/nasm_extension/winnasmcompiler.py`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/rapidgzip/ChunkData.hpp` & `rapidgzip-0.9.0/rapidgzip/ChunkData.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -50,14 +50,38 @@
         {
             return ( encodedOffset == other.encodedOffset ) && ( decodedOffset == other.decodedOffset );
         }
     };
 
     struct Footer
     {
+        /**
+         * The blockBoundary is currently (2023-08-26) unused. It is intended to aid block splitting in order
+         * to split after a gzip footer because then the window is known to be empty, which would save space
+         * and time.
+         * The uncompressed block boundary offset is unambiguous.
+         * The compressed block boundary is more ambiguous. There are three possibilities:
+         *  - The end of the preceding deflate block. The footer start is then the next byte-aligned boundary.
+         *  - The byte-aligned footer start.
+         *  - The byte-aligned footer end, which is the file end or the next gzip stream start.
+         *    For gzip, it is exactly FOOTER_SIZE bytes after the footer start.
+         * Thoughts about the choice:
+         *  - The offset after the footer is more relevant to the intended block splitting improvement.
+         *  - The previous deflate block end contains the most information because the other two possible
+         *    choices can be derived from it by rounding up and adding FOOTER_SIZE. The inverse is not true.
+         *  - The previous block end might be the most stable choice because stopping at that boundary is
+         *    already a requirement for using ISA-l without an exact untilOffset. Stopping at the footer end
+         *    might not work perfectly and might already have read some of the next block.
+         * Currently, the unit tests, test that all possibilities to derive the footer offsets: GzipReader, decodeBlock,
+         * decodeBlockWithInflateWrapper with ISA-L or zlib, return the same value.
+         * That value is currently the footer end because it seemed easier to implement. This might be subjecft to
+         * change until it is actually used for something (e.g. smarter block splitting).
+         * The most complicated to implement but least ambiguous solution would be to add all three boundaries to
+         * this struct.
+         */
         BlockBoundary blockBoundary;
         gzip::Footer gzipFooter;
     };
 
     struct Subblock
     {
         size_t encodedOffset{ 0 };
@@ -105,17 +129,17 @@
             /* Markers should only appear up to the first gzip footer because otherwise a new gzip stream
              * would have started. A new gzip stream must not contain markers because there are no unresolvable
              * back-references! Because of this, it is safe to only update the first CRC32.
              * Beware that we do not only have to compute the CRC32 of markers but also for data that has been
              * been converted from dataWithMarkers inside DecodedData::cleanUnmarkedData. */
             const auto toProcessSize = BaseType::dataSize() - alreadyProcessedSize;
             CRC32Calculator crc32;
-            for ( size_t i = 0; ( i < data.size() ) && ( crc32.streamSize() < toProcessSize ); ++i ) {
-                crc32.update( data[i].data(),
-                              std::min<uint64_t>( toProcessSize - crc32.streamSize(), data[i].size() ) );
+            for ( auto it = DecodedData::Iterator( *this, 0, toProcessSize ); static_cast<bool>( it ); ++it ) {
+                const auto [buffer, size] = *it;
+                crc32.update( buffer, size );
             }
             crc32s.front().prepend( crc32 );
         }
     }
 
     [[nodiscard]] bool
     matchesEncodedOffset( size_t offset ) const noexcept
@@ -140,42 +164,41 @@
     {
         const auto oldMarkerSize = BaseType::dataWithMarkersSize();
         cleanUnmarkedData();
         const auto toProcessSize = oldMarkerSize - BaseType::dataWithMarkersSize();
         if ( toProcessSize > 0 ) {
             CRC32Calculator crc32;
             /* Iterate over contiguous chunks of memory. */
-            for ( size_t i = 0; ( i < data.size() ) && ( crc32.streamSize() < toProcessSize ); ++i ) {
-                crc32.update( data[i].data(),
-                              std::min<uint64_t>( toProcessSize - crc32.streamSize(), data[i].size() ) );
+            for ( auto it = DecodedData::Iterator( *this, 0, toProcessSize ); static_cast<bool>( it ); ++it ) {
+                const auto [buffer, size] = *it;
+                crc32.update( buffer, size );
             }
             /* Note that the data with markers ought not cross footer boundaries because after a footer,
              * a new gzip stream begins, which should be known to not contain any unresolvable backreferences.
              * That's why we can simply merge the CRC32 for the cleaned data with the first CRC32. */
             crc32s.front().prepend( crc32 );
         }
 
         encodedSizeInBits = blockEndOffsetInBits - encodedOffsetInBits;
         decodedSizeInBytes = BaseType::size();
     }
 
-    [[nodiscard]] constexpr size_t
-    size() const noexcept = delete;
-
-    [[nodiscard]] constexpr size_t
-    dataSize() const noexcept = delete;
-
     /**
      * Appends a deflate block boundary.
      */
     void
     appendDeflateBlockBoundary( const size_t encodedOffset,
                                 const size_t decodedOffset )
     {
-        blockBoundaries.emplace_back( BlockBoundary{ encodedOffset, decodedOffset } );
+        if ( blockBoundaries.empty()
+             || ( blockBoundaries.back().encodedOffset != encodedOffset )
+             || ( blockBoundaries.back().decodedOffset != decodedOffset ) )
+        {
+            blockBoundaries.emplace_back( BlockBoundary{ encodedOffset, decodedOffset } );
+        }
     }
 
     /**
      * Appends gzip footer information at the given offset.
      */
     void
     appendFooter( const size_t encodedOffset,
@@ -214,16 +237,19 @@
      * during first-pass decompression. */
     std::vector<BlockBoundary> blockBoundaries;
     std::vector<Footer> footers;
     /* There will be ( footers.size() + 1 ) CRC32 calculators. */
     std::vector<CRC32Calculator> crc32s{ std::vector<CRC32Calculator>( 1 ) };
 
     /* Benchmark results */
+    size_t falsePositiveCount{ 0 };
     double blockFinderDuration{ 0 };
     double decodeDuration{ 0 };
+    double decodeDurationInflateWrapper{ 0 };
+    double decodeDurationIsal{ 0 };
     double appendDuration{ 0 };
 
     bool stoppedPreemptively{ false };
 };
 
 
 inline void
```

### Comparing `rapidgzip-0.8.1/rapidgzip/DecodedData.hpp` & `rapidgzip-0.9.0/rapidgzip/DecodedData.hpp`

 * *Files 16% similar despite different names*

```diff
@@ -28,22 +28,28 @@
 {
 public:
     using WindowView = VectorView<uint8_t>;
 
     class Iterator
     {
     public:
+        /**
+         * This iterator provides a view of the decoded data as requested via an offset and a length.
+         * If no relative offset or length is specified it will create a view of all of the data.
+         * The interface will return subviews as pointer-length pairs because the data might not be
+         * in one contiguous chunk internally.
+         */
         explicit
         Iterator( const DecodedData& decodedData,
-                  const size_t       offset = 0,
+                  const size_t       offsetInChunk = 0,
                   const size_t       size = std::numeric_limits<size_t>::max() ) :
             m_data( decodedData ),
             m_size( size )
         {
-            m_offsetInChunk = offset;
+            m_offsetInChunk = offsetInChunk;
             for ( m_currentChunk = 0; m_currentChunk < m_data.data.size(); ++m_currentChunk ) {
                 const auto& chunk = m_data.data[m_currentChunk];
                 if ( ( m_offsetInChunk < chunk.size() ) && !chunk.empty() ) {
                     m_sizeInChunk = std::min( chunk.size() - m_offsetInChunk, m_size );
                     break;
                 }
                 m_offsetInChunk -= chunk.size();
@@ -98,16 +104,17 @@
     };
 
 public:
     void
     append( DecodedVector&& toAppend )
     {
         if ( !toAppend.empty() ) {
-            data.emplace_back( std::move( toAppend ) );
-            data.back().shrink_to_fit();
+            dataBuffers.emplace_back( std::move( toAppend ) );
+            dataBuffers.back().shrink_to_fit();
+            data.emplace_back( VectorView<uint8_t>( dataBuffers.back().data(), dataBuffers.back().size() ) );
         }
     }
 
     void
     append( DecodedDataView const& buffers );
 
     [[nodiscard]] size_t
@@ -144,14 +151,17 @@
      */
     [[nodiscard]] bool
     containsMarkers() const noexcept
     {
         return !dataWithMarkers.empty();
     }
 
+    [[nodiscard]] size_t
+    countMarkerSymbols() const;
+
     /**
      * Replaces all 16-bit wide marker symbols by looking up the referenced 8-bit symbols in @p window.
      * @note Probably should not be called internally because it is allowed to be shadowed by a child class method.
      */
     void
     applyWindow( WindowView const& window );
 
@@ -174,69 +184,129 @@
     [[nodiscard]] DecodedVector
     getWindowAt( WindowView const& previousWindow,
                  size_t            skipBytes ) const;
 
     void
     shrinkToFit()
     {
-        for ( auto& container : data ) {
+        for ( auto& container : dataBuffers ) {
             container.shrink_to_fit();
         }
         for ( auto& container : dataWithMarkers ) {
             container.shrink_to_fit();
         }
     }
 
     /**
      * Check decoded blocks that account for possible markers whether they actually contain markers and, if not so,
      * convert and move them to actual decoded data.
      */
     void
     cleanUnmarkedData();
 
+#ifdef TEST_DECODED_DATA
+    [[nodiscard]] const std::vector<MarkerVector>&
+    getDataWithMarkers() const noexcept
+    {
+        return dataWithMarkers;
+    }
+
+    [[nodiscard]] const std::vector<VectorView<uint8_t> >&
+    getData() const noexcept
+    {
+        return data;
+    }
+#endif
+
 public:
     size_t encodedOffsetInBits{ std::numeric_limits<size_t>::max() };
     size_t encodedSizeInBits{ 0 };
 
+private:
     /**
      * Use vectors of vectors to avoid reallocations. The order of this data is:
      * - @ref dataWithMarkers (front to back)
      * - @ref data (front to back)
      * This order is fixed because there should be no reason for markers after we got enough data without markers!
      * There is no append( DecodedData ) method because this property might not be retained after using
      * @ref cleanUnmarkedData.
      */
     std::vector<MarkerVector> dataWithMarkers;
-    std::vector<DecodedVector> data;
+    std::vector<MarkerVector> reusedDataBuffers;
+    std::vector<DecodedVector> dataBuffers;
+    std::vector<VectorView<uint8_t> > data;
 };
 
 
 inline void
 DecodedData::append( DecodedDataView const& buffers )
 {
+    static constexpr auto ALLOCATION_CHUNK_SIZE = 128_Ki;
+
+    const auto& appendToEquallySizedChunks =
+        [] ( auto&       targetChunks,
+             const auto& buffer )
+        {
+            constexpr auto ALLOCATION_ELEMENT_COUNT = ALLOCATION_CHUNK_SIZE / sizeof( targetChunks[0][0] );
+
+            if ( targetChunks.empty() ) {
+                targetChunks.emplace_back().reserve( ALLOCATION_ELEMENT_COUNT );
+            }
+
+            for ( size_t nCopied = 0; nCopied < buffer.size(); ) {
+                auto& copyTarget = targetChunks.back();
+                const auto nFreeElements = copyTarget.capacity() - copyTarget.size();
+                if ( nFreeElements == 0 ) {
+                    targetChunks.emplace_back().reserve( ALLOCATION_ELEMENT_COUNT );
+                    continue;
+                }
+
+                const auto nToCopy = std::min( nFreeElements, buffer.size() - nCopied );
+                copyTarget.insert( copyTarget.end(), buffer.begin() + nCopied, buffer.begin() + nCopied + nToCopy );
+                nCopied += nToCopy;
+            }
+        };
+
     if ( buffers.dataWithMarkersSize() > 0 ) {
         if ( !data.empty() ) {
             throw std::invalid_argument( "It is not allowed to append data with markers when fully decoded data "
                                          "has already been appended because the ordering will be wrong!" );
         }
 
-        auto& copied = dataWithMarkers.emplace_back();
-        copied.reserve( buffers.dataWithMarkersSize() );
         for ( const auto& buffer : buffers.dataWithMarkers ) {
-            copied.insert( copied.end(), buffer.begin(), buffer.end() );
+            appendToEquallySizedChunks( dataWithMarkers, buffer );
         }
     }
 
+    /* Add complexity to the already complex dataBuffers + data (views) structure by trying to force the
+     * dataBuffer chunks to 128 KiB makes no sense because this method for appending views is only called
+     * when decompressing with rapidgzip and as soon as we have 32 KiB of symbols, the decompression should
+     * delegate to ISA-L except in pathological edge cases such as very large deflate blocks. */
     if ( buffers.dataSize() > 0 ) {
-        auto& copied = data.emplace_back();
+        auto& copied = dataBuffers.emplace_back();
         copied.reserve( buffers.dataSize() );
         for ( const auto& buffer : buffers.data ) {
             copied.insert( copied.end(), buffer.begin(), buffer.end() );
         }
+        data.emplace_back( VectorView<uint8_t>( copied.data(), copied.size() ) );
+    }
+}
+
+
+[[nodiscard]] inline size_t
+DecodedData::countMarkerSymbols() const
+{
+    size_t result{ 0 };
+    for ( auto& chunk : dataWithMarkers ) {
+        result += std::accumulate( chunk.begin(), chunk.end(), size_t( 0 ),
+                                   [] ( const size_t sum, const uint16_t symbol ) {
+            return sum + ( ( symbol & 0xFF00U ) == 0 ? 0 : 1 );
+        } );
     }
+    return result;
 }
 
 
 inline void
 DecodedData::applyWindow( WindowView const& window )
 {
     const auto markerCount = dataWithMarkersSize();
@@ -252,64 +322,101 @@
             {
                 std::array<uint8_t, 64_Ki> result{};
                 std::iota( result.begin(), result.begin() + 256, 0 );
                 std::copy( window.begin(), window.end(), result.begin() + MAX_WINDOW_SIZE );
                 return result;
             }();
 
-        DecodedVector downcasted( markerCount );
-        size_t offset{ 0 };
         for ( auto& chunk : dataWithMarkers ) {
-            std::transform( chunk.begin(), chunk.end(), downcasted.begin() + offset,
-                            [&fullWindow] ( const auto value ) constexpr noexcept { return fullWindow[value]; } );
-            offset += chunk.size();
+            auto* const target = reinterpret_cast<uint8_t*>( chunk.data() );
+            /* Do not use std::transform because it allows out-of-order execution!
+             * std::transform might be ~3% faster for FASTQ files btu it is hard to measure as timings seem
+             * to vary a lot. Still, we need to be correct before being fast, but maybe something can be
+             * done with inline Assembler or the intermediary "compressed" marker format might also help.
+             * Note that these 3% shouldn't matter because we already are quite faster than before:
+             *     rapidgzip-v0.9.0 : 2706.3 <= 2862.5 +- 2.3 <= 2979.9
+             *     rapidgzip-v0.8.1 : 1988.2 <= 2067.8 +- 1.4 <= 2139.8
+             */
+            for ( size_t i = 0; i < chunk.size(); ++i ) {
+                target[i] = fullWindow[chunk[i]];
+            }
+        }
+    } else {
+        /* For maximum size windows, we can skip one check because even UINT16_MAX is valid. */
+        static_assert( std::numeric_limits<uint16_t>::max() - MAX_WINDOW_SIZE + 1U == MAX_WINDOW_SIZE );
+        if ( window.size() >= MAX_WINDOW_SIZE ) {
+            const MapMarkers<true> mapMarkers( window );
+            for ( auto& chunk : dataWithMarkers ) {
+                /* Do not use std::transform because it allows out-of-order execution and if a later i
+                 * is computed first, it might overwrite values that are need for earlier i's because
+                 * we are transforming in-place into a vector with smaller element size! */
+                auto* const target = reinterpret_cast<uint8_t*>( chunk.data() );
+                for ( size_t i = 0; i < chunk.size(); ++i ) {
+                    target[i] = mapMarkers( chunk[i] );
+                }
+            }
+        } else {
+            const MapMarkers<false> mapMarkers( window );
+            for ( auto& chunk : dataWithMarkers ) {
+                auto* const target = reinterpret_cast<uint8_t*>( chunk.data() );
+                /* Do not use std::transform because it allows out-of-order execution! */
+                for ( size_t i = 0; i < chunk.size(); ++i ) {
+                    target[i] = mapMarkers( chunk[i] );
+                }
+            }
         }
-
-        data.insert( data.begin(), std::move( downcasted ) );
-        dataWithMarkers.clear();
-        return;
     }
 
-    DecodedVector downcasted( markerCount );
-    size_t offset{ 0 };
+    if ( !reusedDataBuffers.empty() ) {
+        throw std::logic_error( "It seems like data already was replaced but we still got markers!" );
+    }
+    std::swap( reusedDataBuffers, dataWithMarkers );
 
-    /* For maximum size windows, we can skip one check because even UINT16_MAX is valid. */
-    static_assert( std::numeric_limits<uint16_t>::max() - MAX_WINDOW_SIZE + 1U == MAX_WINDOW_SIZE );
-    if ( window.size() >= MAX_WINDOW_SIZE ) {
-        const MapMarkers<true> mapMarkers( window );
-        for ( auto& chunk : dataWithMarkers ) {
-            std::transform( chunk.begin(), chunk.end(), downcasted.begin() + offset, mapMarkers );
-            offset += chunk.size();
-        }
-    } else {
-        const MapMarkers<false> mapMarkers( window );
-        for ( auto& chunk : dataWithMarkers ) {
-            std::transform( chunk.begin(), chunk.end(), chunk.begin(), mapMarkers );
-            std::copy( chunk.begin(), chunk.end(), reinterpret_cast<std::uint8_t*>( downcasted.data() + offset ) );
-            offset += chunk.size();
-        }
+    /* Prepend a VectorView to @ref data for each reused chunk buffer. */
+    std::vector<VectorView<uint8_t> > dataViews;
+    dataViews.reserve( reusedDataBuffers.size() + data.size() );
+    for ( auto& chunk : reusedDataBuffers ) {
+        /**
+         * @todo Note that this leaves half of the chunk space unused because the number of elements stays
+         *       the same while the element type size is halved. I assume that shrink_to_fit would be
+         *       expensive. Therefore, it would be nice to simple join neihgboring chunks to fill all available
+         *       space and free the rest of the chunks. But, depending on the individual chunk sizes,
+         *       this can become complex.
+         * @note It is kind of an exception that this works! Because reinterpret_cast with target types
+         *       (unsigned) char* are excepted from the strict aliasing rules. For other types,
+         *       it would be undefined behavior, e.g., trying to reuse a vector of uint32_t as uint16_t!
+         * @see https://en.cppreference.com/w/cpp/language/reinterpret_cast#Type_aliasing
+         */
+        dataViews.emplace_back( VectorView<uint8_t>( reinterpret_cast<uint8_t*>( chunk.data() ), chunk.size() ) );
     }
+    std::move( data.begin(), data.end(), std::back_inserter( dataViews ) );
+    std::swap( data, dataViews );
 
-    data.insert( data.begin(), std::move( downcasted ) );
     dataWithMarkers.clear();
 }
 
 
+/**
+ * @todo Shouldn't this be eqivalent to getWindowAt( previewWindow, size() )?
+ *       Probably can be replaced to reduce code complexity. getWindowAt is more complex and generic and
+ *       was introduced for block splitting while this method exists since the beginning.
+ */
 [[nodiscard]] inline DecodedVector
 DecodedData::getLastWindow( WindowView const& previousWindow ) const
 {
     DecodedVector window( MAX_WINDOW_SIZE, 0 );
     size_t nBytesWritten{ 0 };
 
     /* Fill the result from the back with data from our buffer. */
+    /** @todo use iterator. */
     for ( auto chunk = data.rbegin(); ( chunk != data.rend() ) && ( nBytesWritten < window.size() ); ++chunk ) {
-        for ( auto symbol = chunk->rbegin(); ( symbol != chunk->rend() ) && ( nBytesWritten < window.size() );
-              ++symbol, ++nBytesWritten )
+        for ( size_t i = 0; ( i < chunk->size() ) && ( nBytesWritten < window.size() ); ++i, ++nBytesWritten )
         {
-            window[window.size() - 1 - nBytesWritten] = *symbol;
+            const auto symbol = ( *chunk )[chunk->size() - 1 - i];
+            window[window.size() - 1 - nBytesWritten] = symbol;
         }
     }
 
     /* Fill the result from the back with data from our unresolved buffers. */
     const auto copyFromDataWithMarkers =
         [this, &window, &nBytesWritten] ( const auto& mapMarker )
         {
@@ -440,15 +547,16 @@
         const auto& toDowncast = dataWithMarkers.back();
         /* Try to not only downcast whole chunks of data but also as many bytes as possible for the last chunk. */
         const auto marker = std::find_if(
             toDowncast.rbegin(), toDowncast.rend(),
             [] ( auto value ) { return value > std::numeric_limits<uint8_t>::max(); } );
 
         const auto sizeWithoutMarkers = static_cast<size_t>( std::distance( toDowncast.rbegin(), marker ) );
-        auto downcasted = data.emplace( data.begin(), sizeWithoutMarkers );
+        auto downcasted = dataBuffers.emplace( dataBuffers.begin(), sizeWithoutMarkers );
+        data.insert( data.begin(), VectorView<uint8_t>( downcasted->data(), downcasted->size() ) );
         std::transform( marker.base(), toDowncast.end(), downcasted->begin(),
                         [] ( auto symbol ) { return static_cast<uint8_t>( symbol ); } );
 
         if ( marker == toDowncast.rend() ) {
             dataWithMarkers.pop_back();
         } else {
             dataWithMarkers.back().resize( dataWithMarkers.back().size() - sizeWithoutMarkers );
```

### Comparing `rapidgzip-0.8.1/rapidgzip/DecodedDataView.hpp` & `rapidgzip-0.9.0/rapidgzip/DecodedDataView.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/rapidgzip/Error.hpp` & `rapidgzip-0.9.0/rapidgzip/Error.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
     EOF_ZERO_STRING             = 0x10,
     EOF_UNCOMPRESSED            = 0x11,
 
     EXCEEDED_CL_LIMIT           = 0x20,
     EXCEEDED_SYMBOL_RANGE       = 0x21,
     EXCEEDED_LITERAL_RANGE      = 0x22,
+    EXCEEDED_DISTANCE_RANGE     = 0x23,
     EXCEEDED_WINDOW_RANGE       = 0x24,
 
     EMPTY_INPUT                 = 0x30,
 
     INVALID_HUFFMAN_CODE        = 0x40,
     NON_ZERO_PADDING            = 0x41,
     LENGTH_CHECKSUM_MISMATCH    = 0x42,
@@ -63,14 +64,16 @@
         return "Assumed padding seems to contain some kind of data!";
     case Error::LENGTH_CHECKSUM_MISMATCH:
         return "Integrity check for length of uncompressed deflate block failed!";
     case Error::INVALID_COMPRESSION:
         return "Invalid block compression type!";
     case Error::EXCEEDED_LITERAL_RANGE:
         return "Invalid number of literal/length codes!";
+    case Error::EXCEEDED_DISTANCE_RANGE:
+        return "Invalid number of distance codes!";
     case Error::INVALID_CL_BACKREFERENCE:
         return "Cannot copy last length because this is the first one!";
     case Error::INVALID_BACKREFERENCE:
         return "Backreferenced data does not exist!";
     case Error::INVALID_GZIP_HEADER:
         return "Invalid gzip magic bytes!";
     case Error::INCOMPLETE_GZIP_HEADER:
```

### Comparing `rapidgzip-0.8.1/rapidgzip/GzipBlockFinder.hpp` & `rapidgzip-0.9.0/rapidgzip/GzipBlockFinder.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/rapidgzip/GzipChunkFetcher.hpp` & `rapidgzip-0.9.0/rapidgzip/GzipChunkFetcher.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -53,28 +53,28 @@
         DecompressionError( message )
     {}
 };
 
 
 template<typename T_FetchingStrategy,
          typename T_ChunkData = ChunkData,
-         bool     ENABLE_STATISTICS = false,
-         bool     SHOW_PROFILE = false>
+         bool     ENABLE_STATISTICS = false>
 class GzipChunkFetcher :
-    public BlockFetcher<GzipBlockFinder, T_ChunkData, T_FetchingStrategy, ENABLE_STATISTICS, SHOW_PROFILE>
+    public BlockFetcher<GzipBlockFinder, T_ChunkData, T_FetchingStrategy, ENABLE_STATISTICS>
 {
 public:
     using FetchingStrategy = T_FetchingStrategy;
     using ChunkData = T_ChunkData;
-    using BaseType = BlockFetcher<GzipBlockFinder, ChunkData, FetchingStrategy, ENABLE_STATISTICS, SHOW_PROFILE>;
+    using BaseType = BlockFetcher<GzipBlockFinder, ChunkData, FetchingStrategy, ENABLE_STATISTICS>;
     using BitReader = rapidgzip::BitReader;
     using WindowView = VectorView<uint8_t>;
     using BlockFinder = typename BaseType::BlockFinder;
 
     static constexpr bool REPLACE_MARKERS_IN_PARALLEL = true;
+    static constexpr bool ENABLE_REAL_MARKER_COUNT = false;  // Adds 25% overhead for FASTQ files (worst case)
 
 public:
     GzipChunkFetcher( BitReader                    bitReader,
                       std::shared_ptr<BlockFinder> blockFinder,
                       std::shared_ptr<BlockMap>    blockMap,
                       std::shared_ptr<WindowMap>   windowMap,
                       size_t                       parallelization ) :
@@ -103,23 +103,34 @@
 
     virtual
     ~GzipChunkFetcher()
     {
         m_cancelThreads = true;
         this->stopThreadPool();
 
-        if constexpr ( SHOW_PROFILE ) {
+        if ( BaseType::m_showProfileOnDestruction ) {
             std::stringstream out;
             out << "[GzipChunkFetcher::GzipChunkFetcher] First block access statistics:\n";
-            out << "    Time spent in block finder              : " << m_blockFinderTime << " s\n";
-            out << "    Time spent decoding                     : " << m_decodeTime << " s\n";
-            out << "    Time spent allocating and copying       : " << m_appendTime << " s\n";
-            out << "    Time spent applying the last window     : " << m_applyWindowTime << " s\n";
-            out << "    Replaced marker bytes                   : " << formatBytes( m_markerCount ) << "\n";
-            out << "    Chunks exceeding max. compression ratio : " << m_preemptiveStopCount << "\n";
+            out << "    Number of false positives                : " << m_falsePositiveCount << "\n";
+            out << "    Time spent in block finder               : " << m_blockFinderTime << " s\n";
+            out << "    Time spent decoding with custom inflate  : " << m_decodeTime << " s\n";
+            out << "    Time spent decoding with inflate wrapper : " << m_decodeTimeInflateWrapper << " s\n";
+            out << "    Time spent decoding with ISA-L           : " << m_decodeTimeIsal << " s\n";
+            out << "    Time spent allocating and copying        : " << m_appendTime << " s\n";
+            out << "    Time spent applying the last window      : " << m_applyWindowTime << " s\n";
+            out << "    Replaced marker buffers                  : " << formatBytes( m_markerCount ) << "\n";
+            if constexpr ( ENABLE_REAL_MARKER_COUNT ) {
+                out << "    Actual marker count                      : " << formatBytes( m_realMarkerCount );
+                if ( m_markerCount > 0 ) {
+                    out << " (" << static_cast<double>( m_realMarkerCount ) / static_cast<double>( m_markerCount ) * 100
+                        << " %)";
+                }
+                out << "\n";
+            }
+            out << "    Chunks exceeding max. compression ratio  : " << m_preemptiveStopCount << "\n";
             std::cerr << std::move( out ).str();
         }
     }
 
     /**
      * @param offset The current offset in the decoded data. (Does not have to be a block offset!)
      * Does not return the whole BlockInfo object because it might not fit the chunk from the cache
@@ -203,18 +214,21 @@
                     if ( boundary.encodedOffset != chunkOffset ) {
                         m_unsplitBlocks.emplace( boundary.encodedOffset, lookupKey );
                     }
                 }
             }
             m_nextUnprocessedBlockIndex += subblocks.size();
 
-            if constexpr ( ENABLE_STATISTICS || SHOW_PROFILE ) {
+            if constexpr ( ENABLE_STATISTICS ) {
                 std::scoped_lock lock( m_statisticsMutex );
+                m_falsePositiveCount += chunkData->falsePositiveCount;
                 m_blockFinderTime += chunkData->blockFinderDuration;
                 m_decodeTime += chunkData->decodeDuration;
+                m_decodeTimeInflateWrapper += chunkData->decodeDurationInflateWrapper;
+                m_decodeTimeIsal += chunkData->decodeDurationIsal;
                 m_appendTime += chunkData->appendDuration;
             }
 
             if ( blockOffsetAfterNext >= m_bitReader.size() ) {
                 m_blockMap->finalize();
                 m_blockFinder->finalize();
             }
@@ -268,15 +282,15 @@
     void
     setMaxDecompressedChunkSize( size_t maxDecompressedChunkSize )
     {
         m_maxDecompressedChunkSize = maxDecompressedChunkSize;
     }
 
     [[nodiscard]] size_t
-    maxDecompressedChunkSize( size_t maxDecompressedChunkSize ) const
+    maxDecompressedChunkSize() const
     {
         return m_maxDecompressedChunkSize;
     }
 
 private:
     void
     waitForReplacedMarkers( const std::shared_ptr<ChunkData>& chunkData,
@@ -374,17 +388,51 @@
      * Must be thread-safe because it is submitted to the thread pool.
      */
     void
     replaceMarkers( const std::shared_ptr<ChunkData>& chunkData,
                     const WindowView                  previousWindow )
     {
         [[maybe_unused]] const auto markerCount = chunkData->dataWithMarkersSize();
+        /* This is expensive! It adds 20-30% overhead for the FASTQ file! Therefore disable it.
+         * The result for this statistics for:
+         *     SRR22403185_2.fastq.gz:
+         *         Replaced marker buffers : 329 MiB 550 KiB 191 B
+         *         Actual marker count     : 46 MiB 705 KiB 331 B (14.168 %)
+         *     silesia.tar.gz
+         *         Replaced marker buffers : 70 MiB 575 KiB 654 B
+         *         Actual marker count     : 21 MiB 523 KiB 94 B (30.4849 %)
+         *     4GiB-base64.gz
+         *         Replaced marker buffers : 21 MiB 582 KiB 252 B
+         *         Actual marker count     : 158 KiB 538 B (0.717756 %)
+         *     CTU-13-Dataset.tar.gz
+         *         Replaced marker buffers : 22 GiB 273 MiB 34 KiB 574 B
+         *         Actual marker count     : 2 GiB 687 MiB 490 KiB 119 B (11.9972 %)
+         *
+         * -> An alternative format that uses a mix of 8-bit and 16-bit and maybe a separate 1-bit buffer
+         *    to store which byte is which, would reduce memory usage, and therefore also allocation
+         *    overhead by 80%! Or maybe run-time encode it a la: <n 8-bit values> <8-bit value> ... <m 16-bit values>
+         *    This would hopefully speed up window applying because hopefully long runs of 8-bit values could
+         *    simply be memcopied and even runs of 16-bit values could be processed in a loop.
+         *    This kind of compression would also add overhead though and it proabably would be too difficult
+         *    to do inside deflate::Block, so it should probably be applied in post in
+         *    ChunkData::append( DecodedDataViews ). This might be something that could be optimzied with SIMD,
+         *    the same applies to the equally necessary new ChunkData::applyWindow method.
+         *    -> The count could be 7-bit so that the 8-th bit can be used to store the 8/16-bit value flag.
+         *       In the worst case: interleaved 8-bit and 16-bit values, this would add an overhead of 25%:
+         *       <n><8><n><16hi><16lo> <n><8>...
+         *    Ideally a format that has no overhead even in the worst-case would be nice.
+         *    This would be possible by using 4-bit values for <n> but then the maximum runlength would be 3-bit -> 7,
+         *    which seems insufficient as it might lead to lots of slow execution branching in the applyWindow method.
+         */
+        if constexpr ( ENABLE_STATISTICS && ENABLE_REAL_MARKER_COUNT ) {
+            m_realMarkerCount += chunkData->countMarkerSymbols();
+        }
         [[maybe_unused]] const auto tApplyStart = now();
         chunkData->applyWindow( previousWindow );
-        if constexpr ( ENABLE_STATISTICS || SHOW_PROFILE ) {
+        if constexpr ( ENABLE_STATISTICS ) {
             std::scoped_lock lock( m_statisticsMutex );
             if ( markerCount > 0 ) {
                 m_applyWindowTime += duration( tApplyStart );
             }
             m_markerCount += markerCount;
         }
     }
@@ -423,24 +471,27 @@
          * Suppress this relative benign case.
          * @todo Get rid of the partition offset altogether and "simply" look in the chunk cache for ones where
          *       matchesEncodedOffset returns true. Note that this has problems when the chunk to test for has not
          *       yet found a viable start position. Therefore, it requires some locking and in the worst-case
          *       waiting or if we don't wait, it might result in the same chunk being decompressed twice, once
          *       as a prefetch starting from a guessed position and once as an on-demand fetch given the exact
          *       position. */
-        if ( chunkData && !chunkData->matchesEncodedOffset( blockOffset ) && ( partitionOffset != blockOffset )
-             && ( m_preemptiveStopCount == 0 ) ) {
-            std::cerr << "[Info] Detected a performance problem. Decoding might take longer than necessary. "
-                      << "Please consider opening a performance bug report with "
-                      << "a reproducing compressed file. Detailed information:\n"
-                      << "[Info] Found mismatching block. Need offset " << formatBits( blockOffset )
-                      << ". Look in partition offset: " << formatBits( partitionOffset )
-                      << ". Found possible range: ["
-                      << formatBits( chunkData->encodedOffsetInBits ) << ", "
-                      << formatBits( chunkData->maxEncodedOffsetInBits ) << "]\n";
+        if constexpr ( ENABLE_STATISTICS ) {
+            if ( chunkData && !chunkData->matchesEncodedOffset( blockOffset ) && ( partitionOffset != blockOffset )
+                 && ( m_preemptiveStopCount == 0 ) )
+            {
+                std::cerr << "[Info] Detected a performance problem. Decoding might take longer than necessary. "
+                          << "Please consider opening a performance bug report with "
+                          << "a reproducing compressed file. Detailed information:\n"
+                          << "[Info] Found mismatching block. Need offset " << formatBits( blockOffset )
+                          << ". Look in partition offset: " << formatBits( partitionOffset )
+                          << ". Found possible range: ["
+                          << formatBits( chunkData->encodedOffsetInBits ) << ", "
+                          << formatBits( chunkData->maxEncodedOffsetInBits ) << "]\n";
+            }
         }
 
         /* If we got no block or one with the wrong data, then try again with the real offset, not the
          * speculatively prefetched one. */
         if ( !chunkData
              || ( !chunkData->matchesEncodedOffset( blockOffset )
                   && ( partitionOffset != blockOffset ) ) ) {
@@ -452,19 +503,26 @@
         if ( !chunkData || ( chunkData->encodedOffsetInBits == std::numeric_limits<size_t>::max() ) ) {
             std::stringstream message;
             message << "Decoding failed at block offset " << formatBits( blockOffset ) << "!";
             throw std::domain_error( std::move( message ).str() );
         }
 
         if ( !chunkData->matchesEncodedOffset( blockOffset ) ) {
+            /* This error should be equivalent to trying to start to decode from the requested blockOffset
+             * and failing to do so. It should only happen when a previous decodeBlock call did not stop
+             * on a deflate block boundary. */
             std::stringstream message;
-            message << "Got wrong block to searched offset! Looked for " << std::to_string( blockOffset )
+            message << "Got wrong block to searched offset! Looked for " << blockOffset
                     << " and looked up cache successively for estimated offset "
-                    << std::to_string( partitionOffset ) << " but got block with actual offset "
-                    << std::to_string( blockOffset );
+                    << partitionOffset << " but got block with actual offset ";
+            if ( chunkData->encodedOffsetInBits == chunkData->maxEncodedOffsetInBits ) {
+                message << chunkData->encodedOffsetInBits;
+            } else {
+                message << "[" << chunkData->encodedOffsetInBits << ", " << chunkData->maxEncodedOffsetInBits << "]";
+            }
             throw std::logic_error( std::move( message ).str() );
         }
 
         /* Care has to be taken that we store the correct block offset not the speculative possible range! */
         chunkData->setEncodedOffset( blockOffset );
         return chunkData;
     }
@@ -472,34 +530,40 @@
     [[nodiscard]] ChunkData
     decodeBlock( size_t blockOffset,
                  size_t nextBlockOffset ) const override
     {
         /* The decoded size of the block is only for optimization purposes. Therefore, we do not have to take care
          * of the correct ordering between BlockMap accesses and modifications (the BlockMap is still thread-safe). */
         const auto blockInfo = m_blockMap->getEncodedOffset( blockOffset );
-        return decodeBlock( m_bitReader, blockOffset, nextBlockOffset,
+        return decodeBlock( m_bitReader, blockOffset,
+                            /* untilOffset */
+                            ( blockInfo
+                              ? blockInfo->encodedOffsetInBits + blockInfo->encodedSizeInBits
+                              : nextBlockOffset ),
                             /**
                              * If we are a BGZF file and we have not imported an index, then we can assume the
                              * window to be empty because we should only get offsets at gzip stream starts.
                              * @note This is brittle in case of supporting partial imports of indexes, which would
                              *       not finalize the block finder. Instead it might be better to create the index,
                              *       including windows and decompressed sizes, by the BGZF "block finder" itself.
                              *       It has all data necessary for it including the decompressed size in the gzip
                              *       stream footer!
                              * @note BGZF index offsets should only begin at gzip stream offsets because those
                              *       do not require any window! However, even if this is implemented we cannot
                              *       remove the check against imported indexes because we cannot be sure that the
                              *       indexes were created by us and follow that scheme.
                              */
-                            m_isBgzfFile && !m_blockFinder->finalized()
-                            ? std::make_optional( WindowView{} )
-                            : m_windowMap->get( blockOffset ),
-                            blockInfo ? blockInfo->decodedSizeInBytes : std::optional<size_t>{},
-                            m_cancelThreads, m_crc32Enabled, m_maxDecompressedChunkSize,
-                            /* untilOffsetIsExact */ m_isBgzfFile );
+                            ( m_isBgzfFile && !m_blockFinder->finalized()
+                              ? std::make_optional( WindowView{} )
+                              : m_windowMap->get( blockOffset ) ),
+                            /* decodedSize */ blockInfo ? blockInfo->decodedSizeInBytes : std::optional<size_t>{},
+                            m_cancelThreads,
+                            m_crc32Enabled,
+                            m_maxDecompressedChunkSize,
+                            /* untilOffsetIsExact */ m_isBgzfFile || blockInfo );
     }
 
 public:
     /**
      * @param untilOffset Decode to excluding at least this compressed offset. It can be the offset of the next
      *                    deflate block or next gzip stream but it can also be the starting guess for the block finder
      *                    to find the next deflate block or gzip stream.
@@ -519,32 +583,32 @@
     {
         #ifdef WITH_ISAL
             using InflateWrapper = IsalInflateWrapper;
         #else
             using InflateWrapper = ZlibInflateWrapper;
         #endif
 
-        if ( initialWindow && ( ( decodedSize && ( *decodedSize > 0 ) ) || untilOffsetIsExact ) ) {
+        if ( initialWindow && untilOffsetIsExact ) {
             auto result = decodeBlockWithInflateWrapper<InflateWrapper>(
                 originalBitReader,
                 blockOffset,
                 std::min( untilOffset, originalBitReader.size() ),
                 *initialWindow,
                 decodedSize,
-                crc32Enabled,
-                untilOffsetIsExact );
+                crc32Enabled );
 
             if ( decodedSize && ( result.decodedSizeInBytes != *decodedSize ) ) {
                 std::stringstream message;
                 message << "Decoded chunk size does not match the requested decoded size!\n"
-                        << "  Block offset          : " << blockOffset << "\n"
-                        << "  Until offset          : " << untilOffset << "\n"
-                        << "  Encoded size          : " << ( untilOffset - blockOffset ) << "\n"
-                        << "  Decoded size          : " << result.decodedSizeInBytes << "\n"
-                        << "  Expected decoded size : " << *decodedSize << "\n"
+                        << "  Block offset          : " << blockOffset << " b\n"
+                        << "  Until offset          : " << untilOffset << " b\n"
+                        << "  Encoded size          : " << ( untilOffset - blockOffset ) << " b\n"
+                        << "  Actual encoded size   : " << result.encodedSizeInBits << " b\n"
+                        << "  Decoded size          : " << result.decodedSizeInBytes << " B\n"
+                        << "  Expected decoded size : " << *decodedSize << " B\n"
                         << "  Until offset is exact : " << untilOffsetIsExact << "\n"
                         << "  Initial Window        : " << ( initialWindow
                                                              ? std::to_string( initialWindow->size() )
                                                              : std::string( "None" ) ) << "\n";
                 throw std::runtime_error( std::move( message ).str() );
             }
 
@@ -561,16 +625,16 @@
         const auto tryToDecode =
             [&] ( const std::pair<size_t, size_t>& offset ) -> std::optional<ChunkData>
             {
                 try {
                     /* For decoding, it does not matter whether we seek to offset.first or offset.second but it DOES
                      * matter a lot for interpreting and correcting the encodedSizeInBits in GzipBlockFetcer::get! */
                     bitReader.seek( offset.second );
-                    auto result = decodeBlockWithRapidgzip( &bitReader, untilOffset, initialWindow, crc32Enabled,
-                                                            maxDecompressedChunkSize );
+                    auto result = decodeBlockWithRapidgzip( &bitReader, untilOffset, /* initialWindow */ std::nullopt,
+                                                            crc32Enabled, maxDecompressedChunkSize );
                     result.encodedOffsetInBits = offset.first;
                     result.maxEncodedOffsetInBits = offset.second;
                     /** @todo Avoid out of memory issues for very large compression ratios by using a simple runtime
                      *        length encoding or by only undoing the Huffman coding in parallel and the LZ77 serially,
                      *        or by stopping decoding at a threshold and fall back to serial decoding in that case? */
                     return result;
                 } catch ( const std::exception& exception ) {
@@ -646,14 +710,15 @@
          *    1. Initialize both offsets with possible matches inside the current chunk.
          *    2. Repeat until both offsets are invalid because no further matches were found in the chunk:
          *       1. Try decoding the earlier offset.
          *       2. Update the used offset by searching from last position + 1 until the chunk end.
          */
         const auto tBlockFinderStart = now();
         static constexpr auto CHUNK_SIZE = 8_Ki * BYTE_SIZE;
+        size_t falsePositiveCount{ 0 };
         for ( auto chunkBegin = blockOffset; chunkBegin < untilOffset; chunkBegin += CHUNK_SIZE ) {
             /* Only look in the first 512 KiB of data. If nothing can be found there, then something is likely
              * to be wrong with the file and looking in the rest will also likely fail. And looking in the whole
              * range to be decompressed is multiple times slower than decompression because of the slower
              * block finder and because it requires intensive seeking for false non-compressed block positives. */
             if ( cancelThreads || ( chunkBegin - blockOffset >= 512_Ki * BYTE_SIZE ) ) {
                 break;
@@ -680,42 +745,49 @@
                 }
 
                 /* Try decoding and measure the time. */
                 const auto tBlockFinderStop = now();
                 if ( auto result = tryToDecode( offsetToTest ); result ) {
                     result->blockFinderDuration = duration( tBlockFinderStart, tBlockFinderStop );
                     result->decodeDuration = duration( tBlockFinderStop );
+                    result->falsePositiveCount = falsePositiveCount;
                     return *std::move( result );
                 }
+
+                falsePositiveCount++;
             }
         }
 
         std::stringstream message;
         message << "Failed to find any valid deflate block in [" << formatBits( blockOffset )
                 << ", " << formatBits( untilOffset ) << ")";
         throw NoBlockInRange( std::move( message ).str() );
     }
 
-private:
+
+    /**
+     * @param decodedSize If given, it is used to avoid overallocations. It is NOT used as a stop condition.
+     * @param exactlUntilOffset Decompress until this known bit offset in the encoded stream. It must lie on
+     *                          a deflate block boundary.
+     */
     template<typename InflateWrapper>
     [[nodiscard]] static ChunkData
     decodeBlockWithInflateWrapper( const BitReader&            originalBitReader,
                                    size_t                const blockOffset,
-                                   size_t                const untilOffset,
+                                   size_t                const exactUntilOffset,
                                    WindowView            const initialWindow,
-                                   /** @todo get rid of this and use untilOffsetIsExact instead */
                                    std::optional<size_t> const decodedSize,
-                                   bool                  const crc32Enabled,
-                                   bool                  const untilOffsetIsExact )
+                                   bool                  const crc32Enabled )
     {
+        const auto tStart = now();
+
         BitReader bitReader( originalBitReader );
         bitReader.seek( blockOffset );
-        InflateWrapper deflateWrapper( std::move( bitReader ),
-                                       untilOffsetIsExact ? untilOffset : std::numeric_limits<size_t>::max() );
-        deflateWrapper.setWindow( initialWindow );
+        InflateWrapper inflateWrapper( std::move( bitReader ), exactUntilOffset );
+        inflateWrapper.setWindow( initialWindow );
 
         ChunkData result;
         result.setCRC32Enabled( crc32Enabled );
         result.encodedOffsetInBits = blockOffset;
 
         /**
          * Rpmalloc does worse than standard malloc (Clang 13) for the case when using 128 cores, chunk size 4 MiB
@@ -760,129 +832,294 @@
          *        128 KiB         2.5 GB/s
          *        256 KiB         2.4 GB/s
          *        512 KiB         1.5 GB/s
          *        1   MiB         370 MB/s
          */
         constexpr size_t ALLOCATION_CHUNK_SIZE = 128_Ki;
         size_t alreadyDecoded{ 0 };
-        while( !decodedSize.has_value() || ( alreadyDecoded < *decodedSize ) ) {
+        while( true ) {
             deflate::DecodedVector subchunk( decodedSize
                                              ? std::min( ALLOCATION_CHUNK_SIZE, *decodedSize - alreadyDecoded )
                                              : ALLOCATION_CHUNK_SIZE );
-            std::optional<gzip::Footer> footer;
+            std::optional<typename InflateWrapper::Footer> footer;
 
             /* In order for CRC32 verification to work, we have to append at most one gzip stream per subchunk
-             * because the CRC32 calculator is swapped inside ChunkData::append. */
+             * because the CRC32 calculator is swapped inside ChunkData::append. That's why the stop condition
+             * tests for footer.has_value(). */
             size_t nBytesRead = 0;
             size_t nBytesReadPerCall{ 0 };
             for ( ; ( nBytesRead < subchunk.size() ) && !footer; nBytesRead += nBytesReadPerCall ) {
-                std::tie( nBytesReadPerCall, footer ) = deflateWrapper.readStream( subchunk.data() + nBytesRead,
+                std::tie( nBytesReadPerCall, footer ) = inflateWrapper.readStream( subchunk.data() + nBytesRead,
                                                                                    subchunk.size() - nBytesRead );
                 if ( ( nBytesReadPerCall == 0 ) && !footer ) {
-                    if ( untilOffsetIsExact ) {
-                        break;
-                    }
-                    throw std::runtime_error( "Could not decode as much as requested!" );
+                    break;
                 }
             }
 
             alreadyDecoded += nBytesRead;
 
             subchunk.resize( nBytesRead );
             subchunk.shrink_to_fit();
             result.append( std::move( subchunk ) );
             if ( footer ) {
-                result.appendFooter( deflateWrapper.tellEncoded(), alreadyDecoded, *footer );
+                result.appendFooter( footer->footerEndEncodedOffset, alreadyDecoded, footer->gzipFooter );
             }
 
-            if ( ( nBytesReadPerCall == 0 ) && !footer && untilOffsetIsExact ) {
+            if ( ( nBytesReadPerCall == 0 ) && !footer ) {
                 break;
             }
         }
 
         uint8_t dummy{ 0 };
-        const auto [nBytesReadPerCall, footer] = deflateWrapper.readStream( &dummy, 1 );
+        const auto [nBytesReadPerCall, footer] = inflateWrapper.readStream( &dummy, 1 );
         if ( ( nBytesReadPerCall == 0 ) && footer ) {
-            result.appendFooter( deflateWrapper.tellEncoded(), alreadyDecoded, *footer );
+            result.appendFooter( footer->footerEndEncodedOffset, alreadyDecoded, footer->gzipFooter );
         }
 
-        /* We cannot arbitarily use bitReader.tell here, because the zlib wrapper buffers input read from BitReader.
-         * If untilOffset is nullopt, then we are to read to the end of the file. */
-        result.finalize( untilOffset );
+        if ( exactUntilOffset != inflateWrapper.tellCompressed() ) {
+            std::stringstream message;
+            message << "The inflate wrapper offset (" << inflateWrapper.tellCompressed() << ") "
+                    << "does not match the requested exact stop offset: " << exactUntilOffset << ". "
+                    << "The archive or the index may be corrupted or the stop condition might contain a bug. "
+                    << "Decoded: " << alreadyDecoded << " B";
+            if ( decodedSize ) {
+                 message << " out of requested " << *decodedSize << " B";
+            }
+            message << ".";
+            throw std::runtime_error( std::move( message ).str() );
+        }
+
+        result.finalize( exactUntilOffset );
+        result.decodeDurationInflateWrapper = duration( tStart );
         return result;
     }
 
+
+#ifdef WITH_ISAL
+    /**
+     * This is called from @ref decodeBlockWithRapidgzip in case the window has been fully resolved so that
+     * normal decompression instead of two-staged one becomes possible.
+     *
+     * @param untilOffset In contrast to @ref decodeBlockWithInflateWrapper, this may be an inexact guess
+     *                    from which another thread starts decoding!
+     * @note This code is copy-pasted from decodeBlockWithInflateWrapper and adjusted to use the stopping
+     *       points and deflate block properties as stop criterion.
+     */
+    [[nodiscard]] static ChunkData
+    finishDecodeBlockWithIsal( BitReader* const bitReader,
+                               size_t     const untilOffset,
+                               WindowView const initialWindow,
+                               size_t     const maxDecompressedChunkSize,
+                               ChunkData&&      result )
+    {
+        if ( bitReader == nullptr ) {
+            throw std::invalid_argument( "BitReader may not be nullptr!" );
+        }
+
+        const auto tStart = now();
+        auto nextBlockOffset = bitReader->tell();
+        bool stoppingPointReached{ false };
+        auto alreadyDecoded = result.size();
+
+        if ( ( alreadyDecoded > 0 ) && !bitReader->eof() ) {
+            result.appendDeflateBlockBoundary( nextBlockOffset, alreadyDecoded );
+        }
+
+        IsalInflateWrapper inflateWrapper{ BitReader( *bitReader ) };
+        inflateWrapper.setWindow( initialWindow );
+        inflateWrapper.setStoppingPoints( static_cast<StoppingPoint>( StoppingPoint::END_OF_BLOCK |
+                                                                      StoppingPoint::END_OF_BLOCK_HEADER |
+                                                                      StoppingPoint::END_OF_STREAM_HEADER ) );
+
+        constexpr size_t ALLOCATION_CHUNK_SIZE = 128_Ki;
+        while( !stoppingPointReached ) {
+            deflate::DecodedVector subchunk( ALLOCATION_CHUNK_SIZE );
+            std::optional<IsalInflateWrapper::Footer> footer;
+
+            /* In order for CRC32 verification to work, we have to append at most one gzip stream per subchunk
+             * because the CRC32 calculator is swapped inside ChunkData::append. */
+            size_t nBytesRead = 0;
+            size_t nBytesReadPerCall{ 0 };
+            while ( ( nBytesRead < subchunk.size() ) && !footer && !stoppingPointReached ) {
+                std::tie( nBytesReadPerCall, footer ) = inflateWrapper.readStream( subchunk.data() + nBytesRead,
+                                                                                   subchunk.size() - nBytesRead );
+                nBytesRead += nBytesReadPerCall;
+
+                /* We cannot stop decoding after a final block because the following decoder does not
+                 * expect to start a gzip footer. Put another way, we are interested in START_OF_BLOCK
+                 * not END_OF_BLOCK and therefore we have to infer one from the other. */
+                bool isBlockStart{ false };
+
+                switch ( inflateWrapper.stoppedAt() )
+                {
+                case StoppingPoint::END_OF_STREAM_HEADER:
+                    isBlockStart = true;
+                    break;
+
+                case StoppingPoint::END_OF_BLOCK:
+                    isBlockStart = !inflateWrapper.isFinalBlock();
+                    break;
+
+                case StoppingPoint::END_OF_BLOCK_HEADER:
+                    if ( ( ( nextBlockOffset >= untilOffset )
+                           && !inflateWrapper.isFinalBlock()
+                           && ( inflateWrapper.compressionType() != deflate::CompressionType::FIXED_HUFFMAN ) )
+                         || ( nextBlockOffset == untilOffset ) ) {
+                        stoppingPointReached = true;
+                    }
+                    break;
+
+                case StoppingPoint::NONE:
+                    if ( ( nBytesReadPerCall == 0 ) && !footer ) {
+                        stoppingPointReached = true;
+                    }
+                    break;
+
+                default:
+                    throw std::logic_error( "Got stopping point of a type that was not requested!" );
+                }
+
+                if ( isBlockStart ) {
+                    nextBlockOffset = inflateWrapper.tellCompressed();
+
+                    /* Do not push back the first boundary because it is redundant as it should contain the same encoded
+                     * offset as @ref result and it also would have the same problem that the real offset is ambiguous
+                     * for non-compressed blocks. */
+                    if ( alreadyDecoded + nBytesRead > 0 ) {
+                        result.appendDeflateBlockBoundary( nextBlockOffset, alreadyDecoded + nBytesRead );
+                    }
+
+                    if ( alreadyDecoded >= maxDecompressedChunkSize ) {
+                        stoppingPointReached = true;
+                        result.stoppedPreemptively = true;
+                        break;
+                    }
+                }
+            }
+
+            alreadyDecoded += nBytesRead;
+
+            subchunk.resize( nBytesRead );
+            subchunk.shrink_to_fit();
+            result.append( std::move( subchunk ) );
+            if ( footer ) {
+                nextBlockOffset = inflateWrapper.tellCompressed();
+                result.appendFooter( footer->footerEndEncodedOffset, alreadyDecoded, footer->gzipFooter );
+            }
+
+            if ( ( inflateWrapper.stoppedAt() == StoppingPoint::NONE )
+                 && ( nBytesReadPerCall == 0 ) && !footer ) {
+                break;
+            }
+        }
+
+        uint8_t dummy{ 0 };
+        const auto [nBytesReadPerCall, footer] = inflateWrapper.readStream( &dummy, 1 );
+        if ( ( inflateWrapper.stoppedAt() == StoppingPoint::NONE ) && ( nBytesReadPerCall == 0 ) && footer ) {
+            nextBlockOffset = inflateWrapper.tellCompressed();
+            result.appendFooter( footer->footerEndEncodedOffset, alreadyDecoded, footer->gzipFooter );
+        }
+
+        result.finalize( nextBlockOffset );
+        result.decodeDurationIsal = duration( tStart );
+        /**
+         * Without the std::move, performance is halved! It seems like copy elision on return does not work
+         * with function arguments! @see https://en.cppreference.com/w/cpp/language/copy_elision
+         * > In a return statement, when the operand is the name of a non-volatile object with automatic
+         * > storage duration, **which isn't a function parameter** [...]
+         * And that is only the non-mandatory copy elision, which isn't even guaranteed in C++17!
+         */
+        return std::move( result );
+    }
+#endif  // ifdef WITH_ISAL
+
+
     [[nodiscard]] static ChunkData
-    decodeBlockWithRapidgzip( BitReader*                      bitReader,
-                              size_t                          untilOffset,
+    decodeBlockWithRapidgzip( BitReader*                const bitReader,
+                              size_t                    const untilOffset,
                               std::optional<WindowView> const initialWindow,
-                              bool                            crc32Enabled,
-                              size_t                          maxDecompressedChunkSize )
+                              bool                      const crc32Enabled,
+                              size_t                    const maxDecompressedChunkSize )
     {
         if ( bitReader == nullptr ) {
             throw std::invalid_argument( "BitReader must be non-null!" );
         }
 
-        const auto chunkOffset = bitReader->tell();
+        ChunkData result;
+        result.setCRC32Enabled( crc32Enabled );
+        result.encodedOffsetInBits = bitReader->tell();
+
+    #ifdef WITH_ISAL
+        if ( initialWindow ) {
+            return finishDecodeBlockWithIsal( bitReader, untilOffset, *initialWindow, maxDecompressedChunkSize,
+                                              std::move( result ) );
+        }
+    #endif
 
         /* If true, then read the gzip header. We cannot simply check the gzipHeader optional because we might
          * start reading in the middle of a gzip stream and will not meet the gzip header for a while or never. */
         bool isAtStreamEnd = false;
         size_t streamBytesRead = 0;
         size_t totalBytesRead = 0;
         std::optional<gzip::Header> gzipHeader;
 
         std::optional<deflate::Block<> > block;
         block.emplace();
         if ( initialWindow ) {
             block->setInitialWindow( *initialWindow );
         }
 
-        ChunkData result;
-        result.setCRC32Enabled( crc32Enabled );
-        result.encodedOffsetInBits = bitReader->tell();
-
         /* Loop over possibly gzip streams and deflate blocks. We cannot use GzipReader even though it does
          * something very similar because GzipReader only works with fully decodable streams but we
          * might want to return buffer with placeholders in case we don't know the initial window, yet! */
         size_t nextBlockOffset{ 0 };
+        size_t cleanDataCount{ 0 };
         while ( true )
         {
             if ( isAtStreamEnd ) {
                 const auto headerOffset = bitReader->tell();
                 const auto [header, error] = gzip::readHeader( *bitReader );
                 if ( error != Error::NONE ) {
                     std::stringstream message;
                     message << "Failed to read gzip header at offset " << formatBits( headerOffset )
                             << " because of error: " << toString( error );
                     throw std::domain_error( std::move( message ).str() );
                 }
 
+            #ifdef WITH_ISAL
+                return finishDecodeBlockWithIsal( bitReader, untilOffset, /* initialWindow */ {},
+                                                  maxDecompressedChunkSize, std::move( result ) );
+            #endif
+
                 gzipHeader = std::move( header );
                 block.emplace();
                 block->setInitialWindow();
 
-                nextBlockOffset = bitReader->tell();
-                if ( nextBlockOffset >= untilOffset ) {
-                    break;
-                }
-
                 isAtStreamEnd = false;
             }
 
             nextBlockOffset = bitReader->tell();
 
             if ( totalBytesRead >= maxDecompressedChunkSize ) {
                 result.stoppedPreemptively = true;
                 break;
             }
 
+        #ifdef WITH_ISAL
+            if ( cleanDataCount >= deflate::MAX_WINDOW_SIZE ) {
+                const deflate::DecodedVector window = result.getLastWindow( {} );
+                return finishDecodeBlockWithIsal( bitReader, untilOffset,
+                                                  VectorView<uint8_t>( window.data(), window.size() ),
+                                                  maxDecompressedChunkSize, std::move( result ) );
+            }
+        #endif
+
             if ( auto error = block->readHeader( *bitReader ); error != Error::NONE ) {
                 std::stringstream message;
-                message << "Failed to read deflate block header at offset " << formatBits( chunkOffset )
+                message << "Failed to read deflate block header at offset " << formatBits( result.encodedOffsetInBits )
                         << " (position after trying: " << formatBits( bitReader->tell() ) << ": "
                         << toString( error );
                 throw std::domain_error( std::move( message ).str() );
             }
 
             /**
              * Preemptive Stop Condition.
@@ -908,19 +1145,21 @@
             /* Loop until we have read the full contents of the current deflate block-> */
             size_t blockBytesRead{ 0 };
             while ( !block->eob() )
             {
                 const auto [bufferViews, error] = block->read( *bitReader, std::numeric_limits<size_t>::max() );
                 if ( error != Error::NONE ) {
                     std::stringstream message;
-                    message << "Failed to decode deflate block at " << formatBits( chunkOffset )
+                    message << "Failed to decode deflate block at " << formatBits( result.encodedOffsetInBits )
                             << " because of: " << toString( error );
                     throw std::domain_error( std::move( message ).str() );
                 }
 
+                cleanDataCount += bufferViews.dataSize();
+
                 const auto tAppendStart = now();
                 result.append( bufferViews );
                 result.appendDuration += duration( tAppendStart );
                 blockBytesRead += bufferViews.size();
 
                 /* Non-compressed deflate blocks are limited to 64 KiB and the largest Dynamic Huffman Coding
                  * deflate blocks I have seen were 128 KiB in compressed size. With a maximum compression
@@ -937,16 +1176,16 @@
                                               "encountered. This is not supported to avoid out-of-memory errors." );
                 }
             }
             streamBytesRead += blockBytesRead;
             totalBytesRead += blockBytesRead;
 
             if ( block->isLastBlock() ) {
-                const auto footerOffset = bitReader->tell();
                 const auto footer = gzip::readFooter( *bitReader );
+                const auto footerOffset = bitReader->tell();
 
                 /* We only check for the stream size and CRC32 if we have read the whole stream including the header! */
                 if ( gzipHeader ) {
                     if ( streamBytesRead != footer.uncompressedSize ) {
                         std::stringstream message;
                         message << "Mismatching size (" << streamBytesRead << " <-> footer: "
                                 << footer.uncompressedSize << ") for gzip stream!";
@@ -969,19 +1208,23 @@
 
         result.finalize( nextBlockOffset );
         return result;
     }
 
 private:
     /* Members for benchmark statistics */
+    size_t m_falsePositiveCount{ 0 };
     double m_applyWindowTime{ 0 };
     double m_blockFinderTime{ 0 };
     double m_decodeTime{ 0 };
+    double m_decodeTimeInflateWrapper{ 0 };
+    double m_decodeTimeIsal{ 0 };
     double m_appendTime{ 0 };
     uint64_t m_markerCount{ 0 };
+    uint64_t m_realMarkerCount{ 0 };
     uint64_t m_preemptiveStopCount{ 0 };
     mutable std::mutex m_statisticsMutex;
 
     std::atomic<bool> m_cancelThreads{ false };
     std::atomic<bool> m_crc32Enabled{ true };
 
     /* Variables required by decodeBlock and which therefore should be either const or locked. */
```

### Comparing `rapidgzip-0.8.1/rapidgzip/GzipReader.hpp` & `rapidgzip-0.9.0/rapidgzip/GzipReader.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -9,38 +9,28 @@
 #include <string>
 #include <string_view>
 #include <stdexcept>
 #include <utility>
 
 #include <crc32.hpp>
 #include <DecodedDataView.hpp>
+#include <definitions.hpp>
 #include <deflate.hpp>
 #include <FileUtils.hpp>
 #include <filereader/FileReader.hpp>
 #include <filereader/Standard.hpp>
 #include <gzip.hpp>
 
 #ifdef WITH_PYTHON_SUPPORT
     #include <filereader/Python.hpp>
 #endif
 
 
 namespace rapidgzip
 {
-enum StoppingPoint : uint32_t
-{
-    NONE                 = 0U,
-    END_OF_STREAM_HEADER = 1U << 0U,
-    END_OF_STREAM        = 1U << 1U,  // after gzip footer has been read
-    END_OF_BLOCK_HEADER  = 1U << 2U,
-    END_OF_BLOCK         = 1U << 3U,
-    ALL                  = 0xFFFF'FFFFU,
-};
-
-
 /**
  * A strictly sequential gzip interface that can iterate over multiple gzip streams and of course deflate blocks.
  * It cannot seek back nor is it parallelized but it can be used to implement a parallelization scheme.
  */
 class GzipReader :
     public FileReader
 {
@@ -145,15 +135,15 @@
     clearerr() final
     {
         m_bitReader.clearerr();
         m_atEndOfFile = false;
         throw std::invalid_argument( "Not fully tested!" );
     }
 
-    [[nodiscard]] size_t
+    size_t
     read( char*  outputBuffer,
           size_t nBytesToRead ) final
     {
         return read( -1, outputBuffer, nBytesToRead );
     }
 
     /* Gzip specific methods */
@@ -184,15 +174,15 @@
      * @param[out] outputBuffer should at least be large enough to hold @p nBytesToRead bytes
      * @return number of bytes written
      */
     size_t
     read( const int     outputFileDescriptor = -1,
           char* const   outputBuffer         = nullptr,
           const size_t  nBytesToRead         = std::numeric_limits<size_t>::max(),
-          StoppingPoint stoppingPoint        = StoppingPoint::NONE )
+          StoppingPoint stoppingPoints       = StoppingPoint::NONE )
     {
         const auto writeFunctor =
             [nBytesDecoded = uint64_t( 0 ), outputFileDescriptor, outputBuffer]
             ( const void* const buffer,
               uint64_t    const size ) mutable
             {
                 auto* const currentBufferPosition = outputBuffer == nullptr ? nullptr : outputBuffer + nBytesDecoded;
@@ -202,21 +192,21 @@
                  *       important as for the multi-threaded version because decoding is the bottlneck for the
                  *       sequential version.
                  */
                 ::writeAll( outputFileDescriptor, currentBufferPosition, buffer, size );
                 nBytesDecoded += size;
             };
 
-        return read( writeFunctor, nBytesToRead, stoppingPoint );
+        return read( writeFunctor, nBytesToRead, stoppingPoints );
     }
 
     size_t
     read( const WriteFunctor& writeFunctor,
           const size_t        nBytesToRead = std::numeric_limits<size_t>::max(),
-          const StoppingPoint stoppingPoint = StoppingPoint::NONE )
+          const StoppingPoint stoppingPoints = StoppingPoint::NONE )
     {
         size_t nBytesDecoded = 0;
 
         /* This loop is basically a state machine over m_currentPoint and will process different things
          * depending on m_currentPoint and after each processing step it needs to recheck for EOF!
          * First read metadata so that even with nBytesToRead == 0, the position can be advanced over those. */
         while ( !m_bitReader.eof() && !eof() ) {
@@ -270,15 +260,15 @@
                 }
             }
 
         #ifdef WITH_PYTHON_SUPPORT
             checkPythonSignalHandlers();
         #endif
 
-            if ( m_currentPoint.has_value() && testFlags( *m_currentPoint, stoppingPoint ) ) {
+            if ( m_currentPoint.has_value() && testFlags( *m_currentPoint, stoppingPoints ) ) {
                 break;
             }
         }
 
         m_currentPosition += nBytesDecoded;
         return nBytesDecoded;
     }
@@ -515,26 +505,8 @@
 
     if ( m_bitReader.eof() ) {
         m_atEndOfFile = true;
     }
 
     m_currentPoint = StoppingPoint::END_OF_STREAM;
 }
-
-
-[[nodiscard]] inline std::string
-toString( StoppingPoint stoppingPoint )
-{
-    // *INDENT-OFF*
-    switch ( stoppingPoint )
-    {
-    case StoppingPoint::NONE                 : return "None";
-    case StoppingPoint::END_OF_STREAM_HEADER : return "End of Stream Header";
-    case StoppingPoint::END_OF_STREAM        : return "End of Stream";
-    case StoppingPoint::END_OF_BLOCK_HEADER  : return "End of Block Header";
-    case StoppingPoint::END_OF_BLOCK         : return "End of Block";
-    case StoppingPoint::ALL                  : return "All";
-    };
-    return "Unknown";
-    // *INDENT-ON*
-}
 }  // namespace rapidgzip
```

### Comparing `rapidgzip-0.8.1/rapidgzip/MarkerReplacement.hpp` & `rapidgzip-0.9.0/rapidgzip/MarkerReplacement.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/rapidgzip/ParallelGzipReader.hpp` & `rapidgzip-0.9.0/rapidgzip/ParallelGzipReader.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -35,32 +35,30 @@
 
 namespace rapidgzip
 {
 /**
  * @note Calls to this class are not thread-safe! Even though they use threads to evaluate them in parallel.
  */
 template<typename T_ChunkData = ChunkData,
-         bool ENABLE_STATISTICS = false,
-         bool SHOW_PROFILE = false>
+         bool ENABLE_STATISTICS = false>
 class ParallelGzipReader final :
     public FileReader
 
 {
 public:
     using ChunkData = T_ChunkData;
     /**
      * The fetching strategy should support parallelization via prefetching for sequential accesses while
      * avoiding a lot of useless prefetches for random or multi-stream sequential accesses like those occuring
      * via ratarmount.
      * The fetching strategy does not have to and also should not account for backward and strided accesses
      * because the prefetch and cache units are very large and striding or backward accessing over multiple
      * megabytes should be extremely rare.
      */
-    using ChunkFetcher = rapidgzip::GzipChunkFetcher<FetchingStrategy::FetchMultiStream, ChunkData,
-                                                   ENABLE_STATISTICS, SHOW_PROFILE>;
+    using ChunkFetcher = rapidgzip::GzipChunkFetcher<FetchingStrategy::FetchMultiStream, ChunkData, ENABLE_STATISTICS>;
     using BlockFinder = typename ChunkFetcher::BlockFinder;
     using BitReader = rapidgzip::BitReader;
     using WriteFunctor = std::function<void ( const std::shared_ptr<ChunkData>&, size_t, size_t )>;
 
 public:
     /**
      * Quick benchmarks for spacing on AMD Ryzen 3900X 12-core.
@@ -209,15 +207,15 @@
             [this] () {
                 return std::make_unique<BlockFinder>(
                     UniqueFileReader( m_sharedFileReader->clone() ),
                     /* spacing in bytes */ m_chunkSizeInBytes );
             }
         )
     {
-        m_sharedFileReader->setStatisticsEnabled( ENABLE_STATISTICS && SHOW_PROFILE );
+        m_sharedFileReader->setStatisticsEnabled( ENABLE_STATISTICS );
         if ( !m_bitReader.seekable() ) {
             throw std::invalid_argument( "Parallel BZ2 Reader will not work on non-seekable input like stdin (yet)!" );
         }
     }
 
 #ifdef WITH_PYTHON_SUPPORT
     /* These constructor overloads are for easier construction in the Cython-interface.
@@ -240,23 +238,38 @@
                         size_t    parallelization = 0 ) :
         ParallelGzipReader( std::make_unique<PythonFileReader>( pythonObject ), parallelization )
     {}
 #endif
 
     ~ParallelGzipReader()
     {
-        if constexpr ( SHOW_PROFILE ) {
+        if ( m_showProfileOnDestruction && ENABLE_STATISTICS ) {
             std::cerr << "[ParallelGzipReader] Time spent:";
             std::cerr << "\n    Writing to output         : " << m_writeOutputTime << " s";
             std::cerr << "\n    Computing CRC32           : " << m_crc32Time << " s";
             std::cerr << "\n    Number of verified CRC32s : " << m_verifiedCRC32Count;
             std::cerr << std::endl;
         }
     }
 
+    /**
+     * @note Only will work if ENABLE_STATISTICS is true.
+     */
+    void
+    setShowProfileOnDestruction( bool showProfileOnDestruction )
+    {
+        m_showProfileOnDestruction = showProfileOnDestruction;
+        if ( m_chunkFetcher ) {
+            m_chunkFetcher->setShowProfileOnDestruction( m_showProfileOnDestruction );
+        }
+        if ( m_sharedFileReader ) {
+            m_sharedFileReader->setShowProfileOnDestruction( m_showProfileOnDestruction );
+        }
+    }
+
     /* FileReader overrides */
 
     [[nodiscard]] UniqueFileReader
     clone() const override
     {
         throw std::logic_error( "Not implemented!" );
     }
@@ -420,22 +433,22 @@
             checkPythonSignalHandlers();
         #endif
 
             const auto nBytesToDecode = std::min( blockSize - offsetInBlock, nBytesToRead - nBytesDecoded );
 
             [[maybe_unused]] const auto tCRC32Start = now();
             processCRC32( chunkData, offsetInBlock, nBytesToDecode );
-            if constexpr ( ENABLE_STATISTICS || SHOW_PROFILE ) {
+            if constexpr ( ENABLE_STATISTICS ) {
                 m_crc32Time += duration( tCRC32Start );
             }
 
             if ( writeFunctor ) {
                 [[maybe_unused]] const auto tWriteStart = now();
                 writeFunctor( chunkData, offsetInBlock, nBytesToDecode );
-                if constexpr ( ENABLE_STATISTICS || SHOW_PROFILE ) {
+                if constexpr ( ENABLE_STATISTICS ) {
                     m_writeOutputTime += duration( tWriteStart );
                 }
             }
 
             nBytesDecoded += nBytesToDecode;
             m_currentPosition += nBytesToDecode;
         }
@@ -624,14 +637,23 @@
         return m_maxDecompressedChunkSize;
     }
 
 private:
     void
     setBlockOffsets( std::map<size_t, size_t> offsets )
     {
+        /**
+         * @todo Join very small consecutive block offsets until it roughly reflects the chunk size?
+         * Because currently, the version with the BGZI index is slower than without!
+         * rapidgzip -d -o /dev/null 4GiB-base64.bgz
+         * > Decompressed in total 4294967296 B in 0.565016 s -> 7601.49 MB/s
+         * rapidgzip -d -o /dev/null --import-index 4GiB-base64.bgz
+         * > Decompressed in total 4294901760 B in 1.22275 s -> 3512.5 MB/s
+         */
+
         if ( offsets.empty() ) {
             if ( m_blockMap->dataBlockCount() == 0 ) {
                 return;
             }
             throw std::invalid_argument( "May not clear offsets. Construct a new ParallelGzipReader instead!" );
         }
 
@@ -649,46 +671,85 @@
     {
         if ( index.checkpoints.empty() ) {
             return;
         }
 
         /* Generate simple compressed to uncompressed offset map from index. */
         std::map<size_t, size_t> newBlockOffsets;
-        for ( const auto& checkpoint : index.checkpoints ) {
+        for ( size_t i = 0; i < index.checkpoints.size(); ++i ) {
+            const auto& checkpoint = index.checkpoints[i];
+
+            /**
+             * Skip emission of an index, if the next checkpoint would still let us be below the chunk size.
+             * Always copy the zeroth index as is necessary for a valid index!
+             *
+             * This is for merging very small index points as might happen when importing BGZF indexes.
+             * Small index will lead to relatively larger overhead for the threading and will degrade performance:
+             * Merge n blocks:
+             *     0 -> ~3.3 GB/s, Total existing blocks: 65793
+             *     2 -> ~5.0 GB/s, Total existing blocks: 32897
+             *     4 -> ~5.7 GB/s, Total existing blocks: 16449
+             *     8 -> ~6.0 GB/s, Total existing blocks: 8225
+             *    16 -> ~6.8 GB/s, Total existing blocks: 4113
+             *    32 -> ~6.8 GB/s, Total existing blocks: 2057
+             *    64 -> ~7.2 GB/s, Total existing blocks: 1029
+             *   128 -> ~6.9 GB/s, Total existing blocks: 515
+             *
+             * Without index import (chunk size 4 MiB):
+             * src/tools/rapidgzip -d -o /dev/null 4GiB-base64.bgz
+             *   Total existing blocks: 766 blocks
+             *   Index reading took: 0.00259098 s
+             *
+             *   Decompressed in total 4294967296 B in 0.580731 s -> 7395.79 MB/s
+             *   Decompressed in total 4294967296 B in 0.576022 s -> 7456.26 MB/s
+             *   Decompressed in total 4294967296 B in 0.597594 s -> 7187.1 MB/s
+             */
+            if ( !newBlockOffsets.empty() && ( i + 1 < index.checkpoints.size() )
+                 && ( index.checkpoints[i + 1].uncompressedOffsetInBytes - newBlockOffsets.rbegin()->second
+                      <= m_chunkSizeInBytes ) )
+            {
+                continue;
+            }
+
             newBlockOffsets.emplace( checkpoint.compressedOffsetInBits, checkpoint.uncompressedOffsetInBytes );
+
+            /* Copy window data.
+             * For some reason, indexed_gzip also stores windows for the very last checkpoint at the end of the file,
+             * which is useless because there is nothing thereafter. But, don't filter it here so that exportIndex
+             * mirrors importIndex better. */
+            m_windowMap->emplace( checkpoint.compressedOffsetInBits,
+                                  WindowMap::Window( checkpoint.window.data(),
+                                                     checkpoint.window.data() + checkpoint.window.size() ) );
         }
 
         /* Input file-end offset if not included in checkpoints. */
         if ( const auto fileEndOffset = newBlockOffsets.find( index.compressedSizeInBytes * 8 );
              fileEndOffset == newBlockOffsets.end() )
         {
             newBlockOffsets.emplace( index.compressedSizeInBytes * 8, index.uncompressedSizeInBytes );
         } else if ( fileEndOffset->second != index.uncompressedSizeInBytes ) {
             throw std::invalid_argument( "Index has contradicting information for the file end information!" );
         }
 
         setBlockOffsets( std::move( newBlockOffsets ) );
 
-        /* Copy window data. */
-        for ( const auto& checkpoint : index.checkpoints ) {
-            /* For some reason, indexed_gzip also stores windows for the very last checkpoint at the end of the file,
-             * which is useless because there is nothing thereafter. But, don't filter it here so that exportIndex
-             * mirrors importIndex better. */
-            m_windowMap->emplace( checkpoint.compressedOffsetInBits,
-                                  WindowMap::Window( checkpoint.window.data(),
-                                                     checkpoint.window.data() + checkpoint.window.size() ) );
-        }
         chunkFetcher().clearCache();
     }
 
+    void
+    importIndex( UniqueFileReader indexFile )
+    {
+        setBlockOffsets( readGzipIndex( std::move( indexFile ), m_sharedFileReader->clone() ) );
+    }
+
 #ifdef WITH_PYTHON_SUPPORT
     void
     importIndex( PyObject* pythonObject )
     {
-        setBlockOffsets( readGzipIndex( std::make_unique<PythonFileReader>( pythonObject ) ) );
+        importIndex( std::make_unique<PythonFileReader>( pythonObject ) );
     }
 
     void
     exportIndex( PyObject* pythonObject )
     {
         const auto file = std::make_unique<PythonFileReader>( pythonObject );
         const auto checkedWrite =
@@ -777,14 +838,15 @@
 
         if ( !m_chunkFetcher ) {
             throw std::logic_error( "Block fetcher should have been initialized!" );
         }
 
         m_chunkFetcher->setCRC32Enabled( m_crc32.enabled() );
         m_chunkFetcher->setMaxDecompressedChunkSize( m_maxDecompressedChunkSize );
+        m_chunkFetcher->setShowProfileOnDestruction( m_showProfileOnDestruction );
 
         return *m_chunkFetcher;
     }
 
     void
     setBlockFinderOffsets( const std::map<size_t, size_t>& offsets )
     {
@@ -859,14 +921,15 @@
     std::unique_ptr<SharedFileReader> m_sharedFileReader;
     BitReader m_bitReader{ UniqueFileReader( m_sharedFileReader->clone() ) };
 
     size_t m_currentPosition = 0;  /**< the current position as can only be modified with read or seek calls. */
     bool m_atEndOfFile = false;
 
     /** Benchmarking */
+    bool m_showProfileOnDestruction{ false };
     double m_writeOutputTime{ 0 };
     double m_crc32Time{ 0 };
     uint64_t m_verifiedCRC32Count{ 0 };
 
     size_t const m_fetcherParallelization;
     /** The block finder is much faster than the fetcher and therefore does not require es much parallelization! */
     size_t const m_finderParallelization{ ceilDiv( m_fetcherParallelization, 8U ) };
```

### Comparing `rapidgzip-0.8.1/rapidgzip/WindowMap.hpp` & `rapidgzip-0.9.0/rapidgzip/WindowMap.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/rapidgzip/blockfinder/Bgzf.hpp` & `rapidgzip-0.9.0/rapidgzip/blockfinder/Bgzf.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,16 @@
         0x00, 0x00, 0x00, 0x00,             /* gzip footer CRC32 */
         0x00, 0x00, 0x00, 0x00              /* gzip footer uncompressed size */
     };
 
 public:
     explicit
     Bgzf( UniqueFileReader fileReader ) :
-        m_fileReader( std::move( fileReader ) )
+        m_fileReader( std::move( fileReader ) ),
+        m_currentBlockOffset( m_fileReader->tell() )
     {
         HeaderBytes header;
         const auto nBytesRead = m_fileReader->read( reinterpret_cast<char*>( header.data() ), header.size() );
         if ( nBytesRead != header.size() ) {
             throw std::invalid_argument( "Could not read enough data from given file!" );
         }
 
@@ -125,15 +126,15 @@
             throw std::invalid_argument( "Could not read enough data from given file for BGZF footer!" );
         }
 
         if ( footer != BGZF_FOOTER ) {
             throw std::invalid_argument( "Given file does not end with a BGZF footer!" );
         }
 
-        m_fileReader->seek( 0 );
+        m_fileReader->seek( m_currentBlockOffset );
     }
 
     [[nodiscard]] static bool
     isBgzfFile( const UniqueFileReader& file )
     {
         const auto oldPos = file->tell();
```

### Comparing `rapidgzip-0.8.1/rapidgzip/blockfinder/DynamicHuffman.hpp` & `rapidgzip-0.9.0/rapidgzip/blockfinder/DynamicHuffman.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,16 @@
  * - 0b0  Final Block: We ignore uninteresting final blocks (filter 50%)
  * - 0b10 Compression Type Dynamic Huffman (filters 75%)
  * - (Anything but 0b1111) + 1 bit
  *   Code Count 257 + (5-bit) <= 286, i.e., (5-bit) <= 29 (31 is 0b11111, 30 is 0b11110)
  *   (filters out 2 /32 = 6.25%)
  *   Beware that the >highest< 4 bits may not be 1 but this that we requrie all 5-bits to
  *   determine validity because they are lower significant first!
+ * - (Anything but 0b1111) + 1 bit
+ *   Distance Code Count 1 + (5-bits) <= 30 <=> (5-bits) <= 29 -> filters out 6.25%
  * The returned position is only 0 if all of the above holds for a bitCount of 13
  * Next would be the 3-bit precode code lengths. One or two alone does not allow any filtering at all.
  * I think starting from three, it might become possible, e.g., if any two are 1, then all others must
  * be of 0-length because the tree is filled already.
  */
 template<uint8_t bitCount>
 constexpr bool
@@ -56,14 +58,20 @@
         if constexpr ( bitCount < 1U + 2U + 5U ) {
             return matches;
         }
         const auto codeCount = bits & nLowestBitsSet<uint32_t, 5U>();
         bits >>= 5U;
         matches &= codeCount <= 29;
 
+        /* Bits 8-12: distance count */
+        if constexpr ( bitCount < 1U + 2U + 5U + 5U ) {
+            return matches;
+        }
+        const auto distanceCodeCount = bits & nLowestBitsSet<uint32_t, 5U>();
+        matches &= distanceCodeCount <= 29;
         return matches;
     }
 }
 
 
 constexpr uint32_t MAX_EVALUATED_BITS = 13;
 
@@ -273,14 +281,18 @@
                         error = readDistanceAndLiteralCodeLengths(
                             literalCL, bitReader, precodeHC, literalCodeCount + distanceCodeCount );
                         /* Using this theoretically derivable position avoids a possibly costly call to tell()
                          * to save the old offset. */
                         bitReader.seek( static_cast<long long int>( offset ) + 13 + ALL_PRECODE_BITS );
                     }
 
+                    if ( UNLIKELY( literalCL[deflate::END_OF_BLOCK_SYMBOL] == 0 ) ) [[unlikely]] {
+                        error = Error::INVALID_CODE_LENGTHS;
+                    }
+
                     /* Check distance code lengths. */
                     if ( UNLIKELY( error == Error::NONE ) ) [[unlikely]] {
                         HuffmanCodingCheckOnly<uint16_t, MAX_CODE_LENGTH,
                                                uint8_t, MAX_DISTANCE_SYMBOL_COUNT> distanceHC;
                         error = distanceHC.initializeFromLengths(
                             VectorView<uint8_t>( literalCL.data() + literalCodeCount, distanceCodeCount ) );
                     }
```

### Comparing `rapidgzip-0.8.1/rapidgzip/blockfinder/PigzNaive.hpp` & `rapidgzip-0.9.0/rapidgzip/blockfinder/PigzNaive.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/rapidgzip/blockfinder/PigzParallel.hpp` & `rapidgzip-0.9.0/rapidgzip/blockfinder/PigzParallel.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/rapidgzip/blockfinder/PigzStringView.hpp` & `rapidgzip-0.9.0/rapidgzip/blockfinder/PigzStringView.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/rapidgzip/blockfinder/Uncompressed.hpp` & `rapidgzip-0.9.0/rapidgzip/blockfinder/Uncompressed.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/rapidgzip/blockfinder/precodecheck/BruteForceLUT.hpp` & `rapidgzip-0.9.0/rapidgzip/blockfinder/precodecheck/BruteForceLUT.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/rapidgzip/blockfinder/precodecheck/SingleCompressedLUT.hpp` & `rapidgzip-0.9.0/rapidgzip/blockfinder/precodecheck/SingleCompressedLUT.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/rapidgzip/blockfinder/precodecheck/SingleLUT.hpp` & `rapidgzip-0.9.0/rapidgzip/blockfinder/precodecheck/SingleLUT.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/rapidgzip/blockfinder/precodecheck/WalkTreeCompressedLUT.hpp` & `rapidgzip-0.9.0/rapidgzip/blockfinder/precodecheck/WalkTreeCompressedLUT.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/rapidgzip/blockfinder/precodecheck/WalkTreeLUT.hpp` & `rapidgzip-0.9.0/rapidgzip/blockfinder/precodecheck/WalkTreeLUT.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -197,17 +197,23 @@
            + LUT[( precodeBits >> ( 3U * CACHED_BITS ) ) & nLowestBitsSet<uint64_t, CACHED_BITS>()]
            /* The last requires no bit masking because BitReader::read already has masked to the lowest 57 bits
             * and this shifts 48 bits to the right, leaving only 9 (<12) bits set anyways. */
            + LUT[( precodeBits >> ( 4U * CACHED_BITS ) )];
 }
 
 
-/* 5 * 5 = 25 bits LUT map to bool, i.e., 2^22 B = 4 MiB! */
+/**
+ * @todo Correctly parameterize everything so that it works with other values than 5.
+ * 4 * 5 = 20 bits LUT map to bool, i.e., 2^17 B = 512 KiB! -> segfault
+ * 5 * 5 = 25 bits LUT map to bool, i.e., 2^22 B =   4 MiB!
+ * 6 * 5 = 30 bits LUT map to bool, i.e., 2^27 B =  32 MiB! -> testPrecodeCheck fails
+ */
+static constexpr auto PRECODE_FREQUENCIES_LUT_COUNT = 5U;
 static constexpr auto PRECODE_FREQUENCIES_1_TO_5_VALID_LUT =
-    createPrecodeFrequenciesValidLUT<UNIFORM_FREQUENCY_BITS, 5>();
+    createPrecodeFrequenciesValidLUT<UNIFORM_FREQUENCY_BITS, PRECODE_FREQUENCIES_LUT_COUNT>();
 
 
 /**
  * @note Requires 4 (precode count) + 57 (maximum precode count * 3) bits to check for validity.
  *       Get all 57 bits at once to avoid a data dependency on the precode count. Note that this is only
  *       possible assuming a 64-bit gzip footer, else, this could be a wrong transformation because it wouldn't
  *       be able to find very small deflate blocks close to the end of the file. because they trigger an EOF.
@@ -222,15 +228,15 @@
     const auto precodeBits = next57Bits & nLowestBitsSet<uint64_t>( codeLengthCount * PRECODE_BITS );
     const auto bitLengthFrequencies = precodesToHistogram<4>( precodeBits );
 
     /* Lookup in LUT and subtable (64 values in uint64_t) */
     const auto valueToLookUp = bitLengthFrequencies >> UNIFORM_FREQUENCY_BITS;  // ignore non-zero-counts;
     {
         const auto bitToLookUp = 1ULL << ( valueToLookUp % 64 );
-        constexpr auto INDEX_BIT_COUNT = UNIFORM_FREQUENCY_BITS * 5 - 6 /* log2 64 = 6 */;
+        constexpr auto INDEX_BIT_COUNT = UNIFORM_FREQUENCY_BITS * PRECODE_FREQUENCIES_LUT_COUNT - 6 /* log2 64 = 6 */;
         const auto elementIndex = ( valueToLookUp / 64 ) & nLowestBitsSet<CompressedHistogram, INDEX_BIT_COUNT>();
         if ( ( PRECODE_FREQUENCIES_1_TO_5_VALID_LUT[elementIndex] & bitToLookUp ) == 0 ) {
             /* Might also be bloating not only invalid. */
             return rapidgzip::Error::INVALID_CODE_LENGTHS;
         }
     }
```

### Comparing `rapidgzip-0.8.1/rapidgzip/blockfinder/precodecheck/WithoutLUT.hpp` & `rapidgzip-0.9.0/rapidgzip/blockfinder/precodecheck/WithoutLUT.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/rapidgzip/crc32.hpp` & `rapidgzip-0.9.0/rapidgzip/crc32.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/rapidgzip/deflate.hpp` & `rapidgzip-0.9.0/rapidgzip/deflate.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -20,34 +20,45 @@
 #include <optional>
 #include <stdexcept>
 #include <type_traits>
 #include <utility>
 #include <vector>
 
 #include <BitReader.hpp>
-#include <huffman/HuffmanCodingDoubleLiteralCached.hpp>
-#include <huffman/HuffmanCodingLinearSearch.hpp>
+//#include <huffman/HuffmanCodingLinearSearch.hpp>
 #include <huffman/HuffmanCodingSymbolsPerLength.hpp>
 #include <huffman/HuffmanCodingReversedBitsCachedCompressed.hpp>
 #include <huffman/HuffmanCodingReversedBitsCached.hpp>
-#include <huffman/HuffmanCodingReversedCodesPerLength.hpp>
+//#include <huffman/HuffmanCodingReversedCodesPerLength.hpp>
+
+#ifdef WITH_ISAL
+    //#include <huffman/HuffmanCodingDistanceISAL.hpp>
+    #include <huffman/HuffmanCodingISAL.hpp>
+#else
+    #include <huffman/HuffmanCodingDoubleLiteralCached.hpp>
+#endif
 
 #include "DecodedDataView.hpp"
 #include "definitions.hpp"
 #include "Error.hpp"
 #include "gzip.hpp"
 #include "MarkerReplacement.hpp"
+#include "RFCTables.hpp"
 
 
 namespace rapidgzip
 {
 namespace deflate
 {
+#ifdef WITH_ISAL
+using LiteralOrLengthHuffmanCoding = HuffmanCodingISAL;
+#else
 using LiteralOrLengthHuffmanCoding =
     HuffmanCodingDoubleLiteralCached<uint16_t, MAX_CODE_LENGTH, uint16_t, MAX_LITERAL_HUFFMAN_CODE_COUNT>;
+#endif
 
 /**
  * Because the fixed Huffman coding is used by different threads it HAS TO BE immutable. It is constant anyway
  * but it also MUST NOT have mutable members. This means that HuffmanCodingDoubleLiteralCached does NOT work
  * because it internally saves the second symbol.
  * @todo Make it such that the implementations can handle the case that the construction might result in
  *       larger symbol values than are allowed to appear in the first place! I.e., cut-off construction there.
@@ -151,19 +162,55 @@
  *     Apply precode HC         : 0.0182615 s
  *     Create distance HC       : 0.00743017 s
  *     Create literal HC        : 0.0440123 s
  */
 using PrecodeHuffmanCoding = HuffmanCodingReversedBitsCachedCompressed<uint8_t, MAX_PRECODE_LENGTH,
                                                                        uint8_t, MAX_PRECODE_COUNT>;
 
-/* HuffmanCodingReversedBitsCached is definitely faster for silesia.tar.gz which has more back-references than
+/**
+ * HuffmanCodingReversedBitsCached is definitely faster for silesia.tar.gz which has more back-references than
  * base64.gz for which the difference in changing this Huffman coding is negligible. Note that we can't use
- * double caching for this because that would mean merging the cache with ne next literal/length Huffman code! */
+ * double caching for this because that would mean merging the cache with ne next literal/length Huffman code!
+ *
+ * HuffmanCodingDistanceISAL:
+ *
+ *     m rapidgzip && src/tools/rapidgzip -d -o /dev/null 10xSRR22403185_2.fastq.gz
+ *     Decompressed in total 3618153020 B in:
+ *         1.60722 s -> 2251.18 MB/s
+ *         1.63562 s -> 2212.1 MB/s
+ *         1.63213 s -> 2216.83 MB/s
+ *
+ *     m rapidgzip && src/tools/rapidgzip -d -o /dev/null test-files/silesia/20xsilesia.tar.gz
+ *     Decompressed in total 4239155200 B in:
+ *         1.10059 s -> 3851.72 MB/s
+ *         1.13037 s -> 3750.25 MB/s
+ *         1.16631 s -> 3634.66 MB/s
+ *         1.12481 s -> 3768.77 MB/s
+ *
+ * HuffmanCodingReversedBitsCached:
+ *
+ *     m rapidgzip && src/tools/rapidgzip -d -o /dev/null 10xSRR22403185_2.fastq.g
+ *     Decompressed in total 3618153020 B in:
+ *         1.61128 s -> 2245.52 MB/s
+ *         1.61067 s -> 2246.36 MB/s
+ *         1.65374 s -> 2187.86 MB/s
+ *         1.60478 s -> 2254.61 MB/s
+ *
+ *     m rapidgzip && src/tools/rapidgzip -d -o /dev/null test-files/silesia/20xsilesia.tar.gz
+ *     Decompressed in total 4239155200 B in:
+ *         1.11193 s -> 3812.43 MB/s
+ *         1.0941 s -> 3874.56 MB/s
+ *         1.0993 s -> 3856.23 MB/s
+ *
+ * -> ISA-l is actually slightly (~1-2%) slower than my own simple distance Huffman decoder.
+ *    Probably because the table is small enough that short/long caching hinders performance more than it helps.
+ **/
 using DistanceHuffmanCoding = HuffmanCodingReversedBitsCached<uint16_t, MAX_CODE_LENGTH,
                                                               uint8_t, MAX_DISTANCE_SYMBOL_COUNT>;
+//using DistanceHuffmanCoding = HuffmanCodingDistanceISAL;
 
 /* Include 256 safety buffer so that we can avoid branches while filling. */
 using LiteralAndDistanceCLBuffer = std::array<uint8_t, MAX_LITERAL_OR_LENGTH_SYMBOLS + MAX_DISTANCE_SYMBOL_COUNT + 256>;
 
 
 [[nodiscard]] constexpr FixedHuffmanCoding
 createFixedHC()
@@ -188,78 +235,14 @@
         throw std::logic_error( "Fixed Huffman Tree could not be created!" );
     }
 
     return result;
 }
 
 
-[[nodiscard]] constexpr uint16_t
-calculateDistance( uint16_t distance,
-                   uint8_t  extraBitsCount,
-                   uint16_t extraBits ) noexcept
-{
-    assert( distance >= 4 );
-    return 1U + ( 1U << ( extraBitsCount + 1U ) ) + ( ( distance % 2U ) << extraBitsCount ) + extraBits;
-};
-
-
-[[nodiscard]] constexpr uint16_t
-calculateDistance( uint16_t distance ) noexcept
-{
-    assert( distance >= 4 );
-    const auto extraBitsCount = ( distance - 2U ) / 2U;
-    return 1U + ( 1U << ( extraBitsCount + 1U ) ) + ( ( distance % 2U ) << extraBitsCount );
-};
-
-
-using DistanceLUT = std::array<uint16_t, 30>;
-
-[[nodiscard]] constexpr DistanceLUT
-createDistanceLUT() noexcept
-{
-    DistanceLUT result{};
-    for ( uint16_t i = 0; i < 4; ++i ) {
-        result[i] = i + 1;
-    }
-    for ( uint16_t i = 4; i < result.size(); ++i ) {
-        result[i] = calculateDistance( i );
-    }
-    return result;
-}
-
-
-alignas( 8 ) static constexpr DistanceLUT
-distanceLUT = createDistanceLUT();
-
-
-[[nodiscard]] constexpr uint16_t
-calculateLength( uint16_t code ) noexcept
-{
-    assert( code < 285 - 261 );
-    const auto extraBits = code / 4U;
-    return 3U + ( 1U << ( extraBits + 2U ) ) + ( ( code % 4U ) << extraBits );
-};
-
-
-using LengthLUT = std::array<uint16_t, 285 - 261>;
-
-[[nodiscard]] constexpr LengthLUT
-createLengthLUT() noexcept
-{
-    LengthLUT result{};
-    for ( uint16_t i = 0; i < result.size(); ++i ) {
-        result[i] = calculateLength( i );
-    }
-    return result;
-}
-
-
-alignas( 8 ) static constexpr LengthLUT
-lengthLUT = createLengthLUT();
-
 namespace
 {
 /**
  * @note Initially this was a static member of Block but when compiling with the manylinux_2_28 container,
  *       which contains "g++ (GCC) 11.2.1 20220127 (Red Hat 11.2.1-9)", I'd get redefinition errors for this
  *       even though it compiles fine with "g++ (Ubuntu 11.2.0-19ubuntu1) 11.2.0".
  *       I suspect that it does not like static methods inside templated classes. Multiple instantiations
@@ -342,14 +325,15 @@
 class BlockStatistics
 {
 public:
     uint64_t failedPrecodeInit{ 0 };
     uint64_t failedDistanceInit{ 0 };
     uint64_t failedLiteralInit{ 0 };
     uint64_t failedPrecodeApply{ 0 };
+    uint64_t missingEOBSymbol{ 0 };
 
     std::array<uint64_t, /* codeLengthCount - 4 is 4 bits = 16 possible values */ 16> precodeCLHistogram{};
 
     struct {
         uint32_t precode{ 0 };
         uint32_t distance{ 0 };
         uint32_t literal{ 0 };  // Minimum value is 257!
@@ -461,20 +445,14 @@
      * Reads the dynamic Huffman code. This is called by @ref readHeader after reading the first three header bits
      * and determining that it is a dynamic Huffman encoded block.
      * @note Normally, you want to call @ref readHeader instead. This is only for very specific edge use cases!
      */
     [[nodiscard]] Error
     readDynamicHuffmanCoding( BitReader& bitReader );
 
-    [[nodiscard]] constexpr const auto&
-    window() const noexcept
-    {
-        return m_window;
-    }
-
     [[nodiscard]] constexpr size_t
     uncompressedSize() const noexcept
     {
         return m_compressionType == CompressionType::UNCOMPRESSED ? m_uncompressedSize : 0;
     }
 
     /**
@@ -556,14 +534,23 @@
              typename HuffmanCoding>
     [[nodiscard]] std::pair<size_t, Error>
     readInternalCompressed( BitReader&           bitReader,
                             size_t               nMaxToDecode,
                             Window&              window,
                             const HuffmanCoding& coding );
 
+#ifdef WITH_ISAL
+    template<typename Window>
+    [[nodiscard]] std::pair<size_t, Error>
+    readInternalCompressedIsal( BitReader&                bitReader,
+                                size_t                    nMaxToDecode,
+                                Window&                   window,
+                                const HuffmanCodingISAL& coding );
+#endif
+
     [[nodiscard]] static uint16_t
     getLength( uint16_t   code,
                BitReader& bitReader );
 
     [[nodiscard]] std::pair<uint16_t, Error>
     getDistance( BitReader& bitReader ) const;
 
@@ -774,14 +761,18 @@
 
     const auto literalCodeCount = 257 + bitReader.read<5>();
     if ( literalCodeCount > MAX_LITERAL_OR_LENGTH_SYMBOLS ) {
         durations.readDynamicHeader += duration( times.readDynamicStart );
         return Error::EXCEEDED_LITERAL_RANGE;
     }
     const auto distanceCodeCount = 1 + bitReader.read<5>();
+    if ( distanceCodeCount > MAX_DISTANCE_SYMBOL_COUNT ) {
+        durations.readDynamicHeader += duration( times.readDynamicStart );
+        return Error::EXCEEDED_DISTANCE_RANGE;
+    }
     const auto codeLengthCount = 4 + bitReader.read<4>();
 
     if constexpr ( ENABLE_STATISTICS ) {
         this->precodeCLHistogram[codeLengthCount - 4]++;
         this->codeCounts.precode = codeLengthCount;
         this->codeCounts.distance = distanceCodeCount;
         this->codeCounts.literal = literalCodeCount;
@@ -826,14 +817,23 @@
         if constexpr ( ENABLE_STATISTICS ) {
             this->failedPrecodeApply++;
             durations.readDynamicHeader += duration( times.readDynamicStart );
         }
         return precodeApplyError;
     }
 
+    /* Check for end-of-block symbol to have a non-zero code length. */
+    if ( m_literalCL[deflate::END_OF_BLOCK_SYMBOL] == 0 ) {
+        if constexpr ( ENABLE_STATISTICS ) {
+            durations.readDynamicHeader += duration( times.readDynamicStart );
+            this->missingEOBSymbol++;
+        }
+        return Error::INVALID_CODE_LENGTHS;
+    }
+
     /* Create distance HC
      * When encoding base64-encoded random-data, I encountered a length of 9, so uint16_t is necessary! */
     error = m_distanceHC.initializeFromLengths(
         VectorView<uint8_t>( m_literalCL.data() + literalCodeCount, distanceCodeCount ) );
 
     if constexpr ( ENABLE_STATISTICS ) {
         times.createdDistanceHC = now();
@@ -888,14 +888,17 @@
 template<bool ENABLE_STATISTICS>
 std::pair<uint16_t, Error>
 Block<ENABLE_STATISTICS>::getDistance( BitReader& bitReader ) const
 {
     uint16_t distance = 0;
     if ( m_compressionType == CompressionType::FIXED_HUFFMAN ) {
         distance = reverseBits( static_cast<uint8_t>( bitReader.read<5>() ) ) >> 3U;
+        if ( UNLIKELY( distance >= MAX_DISTANCE_SYMBOL_COUNT ) ) [[unlikely]] {
+            return { 0, Error::EXCEEDED_DISTANCE_RANGE };
+        }
     } else {
         const auto decodedDistance = m_distanceHC.decode( bitReader );
         if ( UNLIKELY( !decodedDistance ) ) [[unlikely]] {
             return { 0, Error::INVALID_HUFFMAN_CODE };
         }
         distance = static_cast<uint16_t>( *decodedDistance );
     }
@@ -1143,15 +1146,24 @@
         /* This does not take into account nMaxToDecode to avoid additional state to keep track off. */
         return readInternalUncompressed( bitReader, window );
     }
 
     if ( m_compressionType == CompressionType::FIXED_HUFFMAN ) {
         return readInternalCompressed( bitReader, nMaxToDecode, window, m_fixedHC );
     }
+
+#ifdef WITH_ISAL
+    if constexpr ( std::is_same_v<LiteralOrLengthHuffmanCoding, HuffmanCodingISAL> ) {
+        return readInternalCompressedIsal( bitReader, nMaxToDecode, window, m_literalHC );
+    } else {
+        return readInternalCompressed( bitReader, nMaxToDecode, window, m_literalHC );
+    }
+#else
     return readInternalCompressed( bitReader, nMaxToDecode, window, m_literalHC );
+#endif
 }
 
 
 template<bool ENABLE_STATISTICS>
 template<typename Window>
 std::pair<size_t, Error>
 Block<ENABLE_STATISTICS>::readInternalUncompressed( BitReader& bitReader,
@@ -1226,15 +1238,15 @@
             }
 
             appendToWindow( window, code );
             ++nBytesRead;
             continue;
         }
 
-        if ( UNLIKELY( code == 256 ) ) [[unlikely]] {
+        if ( UNLIKELY( code == END_OF_BLOCK_SYMBOL /* 256 */ ) ) [[unlikely]] {
             m_atEndOfBlock = true;
             break;
         }
 
         if ( UNLIKELY( code > 285 ) ) [[unlikely]] {
             return { nBytesRead, Error::INVALID_HUFFMAN_CODE };
         }
@@ -1262,14 +1274,96 @@
     }
 
     m_decodedBytes += nBytesRead;
     return { nBytesRead, Error::NONE };
 }
 
 
+#ifdef WITH_ISAL
+template<bool ENABLE_STATISTICS>
+template<typename Window>
+std::pair<size_t, Error>
+Block<ENABLE_STATISTICS>::readInternalCompressedIsal
+(
+    BitReader&               bitReader,
+    size_t                   nMaxToDecode,
+    Window&                  window,
+    const HuffmanCodingISAL& coding )
+{
+    if ( !coding.isValid() ) {
+        throw std::invalid_argument( "No Huffman coding loaded! Call readHeader first!" );
+    }
+
+    constexpr bool containsMarkerBytes = std::is_same_v<std::decay_t<decltype( *window.data() ) >, uint16_t>;
+
+    nMaxToDecode = std::min( nMaxToDecode, window.size() - MAX_RUN_LENGTH );
+
+    size_t nBytesRead{ 0 };
+    for ( nBytesRead = 0; nBytesRead < nMaxToDecode; )
+    {
+        auto [symbol, symbolCount] = coding.decode( bitReader );
+        if ( symbolCount == 0 ) {
+            return { nBytesRead, Error::INVALID_HUFFMAN_CODE };
+        }
+
+        for ( ; symbolCount > 0; symbolCount--, symbol >>= 8 ) {
+            const auto code = static_cast<uint16_t>( symbol & 0xFFFFU );
+
+            if ( ( code <= 255 ) || ( symbolCount > 1 ) ) {
+                if constexpr ( ENABLE_STATISTICS ) {
+                    symbolTypes.literal++;
+                }
+
+                appendToWindow( window, static_cast<uint8_t>( code ) );
+                ++nBytesRead;
+                continue;
+            }
+
+            if ( UNLIKELY( code == END_OF_BLOCK_SYMBOL /* 256 */ ) ) [[unlikely]] {
+                m_atEndOfBlock = true;
+                m_decodedBytes += nBytesRead;
+                return { nBytesRead, Error::NONE };
+            }
+
+            static constexpr auto MAX_LIT_LEN_SYM = 512U;
+            if ( UNLIKELY( code > MAX_LIT_LEN_SYM ) ) [[unlikely]] {
+                return { nBytesRead, Error::INVALID_HUFFMAN_CODE };
+            }
+
+            if constexpr ( ENABLE_STATISTICS ) {
+                symbolTypes.backreference++;
+            }
+
+            /* If the next symbol is a repeat length, read in the length extra bits, the distance code, the distance
+             * extra bits. Then write out the corresponding data and update the state data accordingly. */
+            const auto length = symbol - 254U;
+            if ( length != 0 ) {
+                const auto [distance, error] = getDistance( bitReader );
+                if ( error != Error::NONE ) {
+                    return { nBytesRead, error };
+                }
+
+                if constexpr ( !containsMarkerBytes ) {
+                    if ( distance > m_decodedBytes + nBytesRead ) {
+                        return { nBytesRead, Error::EXCEEDED_WINDOW_RANGE };
+                    }
+                }
+
+                resolveBackreference( window, distance, length );
+                nBytesRead += length;
+            }
+        }
+    }
+
+    m_decodedBytes += nBytesRead;
+    return { nBytesRead, Error::NONE };
+}
+#endif  // ifdef WITH_ISAL
+
+
 template<bool ENABLE_STATISTICS>
 void
 Block<ENABLE_STATISTICS>::setInitialWindow( VectorView<uint8_t> const& initialWindow )
 {
     if ( !m_containsMarkerBytes ) {
         return;
     }
```

### Comparing `rapidgzip-0.8.1/rapidgzip/gzip.hpp` & `rapidgzip-0.9.0/rapidgzip/gzip.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/rapidgzip/huffman/HuffmanCodingBase.hpp` & `rapidgzip-0.9.0/rapidgzip/huffman/HuffmanCodingBase.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         }
 
         if ( UNLIKELY( codeLengths.size() > MAX_SYMBOL_COUNT ) ) [[unlikely]] {
             throw std::invalid_argument( "The range of the symbol type cannot represent the implied alphabet!" );
         }
 
         /* A maximum code length of 0 is valid! It happens when encoding this with pigz:
-         * python3 -c 'import sys; sys.stdout.buffer.write(bytes(range(256)))' | pigz > 0CL.pgz */
+         * python3 -c 'import sys; sys.stdout.buffer.write(bytes(range(256)))' | pigz > 0CL.pigz */
         m_maxCodeLength = getMax( codeLengths );
 
         m_minCodeLength = getMinPositive( codeLengths );
         if ( UNLIKELY( m_maxCodeLength > MAX_CODE_LENGTH ) ) [[unlikely]] {
             throw std::invalid_argument( "The range of the code type cannot represent the given code lengths!" );
         }
```

### Comparing `rapidgzip-0.8.1/rapidgzip/huffman/HuffmanCodingCheckOnly.hpp` & `rapidgzip-0.9.0/rapidgzip/huffman/HuffmanCodingCheckOnly.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/rapidgzip/huffman/HuffmanCodingDoubleLiteralCached.hpp` & `rapidgzip-0.9.0/rapidgzip/huffman/HuffmanCodingDoubleLiteralCached.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/rapidgzip/huffman/HuffmanCodingLinearSearch.hpp` & `rapidgzip-0.9.0/rapidgzip/huffman/HuffmanCodingLinearSearch.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/rapidgzip/huffman/HuffmanCodingReversedBitsCached.hpp` & `rapidgzip-0.9.0/rapidgzip/huffman/HuffmanCodingReversedBitsCached.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/rapidgzip/huffman/HuffmanCodingReversedBitsCachedCompressed.hpp` & `rapidgzip-0.9.0/rapidgzip/huffman/HuffmanCodingReversedBitsCachedCompressed.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/rapidgzip/huffman/HuffmanCodingReversedCodesPerLength.hpp` & `rapidgzip-0.9.0/rapidgzip/huffman/HuffmanCodingReversedCodesPerLength.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/rapidgzip/huffman/HuffmanCodingSymbolsPerLength.hpp` & `rapidgzip-0.9.0/rapidgzip/huffman/HuffmanCodingSymbolsPerLength.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/rapidgzip/precode.hpp` & `rapidgzip-0.9.0/rapidgzip/precode.hpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/rapidgzip.cpp` & `rapidgzip-0.9.0/rapidgzip.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.0 */
+/* Generated by Cython 3.0.2 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "rapidgzip/ParallelGzipReader.hpp",
             "tools/rapidgzip.cpp"
@@ -48,18 +48,23 @@
 
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#define CYTHON_ABI "3_0_0"
+#if CYTHON_LIMITED_API
+#define __PYX_EXTRA_ABI_MODULE_NAME "limited"
+#else
+#define __PYX_EXTRA_ABI_MODULE_NAME ""
+#endif
+#define CYTHON_ABI "3_0_2" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030000F0
+#define CYTHON_HEX_VERSION 0x030002F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -84,14 +89,15 @@
 #endif
 #ifndef PY_LONG_LONG
   #define PY_LONG_LONG LONG_LONG
 #endif
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
+#define __PYX_LIMITED_VERSION_HEX PY_VERSION_HEX
 #if defined(GRAALVM_PYTHON)
   /* For very preliminary testing purposes. Most variables are set the same as PyPy.
      The existence of this section does not imply that anything works or is even tested */
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 1
@@ -150,16 +156,17 @@
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
-  #undef CYTHON_USE_TYPE_SPECS
-  #define CYTHON_USE_TYPE_SPECS 0
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
@@ -203,14 +210,18 @@
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(CYTHON_LIMITED_API)
+  #ifdef Py_LIMITED_API
+    #undef __PYX_LIMITED_VERSION_HEX
+    #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
+  #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 1
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_CLINE_IN_TRACEBACK
   #define CYTHON_CLINE_IN_TRACEBACK 0
@@ -250,15 +261,15 @@
     #define CYTHON_PEP487_INIT_SUBCLASS 1
   #endif
   #undef CYTHON_PEP489_MULTI_PHASE_INIT
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_MODULE_STATE
   #define CYTHON_USE_MODULE_STATE 1
   #ifndef CYTHON_USE_TP_FINALIZE
-    #define CYTHON_USE_TP_FINALIZE 1
+    #define CYTHON_USE_TP_FINALIZE 0
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
@@ -472,14 +483,22 @@
 #ifndef CYTHON_NCP_UNUSED
 # if CYTHON_COMPILING_IN_CPYTHON
 #  define CYTHON_NCP_UNUSED
 # else
 #  define CYTHON_NCP_UNUSED CYTHON_UNUSED
 # endif
 #endif
+#ifndef CYTHON_USE_CPP_STD_MOVE
+  #if defined(__cplusplus) && (\
+    __cplusplus >= 201103L || (defined(_MSC_VER) && _MSC_VER >= 1600))
+    #define CYTHON_USE_CPP_STD_MOVE 1
+  #else
+    #define CYTHON_USE_CPP_STD_MOVE 0
+  #endif
+#endif
 #define __Pyx_void_to_None(void_result) ((void)(void_result), Py_INCREF(Py_None), Py_None)
 #ifdef _MSC_VER
     #ifndef _MSC_STDINT_H_
         #if _MSC_VER < 1300
             typedef unsigned char     uint8_t;
             typedef unsigned short    uint16_t;
             typedef unsigned int      uint32_t;
@@ -587,67 +606,97 @@
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_DefaultClassType PyClass_Type
   #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
   #define __Pyx_DefaultClassType PyType_Type
-#if PY_VERSION_HEX >= 0x030B00A1
-    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
+#if CYTHON_COMPILING_IN_LIMITED_API
+    static CYTHON_INLINE PyObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
-        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
-        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *empty=NULL;
-        const char *fn_cstr=NULL;
-        const char *name_cstr=NULL;
-        PyCodeObject *co=NULL, *result=NULL;
+        PyObject *exception_table = NULL;
+        PyObject *types_module=NULL, *code_type=NULL, *result=NULL;
+        PyObject *version_info; // borrowed
+        PyObject *py_minor_version = NULL;
+        long minor_version = 0;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
-        if (!(kwds=PyDict_New())) goto end;
-        if (!(argcount=PyLong_FromLong(a))) goto end;
-        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
-        if (!(posonlyargcount=PyLong_FromLong(p))) goto end;
-        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
-        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
-        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
-        if (!(nlocals=PyLong_FromLong(l))) goto end;
-        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
-        if (!(stacksize=PyLong_FromLong(s))) goto end;
-        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
-        if (!(flags=PyLong_FromLong(f))) goto end;
-        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
-        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
-        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
-        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
-        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto end;
-        if (!(empty = PyTuple_New(0))) goto end;
-        result = (PyCodeObject*) PyObject_Call(replace, empty, kwds);
+        #if __PYX_LIMITED_VERSION_HEX >= 0x030B0000
+        minor_version = 11; // we don't yet need to distinguish between versions > 11
+        #else
+        if (!(version_info = PySys_GetObject("version_info"))) goto end;
+        if (!(py_minor_version = PySequence_GetItem(version_info, 1))) goto end;
+        minor_version = PyLong_AsLong(py_minor_version);
+        if (minor_version == -1 && PyErr_Occurred()) goto end;
+        #endif
+        if (!(types_module = PyImport_ImportModule("types"))) goto end;
+        if (!(code_type = PyObject_GetAttrString(types_module, "CodeType"))) goto end;
+        if (minor_version <= 7) {
+            (void)p;
+            result = PyObject_CallFunction(code_type, "iiiiiOOOOOOiOO", a, k, l, s, f, code,
+                          c, n, v, fn, name, fline, lnos, fv, cell);
+        } else if (minor_version <= 10) {
+            result = PyObject_CallFunction(code_type, "iiiiiiOOOOOOiOO", a,p, k, l, s, f, code,
+                          c, n, v, fn, name, fline, lnos, fv, cell);
+        } else {
+            if (!(exception_table = PyBytes_FromStringAndSize(NULL, 0))) goto end;
+            result = PyObject_CallFunction(code_type, "iiiiiiOOOOOOOiOO", a,p, k, l, s, f, code,
+                          c, n, v, fn, name, name, fline, lnos, exception_table, fv, cell);
+        }
     end:
-        Py_XDECREF((PyObject*) co);
-        Py_XDECREF(kwds);
-        Py_XDECREF(argcount);
-        Py_XDECREF(posonlyargcount);
-        Py_XDECREF(kwonlyargcount);
-        Py_XDECREF(nlocals);
-        Py_XDECREF(stacksize);
-        Py_XDECREF(replace);
-        Py_XDECREF(empty);
+        Py_XDECREF(code_type);
+        Py_XDECREF(exception_table);
+        Py_XDECREF(types_module);
+        Py_XDECREF(py_minor_version);
         if (type) {
             PyErr_Restore(type, value, traceback);
         }
         return result;
     }
+    #ifndef CO_OPTIMIZED
+    #define CO_OPTIMIZED 0x0001
+    #endif
+    #ifndef CO_NEWLOCALS
+    #define CO_NEWLOCALS 0x0002
+    #endif
+    #ifndef CO_VARARGS
+    #define CO_VARARGS 0x0004
+    #endif
+    #ifndef CO_VARKEYWORDS
+    #define CO_VARKEYWORDS 0x0008
+    #endif
+    #ifndef CO_ASYNC_GENERATOR
+    #define CO_ASYNC_GENERATOR 0x0200
+    #endif
+    #ifndef CO_GENERATOR
+    #define CO_GENERATOR 0x0020
+    #endif
+    #ifndef CO_COROUTINE
+    #define CO_COROUTINE 0x0080
+    #endif
+#elif PY_VERSION_HEX >= 0x030B0000
+  static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
+                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
+                                                    PyObject *fv, PyObject *cell, PyObject* fn,
+                                                    PyObject *name, int fline, PyObject *lnos) {
+    PyCodeObject *result;
+    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);  // we don't have access to __pyx_empty_bytes here
+    if (!empty_bytes) return NULL;
+    result =
+      #if PY_VERSION_HEX >= 0x030C0000
+        PyUnstable_Code_NewWithPosOnlyArgs
+      #else
+        PyCode_NewWithPosOnlyArgs
+      #endif
+        (a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, name, fline, lnos, empty_bytes);
+    Py_DECREF(empty_bytes);
+    return result;
+  }
 #elif PY_VERSION_HEX >= 0x030800B2 && !CYTHON_COMPILING_IN_PYPY
   #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_NewWithPosOnlyArgs(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
   #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
@@ -739,15 +788,15 @@
                                             size_t nargsf, PyObject *kwnames);
   #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  ((size_t)1 << (8 * sizeof(size_t) - 1))
   #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(((size_t)(n)) & ~__Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET))
 #else
   #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  0
   #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(n))
 #endif
-#if PY_VERSION_HEX < 0x030900B1
+#if __PYX_LIMITED_VERSION_HEX < 0x030900B1
   #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  ((void)m, PyType_FromSpecWithBases(s, b))
   typedef PyObject *(*__Pyx_PyCMethod)(PyObject *, PyTypeObject *, PyObject *const *, size_t, PyObject *);
 #else
   #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  PyType_FromModuleAndSpec(m, s, b)
   #define __Pyx_PyCMethod  PyCMethod
 #endif
 #ifndef METH_METHOD
@@ -889,14 +938,19 @@
   #define __Pyx_PyType_HasFeature(type, feature)  ((__Pyx_PyType_GetFlags(type) & (feature)) != 0)
   #define __Pyx_PyObject_GetIterNextFunc(obj)  (Py_TYPE(obj)->tp_iternext)
 #else
   #define __Pyx_PyType_GetFlags(tp)   (PyType_GetFlags((PyTypeObject *)tp))
   #define __Pyx_PyType_HasFeature(type, feature)  PyType_HasFeature(type, feature)
   #define __Pyx_PyObject_GetIterNextFunc(obj)  PyIter_Next
 #endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_SetItemOnTypeDict(tp, k, v) PyObject_GenericSetAttr((PyObject*)tp, k, v)
+#else
+  #define __Pyx_SetItemOnTypeDict(tp, k, v) PyDict_SetItem(tp->tp_dict, k, v)
+#endif
 #if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
     PyTypeObject *type = Py_TYPE(obj);\
     assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
     PyObject_GC_Del(obj);\
     Py_DECREF(type);\
 }
@@ -1015,17 +1069,33 @@
   #define __Pyx_SET_REFCNT(obj, refcnt) Py_SET_REFCNT(obj, refcnt)
   #define __Pyx_SET_SIZE(obj, size) Py_SET_SIZE(obj, size)
 #else
   #define __Pyx_SET_REFCNT(obj, refcnt) Py_REFCNT(obj) = (refcnt)
   #define __Pyx_SET_SIZE(obj, size) Py_SIZE(obj) = (size)
 #endif
 #if CYTHON_ASSUME_SAFE_MACROS
+  #define __Pyx_PySequence_ITEM(o, i) PySequence_ITEM(o, i)
   #define __Pyx_PySequence_SIZE(seq)  Py_SIZE(seq)
+  #define __Pyx_PyTuple_SET_ITEM(o, i, v) (PyTuple_SET_ITEM(o, i, v), (0))
+  #define __Pyx_PyList_SET_ITEM(o, i, v) (PyList_SET_ITEM(o, i, v), (0))
+  #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_GET_SIZE(o)
+  #define __Pyx_PyList_GET_SIZE(o) PyList_GET_SIZE(o)
+  #define __Pyx_PySet_GET_SIZE(o) PySet_GET_SIZE(o)
+  #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_GET_SIZE(o)
+  #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_GET_SIZE(o)
 #else
+  #define __Pyx_PySequence_ITEM(o, i) PySequence_GetItem(o, i)
   #define __Pyx_PySequence_SIZE(seq)  PySequence_Size(seq)
+  #define __Pyx_PyTuple_SET_ITEM(o, i, v) PyTuple_SetItem(o, i, v)
+  #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
+  #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
+  #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
+  #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
+  #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
+  #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
   #define PyInt_Type                   PyLong_Type
   #define PyInt_Check(op)              PyLong_Check(op)
   #define PyInt_CheckExact(op)         PyLong_CheckExact(op)
   #define __Pyx_Py3Int_Check(op)       PyLong_Check(op)
@@ -1437,23 +1507,23 @@
 
 /*--- Type declarations ---*/
 struct __pyx_obj_9rapidgzip__RapidgzipFile;
 
 /* "rapidgzip.pyx":60
  *         pass
  * 
- * ctypedef ParallelGzipReader[RapidgzipChunkData, TrueValue, TrueValue] ParallelGzipReaderVerbose             # <<<<<<<<<<<<<<
+ * ctypedef ParallelGzipReader[RapidgzipChunkData, TrueValue] ParallelGzipReaderVerbose             # <<<<<<<<<<<<<<
  * ctypedef ParallelGzipReader[RapidgzipChunkData] ParallelGzipReaderNonVerbose
  * 
  */
-typedef rapidgzip::ParallelGzipReader<rapidgzip::ChunkData,true,true>  __pyx_t_9rapidgzip_ParallelGzipReaderVerbose;
+typedef rapidgzip::ParallelGzipReader<rapidgzip::ChunkData,true>  __pyx_t_9rapidgzip_ParallelGzipReaderVerbose;
 
 /* "rapidgzip.pyx":61
  * 
- * ctypedef ParallelGzipReader[RapidgzipChunkData, TrueValue, TrueValue] ParallelGzipReaderVerbose
+ * ctypedef ParallelGzipReader[RapidgzipChunkData, TrueValue] ParallelGzipReaderVerbose
  * ctypedef ParallelGzipReader[RapidgzipChunkData] ParallelGzipReaderNonVerbose             # <<<<<<<<<<<<<<
  * 
  * 
  */
 typedef rapidgzip::ParallelGzipReader<rapidgzip::ChunkData>  __pyx_t_9rapidgzip_ParallelGzipReaderNonVerbose;
 
 /* "rapidgzip.pyx":82
@@ -1627,33 +1697,50 @@
 /* BytesEquals.proto */
 static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
 
 /* UnicodeEquals.proto */
 static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
 
 /* fastcall.proto */
-#define __Pyx_Arg_VARARGS(args, i) PyTuple_GET_ITEM(args, i)
+#if CYTHON_AVOID_BORROWED_REFS
+    #define __Pyx_Arg_VARARGS(args, i) PySequence_GetItem(args, i)
+#elif CYTHON_ASSUME_SAFE_MACROS
+    #define __Pyx_Arg_VARARGS(args, i) PyTuple_GET_ITEM(args, i)
+#else
+    #define __Pyx_Arg_VARARGS(args, i) PyTuple_GetItem(args, i)
+#endif
+#if CYTHON_AVOID_BORROWED_REFS
+    #define __Pyx_Arg_NewRef_VARARGS(arg) __Pyx_NewRef(arg)
+    #define __Pyx_Arg_XDECREF_VARARGS(arg) Py_XDECREF(arg)
+#else
+    #define __Pyx_Arg_NewRef_VARARGS(arg) arg // no-op
+    #define __Pyx_Arg_XDECREF_VARARGS(arg) // no-op - arg is borrowed
+#endif
 #define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
 #define __Pyx_KwValues_VARARGS(args, nargs) NULL
 #define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
 #define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
 #if CYTHON_METH_FASTCALL
     #define __Pyx_Arg_FASTCALL(args, i) args[i]
     #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
     #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
     static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
     #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg // no-op, __Pyx_Arg_FASTCALL is direct and this needs
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg)  // no-op - arg was returned from array
 #else
     #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
     #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
     #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
     #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
     #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) __Pyx_Arg_NewRef_VARARGS(arg)
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg) __Pyx_Arg_XDECREF_VARARGS(arg)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
 #define __Pyx_ArgsSlice_VARARGS(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_VARARGS(args, start), stop - start)
 #define __Pyx_ArgsSlice_FASTCALL(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_FASTCALL(args, start), stop - start)
 #else
 #define __Pyx_ArgsSlice_VARARGS(args, start, stop) PyTuple_GetSlice(args, start, stop)
 #define __Pyx_ArgsSlice_FASTCALL(args, start, stop) PyTuple_GetSlice(args, start, stop)
 #endif
 
@@ -1694,15 +1781,15 @@
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
 #if !CYTHON_VECTORCALL
 #if PY_VERSION_HEX >= 0x03080000
   #include "frameobject.h"
-#if PY_VERSION_HEX >= 0x030b00a6
+#if PY_VERSION_HEX >= 0x030b00a6 && !CYTHON_COMPILING_IN_LIMITED_API
   #ifndef Py_BUILD_CORE
     #define Py_BUILD_CORE 1
   #endif
   #include "internal/pycore_frame.h"
 #endif
   #define __Pxy_PyFrame_Initialize_Offsets()
   #define __Pyx_PyFrame_GetLocalsplus(frame)  ((frame)->f_localsplus)
@@ -1921,30 +2008,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_0
-#define __PYX_HAVE_RT_ImportType_proto_3_0_0
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_2
+#define __PYX_HAVE_RT_ImportType_proto_3_0_2
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_2(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_2(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_0 {
-   __Pyx_ImportType_CheckSize_Error_3_0_0 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_0 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_0 = 2
+enum __Pyx_ImportType_CheckSize_3_0_2 {
+   __Pyx_ImportType_CheckSize_Error_3_0_2 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_2 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_2 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_2(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_2 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportDottedModule.proto */
 static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
@@ -1959,15 +2046,30 @@
 #if !CYTHON_USE_TYPE_SPECS
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
 #else
 static PyTypeObject* __Pyx_FetchCommonTypeFromSpec(PyObject *module, PyType_Spec *spec, PyObject *bases);
 #endif
 
 /* PyMethodNew.proto */
-#if PY_MAJOR_VERSION >= 3
+#if CYTHON_COMPILING_IN_LIMITED_API
+static PyObject *__Pyx_PyMethod_New(PyObject *func, PyObject *self, PyObject *typ) {
+    PyObject *typesModule=NULL, *methodType=NULL, *result=NULL;
+    CYTHON_UNUSED_VAR(typ);
+    if (!self)
+        return __Pyx_NewRef(func);
+    typesModule = PyImport_ImportModule("types");
+    if (!typesModule) return NULL;
+    methodType = PyObject_GetAttrString(typesModule, "MethodType");
+    Py_DECREF(typesModule);
+    if (!methodType) return NULL;
+    result = PyObject_CallFunctionObjArgs(methodType, func, self, NULL);
+    Py_DECREF(methodType);
+    return result;
+}
+#elif PY_MAJOR_VERSION >= 3
 static PyObject *__Pyx_PyMethod_New(PyObject *func, PyObject *self, PyObject *typ) {
     CYTHON_UNUSED_VAR(typ);
     if (!self)
         return __Pyx_NewRef(func);
     return PyMethod_New(func, self);
 }
 #else
@@ -1983,47 +2085,50 @@
 #define __Pyx_CyFunction_USED
 #define __Pyx_CYFUNCTION_STATICMETHOD  0x01
 #define __Pyx_CYFUNCTION_CLASSMETHOD   0x02
 #define __Pyx_CYFUNCTION_CCLASS        0x04
 #define __Pyx_CYFUNCTION_COROUTINE     0x08
 #define __Pyx_CyFunction_GetClosure(f)\
     (((__pyx_CyFunctionObject *) (f))->func_closure)
-#if PY_VERSION_HEX < 0x030900B1
+#if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_CyFunction_GetClassObj(f)\
       (((__pyx_CyFunctionObject *) (f))->func_classobj)
 #else
   #define __Pyx_CyFunction_GetClassObj(f)\
       ((PyObject*) ((PyCMethodObject *) (f))->mm_class)
 #endif
 #define __Pyx_CyFunction_SetClassObj(f, classobj)\
     __Pyx__CyFunction_SetClassObj((__pyx_CyFunctionObject *) (f), (classobj))
 #define __Pyx_CyFunction_Defaults(type, f)\
     ((type *)(((__pyx_CyFunctionObject *) (f))->defaults))
 #define __Pyx_CyFunction_SetDefaultsGetter(f, g)\
     ((__pyx_CyFunctionObject *) (f))->defaults_getter = (g)
 typedef struct {
-#if PY_VERSION_HEX < 0x030900B1
+#if CYTHON_COMPILING_IN_LIMITED_API
+    PyObject_HEAD
+    PyObject *func;
+#elif PY_VERSION_HEX < 0x030900B1
     PyCFunctionObject func;
 #else
     PyCMethodObject func;
 #endif
 #if CYTHON_BACKPORT_VECTORCALL
     __pyx_vectorcallfunc func_vectorcall;
 #endif
-#if PY_VERSION_HEX < 0x030500A0
+#if PY_VERSION_HEX < 0x030500A0 || CYTHON_COMPILING_IN_LIMITED_API
     PyObject *func_weakreflist;
 #endif
     PyObject *func_dict;
     PyObject *func_name;
     PyObject *func_qualname;
     PyObject *func_doc;
     PyObject *func_globals;
     PyObject *func_code;
     PyObject *func_closure;
-#if PY_VERSION_HEX < 0x030900B1
+#if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     PyObject *func_classobj;
 #endif
     void *defaults;
     int defaults_pyobjects;
     size_t defaults_size;  // used by FusedFunction for copying defaults
     int flags;
     PyObject *defaults_tuple;
@@ -2278,15 +2383,15 @@
 static const char __pyx_k__6[] = "";
 static const char __pyx_k__7[] = "*";
 static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_io[] = "io";
 static const char __pyx_k_os[] = "os";
 static const char __pyx_k_rb[] = "rb";
 static const char __pyx_k_wb[] = "wb";
-static const char __pyx_k__46[] = "?";
+static const char __pyx_k__45[] = "?";
 static const char __pyx_k_arg[] = "arg";
 static const char __pyx_k_cli[] = "cli";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_sys[] = "sys";
 static const char __pyx_k_args[] = "args";
 static const char __pyx_k_argv[] = "argv";
 static const char __pyx_k_dict[] = "__dict__";
@@ -2300,15 +2405,15 @@
 static const char __pyx_k_read[] = "read";
 static const char __pyx_k_seek[] = "seek";
 static const char __pyx_k_self[] = "self";
 static const char __pyx_k_size[] = "size";
 static const char __pyx_k_spec[] = "__spec__";
 static const char __pyx_k_tell[] = "tell";
 static const char __pyx_k_test[] = "__test__";
-static const char __pyx_k_0_8_1[] = "0.8.1";
+static const char __pyx_k_0_9_0[] = "0.9.0";
 static const char __pyx_k_cargs[] = "cargs";
 static const char __pyx_k_close[] = "close";
 static const char __pyx_k_enter[] = "__enter__";
 static const char __pyx_k_super[] = "super";
 static const char __pyx_k_buffer[] = "buffer";
 static const char __pyx_k_closed[] = "closed";
 static const char __pyx_k_enable[] = "enable";
@@ -2484,15 +2589,15 @@
   #if CYTHON_USE_MODULE_STATE
   #endif
   #if CYTHON_USE_MODULE_STATE
   PyObject *__pyx_type_9rapidgzip__RapidgzipFile;
   #endif
   PyTypeObject *__pyx_ptype_9rapidgzip__RapidgzipFile;
   PyObject *__pyx_kp_u_;
-  PyObject *__pyx_kp_u_0_8_1;
+  PyObject *__pyx_kp_u_0_9_0;
   PyObject *__pyx_kp_u_Expected_file_name_string_file_d;
   PyObject *__pyx_kp_u_Invalid_file_object;
   PyObject *__pyx_kp_u_Parallelization_argument_must_be;
   PyObject *__pyx_n_s_RapidgzipFile;
   PyObject *__pyx_n_s_RapidgzipFile_2;
   PyObject *__pyx_n_s_RapidgzipFile___init;
   PyObject *__pyx_n_s_RapidgzipFile___reduce_cython;
@@ -2515,15 +2620,15 @@
   PyObject *__pyx_n_s_RapidgzipFile_size;
   PyObject *__pyx_n_s_RapidgzipFile_tell;
   PyObject *__pyx_n_s_RapidgzipFile_tell_compressed;
   PyObject *__pyx_n_s_RawIOBase;
   PyObject *__pyx_n_s_SEEK_SET;
   PyObject *__pyx_n_s_TypeError;
   PyObject *__pyx_n_s_UnsupportedOperation;
-  PyObject *__pyx_n_s__46;
+  PyObject *__pyx_n_s__45;
   PyObject *__pyx_kp_u__6;
   PyObject *__pyx_n_s__7;
   PyObject *__pyx_n_s_arg;
   PyObject *__pyx_n_s_args;
   PyObject *__pyx_n_s_argv;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_available_block_offsets;
@@ -2630,15 +2735,14 @@
   PyObject *__pyx_tuple__27;
   PyObject *__pyx_tuple__32;
   PyObject *__pyx_tuple__34;
   PyObject *__pyx_tuple__36;
   PyObject *__pyx_tuple__37;
   PyObject *__pyx_tuple__41;
   PyObject *__pyx_tuple__43;
-  PyObject *__pyx_tuple__44;
   PyObject *__pyx_codeobj__9;
   PyObject *__pyx_codeobj__11;
   PyObject *__pyx_codeobj__13;
   PyObject *__pyx_codeobj__14;
   PyObject *__pyx_codeobj__15;
   PyObject *__pyx_codeobj__16;
   PyObject *__pyx_codeobj__18;
@@ -2655,15 +2759,15 @@
   PyObject *__pyx_codeobj__31;
   PyObject *__pyx_codeobj__33;
   PyObject *__pyx_codeobj__35;
   PyObject *__pyx_codeobj__38;
   PyObject *__pyx_codeobj__39;
   PyObject *__pyx_codeobj__40;
   PyObject *__pyx_codeobj__42;
-  PyObject *__pyx_codeobj__45;
+  PyObject *__pyx_codeobj__44;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
@@ -2702,15 +2806,15 @@
   #ifdef __Pyx_FusedFunction_USED
   Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
   #endif
   Py_CLEAR(clear_module_state->__pyx_ptype_7cpython_4type_type);
   Py_CLEAR(clear_module_state->__pyx_ptype_9rapidgzip__RapidgzipFile);
   Py_CLEAR(clear_module_state->__pyx_type_9rapidgzip__RapidgzipFile);
   Py_CLEAR(clear_module_state->__pyx_kp_u_);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_0_8_1);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_0_9_0);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Expected_file_name_string_file_d);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Invalid_file_object);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Parallelization_argument_must_be);
   Py_CLEAR(clear_module_state->__pyx_n_s_RapidgzipFile);
   Py_CLEAR(clear_module_state->__pyx_n_s_RapidgzipFile_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_RapidgzipFile___init);
   Py_CLEAR(clear_module_state->__pyx_n_s_RapidgzipFile___reduce_cython);
@@ -2733,15 +2837,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_RapidgzipFile_size);
   Py_CLEAR(clear_module_state->__pyx_n_s_RapidgzipFile_tell);
   Py_CLEAR(clear_module_state->__pyx_n_s_RapidgzipFile_tell_compressed);
   Py_CLEAR(clear_module_state->__pyx_n_s_RawIOBase);
   Py_CLEAR(clear_module_state->__pyx_n_s_SEEK_SET);
   Py_CLEAR(clear_module_state->__pyx_n_s_TypeError);
   Py_CLEAR(clear_module_state->__pyx_n_s_UnsupportedOperation);
-  Py_CLEAR(clear_module_state->__pyx_n_s__46);
+  Py_CLEAR(clear_module_state->__pyx_n_s__45);
   Py_CLEAR(clear_module_state->__pyx_kp_u__6);
   Py_CLEAR(clear_module_state->__pyx_n_s__7);
   Py_CLEAR(clear_module_state->__pyx_n_s_arg);
   Py_CLEAR(clear_module_state->__pyx_n_s_args);
   Py_CLEAR(clear_module_state->__pyx_n_s_argv);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_available_block_offsets);
@@ -2848,15 +2952,14 @@
   Py_CLEAR(clear_module_state->__pyx_tuple__27);
   Py_CLEAR(clear_module_state->__pyx_tuple__32);
   Py_CLEAR(clear_module_state->__pyx_tuple__34);
   Py_CLEAR(clear_module_state->__pyx_tuple__36);
   Py_CLEAR(clear_module_state->__pyx_tuple__37);
   Py_CLEAR(clear_module_state->__pyx_tuple__41);
   Py_CLEAR(clear_module_state->__pyx_tuple__43);
-  Py_CLEAR(clear_module_state->__pyx_tuple__44);
   Py_CLEAR(clear_module_state->__pyx_codeobj__9);
   Py_CLEAR(clear_module_state->__pyx_codeobj__11);
   Py_CLEAR(clear_module_state->__pyx_codeobj__13);
   Py_CLEAR(clear_module_state->__pyx_codeobj__14);
   Py_CLEAR(clear_module_state->__pyx_codeobj__15);
   Py_CLEAR(clear_module_state->__pyx_codeobj__16);
   Py_CLEAR(clear_module_state->__pyx_codeobj__18);
@@ -2873,15 +2976,15 @@
   Py_CLEAR(clear_module_state->__pyx_codeobj__31);
   Py_CLEAR(clear_module_state->__pyx_codeobj__33);
   Py_CLEAR(clear_module_state->__pyx_codeobj__35);
   Py_CLEAR(clear_module_state->__pyx_codeobj__38);
   Py_CLEAR(clear_module_state->__pyx_codeobj__39);
   Py_CLEAR(clear_module_state->__pyx_codeobj__40);
   Py_CLEAR(clear_module_state->__pyx_codeobj__42);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__45);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__44);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
   __pyx_mstate *traverse_module_state = __pyx_mstate(m);
@@ -2898,15 +3001,15 @@
   #ifdef __Pyx_FusedFunction_USED
   Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
   #endif
   Py_VISIT(traverse_module_state->__pyx_ptype_7cpython_4type_type);
   Py_VISIT(traverse_module_state->__pyx_ptype_9rapidgzip__RapidgzipFile);
   Py_VISIT(traverse_module_state->__pyx_type_9rapidgzip__RapidgzipFile);
   Py_VISIT(traverse_module_state->__pyx_kp_u_);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_0_8_1);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_0_9_0);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Expected_file_name_string_file_d);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Invalid_file_object);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Parallelization_argument_must_be);
   Py_VISIT(traverse_module_state->__pyx_n_s_RapidgzipFile);
   Py_VISIT(traverse_module_state->__pyx_n_s_RapidgzipFile_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_RapidgzipFile___init);
   Py_VISIT(traverse_module_state->__pyx_n_s_RapidgzipFile___reduce_cython);
@@ -2929,15 +3032,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_RapidgzipFile_size);
   Py_VISIT(traverse_module_state->__pyx_n_s_RapidgzipFile_tell);
   Py_VISIT(traverse_module_state->__pyx_n_s_RapidgzipFile_tell_compressed);
   Py_VISIT(traverse_module_state->__pyx_n_s_RawIOBase);
   Py_VISIT(traverse_module_state->__pyx_n_s_SEEK_SET);
   Py_VISIT(traverse_module_state->__pyx_n_s_TypeError);
   Py_VISIT(traverse_module_state->__pyx_n_s_UnsupportedOperation);
-  Py_VISIT(traverse_module_state->__pyx_n_s__46);
+  Py_VISIT(traverse_module_state->__pyx_n_s__45);
   Py_VISIT(traverse_module_state->__pyx_kp_u__6);
   Py_VISIT(traverse_module_state->__pyx_n_s__7);
   Py_VISIT(traverse_module_state->__pyx_n_s_arg);
   Py_VISIT(traverse_module_state->__pyx_n_s_args);
   Py_VISIT(traverse_module_state->__pyx_n_s_argv);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_available_block_offsets);
@@ -3044,15 +3147,14 @@
   Py_VISIT(traverse_module_state->__pyx_tuple__27);
   Py_VISIT(traverse_module_state->__pyx_tuple__32);
   Py_VISIT(traverse_module_state->__pyx_tuple__34);
   Py_VISIT(traverse_module_state->__pyx_tuple__36);
   Py_VISIT(traverse_module_state->__pyx_tuple__37);
   Py_VISIT(traverse_module_state->__pyx_tuple__41);
   Py_VISIT(traverse_module_state->__pyx_tuple__43);
-  Py_VISIT(traverse_module_state->__pyx_tuple__44);
   Py_VISIT(traverse_module_state->__pyx_codeobj__9);
   Py_VISIT(traverse_module_state->__pyx_codeobj__11);
   Py_VISIT(traverse_module_state->__pyx_codeobj__13);
   Py_VISIT(traverse_module_state->__pyx_codeobj__14);
   Py_VISIT(traverse_module_state->__pyx_codeobj__15);
   Py_VISIT(traverse_module_state->__pyx_codeobj__16);
   Py_VISIT(traverse_module_state->__pyx_codeobj__18);
@@ -3069,15 +3171,15 @@
   Py_VISIT(traverse_module_state->__pyx_codeobj__31);
   Py_VISIT(traverse_module_state->__pyx_codeobj__33);
   Py_VISIT(traverse_module_state->__pyx_codeobj__35);
   Py_VISIT(traverse_module_state->__pyx_codeobj__38);
   Py_VISIT(traverse_module_state->__pyx_codeobj__39);
   Py_VISIT(traverse_module_state->__pyx_codeobj__40);
   Py_VISIT(traverse_module_state->__pyx_codeobj__42);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__45);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__44);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
 #define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
@@ -3132,15 +3234,15 @@
 #if CYTHON_USE_MODULE_STATE
 #endif
 #if CYTHON_USE_MODULE_STATE
 #define __pyx_type_9rapidgzip__RapidgzipFile __pyx_mstate_global->__pyx_type_9rapidgzip__RapidgzipFile
 #endif
 #define __pyx_ptype_9rapidgzip__RapidgzipFile __pyx_mstate_global->__pyx_ptype_9rapidgzip__RapidgzipFile
 #define __pyx_kp_u_ __pyx_mstate_global->__pyx_kp_u_
-#define __pyx_kp_u_0_8_1 __pyx_mstate_global->__pyx_kp_u_0_8_1
+#define __pyx_kp_u_0_9_0 __pyx_mstate_global->__pyx_kp_u_0_9_0
 #define __pyx_kp_u_Expected_file_name_string_file_d __pyx_mstate_global->__pyx_kp_u_Expected_file_name_string_file_d
 #define __pyx_kp_u_Invalid_file_object __pyx_mstate_global->__pyx_kp_u_Invalid_file_object
 #define __pyx_kp_u_Parallelization_argument_must_be __pyx_mstate_global->__pyx_kp_u_Parallelization_argument_must_be
 #define __pyx_n_s_RapidgzipFile __pyx_mstate_global->__pyx_n_s_RapidgzipFile
 #define __pyx_n_s_RapidgzipFile_2 __pyx_mstate_global->__pyx_n_s_RapidgzipFile_2
 #define __pyx_n_s_RapidgzipFile___init __pyx_mstate_global->__pyx_n_s_RapidgzipFile___init
 #define __pyx_n_s_RapidgzipFile___reduce_cython __pyx_mstate_global->__pyx_n_s_RapidgzipFile___reduce_cython
@@ -3163,15 +3265,15 @@
 #define __pyx_n_s_RapidgzipFile_size __pyx_mstate_global->__pyx_n_s_RapidgzipFile_size
 #define __pyx_n_s_RapidgzipFile_tell __pyx_mstate_global->__pyx_n_s_RapidgzipFile_tell
 #define __pyx_n_s_RapidgzipFile_tell_compressed __pyx_mstate_global->__pyx_n_s_RapidgzipFile_tell_compressed
 #define __pyx_n_s_RawIOBase __pyx_mstate_global->__pyx_n_s_RawIOBase
 #define __pyx_n_s_SEEK_SET __pyx_mstate_global->__pyx_n_s_SEEK_SET
 #define __pyx_n_s_TypeError __pyx_mstate_global->__pyx_n_s_TypeError
 #define __pyx_n_s_UnsupportedOperation __pyx_mstate_global->__pyx_n_s_UnsupportedOperation
-#define __pyx_n_s__46 __pyx_mstate_global->__pyx_n_s__46
+#define __pyx_n_s__45 __pyx_mstate_global->__pyx_n_s__45
 #define __pyx_kp_u__6 __pyx_mstate_global->__pyx_kp_u__6
 #define __pyx_n_s__7 __pyx_mstate_global->__pyx_n_s__7
 #define __pyx_n_s_arg __pyx_mstate_global->__pyx_n_s_arg
 #define __pyx_n_s_args __pyx_mstate_global->__pyx_n_s_args
 #define __pyx_n_s_argv __pyx_mstate_global->__pyx_n_s_argv
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_available_block_offsets __pyx_mstate_global->__pyx_n_s_available_block_offsets
@@ -3278,15 +3380,14 @@
 #define __pyx_tuple__27 __pyx_mstate_global->__pyx_tuple__27
 #define __pyx_tuple__32 __pyx_mstate_global->__pyx_tuple__32
 #define __pyx_tuple__34 __pyx_mstate_global->__pyx_tuple__34
 #define __pyx_tuple__36 __pyx_mstate_global->__pyx_tuple__36
 #define __pyx_tuple__37 __pyx_mstate_global->__pyx_tuple__37
 #define __pyx_tuple__41 __pyx_mstate_global->__pyx_tuple__41
 #define __pyx_tuple__43 __pyx_mstate_global->__pyx_tuple__43
-#define __pyx_tuple__44 __pyx_mstate_global->__pyx_tuple__44
 #define __pyx_codeobj__9 __pyx_mstate_global->__pyx_codeobj__9
 #define __pyx_codeobj__11 __pyx_mstate_global->__pyx_codeobj__11
 #define __pyx_codeobj__13 __pyx_mstate_global->__pyx_codeobj__13
 #define __pyx_codeobj__14 __pyx_mstate_global->__pyx_codeobj__14
 #define __pyx_codeobj__15 __pyx_mstate_global->__pyx_codeobj__15
 #define __pyx_codeobj__16 __pyx_mstate_global->__pyx_codeobj__16
 #define __pyx_codeobj__18 __pyx_mstate_global->__pyx_codeobj__18
@@ -3303,15 +3404,15 @@
 #define __pyx_codeobj__31 __pyx_mstate_global->__pyx_codeobj__31
 #define __pyx_codeobj__33 __pyx_mstate_global->__pyx_codeobj__33
 #define __pyx_codeobj__35 __pyx_mstate_global->__pyx_codeobj__35
 #define __pyx_codeobj__38 __pyx_mstate_global->__pyx_codeobj__38
 #define __pyx_codeobj__39 __pyx_mstate_global->__pyx_codeobj__39
 #define __pyx_codeobj__40 __pyx_mstate_global->__pyx_codeobj__40
 #define __pyx_codeobj__42 __pyx_mstate_global->__pyx_codeobj__42
-#define __pyx_codeobj__45 __pyx_mstate_global->__pyx_codeobj__45
+#define __pyx_codeobj__44 __pyx_mstate_global->__pyx_codeobj__44
 /* #### Code section: module_code ### */
 
 /* "string.from_py":13
  * 
  * @cname("__pyx_convert_string_from_py_std__in_string")
  * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t length = 0
@@ -3525,38 +3626,50 @@
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_file = 0;
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[1] = {0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_isFileObject (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 64, __pyx_L3_error)
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_file,0};
-    PyObject* values[1] = {0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_file)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_file)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 64, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_isFileObject") < 0)) __PYX_ERR(0, 64, __pyx_L3_error)
       }
@@ -3566,22 +3679,35 @@
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_file = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("_isFileObject", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 64, __pyx_L3_error)
+  goto __pyx_L3_error;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("rapidgzip._isFileObject", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9rapidgzip__isFileObject(__pyx_self, __pyx_v_file);
 
   /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9rapidgzip__isFileObject(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_file) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
@@ -3808,38 +3934,50 @@
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_file = 0;
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[1] = {0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_hasValidFileno (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 72, __pyx_L3_error)
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_file,0};
-    PyObject* values[1] = {0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_file)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_file)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 72, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_hasValidFileno") < 0)) __PYX_ERR(0, 72, __pyx_L3_error)
       }
@@ -3849,22 +3987,35 @@
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_file = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("_hasValidFileno", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 72, __pyx_L3_error)
+  goto __pyx_L3_error;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("rapidgzip._hasValidFileno", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9rapidgzip_2_hasValidFileno(__pyx_self, __pyx_v_file);
 
   /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9rapidgzip_2_hasValidFileno(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_file) {
   PyObject *__pyx_v_fileno = NULL;
   PyObject *__pyx_r = NULL;
@@ -3938,24 +4089,26 @@
  *         return isinstance(fileno, int) and fileno >= 0
  *     except Exception:
  */
       __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_file, __pyx_n_s_fileno); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 77, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_8 = NULL;
       __pyx_t_9 = 0;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
+      #if CYTHON_UNPACK_METHODS
+      if (likely(PyMethod_Check(__pyx_t_7))) {
         __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
         if (likely(__pyx_t_8)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
           __Pyx_INCREF(__pyx_t_8);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_7, function);
           __pyx_t_9 = 1;
         }
       }
+      #endif
       {
         PyObject *__pyx_callargs[1] = {__pyx_t_8, };
         __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_9, 0+__pyx_t_9);
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
         if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 77, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
@@ -4093,26 +4246,33 @@
 
 /* Python wrapper */
 static int __pyx_pw_9rapidgzip_14_RapidgzipFile_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_9rapidgzip_14_RapidgzipFile_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_file = 0;
   PyObject *__pyx_v_parallelization = 0;
   PyObject *__pyx_v_verbose = 0;
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[3] = {0,0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 86, __pyx_L3_error)
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_file,&__pyx_n_s_parallelization,&__pyx_n_s_verbose,0};
-    PyObject* values[3] = {0,0,0};
-    values[2] = ((PyObject *)Py_False);
+    values[2] = __Pyx_Arg_NewRef_VARARGS(((PyObject *)Py_False));
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  3: values[2] = __Pyx_Arg_VARARGS(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = __Pyx_Arg_VARARGS(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -4120,29 +4280,35 @@
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_file)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_file)) != 0)) {
+          (void)__Pyx_Arg_NewRef_VARARGS(values[0]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 86, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallelization)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallelization)) != 0)) {
+          (void)__Pyx_Arg_NewRef_VARARGS(values[1]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 86, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 2, 3, 1); __PYX_ERR(0, 86, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_verbose);
-          if (value) { values[2] = value; kw_args--; }
+          if (value) { values[2] = __Pyx_Arg_NewRef_VARARGS(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 86, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__cinit__") < 0)) __PYX_ERR(0, 86, __pyx_L3_error)
       }
@@ -4159,22 +4325,35 @@
     __pyx_v_file = values[0];
     __pyx_v_parallelization = values[1];
     __pyx_v_verbose = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 2, 3, __pyx_nargs); __PYX_ERR(0, 86, __pyx_L3_error)
+  goto __pyx_L3_error;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("rapidgzip._RapidgzipFile.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9rapidgzip_14_RapidgzipFile___cinit__(((struct __pyx_obj_9rapidgzip__RapidgzipFile *)__pyx_v_self), __pyx_v_file, __pyx_v_parallelization, __pyx_v_verbose);
 
   /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static int __pyx_pf_9rapidgzip_14_RapidgzipFile___cinit__(struct __pyx_obj_9rapidgzip__RapidgzipFile *__pyx_v_self, PyObject *__pyx_v_file, PyObject *__pyx_v_parallelization, PyObject *__pyx_v_verbose) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
@@ -4323,24 +4502,26 @@
  *                 self.gzipReaderVerbose = new ParallelGzipReaderVerbose(<int>file.fileno(), <int>parallelization)
  *             elif _isFileObject(file):
  */
     __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_hasValidFileno); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 102, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_10 = NULL;
     __pyx_t_8 = 0;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
+    #if CYTHON_UNPACK_METHODS
+    if (unlikely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_10)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_10);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
         __pyx_t_8 = 1;
       }
     }
+    #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_10, __pyx_v_file};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
       if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 102, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
@@ -4356,24 +4537,26 @@
  *             elif _isFileObject(file):
  *                 self.gzipReaderVerbose = new ParallelGzipReaderVerbose(<PyObject*>file, <int>parallelization)
  */
       __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_file, __pyx_n_s_fileno); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 103, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_10 = NULL;
       __pyx_t_8 = 0;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
+      #if CYTHON_UNPACK_METHODS
+      if (likely(PyMethod_Check(__pyx_t_6))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_6);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
           __Pyx_INCREF(__pyx_t_10);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_6, function);
           __pyx_t_8 = 1;
         }
       }
+      #endif
       {
         PyObject *__pyx_callargs[1] = {__pyx_t_10, };
         __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 0+__pyx_t_8);
         __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
         if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 103, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
@@ -4406,24 +4589,26 @@
  *                 self.gzipReaderVerbose = new ParallelGzipReaderVerbose(<PyObject*>file, <int>parallelization)
  *             elif isinstance(file, basestring) and hasattr(file, 'encode'):
  */
     __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_isFileObject); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 104, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_10 = NULL;
     __pyx_t_7 = 0;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
+    #if CYTHON_UNPACK_METHODS
+    if (unlikely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_10)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_10);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
         __pyx_t_7 = 1;
       }
     }
+    #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_10, __pyx_v_file};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
       if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 104, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
@@ -4483,24 +4668,26 @@
  *         else:
  *             if isinstance(file, int):
  */
       __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_file, __pyx_n_s_encode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 108, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_10 = NULL;
       __pyx_t_7 = 0;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
+      #if CYTHON_UNPACK_METHODS
+      if (likely(PyMethod_Check(__pyx_t_6))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_6);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
           __Pyx_INCREF(__pyx_t_10);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_6, function);
           __pyx_t_7 = 1;
         }
       }
+      #endif
       {
         PyObject *__pyx_callargs[1] = {__pyx_t_10, };
         __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_7, 0+__pyx_t_7);
         __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
         if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 108, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
@@ -4581,24 +4768,26 @@
  *                 self.gzipReader = new ParallelGzipReaderNonVerbose(<int>file.fileno(), <int>parallelization)
  *             elif _isFileObject(file):
  */
     __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_hasValidFileno); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 112, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_10 = NULL;
     __pyx_t_8 = 0;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
+    #if CYTHON_UNPACK_METHODS
+    if (unlikely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_10)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_10);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
         __pyx_t_8 = 1;
       }
     }
+    #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_10, __pyx_v_file};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
       if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 112, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
@@ -4614,24 +4803,26 @@
  *             elif _isFileObject(file):
  *                 self.gzipReader = new ParallelGzipReaderNonVerbose(<PyObject*>file, <int>parallelization)
  */
       __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_file, __pyx_n_s_fileno); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 113, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_10 = NULL;
       __pyx_t_8 = 0;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
+      #if CYTHON_UNPACK_METHODS
+      if (likely(PyMethod_Check(__pyx_t_6))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_6);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
           __Pyx_INCREF(__pyx_t_10);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_6, function);
           __pyx_t_8 = 1;
         }
       }
+      #endif
       {
         PyObject *__pyx_callargs[1] = {__pyx_t_10, };
         __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 0+__pyx_t_8);
         __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
         if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 113, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
@@ -4664,24 +4855,26 @@
  *                 self.gzipReader = new ParallelGzipReaderNonVerbose(<PyObject*>file, <int>parallelization)
  *             elif isinstance(file, basestring) and hasattr(file, 'encode'):
  */
     __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_isFileObject); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 114, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_10 = NULL;
     __pyx_t_7 = 0;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
+    #if CYTHON_UNPACK_METHODS
+    if (unlikely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_10)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_10);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
         __pyx_t_7 = 1;
       }
     }
+    #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_10, __pyx_v_file};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
       if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 114, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
@@ -4741,24 +4934,26 @@
  * 
  *         if self.gzipReader == NULL and self.gzipReaderVerbose == NULL:
  */
       __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_file, __pyx_n_s_encode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 118, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_10 = NULL;
       __pyx_t_7 = 0;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
+      #if CYTHON_UNPACK_METHODS
+      if (likely(PyMethod_Check(__pyx_t_6))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_6);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
           __Pyx_INCREF(__pyx_t_10);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_6, function);
           __pyx_t_7 = 1;
         }
       }
+      #endif
       {
         PyObject *__pyx_callargs[1] = {__pyx_t_10, };
         __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_7, 0+__pyx_t_7);
         __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
         if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 118, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
@@ -4857,22 +5052,41 @@
  */
 
 /* Python wrapper */
 static int __pyx_pw_9rapidgzip_14_RapidgzipFile_3__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_9rapidgzip_14_RapidgzipFile_3__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED PyObject *__pyx_v_args = 0;
   CYTHON_UNUSED PyObject *__pyx_v_kwargs = 0;
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 125, __pyx_L3_error)
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__init__", 1))) return -1;
   __Pyx_INCREF(__pyx_args);
   __pyx_v_args = __pyx_args;
+  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L3_error;
+  __pyx_L3_error:;
+  __Pyx_DECREF(__pyx_v_args); __pyx_v_args = 0;
+  __Pyx_XDECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
+  __Pyx_AddTraceback("rapidgzip._RapidgzipFile.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return -1;
+  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9rapidgzip_14_RapidgzipFile_2__init__(((struct __pyx_obj_9rapidgzip__RapidgzipFile *)__pyx_v_self), __pyx_v_args, __pyx_v_kwargs);
 
   /* function exit code */
   __Pyx_DECREF(__pyx_v_args);
   __Pyx_XDECREF(__pyx_v_kwargs);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
@@ -4896,17 +5110,18 @@
  *         self.close()
  * 
  */
 
 /* Python wrapper */
 static void __pyx_pw_9rapidgzip_14_RapidgzipFile_5__dealloc__(PyObject *__pyx_v_self); /*proto*/
 static void __pyx_pw_9rapidgzip_14_RapidgzipFile_5__dealloc__(PyObject *__pyx_v_self) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_pf_9rapidgzip_14_RapidgzipFile_4__dealloc__(((struct __pyx_obj_9rapidgzip__RapidgzipFile *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_pf_9rapidgzip_14_RapidgzipFile_4__dealloc__(struct __pyx_obj_9rapidgzip__RapidgzipFile *__pyx_v_self) {
@@ -4928,24 +5143,26 @@
  * 
  *         if self.gzipReader:
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+  #if CYTHON_UNPACK_METHODS
+  if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_4 = 1;
     }
   }
+  #endif
   {
     PyObject *__pyx_callargs[1] = {__pyx_t_3, };
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
@@ -5066,23 +5283,42 @@
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("close (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 139, __pyx_L3_error)
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("close", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "close", 0))) return NULL;
+  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L3_error;
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("rapidgzip._RapidgzipFile.close", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9rapidgzip_14_RapidgzipFile_6close(((struct __pyx_obj_9rapidgzip__RapidgzipFile *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -5232,23 +5468,42 @@
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("closed (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 145, __pyx_L3_error)
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("closed", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "closed", 0))) return NULL;
+  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L3_error;
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("rapidgzip._RapidgzipFile.closed", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9rapidgzip_14_RapidgzipFile_8closed(((struct __pyx_obj_9rapidgzip__RapidgzipFile *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -5373,23 +5628,42 @@
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("fileno (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 151, __pyx_L3_error)
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("fileno", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "fileno", 0))) return NULL;
+  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L3_error;
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("rapidgzip._RapidgzipFile.fileno", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9rapidgzip_14_RapidgzipFile_10fileno(((struct __pyx_obj_9rapidgzip__RapidgzipFile *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -5535,23 +5809,42 @@
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("seekable (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 158, __pyx_L3_error)
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("seekable", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "seekable", 0))) return NULL;
+  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L3_error;
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("rapidgzip._RapidgzipFile.seekable", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9rapidgzip_14_RapidgzipFile_12seekable(((struct __pyx_obj_9rapidgzip__RapidgzipFile *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -5677,38 +5970,50 @@
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_bytes_like = 0;
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[1] = {0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("readinto (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 164, __pyx_L3_error)
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_bytes_like,0};
-    PyObject* values[1] = {0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_bytes_like)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_bytes_like)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 164, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "readinto") < 0)) __PYX_ERR(0, 164, __pyx_L3_error)
       }
@@ -5718,22 +6023,35 @@
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_bytes_like = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("readinto", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 164, __pyx_L3_error)
+  goto __pyx_L3_error;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("rapidgzip._RapidgzipFile.readinto", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9rapidgzip_14_RapidgzipFile_14readinto(((struct __pyx_obj_9rapidgzip__RapidgzipFile *)__pyx_v_self), __pyx_v_bytes_like);
 
   /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9rapidgzip_14_RapidgzipFile_14readinto(struct __pyx_obj_9rapidgzip__RapidgzipFile *__pyx_v_self, PyObject *__pyx_v_bytes_like) {
   long __pyx_v_bytes_count;
   Py_buffer __pyx_v_buffer;
@@ -5983,48 +6301,60 @@
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_offset = 0;
   PyObject *__pyx_v_whence = 0;
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[2] = {0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("seek (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 182, __pyx_L3_error)
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_offset,&__pyx_n_s_whence,0};
-    PyObject* values[2] = {0,0};
-    values[1] = __pyx_k__4;
+    values[1] = __Pyx_Arg_NewRef_FASTCALL(__pyx_k__4);
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_offset)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_offset)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 182, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_whence);
-          if (value) { values[1] = value; kw_args--; }
+          if (value) { values[1] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 182, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "seek") < 0)) __PYX_ERR(0, 182, __pyx_L3_error)
       }
@@ -6039,22 +6369,35 @@
     }
     __pyx_v_offset = values[0];
     __pyx_v_whence = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("seek", 0, 1, 2, __pyx_nargs); __PYX_ERR(0, 182, __pyx_L3_error)
+  goto __pyx_L3_error;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("rapidgzip._RapidgzipFile.seek", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9rapidgzip_14_RapidgzipFile_16seek(((struct __pyx_obj_9rapidgzip__RapidgzipFile *)__pyx_v_self), __pyx_v_offset, __pyx_v_whence);
 
   /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9rapidgzip_14_RapidgzipFile_16seek(struct __pyx_obj_9rapidgzip__RapidgzipFile *__pyx_v_self, PyObject *__pyx_v_offset, PyObject *__pyx_v_whence) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
@@ -6203,23 +6546,42 @@
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("tell (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 189, __pyx_L3_error)
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("tell", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "tell", 0))) return NULL;
+  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L3_error;
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("rapidgzip._RapidgzipFile.tell", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9rapidgzip_14_RapidgzipFile_18tell(((struct __pyx_obj_9rapidgzip__RapidgzipFile *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -6365,23 +6727,42 @@
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("size (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 196, __pyx_L3_error)
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("size", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "size", 0))) return NULL;
+  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L3_error;
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("rapidgzip._RapidgzipFile.size", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9rapidgzip_14_RapidgzipFile_20size(((struct __pyx_obj_9rapidgzip__RapidgzipFile *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -6527,23 +6908,42 @@
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("tell_compressed (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 203, __pyx_L3_error)
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("tell_compressed", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "tell_compressed", 0))) return NULL;
+  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L3_error;
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("rapidgzip._RapidgzipFile.tell_compressed", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9rapidgzip_14_RapidgzipFile_22tell_compressed(((struct __pyx_obj_9rapidgzip__RapidgzipFile *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -6689,23 +7089,42 @@
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("block_offsets_complete (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 210, __pyx_L3_error)
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("block_offsets_complete", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "block_offsets_complete", 0))) return NULL;
+  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L3_error;
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("rapidgzip._RapidgzipFile.block_offsets_complete", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9rapidgzip_14_RapidgzipFile_24block_offsets_complete(((struct __pyx_obj_9rapidgzip__RapidgzipFile *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -6851,23 +7270,42 @@
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("block_offsets (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 217, __pyx_L3_error)
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("block_offsets", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "block_offsets", 0))) return NULL;
+  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L3_error;
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("rapidgzip._RapidgzipFile.block_offsets", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9rapidgzip_14_RapidgzipFile_26block_offsets(((struct __pyx_obj_9rapidgzip__RapidgzipFile *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -7014,23 +7452,42 @@
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("available_block_offsets (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 224, __pyx_L3_error)
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("available_block_offsets", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "available_block_offsets", 0))) return NULL;
+  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L3_error;
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("rapidgzip._RapidgzipFile.available_block_offsets", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9rapidgzip_14_RapidgzipFile_28available_block_offsets(((struct __pyx_obj_9rapidgzip__RapidgzipFile *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -7178,38 +7635,50 @@
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_file = 0;
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[1] = {0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("import_index (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 231, __pyx_L3_error)
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_file,0};
-    PyObject* values[1] = {0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_file)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_file)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 231, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "import_index") < 0)) __PYX_ERR(0, 231, __pyx_L3_error)
       }
@@ -7219,22 +7688,35 @@
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_file = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("import_index", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 231, __pyx_L3_error)
+  goto __pyx_L3_error;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("rapidgzip._RapidgzipFile.import_index", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9rapidgzip_14_RapidgzipFile_30import_index(((struct __pyx_obj_9rapidgzip__RapidgzipFile *)__pyx_v_self), __pyx_v_file);
 
   /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9rapidgzip_14_RapidgzipFile_30import_index(struct __pyx_obj_9rapidgzip__RapidgzipFile *__pyx_v_self, PyObject *__pyx_v_file) {
   PyObject *__pyx_v_fileObject = NULL;
   PyObject *__pyx_r = NULL;
@@ -7287,48 +7769,52 @@
         __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_builtins); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 234, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_open); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 234, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_t_3 = NULL;
         __pyx_t_5 = 0;
-        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
+        #if CYTHON_UNPACK_METHODS
+        if (unlikely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_3)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
             __Pyx_INCREF(__pyx_t_3);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_4, function);
             __pyx_t_5 = 1;
           }
         }
+        #endif
         {
           PyObject *__pyx_callargs[3] = {__pyx_t_3, __pyx_v_file, __pyx_n_u_rb};
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 234, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         }
         __pyx_t_6 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_exit); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 234, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 234, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_3);
         __pyx_t_7 = NULL;
         __pyx_t_5 = 0;
-        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+        #if CYTHON_UNPACK_METHODS
+        if (likely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_7)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
             __Pyx_INCREF(__pyx_t_7);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
             __pyx_t_5 = 1;
           }
         }
+        #endif
         {
           PyObject *__pyx_callargs[1] = {__pyx_t_7, };
           __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
           if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 234, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
@@ -7533,48 +8019,52 @@
         __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_builtins); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 240, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_open); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 240, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_t_2 = NULL;
         __pyx_t_5 = 0;
-        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+        #if CYTHON_UNPACK_METHODS
+        if (unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_2)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
             __Pyx_INCREF(__pyx_t_2);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
             __pyx_t_5 = 1;
           }
         }
+        #endif
         {
           PyObject *__pyx_callargs[3] = {__pyx_t_2, __pyx_v_file, __pyx_n_u_rb};
           __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
           if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 240, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         }
         __pyx_t_6 = __Pyx_PyObject_LookupSpecial(__pyx_t_4, __pyx_n_s_exit); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 240, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_t_2 = __Pyx_PyObject_LookupSpecial(__pyx_t_4, __pyx_n_s_enter); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 240, __pyx_L21_error)
         __Pyx_GOTREF(__pyx_t_2);
         __pyx_t_7 = NULL;
         __pyx_t_5 = 0;
-        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+        #if CYTHON_UNPACK_METHODS
+        if (likely(PyMethod_Check(__pyx_t_2))) {
           __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
           if (likely(__pyx_t_7)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
             __Pyx_INCREF(__pyx_t_7);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_2, function);
             __pyx_t_5 = 1;
           }
         }
+        #endif
         {
           PyObject *__pyx_callargs[1] = {__pyx_t_7, };
           __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
           if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 240, __pyx_L21_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
@@ -7806,38 +8296,50 @@
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_file = 0;
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[1] = {0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("export_index (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 246, __pyx_L3_error)
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_file,0};
-    PyObject* values[1] = {0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_file)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_file)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 246, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "export_index") < 0)) __PYX_ERR(0, 246, __pyx_L3_error)
       }
@@ -7847,22 +8349,35 @@
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_file = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("export_index", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 246, __pyx_L3_error)
+  goto __pyx_L3_error;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("rapidgzip._RapidgzipFile.export_index", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9rapidgzip_14_RapidgzipFile_32export_index(((struct __pyx_obj_9rapidgzip__RapidgzipFile *)__pyx_v_self), __pyx_v_file);
 
   /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9rapidgzip_14_RapidgzipFile_32export_index(struct __pyx_obj_9rapidgzip__RapidgzipFile *__pyx_v_self, PyObject *__pyx_v_file) {
   PyObject *__pyx_v_fileObject = NULL;
   PyObject *__pyx_r = NULL;
@@ -7915,48 +8430,52 @@
         __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_builtins); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 249, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_open); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 249, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_t_3 = NULL;
         __pyx_t_5 = 0;
-        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
+        #if CYTHON_UNPACK_METHODS
+        if (unlikely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_3)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
             __Pyx_INCREF(__pyx_t_3);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_4, function);
             __pyx_t_5 = 1;
           }
         }
+        #endif
         {
           PyObject *__pyx_callargs[3] = {__pyx_t_3, __pyx_v_file, __pyx_n_u_wb};
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 249, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         }
         __pyx_t_6 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_exit); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 249, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 249, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_3);
         __pyx_t_7 = NULL;
         __pyx_t_5 = 0;
-        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+        #if CYTHON_UNPACK_METHODS
+        if (likely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_7)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
             __Pyx_INCREF(__pyx_t_7);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
             __pyx_t_5 = 1;
           }
         }
+        #endif
         {
           PyObject *__pyx_callargs[1] = {__pyx_t_7, };
           __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
           if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 249, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
@@ -8161,48 +8680,52 @@
         __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_builtins); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 255, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_open); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 255, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_t_2 = NULL;
         __pyx_t_5 = 0;
-        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+        #if CYTHON_UNPACK_METHODS
+        if (unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_2)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
             __Pyx_INCREF(__pyx_t_2);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
             __pyx_t_5 = 1;
           }
         }
+        #endif
         {
           PyObject *__pyx_callargs[3] = {__pyx_t_2, __pyx_v_file, __pyx_n_u_wb};
           __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
           if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 255, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         }
         __pyx_t_6 = __Pyx_PyObject_LookupSpecial(__pyx_t_4, __pyx_n_s_exit); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 255, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_t_2 = __Pyx_PyObject_LookupSpecial(__pyx_t_4, __pyx_n_s_enter); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 255, __pyx_L21_error)
         __Pyx_GOTREF(__pyx_t_2);
         __pyx_t_7 = NULL;
         __pyx_t_5 = 0;
-        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+        #if CYTHON_UNPACK_METHODS
+        if (likely(PyMethod_Check(__pyx_t_2))) {
           __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
           if (likely(__pyx_t_7)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
             __Pyx_INCREF(__pyx_t_7);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_2, function);
             __pyx_t_5 = 1;
           }
         }
+        #endif
         {
           PyObject *__pyx_callargs[1] = {__pyx_t_7, };
           __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
           if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 255, __pyx_L21_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
@@ -8433,23 +8956,42 @@
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("join_threads (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 261, __pyx_L3_error)
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("join_threads", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "join_threads", 0))) return NULL;
+  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L3_error;
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("rapidgzip._RapidgzipFile.join_threads", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9rapidgzip_14_RapidgzipFile_34join_threads(((struct __pyx_obj_9rapidgzip__RapidgzipFile *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -8581,23 +9123,42 @@
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 1, __pyx_L3_error)
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
+  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L3_error;
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("rapidgzip._RapidgzipFile.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9rapidgzip_14_RapidgzipFile_36__reduce_cython__(((struct __pyx_obj_9rapidgzip__RapidgzipFile *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -8654,38 +9215,50 @@
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   CYTHON_UNUSED PyObject *__pyx_v___pyx_state = 0;
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[1] = {0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 3, __pyx_L3_error)
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
-    PyObject* values[1] = {0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_state)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_state)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 3, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__setstate_cython__") < 0)) __PYX_ERR(1, 3, __pyx_L3_error)
       }
@@ -8695,22 +9268,35 @@
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v___pyx_state = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 3, __pyx_L3_error)
+  goto __pyx_L3_error;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("rapidgzip._RapidgzipFile.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9rapidgzip_14_RapidgzipFile_38__setstate_cython__(((struct __pyx_obj_9rapidgzip__RapidgzipFile *)__pyx_v_self), __pyx_v___pyx_state);
 
   /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9rapidgzip_14_RapidgzipFile_38__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_9rapidgzip__RapidgzipFile *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
@@ -8768,28 +9354,37 @@
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_filename = 0;
   PyObject *__pyx_v_parallelization = 0;
   PyObject *__pyx_v_verbose = 0;
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[4] = {0,0,0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 275, __pyx_L3_error)
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_filename,&__pyx_n_s_parallelization,&__pyx_n_s_verbose,0};
-    PyObject* values[4] = {0,0,0,0};
-    values[2] = ((PyObject *)((PyObject *)__pyx_int_0));
-    values[3] = ((PyObject *)((PyObject *)Py_False));
+    values[2] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)((PyObject *)__pyx_int_0)));
+    values[3] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)((PyObject *)Py_False)));
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
@@ -8799,36 +9394,42 @@
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 275, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_filename)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_filename)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 275, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 4, 1); __PYX_ERR(0, 275, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallelization);
-          if (value) { values[2] = value; kw_args--; }
+          if (value) { values[2] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 275, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_verbose);
-          if (value) { values[3] = value; kw_args--; }
+          if (value) { values[3] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 275, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 275, __pyx_L3_error)
       }
@@ -8848,22 +9449,35 @@
     __pyx_v_filename = values[1];
     __pyx_v_parallelization = values[2];
     __pyx_v_verbose = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 4, __pyx_nargs); __PYX_ERR(0, 275, __pyx_L3_error)
+  goto __pyx_L3_error;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("rapidgzip.RapidgzipFile.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9rapidgzip_13RapidgzipFile___init__(__pyx_self, __pyx_v_self, __pyx_v_filename, __pyx_v_parallelization, __pyx_v_verbose);
 
   /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9rapidgzip_13RapidgzipFile___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_filename, PyObject *__pyx_v_parallelization, PyObject *__pyx_v_verbose) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
@@ -8882,21 +9496,21 @@
  *         self.name = filename if isinstance(filename, str) else ""
  *         self.mode = 'rb'
  */
   __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 276, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_filename);
   __Pyx_GIVEREF(__pyx_v_filename);
-  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_filename);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_filename)) __PYX_ERR(0, 276, __pyx_L1_error);
   __Pyx_INCREF(__pyx_v_parallelization);
   __Pyx_GIVEREF(__pyx_v_parallelization);
-  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_parallelization);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_parallelization)) __PYX_ERR(0, 276, __pyx_L1_error);
   __Pyx_INCREF(__pyx_v_verbose);
   __Pyx_GIVEREF(__pyx_v_verbose);
-  PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_v_verbose);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_v_verbose)) __PYX_ERR(0, 276, __pyx_L1_error);
   __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile), __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 276, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_gzipReader, __pyx_t_2) < 0) __PYX_ERR(0, 276, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "rapidgzip.pyx":277
@@ -9172,38 +9786,50 @@
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[1] = {0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("fileno (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 298, __pyx_L3_error)
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,0};
-    PyObject* values[1] = {0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 298, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "fileno") < 0)) __PYX_ERR(0, 298, __pyx_L3_error)
       }
@@ -9213,22 +9839,35 @@
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("fileno", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 298, __pyx_L3_error)
+  goto __pyx_L3_error;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("rapidgzip.RapidgzipFile.fileno", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9rapidgzip_13RapidgzipFile_2fileno(__pyx_self, __pyx_v_self);
 
   /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9rapidgzip_13RapidgzipFile_2fileno(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_v_exception = NULL;
   PyObject *__pyx_r = NULL;
@@ -9283,24 +9922,26 @@
       __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_gzipReader); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 300, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_fileno); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 300, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_5 = NULL;
       __pyx_t_7 = 0;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
+      #if CYTHON_UNPACK_METHODS
+      if (likely(PyMethod_Check(__pyx_t_6))) {
         __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
         if (likely(__pyx_t_5)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_6, function);
           __pyx_t_7 = 1;
         }
       }
+      #endif
       {
         PyObject *__pyx_callargs[1] = {__pyx_t_5, };
         __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_7, 0+__pyx_t_7);
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 300, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
@@ -9350,24 +9991,26 @@
         __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_io); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 302, __pyx_L14_error)
         __Pyx_GOTREF(__pyx_t_9);
         __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_UnsupportedOperation); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 302, __pyx_L14_error)
         __Pyx_GOTREF(__pyx_t_10);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         __pyx_t_9 = NULL;
         __pyx_t_7 = 0;
-        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
+        #if CYTHON_UNPACK_METHODS
+        if (unlikely(PyMethod_Check(__pyx_t_10))) {
           __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_10);
           if (likely(__pyx_t_9)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
             __Pyx_INCREF(__pyx_t_9);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_10, function);
             __pyx_t_7 = 1;
           }
         }
+        #endif
         {
           PyObject *__pyx_callargs[1] = {__pyx_t_9, };
           __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_10, __pyx_callargs+1-__pyx_t_7, 0+__pyx_t_7);
           __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
           if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 302, __pyx_L14_error)
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
@@ -9491,38 +10134,50 @@
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[1] = {0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("close (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 304, __pyx_L3_error)
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,0};
-    PyObject* values[1] = {0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 304, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "close") < 0)) __PYX_ERR(0, 304, __pyx_L3_error)
       }
@@ -9532,22 +10187,35 @@
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("close", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 304, __pyx_L3_error)
+  goto __pyx_L3_error;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("rapidgzip.RapidgzipFile.close", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9rapidgzip_13RapidgzipFile_4close(__pyx_self, __pyx_v_self);
 
   /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9rapidgzip_13RapidgzipFile_4close(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
@@ -9603,37 +10271,39 @@
  */
   __pyx_t_3 = __Pyx_CyFunction_GetClassObj(__pyx_self);
   if (!__pyx_t_3) { PyErr_SetString(PyExc_SystemError, "super(): empty __class__ cell"); __PYX_ERR(0, 307, __pyx_L1_error) }
   __Pyx_INCREF(__pyx_t_3);
   __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 307, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_3);
-  PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3)) __PYX_ERR(0, 307, __pyx_L1_error);
   __Pyx_INCREF(__pyx_v_self);
   __Pyx_GIVEREF(__pyx_v_self);
-  PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_v_self);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_v_self)) __PYX_ERR(0, 307, __pyx_L1_error);
   __pyx_t_3 = 0;
   __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 307, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_close); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 307, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   __pyx_t_5 = 0;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
+  #if CYTHON_UNPACK_METHODS
+  if (likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
       __pyx_t_5 = 1;
     }
   }
+  #endif
   {
     PyObject *__pyx_callargs[1] = {__pyx_t_3, };
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 307, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
@@ -9650,24 +10320,26 @@
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_gzipReader); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 308, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_close); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 308, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+  #if CYTHON_UNPACK_METHODS
+  if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_5 = 1;
     }
   }
+  #endif
   {
     PyObject *__pyx_callargs[1] = {__pyx_t_4, };
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 308, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
@@ -9719,38 +10391,50 @@
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   CYTHON_UNUSED PyObject *__pyx_v_self = 0;
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[1] = {0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("readable (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 310, __pyx_L3_error)
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,0};
-    PyObject* values[1] = {0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 310, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "readable") < 0)) __PYX_ERR(0, 310, __pyx_L3_error)
       }
@@ -9760,22 +10444,35 @@
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("readable", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 310, __pyx_L3_error)
+  goto __pyx_L3_error;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("rapidgzip.RapidgzipFile.readable", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9rapidgzip_13RapidgzipFile_6readable(__pyx_self, __pyx_v_self);
 
   /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9rapidgzip_13RapidgzipFile_6readable(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
@@ -9833,28 +10530,37 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_filename = 0;
   PyObject *__pyx_v_parallelization = 0;
   PyObject *__pyx_v_verbose = 0;
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[3] = {0,0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("open (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args);
+  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 314, __pyx_L3_error)
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_filename,&__pyx_n_s_parallelization,&__pyx_n_s_verbose,0};
-    PyObject* values[3] = {0,0,0};
-    values[1] = ((PyObject *)((PyObject *)__pyx_int_0));
-    values[2] = ((PyObject *)((PyObject *)Py_False));
+    values[1] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)((PyObject *)__pyx_int_0)));
+    values[2] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)((PyObject *)Py_False)));
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -9862,29 +10568,32 @@
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_filename)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_filename)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 314, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parallelization);
-          if (value) { values[1] = value; kw_args--; }
+          if (value) { values[1] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 314, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_verbose);
-          if (value) { values[2] = value; kw_args--; }
+          if (value) { values[2] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 314, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "open") < 0)) __PYX_ERR(0, 314, __pyx_L3_error)
       }
@@ -9902,22 +10611,35 @@
     __pyx_v_filename = values[0];
     __pyx_v_parallelization = values[1];
     __pyx_v_verbose = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("open", 0, 1, 3, __pyx_nargs); __PYX_ERR(0, 314, __pyx_L3_error)
+  goto __pyx_L3_error;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("rapidgzip.open", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9rapidgzip_4open(__pyx_self, __pyx_v_filename, __pyx_v_parallelization, __pyx_v_verbose);
 
   /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9rapidgzip_4open(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filename, PyObject *__pyx_v_parallelization, PyObject *__pyx_v_verbose) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
@@ -9938,24 +10660,26 @@
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_RapidgzipFile); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 319, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+  #if CYTHON_UNPACK_METHODS
+  if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_4 = 1;
     }
   }
+  #endif
   {
     PyObject *__pyx_callargs[4] = {__pyx_t_3, __pyx_v_filename, __pyx_v_parallelization, __pyx_v_verbose};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 3+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 319, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
@@ -9993,18 +10717,19 @@
  *     cdef char** cargs = <char**> malloc(len(args) * sizeof(char*))
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_9rapidgzip_7cli(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static PyMethodDef __pyx_mdef_9rapidgzip_7cli = {"cli", (PyCFunction)__pyx_pw_9rapidgzip_7cli, METH_NOARGS, 0};
 static PyObject *__pyx_pw_9rapidgzip_7cli(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("cli (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_r = __pyx_pf_9rapidgzip_6cli(__pyx_self);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -10156,24 +10881,26 @@
  *             cargs[i] = <char*>buffers[i].buf
  * 
  */
       __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_encode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 330, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_7 = NULL;
       __pyx_t_8 = 0;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
+      #if CYTHON_UNPACK_METHODS
+      if (likely(PyMethod_Check(__pyx_t_6))) {
         __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
         if (likely(__pyx_t_7)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
           __Pyx_INCREF(__pyx_t_7);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_6, function);
           __pyx_t_8 = 1;
         }
       }
+      #endif
       {
         PyObject *__pyx_callargs[1] = {__pyx_t_7, };
         __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 0+__pyx_t_8);
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 330, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
@@ -10410,15 +11137,22 @@
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
     __pyx_pw_9rapidgzip_14_RapidgzipFile_5__dealloc__(o);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) - 1);
     PyErr_Restore(etype, eval, etb);
   }
+  #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
   (*Py_TYPE(o)->tp_free)(o);
+  #else
+  {
+    freefunc tp_free = (freefunc)PyType_GetSlot(Py_TYPE(o), Py_tp_free);
+    if (tp_free) tp_free(o);
+  }
+  #endif
 }
 
 static PyMethodDef __pyx_methods_9rapidgzip__RapidgzipFile[] = {
   {"close", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidgzip_14_RapidgzipFile_7close, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"closed", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidgzip_14_RapidgzipFile_9closed, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"fileno", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidgzip_14_RapidgzipFile_11fileno, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"seekable", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9rapidgzip_14_RapidgzipFile_13seekable, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
@@ -10549,15 +11283,15 @@
 #endif
 #endif
 /* #### Code section: pystring_table ### */
 
 static int __Pyx_CreateStringTabAndInitStrings(void) {
   __Pyx_StringTabEntry __pyx_string_tab[] = {
     {&__pyx_kp_u_, __pyx_k_, sizeof(__pyx_k_), 0, 1, 0, 0},
-    {&__pyx_kp_u_0_8_1, __pyx_k_0_8_1, sizeof(__pyx_k_0_8_1), 0, 1, 0, 0},
+    {&__pyx_kp_u_0_9_0, __pyx_k_0_9_0, sizeof(__pyx_k_0_9_0), 0, 1, 0, 0},
     {&__pyx_kp_u_Expected_file_name_string_file_d, __pyx_k_Expected_file_name_string_file_d, sizeof(__pyx_k_Expected_file_name_string_file_d), 0, 1, 0, 0},
     {&__pyx_kp_u_Invalid_file_object, __pyx_k_Invalid_file_object, sizeof(__pyx_k_Invalid_file_object), 0, 1, 0, 0},
     {&__pyx_kp_u_Parallelization_argument_must_be, __pyx_k_Parallelization_argument_must_be, sizeof(__pyx_k_Parallelization_argument_must_be), 0, 1, 0, 0},
     {&__pyx_n_s_RapidgzipFile, __pyx_k_RapidgzipFile, sizeof(__pyx_k_RapidgzipFile), 0, 0, 1, 1},
     {&__pyx_n_s_RapidgzipFile_2, __pyx_k_RapidgzipFile_2, sizeof(__pyx_k_RapidgzipFile_2), 0, 0, 1, 1},
     {&__pyx_n_s_RapidgzipFile___init, __pyx_k_RapidgzipFile___init, sizeof(__pyx_k_RapidgzipFile___init), 0, 0, 1, 1},
     {&__pyx_n_s_RapidgzipFile___reduce_cython, __pyx_k_RapidgzipFile___reduce_cython, sizeof(__pyx_k_RapidgzipFile___reduce_cython), 0, 0, 1, 1},
@@ -10580,15 +11314,15 @@
     {&__pyx_n_s_RapidgzipFile_size, __pyx_k_RapidgzipFile_size, sizeof(__pyx_k_RapidgzipFile_size), 0, 0, 1, 1},
     {&__pyx_n_s_RapidgzipFile_tell, __pyx_k_RapidgzipFile_tell, sizeof(__pyx_k_RapidgzipFile_tell), 0, 0, 1, 1},
     {&__pyx_n_s_RapidgzipFile_tell_compressed, __pyx_k_RapidgzipFile_tell_compressed, sizeof(__pyx_k_RapidgzipFile_tell_compressed), 0, 0, 1, 1},
     {&__pyx_n_s_RawIOBase, __pyx_k_RawIOBase, sizeof(__pyx_k_RawIOBase), 0, 0, 1, 1},
     {&__pyx_n_s_SEEK_SET, __pyx_k_SEEK_SET, sizeof(__pyx_k_SEEK_SET), 0, 0, 1, 1},
     {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
     {&__pyx_n_s_UnsupportedOperation, __pyx_k_UnsupportedOperation, sizeof(__pyx_k_UnsupportedOperation), 0, 0, 1, 1},
-    {&__pyx_n_s__46, __pyx_k__46, sizeof(__pyx_k__46), 0, 0, 1, 1},
+    {&__pyx_n_s__45, __pyx_k__45, sizeof(__pyx_k__45), 0, 0, 1, 1},
     {&__pyx_kp_u__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 1, 0, 0},
     {&__pyx_n_s__7, __pyx_k__7, sizeof(__pyx_k__7), 0, 0, 1, 1},
     {&__pyx_n_s_arg, __pyx_k_arg, sizeof(__pyx_k_arg), 0, 0, 1, 1},
     {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
     {&__pyx_n_s_argv, __pyx_k_argv, sizeof(__pyx_k_argv), 0, 0, 1, 1},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
     {&__pyx_n_s_available_block_offsets, __pyx_k_available_block_offsets, sizeof(__pyx_k_available_block_offsets), 0, 0, 1, 1},
@@ -10974,29 +11708,26 @@
  *     """
  *     filename: can be a file path, a file descriptor, or a file object
  */
   __pyx_tuple__41 = PyTuple_Pack(3, __pyx_n_s_filename, __pyx_n_s_parallelization, __pyx_n_s_verbose); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(0, 314, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__41);
   __Pyx_GIVEREF(__pyx_tuple__41);
   __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rapidgzip_pyx, __pyx_n_s_open, 314, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(0, 314, __pyx_L1_error)
-  __pyx_tuple__43 = PyTuple_Pack(2, ((PyObject *)__pyx_int_0), ((PyObject *)Py_False)); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 314, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__43);
-  __Pyx_GIVEREF(__pyx_tuple__43);
 
   /* "rapidgzip.pyx":322
  * 
  * 
  * def cli():             # <<<<<<<<<<<<<<
  *     args = sys.argv
  *     cdef char** cargs = <char**> malloc(len(args) * sizeof(char*))
  */
-  __pyx_tuple__44 = PyTuple_Pack(6, __pyx_n_s_args, __pyx_n_s_cargs, __pyx_n_s_buffers, __pyx_n_s_i, __pyx_n_s_arg, __pyx_n_s_buffer); if (unlikely(!__pyx_tuple__44)) __PYX_ERR(0, 322, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__44);
-  __Pyx_GIVEREF(__pyx_tuple__44);
-  __pyx_codeobj__45 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__44, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rapidgzip_pyx, __pyx_n_s_cli, 322, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__45)) __PYX_ERR(0, 322, __pyx_L1_error)
+  __pyx_tuple__43 = PyTuple_Pack(6, __pyx_n_s_args, __pyx_n_s_cargs, __pyx_n_s_buffers, __pyx_n_s_i, __pyx_n_s_arg, __pyx_n_s_buffer); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 322, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__43);
+  __Pyx_GIVEREF(__pyx_tuple__43);
+  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rapidgzip_pyx, __pyx_n_s_cli, 322, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 322, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -11091,23 +11822,23 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_0(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_2(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -11490,67 +12221,67 @@
  * 
  *     def close(self):             # <<<<<<<<<<<<<<
  *         if self.gzipReaderVerbose != NULL and not self.gzipReaderVerbose.closed():
  *             self.gzipReaderVerbose.close()
  */
   __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidgzip_14_RapidgzipFile_7close, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_RapidgzipFile_close, NULL, __pyx_n_s_rapidgzip, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile->tp_dict, __pyx_n_s_close, __pyx_t_2) < 0) __PYX_ERR(0, 139, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile, __pyx_n_s_close, __pyx_t_2) < 0) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9rapidgzip__RapidgzipFile);
 
   /* "rapidgzip.pyx":145
  *             self.gzipReader.close()
  * 
  *     def closed(self):             # <<<<<<<<<<<<<<
  *         return (
  *             ( self.gzipReader == NULL or self.gzipReader.closed() )
  */
   __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidgzip_14_RapidgzipFile_9closed, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_RapidgzipFile_closed, NULL, __pyx_n_s_rapidgzip, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 145, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile->tp_dict, __pyx_n_s_closed, __pyx_t_2) < 0) __PYX_ERR(0, 145, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile, __pyx_n_s_closed, __pyx_t_2) < 0) __PYX_ERR(0, 145, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9rapidgzip__RapidgzipFile);
 
   /* "rapidgzip.pyx":151
  *         )
  * 
  *     def fileno(self):             # <<<<<<<<<<<<<<
  *         if self.gzipReader:
  *             return self.gzipReader.fileno()
  */
   __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidgzip_14_RapidgzipFile_11fileno, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_RapidgzipFile_fileno, NULL, __pyx_n_s_rapidgzip, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile->tp_dict, __pyx_n_s_fileno, __pyx_t_2) < 0) __PYX_ERR(0, 151, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile, __pyx_n_s_fileno, __pyx_t_2) < 0) __PYX_ERR(0, 151, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9rapidgzip__RapidgzipFile);
 
   /* "rapidgzip.pyx":158
  *         raise Exception("Invalid file object!")
  * 
  *     def seekable(self):             # <<<<<<<<<<<<<<
  *         return (
  *             ( self.gzipReader != NULL and self.gzipReader.seekable() )
  */
   __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidgzip_14_RapidgzipFile_13seekable, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_RapidgzipFile_seekable, NULL, __pyx_n_s_rapidgzip, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 158, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile->tp_dict, __pyx_n_s_seekable, __pyx_t_2) < 0) __PYX_ERR(0, 158, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile, __pyx_n_s_seekable, __pyx_t_2) < 0) __PYX_ERR(0, 158, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9rapidgzip__RapidgzipFile);
 
   /* "rapidgzip.pyx":164
  *         )
  * 
  *     def readinto(self, bytes_like):             # <<<<<<<<<<<<<<
  *         if not self.gzipReader and not self.gzipReaderVerbose:
  *             raise Exception("Invalid file object!")
  */
   __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidgzip_14_RapidgzipFile_15readinto, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_RapidgzipFile_readinto, NULL, __pyx_n_s_rapidgzip, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile->tp_dict, __pyx_n_s_readinto, __pyx_t_2) < 0) __PYX_ERR(0, 164, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile, __pyx_n_s_readinto, __pyx_t_2) < 0) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9rapidgzip__RapidgzipFile);
 
   /* "rapidgzip.pyx":182
  *         return bytes_count
  * 
  *     def seek(self, offset, whence = io.SEEK_SET):             # <<<<<<<<<<<<<<
@@ -11569,138 +12300,138 @@
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_SEEK_SET); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 182, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 182, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2)) __PYX_ERR(0, 182, __pyx_L1_error);
   __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidgzip_14_RapidgzipFile_17seek, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_RapidgzipFile_seek, NULL, __pyx_n_s_rapidgzip, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 182, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile->tp_dict, __pyx_n_s_seek, __pyx_t_2) < 0) __PYX_ERR(0, 182, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile, __pyx_n_s_seek, __pyx_t_2) < 0) __PYX_ERR(0, 182, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9rapidgzip__RapidgzipFile);
 
   /* "rapidgzip.pyx":189
  *         raise Exception("Invalid file object!")
  * 
  *     def tell(self):             # <<<<<<<<<<<<<<
  *         if self.gzipReader:
  *             return self.gzipReader.tell()
  */
   __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidgzip_14_RapidgzipFile_19tell, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_RapidgzipFile_tell, NULL, __pyx_n_s_rapidgzip, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile->tp_dict, __pyx_n_s_tell, __pyx_t_2) < 0) __PYX_ERR(0, 189, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile, __pyx_n_s_tell, __pyx_t_2) < 0) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9rapidgzip__RapidgzipFile);
 
   /* "rapidgzip.pyx":196
  *         raise Exception("Invalid file object!")
  * 
  *     def size(self):             # <<<<<<<<<<<<<<
  *         if self.gzipReader:
  *             return self.gzipReader.size()
  */
   __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidgzip_14_RapidgzipFile_21size, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_RapidgzipFile_size, NULL, __pyx_n_s_rapidgzip, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile->tp_dict, __pyx_n_s_size, __pyx_t_2) < 0) __PYX_ERR(0, 196, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile, __pyx_n_s_size, __pyx_t_2) < 0) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9rapidgzip__RapidgzipFile);
 
   /* "rapidgzip.pyx":203
  *         raise Exception("Invalid file object!")
  * 
  *     def tell_compressed(self):             # <<<<<<<<<<<<<<
  *         if self.gzipReader:
  *             return self.gzipReader.tellCompressed()
  */
   __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidgzip_14_RapidgzipFile_23tell_compressed, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_RapidgzipFile_tell_compressed, NULL, __pyx_n_s_rapidgzip, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 203, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile->tp_dict, __pyx_n_s_tell_compressed, __pyx_t_2) < 0) __PYX_ERR(0, 203, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile, __pyx_n_s_tell_compressed, __pyx_t_2) < 0) __PYX_ERR(0, 203, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9rapidgzip__RapidgzipFile);
 
   /* "rapidgzip.pyx":210
  *         raise Exception("Invalid file object!")
  * 
  *     def block_offsets_complete(self):             # <<<<<<<<<<<<<<
  *         if self.gzipReader:
  *             return self.gzipReader.blockOffsetsComplete()
  */
   __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidgzip_14_RapidgzipFile_25block_offsets_complete, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_RapidgzipFile_block_offsets_com, NULL, __pyx_n_s_rapidgzip, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile->tp_dict, __pyx_n_s_block_offsets_complete, __pyx_t_2) < 0) __PYX_ERR(0, 210, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile, __pyx_n_s_block_offsets_complete, __pyx_t_2) < 0) __PYX_ERR(0, 210, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9rapidgzip__RapidgzipFile);
 
   /* "rapidgzip.pyx":217
  *         raise Exception("Invalid file object!")
  * 
  *     def block_offsets(self):             # <<<<<<<<<<<<<<
  *         if self.gzipReader:
  *             return self.gzipReader.blockOffsets()
  */
   __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidgzip_14_RapidgzipFile_27block_offsets, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_RapidgzipFile_block_offsets, NULL, __pyx_n_s_rapidgzip, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 217, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile->tp_dict, __pyx_n_s_block_offsets, __pyx_t_2) < 0) __PYX_ERR(0, 217, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile, __pyx_n_s_block_offsets, __pyx_t_2) < 0) __PYX_ERR(0, 217, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9rapidgzip__RapidgzipFile);
 
   /* "rapidgzip.pyx":224
  *         raise Exception("Invalid file object!")
  * 
  *     def available_block_offsets(self):             # <<<<<<<<<<<<<<
  *         if self.gzipReader:
  *             return self.gzipReader.availableBlockOffsets()
  */
   __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidgzip_14_RapidgzipFile_29available_block_offsets, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_RapidgzipFile_available_block_o, NULL, __pyx_n_s_rapidgzip, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 224, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile->tp_dict, __pyx_n_s_available_block_offsets, __pyx_t_2) < 0) __PYX_ERR(0, 224, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile, __pyx_n_s_available_block_offsets, __pyx_t_2) < 0) __PYX_ERR(0, 224, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9rapidgzip__RapidgzipFile);
 
   /* "rapidgzip.pyx":231
  *         raise Exception("Invalid file object!")
  * 
  *     def import_index(self, file):             # <<<<<<<<<<<<<<
  *         if self.gzipReader:
  *             if isinstance(file, str):
  */
   __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidgzip_14_RapidgzipFile_31import_index, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_RapidgzipFile_import_index, NULL, __pyx_n_s_rapidgzip, __pyx_d, ((PyObject *)__pyx_codeobj__28)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 231, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile->tp_dict, __pyx_n_s_import_index, __pyx_t_2) < 0) __PYX_ERR(0, 231, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile, __pyx_n_s_import_index, __pyx_t_2) < 0) __PYX_ERR(0, 231, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9rapidgzip__RapidgzipFile);
 
   /* "rapidgzip.pyx":246
  *         raise Exception("Invalid file object!")
  * 
  *     def export_index(self, file):             # <<<<<<<<<<<<<<
  *         if self.gzipReader:
  *             if isinstance(file, str):
  */
   __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidgzip_14_RapidgzipFile_33export_index, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_RapidgzipFile_export_index, NULL, __pyx_n_s_rapidgzip, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile->tp_dict, __pyx_n_s_export_index, __pyx_t_2) < 0) __PYX_ERR(0, 246, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile, __pyx_n_s_export_index, __pyx_t_2) < 0) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9rapidgzip__RapidgzipFile);
 
   /* "rapidgzip.pyx":261
  *         raise Exception("Invalid file object!")
  * 
  *     def join_threads(self):             # <<<<<<<<<<<<<<
  *         if self.gzipReader:
  *             return self.gzipReader.joinThreads()
  */
   __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidgzip_14_RapidgzipFile_35join_threads, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_RapidgzipFile_join_threads, NULL, __pyx_n_s_rapidgzip, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 261, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile->tp_dict, __pyx_n_s_join_threads, __pyx_t_2) < 0) __PYX_ERR(0, 261, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9rapidgzip__RapidgzipFile, __pyx_n_s_join_threads, __pyx_t_2) < 0) __PYX_ERR(0, 261, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9rapidgzip__RapidgzipFile);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
@@ -11732,15 +12463,15 @@
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_RawIOBase); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 274, __pyx_L1_error);
   __pyx_t_3 = 0;
   __pyx_t_3 = __Pyx_PEP560_update_bases(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_3, __pyx_n_s_RapidgzipFile, __pyx_n_s_RapidgzipFile, (PyObject *) NULL, __pyx_n_s_rapidgzip, (PyObject *) NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
@@ -11825,36 +12556,36 @@
  * 
  * def open(filename, parallelization = 0, verbose = False):             # <<<<<<<<<<<<<<
  *     """
  *     filename: can be a file path, a file descriptor, or a file object
  */
   __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidgzip_5open, 0, __pyx_n_s_open, NULL, __pyx_n_s_rapidgzip, __pyx_d, ((PyObject *)__pyx_codeobj__42)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 314, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__43);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__36);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_open, __pyx_t_3) < 0) __PYX_ERR(0, 314, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "rapidgzip.pyx":322
  * 
  * 
  * def cli():             # <<<<<<<<<<<<<<
  *     args = sys.argv
  *     cdef char** cargs = <char**> malloc(len(args) * sizeof(char*))
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidgzip_7cli, 0, __pyx_n_s_cli, NULL, __pyx_n_s_rapidgzip, __pyx_d, ((PyObject *)__pyx_codeobj__45)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 322, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9rapidgzip_7cli, 0, __pyx_n_s_cli, NULL, __pyx_n_s_rapidgzip, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 322, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_cli, __pyx_t_3) < 0) __PYX_ERR(0, 322, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "rapidgzip.pyx":340
  * 
  * 
- * __version__ = '0.8.1'             # <<<<<<<<<<<<<<
+ * __version__ = '0.9.0'             # <<<<<<<<<<<<<<
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_version, __pyx_kp_u_0_8_1) < 0) __PYX_ERR(0, 340, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_version, __pyx_kp_u_0_9_0) < 0) __PYX_ERR(0, 340, __pyx_L1_error)
 
   /* "rapidgzip.pyx":1
  * """             # <<<<<<<<<<<<<<
  * Cython wrapper for the GzipReader and ParallelGzipReader C++ classes.
  * """
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -12317,37 +13048,70 @@
 {
     PyObject *key = 0, *value = 0;
     Py_ssize_t pos = 0;
     PyObject*** name;
     PyObject*** first_kw_arg = argnames + num_pos_args;
     int kwds_is_tuple = CYTHON_METH_FASTCALL && likely(PyTuple_Check(kwds));
     while (1) {
+        Py_XDECREF(key); key = NULL;
+        Py_XDECREF(value); value = NULL;
         if (kwds_is_tuple) {
-            if (pos >= PyTuple_GET_SIZE(kwds)) break;
+            Py_ssize_t size;
+#if CYTHON_ASSUME_SAFE_MACROS
+            size = PyTuple_GET_SIZE(kwds);
+#else
+            size = PyTuple_Size(kwds);
+            if (size < 0) goto bad;
+#endif
+            if (pos >= size) break;
+#if CYTHON_AVOID_BORROWED_REFS
+            key = __Pyx_PySequence_ITEM(kwds, pos);
+            if (!key) goto bad;
+#elif CYTHON_ASSUME_SAFE_MACROS
             key = PyTuple_GET_ITEM(kwds, pos);
+#else
+            key = PyTuple_GetItem(kwds, pos);
+            if (!key) goto bad;
+#endif
             value = kwvalues[pos];
             pos++;
         }
         else
         {
             if (!PyDict_Next(kwds, &pos, &key, &value)) break;
+#if CYTHON_AVOID_BORROWED_REFS
+            Py_INCREF(key);
+#endif
         }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
+#if CYTHON_AVOID_BORROWED_REFS
+            Py_INCREF(value); // transfer ownership of value to values
+            Py_DECREF(key);
+#endif
+            key = NULL;
+            value = NULL;
             continue;
         }
+#if !CYTHON_AVOID_BORROWED_REFS
+        Py_INCREF(key);
+#endif
+        Py_INCREF(value);
         name = first_kw_arg;
         #if PY_MAJOR_VERSION < 3
         if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
+#if CYTHON_AVOID_BORROWED_REFS
+                    value = NULL;  // ownership transferred to values
+#endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
                 PyObject*** argname = argnames;
@@ -12369,14 +13133,17 @@
                     (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                 #endif
                     PyUnicode_Compare(**name, key)
                 );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
+#if CYTHON_AVOID_BORROWED_REFS
+                    value = NULL; // ownership transferred to values
+#endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
                 PyObject*** argname = argnames;
@@ -12395,14 +13162,16 @@
             goto invalid_keyword_type;
         if (kwds2) {
             if (unlikely(PyDict_SetItem(kwds2, key, value))) goto bad;
         } else {
             goto invalid_keyword;
         }
     }
+    Py_XDECREF(key);
+    Py_XDECREF(value);
     return 0;
 arg_passed_twice:
     __Pyx_RaiseDoubleKeywordsError(function_name, key);
     goto bad;
 invalid_keyword_type:
     PyErr_Format(PyExc_TypeError,
         "%.200s() keywords must be strings", function_name);
@@ -12414,14 +13183,16 @@
         function_name, PyString_AsString(key));
     #else
     PyErr_Format(PyExc_TypeError,
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
 bad:
+    Py_XDECREF(key);
+    Py_XDECREF(value);
     return -1;
 }
 
 /* RaiseArgTupleInvalid */
 static void __Pyx_RaiseArgtupleInvalid(
     const char* func_name,
     int exact,
@@ -12634,23 +13405,24 @@
     return result;
 }
 #endif
 
 /* PyObjectFastCall */
 static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
     PyObject *argstuple;
-    PyObject *result;
+    PyObject *result = 0;
     size_t i;
     argstuple = PyTuple_New((Py_ssize_t)nargs);
     if (unlikely(!argstuple)) return NULL;
     for (i = 0; i < nargs; i++) {
         Py_INCREF(args[i]);
-        PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]);
+        if (__Pyx_PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]) < 0) goto bad;
     }
     result = __Pyx_PyObject_Call(func, argstuple, kwargs);
+  bad:
     Py_DECREF(argstuple);
     return result;
 }
 static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t _nargs, PyObject *kwargs) {
     Py_ssize_t nargs = __Pyx_PyVectorcall_NARGS(_nargs);
 #if CYTHON_COMPILING_IN_CPYTHON
     if (nargs == 0 && kwargs == NULL) {
@@ -12692,15 +13464,19 @@
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
     }
     #endif
     #endif
     #if CYTHON_VECTORCALL
+    #if Py_VERSION_HEX < 0x03090000
     vectorcallfunc f = _PyVectorcall_Function(func);
+    #else
+    vectorcallfunc f = PyVectorcall_Function(func);
+    #endif
     if (f) {
         return f(func, args, (size_t)nargs, kwargs);
     }
     #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
     if (__Pyx_CyFunction_CheckExact(func)) {
         __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
         if (f) return f(func, args, (size_t)nargs, kwargs);
@@ -12926,15 +13702,17 @@
         if (unlikely((PY_SSIZE_T_MAX >> kind_shift) - ulength < char_pos))
             goto overflow;
         ukind = __Pyx_PyUnicode_KIND(uval);
         udata = __Pyx_PyUnicode_DATA(uval);
         if (!CYTHON_PEP393_ENABLED || ukind == result_ukind) {
             memcpy((char *)result_udata + (char_pos << kind_shift), udata, (size_t) (ulength << kind_shift));
         } else {
-            #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030300F0 || defined(_PyUnicode_FastCopyCharacters)
+            #if PY_VERSION_HEX >= 0x030D0000
+            if (unlikely(PyUnicode_CopyCharacters(result_uval, char_pos, uval, 0, ulength) < 0)) goto bad;
+            #elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030300F0 || defined(_PyUnicode_FastCopyCharacters)
             _PyUnicode_FastCopyCharacters(result_uval, char_pos, uval, 0, ulength);
             #else
             Py_ssize_t j;
             for (j=0; j < ulength; j++) {
                 Py_UCS4 uchar = __Pyx_PyUnicode_READ(ukind, udata, j);
                 __Pyx_PyUnicode_WRITE(result_ukind, result_udata, char_pos+j, uchar);
             }
@@ -13202,23 +13980,40 @@
     Py_ssize_t pos = 0;
 #if CYTHON_COMPILING_IN_PYPY
     if (!kw_allowed && PyDict_Next(kw, &pos, &key, 0))
         goto invalid_keyword;
     return 1;
 #else
     if (CYTHON_METH_FASTCALL && likely(PyTuple_Check(kw))) {
-        if (unlikely(PyTuple_GET_SIZE(kw) == 0))
+        Py_ssize_t kwsize;
+#if CYTHON_ASSUME_SAFE_MACROS
+        kwsize = PyTuple_GET_SIZE(kw);
+#else
+        kwsize = PyTuple_Size(kw);
+        if (kwsize < 0) return 0;
+#endif
+        if (unlikely(kwsize == 0))
             return 1;
         if (!kw_allowed) {
+#if CYTHON_ASSUME_SAFE_MACROS
             key = PyTuple_GET_ITEM(kw, 0);
+#else
+            key = PyTuple_GetItem(kw, pos);
+            if (!key) return 0;
+#endif
             goto invalid_keyword;
         }
 #if PY_VERSION_HEX < 0x03090000
-        for (pos = 0; pos < PyTuple_GET_SIZE(kw); pos++) {
+        for (pos = 0; pos < kwsize; pos++) {
+#if CYTHON_ASSUME_SAFE_MACROS
             key = PyTuple_GET_ITEM(kw, pos);
+#else
+            key = PyTuple_GetItem(kw, pos);
+            if (!key) return 0;
+#endif
             if (unlikely(!PyUnicode_Check(key)))
                 goto invalid_keyword_type;
         }
 #endif
         return 1;
     }
     while (PyDict_Next(kw, &pos, &key, 0)) {
@@ -13713,48 +14508,91 @@
 bad:
     return result;
 }
 
 /* ValidateBasesTuple */
 #if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API || CYTHON_USE_TYPE_SPECS
 static int __Pyx_validate_bases_tuple(const char *type_name, Py_ssize_t dictoffset, PyObject *bases) {
-    Py_ssize_t i, n = PyTuple_GET_SIZE(bases);
+    Py_ssize_t i, n;
+#if CYTHON_ASSUME_SAFE_MACROS
+    n = PyTuple_GET_SIZE(bases);
+#else
+    n = PyTuple_Size(bases);
+    if (n < 0) return -1;
+#endif
     for (i = 1; i < n; i++)
     {
+#if CYTHON_AVOID_BORROWED_REFS
+        PyObject *b0 = PySequence_GetItem(bases, i);
+        if (!b0) return -1;
+#elif CYTHON_ASSUME_SAFE_MACROS
         PyObject *b0 = PyTuple_GET_ITEM(bases, i);
+#else
+        PyObject *b0 = PyTuple_GetItem(bases, i);
+        if (!b0) return -1;
+#endif
         PyTypeObject *b;
 #if PY_MAJOR_VERSION < 3
         if (PyClass_Check(b0))
         {
             PyErr_Format(PyExc_TypeError, "base class '%.200s' is an old-style class",
                          PyString_AS_STRING(((PyClassObject*)b0)->cl_name));
+#if CYTHON_AVOID_BORROWED_REFS
+            Py_DECREF(b0);
+#endif
             return -1;
         }
 #endif
         b = (PyTypeObject*) b0;
         if (!__Pyx_PyType_HasFeature(b, Py_TPFLAGS_HEAPTYPE))
         {
             __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
             PyErr_Format(PyExc_TypeError,
                 "base class '" __Pyx_FMT_TYPENAME "' is not a heap type", b_name);
             __Pyx_DECREF_TypeName(b_name);
+#if CYTHON_AVOID_BORROWED_REFS
+            Py_DECREF(b0);
+#endif
             return -1;
         }
+#if !CYTHON_USE_TYPE_SLOTS
+        if (dictoffset == 0) {
+            PyErr_Format(PyExc_TypeError,
+                "extension type '%s.200s': "
+                "unable to validate whether bases have a __dict__ "
+                "when CYTHON_USE_TYPE_SLOTS is off "
+                "(likely because you are building in the limited API). "
+                "Therefore, all extension types with multiple bases "
+                "must add 'cdef dict __dict__' in this compilation mode",
+                type_name);
+#if CYTHON_AVOID_BORROWED_REFS
+            Py_DECREF(b0);
+#endif
+            return -1;
+        }
+#else
         if (dictoffset == 0 && b->tp_dictoffset)
         {
             __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
             PyErr_Format(PyExc_TypeError,
                 "extension type '%.200s' has no __dict__ slot, "
                 "but base type '" __Pyx_FMT_TYPENAME "' has: "
                 "either add 'cdef dict __dict__' to the extension type "
                 "or add '__slots__ = [...]' to the base type",
                 type_name, b_name);
             __Pyx_DECREF_TypeName(b_name);
+#if CYTHON_AVOID_BORROWED_REFS
+            Py_DECREF(b0);
+#endif
             return -1;
         }
+#endif
+#if CYTHON_AVOID_BORROWED_REFS
+        Py_DECREF(b0);
+#endif
     }
     return 0;
 }
 #endif
 
 /* PyType_Ready */
 static int __Pyx_PyType_Ready(PyTypeObject *t) {
@@ -13998,18 +14836,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_0
-#define __PYX_HAVE_RT_ImportType_3_0_0
-static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_2
+#define __PYX_HAVE_RT_ImportType_3_0_2
+static PyTypeObject *__Pyx_ImportType_3_0_2(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_2 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -14055,23 +14893,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_0 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_2 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_0 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_2 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -14101,21 +14939,16 @@
     empty_dict = PyDict_New();
     if (unlikely(!empty_dict))
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
             if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
-                #if CYTHON_COMPILING_IN_LIMITED_API
-                module = PyImport_ImportModuleLevelObject(
-                    name, empty_dict, empty_dict, from_list, 1);
-                #else
                 module = PyImport_ImportModuleLevelObject(
                     name, __pyx_d, empty_dict, from_list, 1);
-                #endif
                 if (unlikely(!module)) {
                     if (unlikely(!PyErr_ExceptionMatches(PyExc_ImportError)))
                         goto bad;
                     PyErr_Clear();
                 }
             }
             level = 0;
@@ -14126,22 +14959,17 @@
             PyObject *py_level = PyInt_FromLong(level);
             if (unlikely(!py_level))
                 goto bad;
             module = PyObject_CallFunctionObjArgs(py_import,
                 name, __pyx_d, empty_dict, from_list, py_level, (PyObject *)NULL);
             Py_DECREF(py_level);
             #else
-            #if CYTHON_COMPILING_IN_LIMITED_API
-            module = PyImport_ImportModuleLevelObject(
-                name, empty_dict, empty_dict, from_list, level);
-            #else
             module = PyImport_ImportModuleLevelObject(
                 name, __pyx_d, empty_dict, from_list, level);
             #endif
-            #endif
         }
     }
 bad:
     Py_XDECREF(empty_dict);
     Py_XDECREF(empty_list);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_import);
@@ -14440,41 +15268,46 @@
     }
     return __Pyx_PyVectorcall_FastCallDict_kw(func, vc, args, nargs, kw);
 }
 #endif
 
 /* CythonFunctionShared */
 static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj) {
-#if PY_VERSION_HEX < 0x030900B1
+#if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     __Pyx_Py_XDECREF_SET(
         __Pyx_CyFunction_GetClassObj(f),
             ((classobj) ? __Pyx_NewRef(classobj) : NULL));
 #else
     __Pyx_Py_XDECREF_SET(
         ((PyCMethodObject *) (f))->mm_class,
         (PyTypeObject*)((classobj) ? __Pyx_NewRef(classobj) : NULL));
 #endif
 }
 static PyObject *
 __Pyx_CyFunction_get_doc(__pyx_CyFunctionObject *op, void *closure)
 {
     CYTHON_UNUSED_VAR(closure);
     if (unlikely(op->func_doc == NULL)) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+        op->func_doc = PyObject_GetAttrString(op->func, "__doc__");
+        if (unlikely(!op->func_doc)) return NULL;
+#else
         if (((PyCFunctionObject*)op)->m_ml->ml_doc) {
 #if PY_MAJOR_VERSION >= 3
             op->func_doc = PyUnicode_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
 #else
             op->func_doc = PyString_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
 #endif
             if (unlikely(op->func_doc == NULL))
                 return NULL;
         } else {
             Py_INCREF(Py_None);
             return Py_None;
         }
+#endif
     }
     Py_INCREF(op->func_doc);
     return op->func_doc;
 }
 static int
 __Pyx_CyFunction_set_doc(__pyx_CyFunctionObject *op, PyObject *value, void *context)
 {
@@ -14487,15 +15320,17 @@
     return 0;
 }
 static PyObject *
 __Pyx_CyFunction_get_name(__pyx_CyFunctionObject *op, void *context)
 {
     CYTHON_UNUSED_VAR(context);
     if (unlikely(op->func_name == NULL)) {
-#if PY_MAJOR_VERSION >= 3
+#if CYTHON_COMPILING_IN_LIMITED_API
+        op->func_name = PyObject_GetAttrString(op->func, "__name__");
+#elif PY_MAJOR_VERSION >= 3
         op->func_name = PyUnicode_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
 #else
         op->func_name = PyString_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
 #endif
         if (unlikely(op->func_name == NULL))
             return NULL;
     }
@@ -14606,18 +15441,18 @@
         return -1;
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     op->defaults_tuple = PyTuple_GET_ITEM(res, 0);
     Py_INCREF(op->defaults_tuple);
     op->defaults_kwdict = PyTuple_GET_ITEM(res, 1);
     Py_INCREF(op->defaults_kwdict);
     #else
-    op->defaults_tuple = PySequence_ITEM(res, 0);
+    op->defaults_tuple = __Pyx_PySequence_ITEM(res, 0);
     if (unlikely(!op->defaults_tuple)) result = -1;
     else {
-        op->defaults_kwdict = PySequence_ITEM(res, 1);
+        op->defaults_kwdict = __Pyx_PySequence_ITEM(res, 1);
         if (unlikely(!op->defaults_kwdict)) result = -1;
     }
     #endif
     Py_DECREF(res);
     return result;
 }
 static int
@@ -14718,15 +15553,23 @@
     is_coroutine = op->flags & __Pyx_CYFUNCTION_COROUTINE;
 #if PY_VERSION_HEX >= 0x03050000
     if (is_coroutine) {
         PyObject *module, *fromlist, *marker = __pyx_n_s_is_coroutine;
         fromlist = PyList_New(1);
         if (unlikely(!fromlist)) return NULL;
         Py_INCREF(marker);
+#if CYTHON_ASSUME_SAFE_MACROS
         PyList_SET_ITEM(fromlist, 0, marker);
+#else
+        if (unlikely(PyList_SetItem(fromlist, 0, marker) < 0)) {
+            Py_DECREF(marker);
+            Py_DECREF(fromlist);
+            return NULL;
+        }
+#endif
         module = PyImport_ImportModuleLevelObject(__pyx_n_s_asyncio_coroutines, NULL, NULL, fromlist, 0);
         Py_DECREF(fromlist);
         if (unlikely(!module)) goto ignore;
         op->func_is_coroutine = __Pyx_PyObject_GetAttrStr(module, marker);
         Py_DECREF(module);
         if (likely(op->func_is_coroutine)) {
             return __Pyx_NewRef(op->func_is_coroutine);
@@ -14734,14 +15577,26 @@
 ignore:
         PyErr_Clear();
     }
 #endif
     op->func_is_coroutine = __Pyx_PyBool_FromLong(is_coroutine);
     return __Pyx_NewRef(op->func_is_coroutine);
 }
+#if CYTHON_COMPILING_IN_LIMITED_API
+static PyObject *
+__Pyx_CyFunction_get_module(__pyx_CyFunctionObject *op, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    return PyObject_GetAttrString(op->func, "__module__");
+}
+static int
+__Pyx_CyFunction_set_module(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    return PyObject_SetAttrString(op->func, "__module__", value);
+}
+#endif
 static PyGetSetDef __pyx_CyFunction_getsets[] = {
     {(char *) "func_doc", (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
     {(char *) "__doc__",  (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
     {(char *) "func_name", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
     {(char *) "__name__", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
     {(char *) "__qualname__", (getter)__Pyx_CyFunction_get_qualname, (setter)__Pyx_CyFunction_set_qualname, 0, 0},
     {(char *) "func_dict", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
@@ -14753,28 +15608,35 @@
     {(char *) "func_code", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
     {(char *) "__code__", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
     {(char *) "func_defaults", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
     {(char *) "__defaults__", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
     {(char *) "__kwdefaults__", (getter)__Pyx_CyFunction_get_kwdefaults, (setter)__Pyx_CyFunction_set_kwdefaults, 0, 0},
     {(char *) "__annotations__", (getter)__Pyx_CyFunction_get_annotations, (setter)__Pyx_CyFunction_set_annotations, 0, 0},
     {(char *) "_is_coroutine", (getter)__Pyx_CyFunction_get_is_coroutine, 0, 0, 0},
+#if CYTHON_COMPILING_IN_LIMITED_API
+    {"__module__", (getter)__Pyx_CyFunction_get_module, (setter)__Pyx_CyFunction_set_module, 0, 0},
+#endif
     {0, 0, 0, 0, 0}
 };
 static PyMemberDef __pyx_CyFunction_members[] = {
+#if !CYTHON_COMPILING_IN_LIMITED_API
     {(char *) "__module__", T_OBJECT, offsetof(PyCFunctionObject, m_module), 0, 0},
+#endif
 #if CYTHON_USE_TYPE_SPECS
     {(char *) "__dictoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_dict), READONLY, 0},
 #if CYTHON_METH_FASTCALL
 #if CYTHON_BACKPORT_VECTORCALL
     {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_vectorcall), READONLY, 0},
 #else
+#if !CYTHON_COMPILING_IN_LIMITED_API
     {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(PyCFunctionObject, vectorcall), READONLY, 0},
 #endif
 #endif
-#if PY_VERSION_HEX < 0x030500A0
+#endif
+#if PY_VERSION_HEX < 0x030500A0 || CYTHON_COMPILING_IN_LIMITED_API
     {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_weakreflist), READONLY, 0},
 #else
     {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(PyCFunctionObject, m_weakreflist), READONLY, 0},
 #endif
 #endif
     {0, 0, 0,  0, 0}
 };
@@ -14789,38 +15651,48 @@
     return PyString_FromString(((PyCFunctionObject*)m)->m_ml->ml_name);
 #endif
 }
 static PyMethodDef __pyx_CyFunction_methods[] = {
     {"__reduce__", (PyCFunction)__Pyx_CyFunction_reduce, METH_VARARGS, 0},
     {0, 0, 0, 0}
 };
-#if PY_VERSION_HEX < 0x030500A0
+#if PY_VERSION_HEX < 0x030500A0 || CYTHON_COMPILING_IN_LIMITED_API
 #define __Pyx_CyFunction_weakreflist(cyfunc) ((cyfunc)->func_weakreflist)
 #else
 #define __Pyx_CyFunction_weakreflist(cyfunc) (((PyCFunctionObject*)cyfunc)->m_weakreflist)
 #endif
 static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject *op, PyMethodDef *ml, int flags, PyObject* qualname,
                                        PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+#if !CYTHON_COMPILING_IN_LIMITED_API
     PyCFunctionObject *cf = (PyCFunctionObject*) op;
+#endif
     if (unlikely(op == NULL))
         return NULL;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    op->func = PyCFunction_NewEx(ml, (PyObject*)op, module);
+    if (unlikely(!op->func)) return NULL;
+#endif
     op->flags = flags;
     __Pyx_CyFunction_weakreflist(op) = NULL;
+#if !CYTHON_COMPILING_IN_LIMITED_API
     cf->m_ml = ml;
     cf->m_self = (PyObject *) op;
+#endif
     Py_XINCREF(closure);
     op->func_closure = closure;
+#if !CYTHON_COMPILING_IN_LIMITED_API
     Py_XINCREF(module);
     cf->m_module = module;
+#endif
     op->func_dict = NULL;
     op->func_name = NULL;
     Py_INCREF(qualname);
     op->func_qualname = qualname;
     op->func_doc = NULL;
-#if PY_VERSION_HEX < 0x030900B1
+#if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     op->func_classobj = NULL;
 #else
     ((PyCMethodObject*)op)->mm_class = NULL;
 #endif
     op->func_globals = globals;
     Py_INCREF(op->func_globals);
     Py_XINCREF(code);
@@ -14858,30 +15730,36 @@
 #endif
     return (PyObject *) op;
 }
 static int
 __Pyx_CyFunction_clear(__pyx_CyFunctionObject *m)
 {
     Py_CLEAR(m->func_closure);
+#if CYTHON_COMPILING_IN_LIMITED_API
+    Py_CLEAR(m->func);
+#else
     Py_CLEAR(((PyCFunctionObject*)m)->m_module);
+#endif
     Py_CLEAR(m->func_dict);
     Py_CLEAR(m->func_name);
     Py_CLEAR(m->func_qualname);
     Py_CLEAR(m->func_doc);
     Py_CLEAR(m->func_globals);
     Py_CLEAR(m->func_code);
+#if !CYTHON_COMPILING_IN_LIMITED_API
 #if PY_VERSION_HEX < 0x030900B1
     Py_CLEAR(__Pyx_CyFunction_GetClassObj(m));
 #else
     {
         PyObject *cls = (PyObject*) ((PyCMethodObject *) (m))->mm_class;
         ((PyCMethodObject *) (m))->mm_class = NULL;
         Py_XDECREF(cls);
     }
 #endif
+#endif
     Py_CLEAR(m->defaults_tuple);
     Py_CLEAR(m->defaults_kwdict);
     Py_CLEAR(m->func_annotations);
     Py_CLEAR(m->func_is_coroutine);
     if (m->defaults) {
         PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
         int i;
@@ -14903,22 +15781,28 @@
 {
     PyObject_GC_UnTrack(m);
     __Pyx__CyFunction_dealloc(m);
 }
 static int __Pyx_CyFunction_traverse(__pyx_CyFunctionObject *m, visitproc visit, void *arg)
 {
     Py_VISIT(m->func_closure);
+#if CYTHON_COMPILING_IN_LIMITED_API
+    Py_VISIT(m->func);
+#else
     Py_VISIT(((PyCFunctionObject*)m)->m_module);
+#endif
     Py_VISIT(m->func_dict);
     Py_VISIT(m->func_name);
     Py_VISIT(m->func_qualname);
     Py_VISIT(m->func_doc);
     Py_VISIT(m->func_globals);
     Py_VISIT(m->func_code);
+#if !CYTHON_COMPILING_IN_LIMITED_API
     Py_VISIT(__Pyx_CyFunction_GetClassObj(m));
+#endif
     Py_VISIT(m->defaults_tuple);
     Py_VISIT(m->defaults_kwdict);
     Py_VISIT(m->func_is_coroutine);
     if (m->defaults) {
         PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
         int i;
         for (i = 0; i < m->defaults_pyobjects; i++)
@@ -14934,67 +15818,123 @@
                                 op->func_qualname, (void *)op);
 #else
     return PyString_FromFormat("<cyfunction %s at %p>",
                                PyString_AsString(op->func_qualname), (void *)op);
 #endif
 }
 static PyObject * __Pyx_CyFunction_CallMethod(PyObject *func, PyObject *self, PyObject *arg, PyObject *kw) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+    PyObject *f = ((__pyx_CyFunctionObject*)func)->func;
+    PyObject *py_name = NULL;
+    PyCFunction meth;
+    int flags;
+    meth = PyCFunction_GetFunction(f);
+    if (unlikely(!meth)) return NULL;
+    flags = PyCFunction_GetFlags(f);
+    if (unlikely(flags < 0)) return NULL;
+#else
     PyCFunctionObject* f = (PyCFunctionObject*)func;
     PyCFunction meth = f->m_ml->ml_meth;
+    int flags = f->m_ml->ml_flags;
+#endif
     Py_ssize_t size;
-    switch (f->m_ml->ml_flags & (METH_VARARGS | METH_KEYWORDS | METH_NOARGS | METH_O)) {
+    switch (flags & (METH_VARARGS | METH_KEYWORDS | METH_NOARGS | METH_O)) {
     case METH_VARARGS:
         if (likely(kw == NULL || PyDict_Size(kw) == 0))
             return (*meth)(self, arg);
         break;
     case METH_VARARGS | METH_KEYWORDS:
         return (*(PyCFunctionWithKeywords)(void*)meth)(self, arg, kw);
     case METH_NOARGS:
         if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+#if CYTHON_ASSUME_SAFE_MACROS
             size = PyTuple_GET_SIZE(arg);
+#else
+            size = PyTuple_Size(arg);
+            if (unlikely(size < 0)) return NULL;
+#endif
             if (likely(size == 0))
                 return (*meth)(self, NULL);
+#if CYTHON_COMPILING_IN_LIMITED_API
+            py_name = __Pyx_CyFunction_get_name((__pyx_CyFunctionObject*)func, NULL);
+            if (!py_name) return NULL;
+            PyErr_Format(PyExc_TypeError,
+                "%.200S() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                py_name, size);
+            Py_DECREF(py_name);
+#else
             PyErr_Format(PyExc_TypeError,
                 "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
                 f->m_ml->ml_name, size);
+#endif
             return NULL;
         }
         break;
     case METH_O:
         if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+#if CYTHON_ASSUME_SAFE_MACROS
             size = PyTuple_GET_SIZE(arg);
+#else
+            size = PyTuple_Size(arg);
+            if (unlikely(size < 0)) return NULL;
+#endif
             if (likely(size == 1)) {
                 PyObject *result, *arg0;
                 #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
                 arg0 = PyTuple_GET_ITEM(arg, 0);
                 #else
-                arg0 = PySequence_ITEM(arg, 0); if (unlikely(!arg0)) return NULL;
+                arg0 = __Pyx_PySequence_ITEM(arg, 0); if (unlikely(!arg0)) return NULL;
                 #endif
                 result = (*meth)(self, arg0);
                 #if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
                 Py_DECREF(arg0);
                 #endif
                 return result;
             }
+#if CYTHON_COMPILING_IN_LIMITED_API
+            py_name = __Pyx_CyFunction_get_name((__pyx_CyFunctionObject*)func, NULL);
+            if (!py_name) return NULL;
+            PyErr_Format(PyExc_TypeError,
+                "%.200S() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                py_name, size);
+            Py_DECREF(py_name);
+#else
             PyErr_Format(PyExc_TypeError,
                 "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
                 f->m_ml->ml_name, size);
+#endif
             return NULL;
         }
         break;
     default:
         PyErr_SetString(PyExc_SystemError, "Bad call flags for CyFunction");
         return NULL;
     }
+#if CYTHON_COMPILING_IN_LIMITED_API
+    py_name = __Pyx_CyFunction_get_name((__pyx_CyFunctionObject*)func, NULL);
+    if (!py_name) return NULL;
+    PyErr_Format(PyExc_TypeError, "%.200S() takes no keyword arguments",
+                 py_name);
+    Py_DECREF(py_name);
+#else
     PyErr_Format(PyExc_TypeError, "%.200s() takes no keyword arguments",
                  f->m_ml->ml_name);
+#endif
     return NULL;
 }
 static CYTHON_INLINE PyObject *__Pyx_CyFunction_Call(PyObject *func, PyObject *arg, PyObject *kw) {
-    return __Pyx_CyFunction_CallMethod(func, ((PyCFunctionObject*)func)->m_self, arg, kw);
+    PyObject *self, *result;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    self = PyCFunction_GetSelf(((__pyx_CyFunctionObject*)func)->func);
+    if (unlikely(!self) && PyErr_Occurred()) return NULL;
+#else
+    self = ((PyCFunctionObject*)func)->m_self;
+#endif
+    result = __Pyx_CyFunction_CallMethod(func, self, arg, kw);
+    return result;
 }
 static PyObject *__Pyx_CyFunction_CallAsMethod(PyObject *func, PyObject *args, PyObject *kw) {
     PyObject *result;
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *) func;
 #if CYTHON_METH_FASTCALL
      __pyx_vectorcallfunc vc = __Pyx_CyFunction_func_vectorcall(cyfunc);
     if (vc) {
@@ -15006,15 +15946,20 @@
 #endif
     }
 #endif
     if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
         Py_ssize_t argc;
         PyObject *new_args;
         PyObject *self;
+#if CYTHON_ASSUME_SAFE_MACROS
         argc = PyTuple_GET_SIZE(args);
+#else
+        argc = PyTuple_Size(args);
+        if (unlikely(!argc) < 0) return NULL;
+#endif
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
 #if PY_MAJOR_VERSION > 2
@@ -15219,15 +16164,15 @@
     0,
     0,
     0,
     0,
 #ifdef Py_TPFLAGS_METHOD_DESCRIPTOR
     Py_TPFLAGS_METHOD_DESCRIPTOR |
 #endif
-#ifdef _Py_TPFLAGS_HAVE_VECTORCALL
+#if defined(_Py_TPFLAGS_HAVE_VECTORCALL) && CYTHON_METH_FASTCALL
     _Py_TPFLAGS_HAVE_VECTORCALL |
 #endif
     Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
     0,
     (traverseproc) __Pyx_CyFunction_traverse,
     (inquiry) __Pyx_CyFunction_clear,
     0,
@@ -15392,18 +16337,29 @@
 error:
     Py_XDECREF(new_bases);
     return NULL;
 }
 
 /* CalculateMetaclass */
 static PyObject *__Pyx_CalculateMetaclass(PyTypeObject *metaclass, PyObject *bases) {
-    Py_ssize_t i, nbases = PyTuple_GET_SIZE(bases);
+    Py_ssize_t i, nbases;
+#if CYTHON_ASSUME_SAFE_MACROS
+    nbases = PyTuple_GET_SIZE(bases);
+#else
+    nbases = PyTuple_Size(bases);
+    if (nbases < 0) return NULL;
+#endif
     for (i=0; i < nbases; i++) {
         PyTypeObject *tmptype;
+#if CYTHON_ASSUME_SAFE_MACROS
         PyObject *tmp = PyTuple_GET_ITEM(bases, i);
+#else
+        PyObject *tmp = PyTuple_GetItem(bases, i);
+        if (!tmp) return NULL;
+#endif
         tmptype = Py_TYPE(tmp);
 #if PY_MAJOR_VERSION < 3
         if (tmptype == &PyClass_Type)
             continue;
 #endif
         if (!metaclass) {
             metaclass = tmptype;
@@ -15791,28 +16747,99 @@
 }
 #endif
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
-#if PY_VERSION_HEX >= 0x030b00a6
+#if PY_VERSION_HEX >= 0x030b00a6 && !CYTHON_COMPILING_IN_LIMITED_API
   #ifndef Py_BUILD_CORE
     #define Py_BUILD_CORE 1
   #endif
   #include "internal/pycore_frame.h"
 #endif
 #if CYTHON_COMPILING_IN_LIMITED_API
+static PyObject *__Pyx_PyCode_Replace_For_AddTraceback(PyObject *code, PyObject *scratch_dict,
+                                                       PyObject *firstlineno, PyObject *name) {
+    PyObject *replace = NULL;
+    if (unlikely(PyDict_SetItemString(scratch_dict, "co_firstlineno", firstlineno))) return NULL;
+    if (unlikely(PyDict_SetItemString(scratch_dict, "co_name", name))) return NULL;
+    replace = PyObject_GetAttrString(code, "replace");
+    if (likely(replace)) {
+        PyObject *result;
+        result = PyObject_Call(replace, __pyx_empty_tuple, scratch_dict);
+        Py_DECREF(replace);
+        return result;
+    }
+    #if __PYX_LIMITED_VERSION_HEX < 0x030780000
+    PyErr_Clear();
+    {
+        PyObject *compiled = NULL, *result = NULL;
+        if (unlikely(PyDict_SetItemString(scratch_dict, "code", code))) return NULL;
+        if (unlikely(PyDict_SetItemString(scratch_dict, "type", (PyObject*)(&PyType_Type)))) return NULL;
+        compiled = Py_CompileString(
+            "out = type(code)(\n"
+            "  code.co_argcount, code.co_kwonlyargcount, code.co_nlocals, code.co_stacksize,\n"
+            "  code.co_flags, code.co_code, code.co_consts, code.co_names,\n"
+            "  code.co_varnames, code.co_filename, co_name, co_firstlineno,\n"
+            "  code.co_lnotab)\n", "<dummy>", Py_file_input);
+        if (!compiled) return NULL;
+        result = PyEval_EvalCode(compiled, scratch_dict, scratch_dict);
+        Py_DECREF(compiled);
+        if (!result) PyErr_Print();
+        Py_DECREF(result);
+        result = PyDict_GetItemString(scratch_dict, "out");
+        if (result) Py_INCREF(result);
+        return result;
+    }
+    #endif
+}
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
+    PyObject *code_object = NULL, *py_py_line = NULL, *py_funcname = NULL, *dict = NULL;
+    PyObject *replace = NULL, *getframe = NULL, *frame = NULL;
+    PyObject *exc_type, *exc_value, *exc_traceback;
+    int success = 0;
     if (c_line) {
         (void) __pyx_cfilenm;
         (void) __Pyx_CLineForTraceback(__Pyx_PyThreadState_Current, c_line);
     }
-    _PyTraceback_Add(funcname, filename, py_line);
+    PyErr_Fetch(&exc_type, &exc_value, &exc_traceback);
+    code_object = Py_CompileString("_getframe()", filename, Py_eval_input);
+    if (unlikely(!code_object)) goto bad;
+    py_py_line = PyLong_FromLong(py_line);
+    if (unlikely(!py_py_line)) goto bad;
+    py_funcname = PyUnicode_FromString(funcname);
+    if (unlikely(!py_funcname)) goto bad;
+    dict = PyDict_New();
+    if (unlikely(!dict)) goto bad;
+    {
+        PyObject *old_code_object = code_object;
+        code_object = __Pyx_PyCode_Replace_For_AddTraceback(code_object, dict, py_py_line, py_funcname);
+        Py_DECREF(old_code_object);
+    }
+    if (unlikely(!code_object)) goto bad;
+    getframe = PySys_GetObject("_getframe");
+    if (unlikely(!getframe)) goto bad;
+    if (unlikely(PyDict_SetItemString(dict, "_getframe", getframe))) goto bad;
+    frame = PyEval_EvalCode(code_object, dict, dict);
+    if (unlikely(!frame) || frame == Py_None) goto bad;
+    success = 1;
+  bad:
+    PyErr_Restore(exc_type, exc_value, exc_traceback);
+    Py_XDECREF(code_object);
+    Py_XDECREF(py_py_line);
+    Py_XDECREF(py_funcname);
+    Py_XDECREF(dict);
+    Py_XDECREF(replace);
+    if (success) {
+        PyTraceBack_Here(
+            (struct _frame*)frame);
+    }
+    Py_XDECREF(frame);
 }
 #else
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
@@ -16234,16 +17261,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
+#if !CYTHON_COMPILING_IN_LIMITED_API
         return _PyLong_FromByteArray(bytes, sizeof(int),
                                      little, !is_unsigned);
+#else
+        PyObject *from_bytes, *result = NULL;
+        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        if (!from_bytes) return NULL;
+        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(int));
+        if (!py_bytes) goto limited_bad;
+        order_str = PyUnicode_FromString(little ? "little" : "big");
+        if (!order_str) goto limited_bad;
+        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
+        if (!arg_tuple) goto limited_bad;
+        kwds = PyDict_New();
+        if (!kwds) goto limited_bad;
+        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        result = PyObject_Call(from_bytes, arg_tuple, kwds);
+        limited_bad:
+        Py_XDECREF(from_bytes);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(order_str);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(kwds);
+        return result;
+#endif
     }
 }
 
 /* CIntToPy */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
@@ -16272,16 +17323,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
+#if !CYTHON_COMPILING_IN_LIMITED_API
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
+#else
+        PyObject *from_bytes, *result = NULL;
+        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        if (!from_bytes) return NULL;
+        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(long));
+        if (!py_bytes) goto limited_bad;
+        order_str = PyUnicode_FromString(little ? "little" : "big");
+        if (!order_str) goto limited_bad;
+        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
+        if (!arg_tuple) goto limited_bad;
+        kwds = PyDict_New();
+        if (!kwds) goto limited_bad;
+        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        result = PyObject_Call(from_bytes, arg_tuple, kwds);
+        limited_bad:
+        Py_XDECREF(from_bytes);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(order_str);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(kwds);
+        return result;
+#endif
     }
 }
 
 /* CIntFromPy */
 static CYTHON_INLINE PY_LONG_LONG __Pyx_PyInt_As_PY_LONG_LONG(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
@@ -16832,15 +17907,16 @@
 static __Pyx_TypeName
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name_2);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
-        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__46));
+        Py_XDECREF(name);
+        name = __Pyx_NewRef(__pyx_n_s__45);
     }
     return name;
 }
 #endif
 
 /* CIntFromPy */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
```

### Comparing `rapidgzip-0.8.1/rapidgzip.egg-info/PKG-INFO` & `rapidgzip-0.9.0/rapidgzip.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidgzip
-Version: 0.8.1
+Version: 0.9.0
 Summary: Parallel random access to gzip files
 Home-page: https://github.com/mxmlnkn/rapidgzip
 Author: Maximilian Knespel
 Author-email: mxmlnkn@github.de
 License: MIT
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
@@ -36,15 +36,15 @@
 ![](https://raw.githubusercontent.com/mxmlnkn/indexed_bzip2/master/python/rapidgzip/rapidgzip.svg)
 
 # Rapidgzip: Parallelized Decompression of Gzip Files with Support for Fast Random Access
 
 [![PyPI version](https://badge.fury.io/py/rapidgzip.svg)](https://badge.fury.io/py/rapidgzip)
 [![Python Version](https://img.shields.io/pypi/pyversions/rapidgzip)](https://pypi.org/project/rapidgzip/)
 [![PyPI Platforms](https://img.shields.io/badge/pypi-linux%20%7C%20macOS%20%7C%20Windows-brightgreen)](https://pypi.org/project/rapidgzip/)
-[![Downloads](https://pepy.tech/badge/pragzip/month)](https://pepy.tech/project/rapidgzip)
+[![Downloads](https://static.pepy.tech/badge/rapidgzip/month)](https://pepy.tech/project/rapidgzip)
 <br>
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](http://opensource.org/licenses/MIT)
 [![Build Status](https://github.com/mxmlnkn/indexed_bzip2/workflows/tests/badge.svg)](https://github.com/mxmlnkn/rapidgzip/actions)
 [![codecov](https://codecov.io/gh/mxmlnkn/indexed_bzip2/branch/master/graph/badge.svg?token=94ZD4UTZQW)](https://codecov.io/gh/mxmlnkn/rapidgzip)
 ![C++17](https://img.shields.io/badge/C++-17-blue.svg)
 [![Discord](https://img.shields.io/discord/783411320354766878?label=discord)](https://discord.gg/Wra6t6akh2)
 [![Telegram](https://img.shields.io/badge/Chat-Telegram-%2330A3E6)](https://t.me/joinchat/FUdXxkXIv6c4Ib8bgaSxNg)
@@ -64,89 +64,46 @@
 This repository was created for visibility reasons and in order to keep indexed_bzip2 and rapidgzip releases separate.
 It will be updated at least for each release.
 Issues regarding rapidgzip should be opened [here](https://github.com/mxmlnkn/rapidgzip/issues).
 
 
 # Table of Contents
 
-1. [Performance](#performance-comparison-with-gzip-module)
-   1. [Decompression with Existing Index](#decompression-with-existing-index)
-   2. [Decompression from Scratch](#decompression-from-scratch)
-2. [Installation](#installation)
+1. [Installation](#installation)
+2. [Performance](#performance)
+   1. [Scaling Benchmarks on 2xAMD EPYC CPU 7702 (2x64 cores)](#scaling-benchmarks-on-2xamd-epyc-cpu-7702-2x64-cores)
+      1. [Decompression of Silesia Corpus](#decompression-of-silesia-corpus)
+      2. [Decompression Gzip-Compressed Base64 Data](#decompression-gzip-compressed-base64-data)
+   2. [Scaling Benchmarks on Ryzen 3900X](#scaling-benchmarks-on-ryzen-3900x)
+      1. [Decompression with Existing Index](#decompression-with-existing-index)
+      2. [Decompression from Scratch](#decompression-from-scratch)
 3. [Usage](#usage)
    1. [Command Line Tool](#command-line-tool)
    2. [Python Library](#python-library)
    3. [Via Ratarmount](#via-ratarmount)
    4. [C++ Library](#c-library)
 4. [Citation](#citation)
 5. [About](#about)
 6. [Internal Architecture](#internal-architecture)
 7. [Tracing the Decoder](#tracing-the-decoder)
 
 
-# Performance
-
-These are simple timing tests for reading all the contents of a gzip file sequentially.
-
-Results are shown for an AMD Ryzen 3900X 12-core (24 virtual cores) processor and with `gzipFilePath="4GiB-base64.gz"`, which is a 4 GiB gzip compressed file with base64 random data.
-
-Be aware that the chunk size requested from the Python code does influence the performance heavily.
-This benchmarks use a chunk size of 512 KiB.
-
-## Decompression with Existing Index
-
-|                        | 4GiB-base64                  | 4GiB-base64     | | 20x-silesia                   | 20x-silesia
-|------------------------|------------------------------|-----------------|-|-------------------------------|---------
-| Uncompressed Size      | 4 GiB                        |                 | | 3.95 GiB                      |
-| Compressed Size        | 3.04 GiB                     |                 | | 1.27 GiB                      |
-| **Module**             | **Bandwidth <br/> / (MB/s)** | **Speedup**     | |  **Bandwidth <br/> / (MB/s)** | **Speedup**
-| gzip                   |  250                         |    1            | |   293                         |  1
-| rapidgzip (0  threads) | 5060                         | 19.5            | |  5580                         | 18.6
-| rapidgzip (1  threads) |  445                         |  1.7            | |   624                         |  2.1
-| rapidgzip (2  threads) |  895                         |  3.5            | |  1190                         |  4.0
-| rapidgzip (6  threads) | 2500                         |  9.6            | |  3330                         | 11.1
-| rapidgzip (12 threads) | 4390                         | 16.9            | |  5810                         | 19.4
-| rapidgzip (24 threads) | 5150                         | 19.9            | |  5960                         | 19.9
-| rapidgzip (32 threads) | 5000                         | 19.3            | |  5640                         | 18.8
-
-
-## Decompression from Scratch
-
-### Python
-
-|                        | 4GiB-base64                  | 4GiB-base64     | | 20x-silesia                   | 20x-silesia
-|------------------------|------------------------------|-----------------|-|-------------------------------|---------
-| Uncompressed Size      | 4 GiB                        |                 | | 3.95 GiB                      |
-| Compressed Size        | 3.04 GiB                     |                 | | 1.27 GiB                      |
-| **Module**             | **Bandwidth <br/> / (MB/s)** | **Speedup**     | |  **Bandwidth <br/> / (MB/s)** | **Speedup**
-| gzip                   |  250                         |    1            | |   293                         |  1
-| rapidgzip (0  threads) | 3290                         | 12.7            | |  1820                         |  6.1
-| rapidgzip (1  threads) |  222                         |  0.9            | |   238                         |  0.8
-| rapidgzip (2  threads) |  435                         |  1.7            | |   415                         |  1.4
-| rapidgzip (6  threads) | 1260                         |  4.9            | |  1140                         |  3.8
-| rapidgzip (12 threads) | 2310                         |  8.9            | |  1550                         |  5.2
-| rapidgzip (24 threads) | 3200                         | 12.4            | |  1890                         |  6.3
-| rapidgzip (32 threads) | 3210                         | 12.4            | |  2060                         |  6.9
-
-Note that rapidgzip is generally faster when given an index because it can delegate the decompression to zlib while it has to use its own gzip decompression engine when no index exists yet.
-
-Note that values deviate roughly by 10% and therefore are rounded.
-
-The code used for benchmarking can be found [here](results/benchmarkPythonModule.py).
-
-
 # Installation
 
 You can simply install it from PyPI:
 
 ```
 python3 -m pip install --upgrade pip  # Recommended for newer manylinux wheels
 python3 -m pip install rapidgzip
+rapidgzip --help
 ```
 
+<details>
+<summary>Advanced Installations</summary>
+
 The latest unreleased development version can be tested out with:
 
 ```bash
 python3 -m pip install --force-reinstall 'git+https://github.com/mxmlnkn/indexed_bzip2.git@master#egginfo=rapidgzip&subdirectory=python/rapidgzip'
 ```
 
 And to build locally, you can use `build` and install the wheel:
@@ -154,14 +111,106 @@
 ```bash
 cd python/rapidgzip
 rm -rf dist
 python3 -m build .
 python3 -m pip install --force-reinstall --user dist/*.whl
 ```
 
+</details>
+
+
+# Performance
+
+Following are benchmarks showing the decompression bandwidth over the number of used cores.
+
+There are two rapidgzip variants shown: `(index)` and `(no index)`.
+Rapidgzip is generally faster when given an index with `--import-index` because it can delegate the decompression to ISA-l or zlib while it has to use its own custom-written gzip decompression engine when no index exists yet.
+Furthermore, decompression can be parallelized more evenly and more effectively when an index exists because the serializing window propagation step is not necessary.
+
+The violin plots show 20 repeated measurements as a single "blob".
+Thin blobs signal very reproducible timings while thick blobs signal a large variance.
+
+
+## Scaling Benchmarks on 2xAMD EPYC CPU 7702 (2x64 cores)
+
+### Decompression of Silesia Corpus
+
+![](https://raw.githubusercontent.com/mxmlnkn/indexed_bzip2/master/results/benchmarks/rapidgzip-0.9.0-scaling-benchmarks-2023-08-30/plots/result-parallel-decompression-silesia-dev-null-bandwidths-number-of-threads.png)
+
+This benchmark uses the [Silesia corpus](https://sun.aei.polsl.pl//~sdeor/index.php?page=silesia) compressed as a .tar.gz file to show the decompression performance.
+However, the compressed dataset is only ~69 MB, which is not sufficiently large to show parallelization over 128 cores.
+That's why the TAR file is repeated as often as there are number of cores in the benchmark times 2 and then compressed into a single large gzip file, which is ~18 GB compressed and 54 GB uncompressed for 128 cores.
+
+Rapidgzip achieves up to 24 GB/s with an index and 12 GB/s without.
+
+Pugz is not shown as comparison because it is not able to decompress the Silesia dataset because it contains binary data, which it cannot handle.
+
+
+### Decompression of Gzip-Compressed Base64 Data
+
+![](https://raw.githubusercontent.com/mxmlnkn/indexed_bzip2/master/results/benchmarks/rapidgzip-0.9.0-scaling-benchmarks-2023-08-30/plots/result-parallel-decompression-base64-dev-null-bandwidths-number-of-threads.png)
+
+This benchmarks uses random data, that has been base64 encoded and then gzip-compressed.
+This is the next best case for rapidgzip after the trivial case of purely random data, which cannot be compressed and therefore can be decompressed with a simple memory copy.
+This next best case results in mostly Huffman-coding compressed data with only very few LZ77 back-references.
+Without LZ77 back-references, parallel decompression can be done more independently and therefore faster than in the case of many LZ77 back-references.
+
+
+### Decompression of Gzip-Compressed FASTQ Data
+
+![](https://raw.githubusercontent.com/mxmlnkn/indexed_bzip2/master/results/benchmarks/rapidgzip-0.9.0-scaling-benchmarks-2023-08-30/plots/result-parallel-decompression-fastq-dev-null-bandwidths-number-of-threads.png)
+
+This benchmarks uses gzip-compressed [FASTQ data](http://ftp.sra.ebi.ac.uk/vol1/fastq/SRR224/085/SRR22403185/SRR22403185_2.fastq.gz).
+That's why the TAR file is repeated as often as there are number of cores in the benchmark to hold the decompression times roughly constant in order to make the benchmark over this large a range feasible.
+This is almost the worst case for rapidgzip because it contains many LZ77 back-references over very long ranges.
+This means that a fallback to ISA-L is not possible and it means that the costly two-staged decoding has to be done for almost all the data.
+This is also the reason why if fails to scale above 64 cores, i.e, to teh second CPU socket.
+The first and second decompression stages are completely independently submitted to a thread pool, which on this NUMA architecture means, that data needs to be costly transferred from one processor socket to the other if the second step for a chunk is not done on the same processor as the first.
+This should be fixable by making the ThreadPool NUMA-aware.
+
+These three scaling plots were created with rapidgzip 0.9.0 while the ones in the [paper](<results/paper/Knespel, Brunst - 2023 - Rapidgzip - Parallel Decompression and Seeking in Gzip Files Using Cache Prefetching.pdf>) were created with 0.5.0.
+
+
+## Scaling Benchmarks on Ryzen 3900X
+
+These benchmarks on my local workstation with a Ryzen 3900X only has 12 cores (24 virtual cores) but the base frequency is much higher than the 2xAMD EPYC CPU 7702.
+
+### Decompression With Existing Index
+
+|                        | 4GiB-base64                  | 4GiB-base64     | | 20x-silesia                   | 20x-silesia
+|------------------------|------------------------------|-----------------|-|-------------------------------|---------
+| Uncompressed Size      | 4 GiB                        |                 | | 3.95 GiB                      |
+| Compressed Size        | 3.04 GiB                     |                 | | 1.27 GiB                      |
+| **Module**             | **Bandwidth <br/> / (MB/s)** | **Speedup**     | |  **Bandwidth <br/> / (MB/s)** | **Speedup**
+| gzip                   |  250                         |    1            | |   293                         |  1
+| rapidgzip (0  threads) | 5179                         | 20.6            | |  5640                         | 18.8
+| rapidgzip (1  threads) |  488                         |  1.9            | |   684                         |  2.3
+| rapidgzip (2  threads) |  902                         |  3.6            | |  1200                         |  4.0
+| rapidgzip (6  threads) | 2617                         | 10.4            | |  3250                         | 10.9
+| rapidgzip (12 threads) | 4463                         | 17.7            | |  5600                         | 18.7
+| rapidgzip (24 threads) | 5240                         | 20.8            | |  5750                         | 19.2
+| rapidgzip (32 threads) | 4929                         | 19.6            | |  5300                         | 17.7
+
+
+### Decompression From Scratch
+
+|                        | 4GiB-base64                  | 4GiB-base64     | | 20x-silesia                   | 20x-silesia
+|------------------------|------------------------------|-----------------|-|-------------------------------|---------
+| Uncompressed Size      | 4 GiB                        |                 | | 3.95 GiB                      |
+| Compressed Size        | 3.04 GiB                     |                 | | 1.27 GiB                      |
+| **Module**             | **Bandwidth <br/> / (MB/s)** | **Speedup**     | |  **Bandwidth <br/> / (MB/s)** | **Speedup**
+| gzip                   |  250                         |    1            | |   293                         |  1
+| rapidgzip (0  threads) | 5060                         | 20.1            | |  2070                         |  6.9
+| rapidgzip (1  threads) |  487                         |  1.9            | |  630                          |  2.1
+| rapidgzip (2  threads) |  839                         |  3.3            | |  694                          |  2.3
+| rapidgzip (6  threads) | 2365                         |  9.4            | |  1740                         |  5.8
+| rapidgzip (12 threads) | 4116                         | 16.4            | |  1900                         |  6.4
+| rapidgzip (24 threads) | 4974                         | 19.8            | |  2040                         |  6.8
+| rapidgzip (32 threads) | 4612                         | 18.3            | |  2580                         |  8.6
+
 
 # Usage
 
 ## Command Line Tool
 
 ```bash
 rapidgzip --help
@@ -258,50 +307,51 @@
 I currently did not yet test integrating it into other projects other than simply manually copying the source in `src/core`, `src/rapidgzip`, and if integrated zlib is desired also `src/external/zlib`.
 If you have suggestions and wishes like support with CMake or Conan, please open an issue.
 
 
 # Citation
 
 A paper describing the implementation details and showing the scaling behavior with up to 128 cores has been submitted to and [accepted](https://www.hpdc.org/2023/program/technical-sessions/) in [ACM HPDC'23](https://www.hpdc.org/2023/), The 32nd International Symposium on High-Performance Parallel and Distributed Computing.
-The author's version can be found [here](<results/paper/Knespel, Brunst - 2023 - Rapidgzip - Parallel Decompression and Seeking in Gzip Files Using Cache Prefetching.pdf>) and the accompanying presentation [here](results/Presentation-2023-06-22.pdf).
+The paper can be accessed [freely on ACM DL](https://doi.org/10.1145/3588195.3592992).
+The accompanying presentation can be found [here](results/Presentation-2023-06-22.pdf).
 
 If you use this software for your scientific publication, please cite it as:
 
 This is preliminiary. The final citation will become available end of June 2023.
 
 ```bibtex
 @inproceedings{rapidgzip,
     author    = {Knespel, Maximilian and Brunst, Holger},
     title     = {Rapidgzip: Parallel Decompression and Seeking in Gzip Files Using Cache Prefetching},
     year      = {2023},
-    % isbn    = {},  % To be released end of June
+    isbn      = {9798400701559},
     publisher = {Association for Computing Machinery},
     address   = {New York, NY, USA},
     url       = {https://doi.org/10.1145/3588195.3592992},
     doi       = {10.1145/3588195.3592992},
     abstract  = {Gzip is a file compression format, which is ubiquitously used. Although a multitude of gzip implementations exist, only pugz can fully utilize current multi-core processor architectures for decompression. Yet, pugz cannot decompress arbitrary gzip files. It requires the decompressed stream to only contain byte values 9–126. In this work, we present a generalization of the parallelization scheme used by pugz that can be reliably applied to arbitrary gzip-compressed data without compromising performance. We show that the requirements on the file contents posed by pugz can be dropped by implementing an architecture based on a cache and a parallelized prefetcher. This architecture can safely handle faulty decompression results, which can appear when threads start decompressing in the middle of a gzip file by using trial and error. Using 128 cores, our implementation reaches 8.7 GB/s decompression bandwidth for gzip-compressed base64-encoded data, a speedup of 55 over the single-threaded GNU gzip, and 5.6 GB/s for the Silesia corpus, a speedup of 33 over GNU gzip.},
     booktitle = {Proceedings of the 32nd International Symposium on High-Performance Parallel and Distributed Computing},
-    % pages   = {16–29},  % To be released end of June
+    pages     = {295–307},
     numpages  = {13},
-    keywords  = {Gzip, Decompression, Parallel Algorithm, Performance, Random Access},
+    keywords  = {gzip, decompression, parallel algorithm, performance, random access},
     location  = {Orlando, FL, USA},
     series    = {HPDC '23},
 }
 ```
 
 # About
 
 This tool originated as a backend for [ratarmount](https://github.com/mxmlnkn/ratarmount).
 After writing the bzip2 backend for [ratarmount](https://github.com/mxmlnkn/indexed_bzip2), my hesitation about reimplementing custom decoders for existing file formats has vastly diminished.
 And, while random access to gzip files did exist with [indexed_gzip](https://github.com/pauldmccarthy/indexed_gzip), it did not support parallel decompression neither for the index creation nor when the index already exists.
-The latter of which is trivial, when ignoring load balancing issues, but parallelizing even the idnex creation is vastly more complicated because decompressing data requires the previous 32 KiB of decompressed data to be known.
+The latter of which is trivial, when ignoring load balancing issues, but parallelizing even the index creation is vastly more complicated because decompressing data requires the previous 32 KiB of decompressed data to be known.
 
 After implementing a production-ready version by improving upon the algorithm used by [pugz](https://github.com/Piezoid/pugz), I submitted a [paper](Citation).
-The review process was double-blind and I was unsure whether pseudonymize Pragzip because it has already been uploaded to Github.
-In the end, I used Rapidgzip during the review process and because I was not sure, which form fields should be filled with the pseudonymized title, I simply stuck with it.
+The review process was double-blind and I was unsure whether to pseudonymize Pragzip because it has already been uploaded to Github.
+In the end, I used "rapidgzip" during the review process and because I was not sure, which form fields should be filled with the pseudonymized title, I simply stuck with it.
 Rapidgzip was chosen for similar reason to rapidgzip, namely the P and RA are acronyms for Parallel and Random Access.
 As rapgzip, did not stick, I used rapidgzip, which now also contains the foremost design goal in its name: being rapidly faster than single-threaded implementations.
 Furthermore, the additional ID could be interpreted to stand for Index and Decompression, making "rapid" a partial backronym.
 
 
 # Internal Architecture
```

### Comparing `rapidgzip-0.8.1/rapidgzip.egg-info/SOURCES.txt` & `rapidgzip-0.9.0/rapidgzip.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 rapidgzip/GzipAnalyzer.hpp
 rapidgzip/GzipBlockFinder.hpp
 rapidgzip/GzipChunkFetcher.hpp
 rapidgzip/GzipReader.hpp
 rapidgzip/IndexFileFormat.hpp
 rapidgzip/MarkerReplacement.hpp
 rapidgzip/ParallelGzipReader.hpp
+rapidgzip/RFCTables.hpp
 rapidgzip/WindowMap.hpp
 rapidgzip/crc32.hpp
 rapidgzip/definitions.hpp
 rapidgzip/deflate.hpp
 rapidgzip/gzip.hpp
 rapidgzip/isal.hpp
 rapidgzip/precode.hpp
@@ -119,15 +120,17 @@
 rapidgzip/blockfinder/precodecheck/SingleCompressedLUT.hpp
 rapidgzip/blockfinder/precodecheck/SingleLUT.hpp
 rapidgzip/blockfinder/precodecheck/WalkTreeCompressedLUT.hpp
 rapidgzip/blockfinder/precodecheck/WalkTreeLUT.hpp
 rapidgzip/blockfinder/precodecheck/WithoutLUT.hpp
 rapidgzip/huffman/HuffmanCodingBase.hpp
 rapidgzip/huffman/HuffmanCodingCheckOnly.hpp
+rapidgzip/huffman/HuffmanCodingDistanceISAL.hpp
 rapidgzip/huffman/HuffmanCodingDoubleLiteralCached.hpp
+rapidgzip/huffman/HuffmanCodingISAL.hpp
 rapidgzip/huffman/HuffmanCodingLinearSearch.hpp
 rapidgzip/huffman/HuffmanCodingReversedBitsCached.hpp
 rapidgzip/huffman/HuffmanCodingReversedBitsCachedCompressed.hpp
 rapidgzip/huffman/HuffmanCodingReversedCodesPerLength.hpp
 rapidgzip/huffman/HuffmanCodingSymbolsPerLength.hpp
 tools/licenses.cpp
 tools/rapidgzip.cpp
```

### Comparing `rapidgzip-0.8.1/rapidgzip.pyx` & `rapidgzip-0.9.0/rapidgzip.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 cdef extern from "tools/rapidgzip.cpp":
     int rapidgzipCLI(int, char**) except +
 
 cdef extern from "rapidgzip/ParallelGzipReader.hpp" namespace "rapidgzip":
     cppclass ChunkData
 
-    cppclass ParallelGzipReader[ChunkData, ENABLE_STATISTICS=*, SHOW_PROFILE=*]:
+    cppclass ParallelGzipReader[ChunkData, ENABLE_STATISTICS=*]:
         ParallelGzipReader(string, size_t) except +
         ParallelGzipReader(int, size_t) except +
         ParallelGzipReader(PyObject*, size_t) except +
 
         bool eof() except +
         int fileno() except +
         bool seekable() except +
@@ -53,15 +53,15 @@
     # Must be inside an "extern" section or else Cython will try to generate a struct named
     # "true", which does not compile.
     cdef cppclass TrueValue "true":
         pass
     cdef cppclass RapidgzipChunkData "rapidgzip::ChunkData":
         pass
 
-ctypedef ParallelGzipReader[RapidgzipChunkData, TrueValue, TrueValue] ParallelGzipReaderVerbose
+ctypedef ParallelGzipReader[RapidgzipChunkData, TrueValue] ParallelGzipReaderVerbose
 ctypedef ParallelGzipReader[RapidgzipChunkData] ParallelGzipReaderNonVerbose
 
 
 def _isFileObject(file):
     return (
         hasattr(file, 'read') and callable(getattr(file, 'read'))
         and hasattr(file, 'seek') and callable(getattr(file, 'seek'))
@@ -333,8 +333,8 @@
         return rapidgzipCLI(len(args), cargs)
     finally:
         free(cargs)
         for buffer in buffers:
             PyBuffer_Release(&buffer)
 
 
-__version__ = '0.8.1'
+__version__ = '0.9.0'
```

### Comparing `rapidgzip-0.8.1/rapidgzip.svg` & `rapidgzip-0.9.0/rapidgzip.svg`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/setup.cfg` & `rapidgzip-0.9.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rapidgzip
-version = 0.8.1
+version = 0.9.0
 description = Parallel random access to gzip files
 url = https://github.com/mxmlnkn/rapidgzip
 author = Maximilian Knespel
 author_email = mxmlnkn@github.de
 license = MIT
 license_files = 
 	LICENSE-APACHE
```

### Comparing `rapidgzip-0.8.1/setup.py` & `rapidgzip-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/tools/licenses.cpp` & `rapidgzip-0.9.0/tools/licenses.cpp`

 * *Files identical despite different names*

### Comparing `rapidgzip-0.8.1/tools/rapidgzip.cpp` & `rapidgzip-0.9.0/tools/rapidgzip.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 decompressParallel( const Reader&       reader,
                     const std::string&  indexLoadPath,
                     const std::string&  indexSavePath,
                     const WriteFunctor& writeFunctor,
                     const bool          verbose )
 {
     if ( !indexLoadPath.empty() ) {
-        reader->setBlockOffsets( readGzipIndex( std::make_unique<StandardFileReader>( indexLoadPath ) ) );
+        reader->importIndex( std::make_unique<StandardFileReader>( indexLoadPath ) );
 
         if ( verbose && ( !indexSavePath.empty() || !indexLoadPath.empty() ) ) {
             printIndexAnalytics( reader );
         }
     }
 
     const auto totalBytesRead = reader->read( writeFunctor );
@@ -151,22 +151,24 @@
          typename WriteFunctor = std::function<void ( const std::shared_ptr<ChunkData>&, size_t, size_t )> >
 size_t
 decompressParallel( const Arguments&    args,
                     UniqueFileReader    inputFile,
                     const WriteFunctor& writeFunctor )
 {
     if ( args.verbose ) {
-        using Reader = rapidgzip::ParallelGzipReader<ChunkData, /* enable statistics */ true, /* show profile */ true>;
+        using Reader = rapidgzip::ParallelGzipReader<ChunkData, /* enable statistics */ true>;
         auto reader = std::make_unique<Reader>( std::move( inputFile ), args.decoderParallelism, args.chunkSize );
+        reader->setShowProfileOnDestruction( true );
         reader->setCRC32Enabled( args.crc32Enabled );
         return decompressParallel( std::move( reader ), args.indexLoadPath, args.indexSavePath, writeFunctor,
                                    args.verbose );
     } else {
-        using Reader = rapidgzip::ParallelGzipReader<ChunkData, /* enable statistics */ false, /* show profile */ false>;
+        using Reader = rapidgzip::ParallelGzipReader<ChunkData, /* enable statistics */ false>;
         auto reader = std::make_unique<Reader>( std::move( inputFile ), args.decoderParallelism, args.chunkSize );
+        reader->setShowProfileOnDestruction( false );
         reader->setCRC32Enabled( args.crc32Enabled );
         return decompressParallel( std::move( reader ), args.indexLoadPath, args.indexSavePath, writeFunctor,
                                    args.verbose );
     }
 }
 
 
@@ -257,15 +259,15 @@
     if ( parsedArgs.count( "help" ) > 0 ) {
         printHelp( options );
         return 0;
     }
 
     if ( parsedArgs.count( "version" ) > 0 ) {
         std::cout << "rapidgzip, CLI to the parallelized, indexed, and seekable gzip decoding library rapidgzip "
-                  << "version 0.8.1.\n";
+                  << "version 0.9.0.\n";
         return 0;
     }
 
     if ( parsedArgs.count( "oss-attributions" ) > 0 ) {
         std::cout << licenses::CXXOPTS << "\n"
         #ifdef WITH_ISAL
                   << licenses::ISAL << "\n"
@@ -371,63 +373,43 @@
         }
         const auto outputFileDescriptor = outputFile ? outputFile->fd() : -1;
 
         uint64_t newlineCount{ 0 };
 
         const auto t0 = now();
 
-        size_t totalBytesRead{ 0 };
-        if ( args.decoderParallelism == 1 ) {
-            const auto writeAndCount =
-                [outputFileDescriptor, countLines, &newlineCount]
-                ( const void* const buffer,
-                  uint64_t const    size )
-                {
-                    if ( outputFileDescriptor >= 0 ) {
-                        writeAllToFd( outputFileDescriptor, buffer, size );
-                    }
-                    if ( countLines ) {
-                        newlineCount += countNewlines( { reinterpret_cast<const char*>( buffer ),
-                                                         static_cast<size_t>( size ) } );
+        const auto writeAndCount =
+            [outputFileDescriptor, countLines, &newlineCount]
+            ( const std::shared_ptr<rapidgzip::ChunkData>& chunkData,
+              size_t const                               offsetInBlock,
+              size_t const                               dataToWriteSize )
+            {
+                writeAll( chunkData, outputFileDescriptor, offsetInBlock, dataToWriteSize );
+                if ( countLines ) {
+                    using rapidgzip::deflate::DecodedData;
+                    for ( auto it = DecodedData::Iterator( *chunkData, offsetInBlock, dataToWriteSize );
+                          static_cast<bool>( it ); ++it )
+                    {
+                        const auto& [buffer, size] = *it;
+                        newlineCount += countNewlines( { reinterpret_cast<const char*>( buffer ), size } );
                     }
-                };
+                }
+            };
 
-            rapidgzip::GzipReader gzipReader{ std::move( inputFile ) };
-            gzipReader.setCRC32Enabled( args.crc32Enabled );
-            totalBytesRead = gzipReader.read( writeAndCount );
-        } else {
-            const auto writeAndCount =
-                [outputFileDescriptor, countLines, &newlineCount]
-                ( const std::shared_ptr<rapidgzip::ChunkData>& chunkData,
-                  size_t const                               offsetInBlock,
-                  size_t const                               dataToWriteSize )
-                {
-                    writeAll( chunkData, outputFileDescriptor, offsetInBlock, dataToWriteSize );
-                    if ( countLines ) {
-                        using rapidgzip::deflate::DecodedData;
-                        for ( auto it = DecodedData::Iterator( *chunkData, offsetInBlock, dataToWriteSize );
-                              static_cast<bool>( it ); ++it )
-                        {
-                            const auto& [buffer, size] = *it;
-                            newlineCount += countNewlines( { reinterpret_cast<const char*>( buffer ), size } );
-                        }
-                    }
-                };
+        args.chunkSize = parsedArgs["chunk-size"].as<unsigned int>() * 1_Ki;
 
-            args.chunkSize = parsedArgs["chunk-size"].as<unsigned int>() * 1_Ki;
+        size_t totalBytesRead{ 0 };
+        if ( ( outputFileDescriptor == -1 ) && args.indexSavePath.empty() && countBytes ) {
+            /* Need to do nothing with the chunks because decompressParallel returns the decompressed size. */
+            const auto doNothing = [] ( const auto&, size_t, size_t ) {};
 
-            if ( ( outputFileDescriptor == -1 ) && args.indexSavePath.empty() && countBytes ) {
-                /* Need to do nothing with the chunks because decompressParallel returns the decompressed size. */
-                const auto doNothing = [] ( const auto&, size_t, size_t ) {};
-
-                totalBytesRead = decompressParallel<rapidgzip::ChunkDataCounter>(
-                    args, std::move( inputFile ), doNothing );
-            } else {
-                totalBytesRead = decompressParallel<rapidgzip::ChunkData>( args, std::move( inputFile ), writeAndCount );
-            }
+            totalBytesRead = decompressParallel<rapidgzip::ChunkDataCounter>(
+                args, std::move( inputFile ), doNothing );
+        } else {
+            totalBytesRead = decompressParallel<rapidgzip::ChunkData>( args, std::move( inputFile ), writeAndCount );
         }
 
         const auto writeToStdErr = outputFile && outputFile->writingToStdout();
         if ( outputFile ) {
             outputFile->truncate( totalBytesRead );
             outputFile.reset();  // Close the file here to include it in the time measurement.
         }
```

