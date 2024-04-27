# Comparing `tmp/uvx-2.0.3.tar.gz` & `tmp/uvx-2.0.5.tar.gz`

## Comparing `uvx-2.0.3.tar` & `uvx-2.0.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 uvx-2.0.3/Cargo.toml
--rw-rw-r--   0     1000     1000       77 2024-04-15 17:07:31.000000 uvx-2.0.3/.cargo/config.toml
--rw-rw-r--   0     1000     1000      686 2024-04-11 15:03:17.000000 uvx-2.0.3/.gitignore
--rw-rw-r--   0     1000     1000      558 2024-04-26 20:59:05.000000 uvx-2.0.3/CHANGELOG.md
--rw-rw-r--   0     1000     1000    86384 2024-04-26 20:59:17.000000 uvx-2.0.3/Cargo.lock
--rw-rw-r--   0     1000     1000     2203 2024-04-26 19:03:51.000000 uvx-2.0.3/README.md
--rwxrwxr-x   0     1000     1000      235 2024-04-26 18:24:22.000000 uvx-2.0.3/build.sh
--rw-rw-r--   0     1000     1000      106 2024-04-15 17:06:44.000000 uvx-2.0.3/rustfmt.toml
--rw-rw-r--   0     1000     1000     1821 2024-04-24 20:50:38.000000 uvx-2.0.3/src/animate.rs
--rw-rw-r--   0     1000     1000     9727 2024-04-24 20:50:21.000000 uvx-2.0.3/src/cli.rs
--rw-rw-r--   0     1000     1000     2314 2024-04-26 20:57:40.000000 uvx-2.0.3/src/cmd.rs
--rw-rw-r--   0     1000     1000      618 2024-04-24 20:49:18.000000 uvx-2.0.3/src/commands/completions.rs
--rw-rw-r--   0     1000     1000     2250 2024-04-24 20:49:13.000000 uvx-2.0.3/src/commands/ensurepath.rs
--rw-rw-r--   0     1000     1000     1617 2024-04-24 20:48:26.000000 uvx-2.0.3/src/commands/inject.rs
--rw-rw-r--   0     1000     1000     5022 2024-04-24 20:48:10.000000 uvx-2.0.3/src/commands/install.rs
--rw-rw-r--   0     1000     1000     2511 2024-04-24 20:45:17.000000 uvx-2.0.3/src/commands/list.rs
--rw-rw-r--   0     1000     1000      312 2024-04-15 19:40:37.000000 uvx-2.0.3/src/commands/mod.rs
--rw-rw-r--   0     1000     1000     2200 2024-04-24 20:43:02.000000 uvx-2.0.3/src/commands/reinstall.rs
--rw-rw-r--   0     1000     1000     1346 2024-04-24 20:41:37.000000 uvx-2.0.3/src/commands/reinstall_all.rs
--rw-rw-r--   0     1000     1000     4039 2024-04-24 20:42:18.000000 uvx-2.0.3/src/commands/run.rs
--rw-rw-r--   0     1000     1000      621 2024-04-24 20:39:59.000000 uvx-2.0.3/src/commands/runpip.rs
--rw-rw-r--   0     1000     1000     1195 2024-04-24 20:39:49.000000 uvx-2.0.3/src/commands/runpython.rs
--rw-rw-r--   0     1000     1000      527 2024-04-24 20:39:25.000000 uvx-2.0.3/src/commands/runuv.rs
--rw-rw-r--   0     1000     1000     3192 2024-04-26 20:57:17.000000 uvx-2.0.3/src/commands/self_update.rs
--rw-rw-r--   0     1000     1000     1631 2024-04-24 20:35:19.000000 uvx-2.0.3/src/commands/uninject.rs
--rw-rw-r--   0     1000     1000     2019 2024-04-24 20:34:30.000000 uvx-2.0.3/src/commands/uninstall.rs
--rw-rw-r--   0     1000     1000      948 2024-04-24 20:34:02.000000 uvx-2.0.3/src/commands/uninstall_all.rs
--rw-rw-r--   0     1000     1000     4054 2024-04-24 20:33:47.000000 uvx-2.0.3/src/commands/upgrade.rs
--rw-rw-r--   0     1000     1000     1021 2024-04-24 20:32:19.000000 uvx-2.0.3/src/commands/upgrade_all.rs
--rw-rw-r--   0     1000     1000      962 2024-04-24 20:32:00.000000 uvx-2.0.3/src/helpers.rs
--rw-rw-r--   0     1000     1000     1026 2024-04-24 20:02:25.000000 uvx-2.0.3/src/main.rs
--rw-rw-r--   0     1000     1000     8457 2024-04-26 20:37:12.000000 uvx-2.0.3/src/metadata.rs
--rw-rw-r--   0     1000     1000     4477 2024-04-24 20:41:56.000000 uvx-2.0.3/src/pip.rs
--rw-rw-r--   0     1000     1000     3692 2024-04-24 20:26:38.000000 uvx-2.0.3/src/symlinks.rs
--rw-rw-r--   0     1000     1000     3768 2024-04-24 20:51:25.000000 uvx-2.0.3/src/uv.rs
--rw-rw-r--   0     1000     1000     2352 2024-04-24 20:51:25.000000 uvx-2.0.3/src/venv.rs
--rw-rw-r--   0     1000     1000      819 2024-04-26 18:46:18.000000 uvx-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     2677 1970-01-01 00:00:00.000000 uvx-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 uvx-2.0.5/Cargo.toml
+-rw-rw-r--   0     1000     1000       77 2024-04-15 17:07:31.000000 uvx-2.0.5/.cargo/config.toml
+-rw-rw-r--   0     1000     1000      686 2024-04-11 15:03:17.000000 uvx-2.0.5/.gitignore
+-rw-rw-r--   0     1000     1000      717 2024-04-26 21:14:32.000000 uvx-2.0.5/CHANGELOG.md
+-rw-rw-r--   0     1000     1000    92159 2024-04-26 21:14:04.000000 uvx-2.0.5/Cargo.lock
+-rw-rw-r--   0     1000     1000     2203 2024-04-26 19:03:51.000000 uvx-2.0.5/README.md
+-rwxrwxr-x   0     1000     1000      235 2024-04-26 18:24:22.000000 uvx-2.0.5/build.sh
+-rw-rw-r--   0     1000     1000      106 2024-04-15 17:06:44.000000 uvx-2.0.5/rustfmt.toml
+-rw-rw-r--   0     1000     1000     1821 2024-04-24 20:50:38.000000 uvx-2.0.5/src/animate.rs
+-rw-rw-r--   0     1000     1000     9727 2024-04-24 20:50:21.000000 uvx-2.0.5/src/cli.rs
+-rw-rw-r--   0     1000     1000     2314 2024-04-26 20:57:40.000000 uvx-2.0.5/src/cmd.rs
+-rw-rw-r--   0     1000     1000      618 2024-04-24 20:49:18.000000 uvx-2.0.5/src/commands/completions.rs
+-rw-rw-r--   0     1000     1000     2250 2024-04-24 20:49:13.000000 uvx-2.0.5/src/commands/ensurepath.rs
+-rw-rw-r--   0     1000     1000     1617 2024-04-24 20:48:26.000000 uvx-2.0.5/src/commands/inject.rs
+-rw-rw-r--   0     1000     1000     5187 2024-04-26 21:07:25.000000 uvx-2.0.5/src/commands/install.rs
+-rw-rw-r--   0     1000     1000     2511 2024-04-24 20:45:17.000000 uvx-2.0.5/src/commands/list.rs
+-rw-rw-r--   0     1000     1000      312 2024-04-15 19:40:37.000000 uvx-2.0.5/src/commands/mod.rs
+-rw-rw-r--   0     1000     1000     2200 2024-04-24 20:43:02.000000 uvx-2.0.5/src/commands/reinstall.rs
+-rw-rw-r--   0     1000     1000     1346 2024-04-24 20:41:37.000000 uvx-2.0.5/src/commands/reinstall_all.rs
+-rw-rw-r--   0     1000     1000     4039 2024-04-24 20:42:18.000000 uvx-2.0.5/src/commands/run.rs
+-rw-rw-r--   0     1000     1000      621 2024-04-24 20:39:59.000000 uvx-2.0.5/src/commands/runpip.rs
+-rw-rw-r--   0     1000     1000     1195 2024-04-24 20:39:49.000000 uvx-2.0.5/src/commands/runpython.rs
+-rw-rw-r--   0     1000     1000      527 2024-04-24 20:39:25.000000 uvx-2.0.5/src/commands/runuv.rs
+-rw-rw-r--   0     1000     1000     3192 2024-04-26 20:57:17.000000 uvx-2.0.5/src/commands/self_update.rs
+-rw-rw-r--   0     1000     1000     1631 2024-04-24 20:35:19.000000 uvx-2.0.5/src/commands/uninject.rs
+-rw-rw-r--   0     1000     1000     2019 2024-04-24 20:34:30.000000 uvx-2.0.5/src/commands/uninstall.rs
+-rw-rw-r--   0     1000     1000      948 2024-04-24 20:34:02.000000 uvx-2.0.5/src/commands/uninstall_all.rs
+-rw-rw-r--   0     1000     1000     4054 2024-04-24 20:33:47.000000 uvx-2.0.5/src/commands/upgrade.rs
+-rw-rw-r--   0     1000     1000     1021 2024-04-24 20:32:19.000000 uvx-2.0.5/src/commands/upgrade_all.rs
+-rw-rw-r--   0     1000     1000      962 2024-04-24 20:32:00.000000 uvx-2.0.5/src/helpers.rs
+-rw-rw-r--   0     1000     1000     1026 2024-04-24 20:02:25.000000 uvx-2.0.5/src/main.rs
+-rw-rw-r--   0     1000     1000     8457 2024-04-26 20:37:12.000000 uvx-2.0.5/src/metadata.rs
+-rw-rw-r--   0     1000     1000     4477 2024-04-24 20:41:56.000000 uvx-2.0.5/src/pip.rs
+-rw-rw-r--   0     1000     1000     3692 2024-04-24 20:26:38.000000 uvx-2.0.5/src/symlinks.rs
+-rw-rw-r--   0     1000     1000     3768 2024-04-24 20:51:25.000000 uvx-2.0.5/src/uv.rs
+-rw-rw-r--   0     1000     1000     2352 2024-04-24 20:51:25.000000 uvx-2.0.5/src/venv.rs
+-rw-rw-r--   0     1000     1000      819 2024-04-26 18:46:18.000000 uvx-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2677 1970-01-01 00:00:00.000000 uvx-2.0.5/PKG-INFO
```

### Comparing `uvx-2.0.3/Cargo.toml` & `uvx-2.0.5/Cargo.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 [package]
 name = "uvx"
-version = "2.0.3"
+version = "2.0.5"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 # [lib]
 # name = "uvx"
 # crate-type = ["cdylib"]
 
 [dependencies]
 # cli
 clap = { version = "4.5.4", features = ["derive"] }
-# python
-# pyo3 = { version = "0.20.0", features = ["extension-module"] }
-# pyo3-asyncio = { version = "0.20.0", features = ["tokio-runtime"] }
 # async
 tokio = "1.4"
 # serialize
-rmp-serde = "1.1.2"
-serde = { version = "1.0.197", features = ["derive"] }
-serde_json = "1.0.115"
+rmp-serde = "1.2.0"
+serde = { version = "1.0.198", features = ["derive"] }
+serde_json = "1.0.116"
 # helpers
 home = "0.5.9"
 itertools = "0.12.1"
 # fancy
 anstyle = "1.0.6"
 owo-colors = "4.0.0"
-# dbg-pls = { version = "0.4.3", features = ["pretty", "colors", "derive"] }
 # uv
-# uv-requirements = { git = "https://github.com/astral-sh/uv.git", tag = "0.1.31" }
-install-wheel-rs = { git = "https://github.com/astral-sh/uv.git", tag = "0.1.31" }
-uv-interpreter = { git = "https://github.com/astral-sh/uv.git", tag = "0.1.31" }
-uv-installer = { git = "https://github.com/astral-sh/uv.git", tag = "0.1.31" }
-uv-cache = { git = "https://github.com/astral-sh/uv.git", tag = "0.1.31" }
-pep508_rs = { git = "https://github.com/astral-sh/uv.git", tag = "0.1.31" }
-async_http_range_reader = "=0.7.0" # pin to specific version which uv expects
+# uv-requirements = { git = "https://github.com/astral-sh/uv.git", tag = "0.1.38" }
+install-wheel-rs = { git = "https://github.com/astral-sh/uv.git", tag = "0.1.38" }
+uv-interpreter = { git = "https://github.com/astral-sh/uv.git", tag = "0.1.38" }
+uv-installer = { git = "https://github.com/astral-sh/uv.git", tag = "0.1.38" }
+uv-cache = { git = "https://github.com/astral-sh/uv.git", tag = "0.1.38" }
+pep508_rs = { git = "https://github.com/astral-sh/uv.git", tag = "0.1.38" }
 directories = "5.0.1"
 configparser = "3.0.4"
 tempfile = "3.10.1"
-chrono = "0.4.37"
+chrono = "0.4.38"
 subprocess = "0.2.9"
 clap_complete = "4.5.2"
 regex = "1.10.4"
+
+# security bumps/pins:
+rustls = "0.23.5"
```

### Comparing `uvx-2.0.3/.gitignore` & `uvx-2.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `uvx-2.0.3/CHANGELOG.md` & `uvx-2.0.5/CHANGELOG.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.0.5 (2024-04-26)
+
+### Updates
+
+* **cargo**: bump dependencies
+
+## v2.0.4 (2024-04-26)
+
+### Fix
+
+* **install**: show warnings if creating symlinks fails
+
 ## v2.0.3 (2024-04-26)
 
 ### Fix
 
 * **self-update**: fall back to global Python if local (e.g. venv) one can not be found
 
 ## v2.0.2 (2024-04-26)
```

### Comparing `uvx-2.0.3/Cargo.lock` & `uvx-2.0.5/Cargo.lock`

 * *Files 8% similar despite different names*

```diff
@@ -118,14 +118,23 @@
 [[package]]
 name = "anyhow"
 version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f538837af36e6f6a9be0faa67f9a314f8119e4e4b5867c6ab40ed60360142519"
 
 [[package]]
+name = "arbitrary"
+version = "1.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7d5a26814d8dcb93b0e5a0ff3c6d80a8843bafb21b39e8e18a6f05471870e110"
+dependencies = [
+ "derive_arbitrary",
+]
+
+[[package]]
 name = "async-channel"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f28243a43d821d11341ab73c80bed182dc015c514b951616cf79bd4af39af0c3"
 dependencies = [
  "concurrent-queue",
  "event-listener",
@@ -137,14 +146,15 @@
 [[package]]
 name = "async-compression"
 version = "0.4.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "07dbbf24db18d609b1462965249abdf49129ccad073ec257da372adc83259c60"
 dependencies = [
  "brotli",
+ "bzip2",
  "flate2",
  "futures-core",
  "futures-io",
  "memchr",
  "pin-project-lite",
  "tokio",
  "zstd",
@@ -160,17 +170,17 @@
  "proc-macro2",
  "quote",
  "syn 2.0.58",
 ]
 
 [[package]]
 name = "async_http_range_reader"
-version = "0.7.0"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf8eeab30c68da4dc2c51f3afc4327ab06fe0f3f028ca423f7ca398c7ed8c5e7"
+checksum = "8561e6613f8361df8bed11c0eef05b98384643bc81f6b753eec7c1d91f097509"
 dependencies = [
  "bisection",
  "futures",
  "http-content-range",
  "itertools",
  "memmap2",
  "reqwest",
@@ -199,14 +209,41 @@
 [[package]]
 name = "autocfg"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
+name = "aws-lc-rs"
+version = "1.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5509d663b2c00ee421bda8d6a24d6c42e15970957de1701b8df9f6fbe5707df1"
+dependencies = [
+ "aws-lc-sys",
+ "mirai-annotations",
+ "paste",
+ "zeroize",
+]
+
+[[package]]
+name = "aws-lc-sys"
+version = "0.15.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8d5d317212c2a78d86ba6622e969413c38847b62f48111f8b763af3dac2f9840"
+dependencies = [
+ "bindgen",
+ "cc",
+ "cmake",
+ "dunce",
+ "fs_extra",
+ "libc",
+ "paste",
+]
+
+[[package]]
 name = "backoff"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b62ddb9cb1ec0a098ad4bbf9344d0713fa193ae1a80af55febcff2627b6a00c1"
 dependencies = [
  "futures-core",
  "getrandom",
@@ -235,23 +272,40 @@
 name = "base64"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
 
 [[package]]
 name = "base64"
-version = "0.21.7"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
+checksum = "9475866fec1451be56a3c2400fd081ff546538961565ccb5b7142cbd22bc7a51"
 
 [[package]]
-name = "base64"
-version = "0.22.0"
+name = "bindgen"
+version = "0.69.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9475866fec1451be56a3c2400fd081ff546538961565ccb5b7142cbd22bc7a51"
+checksum = "a00dc851838a2120612785d195287475a3ac45514741da670b735818822129a0"
+dependencies = [
+ "bitflags 2.5.0",
+ "cexpr",
+ "clang-sys",
+ "itertools",
+ "lazy_static",
+ "lazycell",
+ "log",
+ "prettyplease",
+ "proc-macro2",
+ "quote",
+ "regex",
+ "rustc-hash",
+ "shlex",
+ "syn 2.0.58",
+ "which 4.4.2",
+]
 
 [[package]]
 name = "bisection"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "021e079a1bab0ecce6cf4b4b74c0c37afa4a697136eb3b127875c84a8f04a8c3"
 
@@ -356,17 +410,38 @@
 [[package]]
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
+name = "bzip2"
+version = "0.4.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bdb116a6ef3f6c3698828873ad02c3014b3c85cadb88496095628e3ef1e347f8"
+dependencies = [
+ "bzip2-sys",
+ "libc",
+]
+
+[[package]]
+name = "bzip2-sys"
+version = "0.1.11+1.0.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "736a955f3fa7875102d57c82b8cac37ec45224a07fd32d58f9f7a186b6cd4cdc"
+dependencies = [
+ "cc",
+ "libc",
+ "pkg-config",
+]
+
+[[package]]
 name = "cache-key"
 version = "0.0.1"
-source = "git+https://github.com/astral-sh/uv.git?tag=0.1.31#7bcca28b12cd12a6fdf902ec8ae2c48630ba7356"
+source = "git+https://github.com/astral-sh/uv.git?tag=0.1.38#0b23caa18d7eb2f874d73e57b7b4bdf35e881a46"
 dependencies = [
  "hex",
  "seahash",
  "url",
 ]
 
 [[package]]
@@ -408,14 +483,23 @@
 checksum = "2678b2e3449475e95b0aa6f9b506a28e61b3dc8996592b983695e8ebb58a8b41"
 dependencies = [
  "jobserver",
  "libc",
 ]
 
 [[package]]
+name = "cexpr"
+version = "0.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6fac387a98bb7c37292057cffc56d62ecb629900026402633ae9160df93a8766"
+dependencies = [
+ "nom",
+]
+
+[[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "charset"
@@ -425,28 +509,39 @@
 dependencies = [
  "base64 0.13.1",
  "encoding_rs",
 ]
 
 [[package]]
 name = "chrono"
-version = "0.4.37"
+version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a0d04d43504c61aa6c7531f1871dd0d418d91130162063b789da00fd7057a5e"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits",
  "serde",
  "wasm-bindgen",
  "windows-targets 0.52.5",
 ]
 
 [[package]]
+name = "clang-sys"
+version = "1.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "67523a3b4be3ce1989d607a828d036249522dd9c1c8de7f4dd2dae43a37369d1"
+dependencies = [
+ "glob",
+ "libc",
+ "libloading",
+]
+
+[[package]]
 name = "clap"
 version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "90bc066a67923782aa8515dbaea16946c5bcc5addbd668bb80af688e53e548a0"
 dependencies = [
  "clap_builder",
  "clap_derive",
@@ -488,14 +583,23 @@
 [[package]]
 name = "clap_lex"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
 
 [[package]]
+name = "cmake"
+version = "0.1.50"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a31c789563b815f77f4250caee12365734369f942439b7defd71e18a48197130"
+dependencies = [
+ "cc",
+]
+
+[[package]]
 name = "colorchoice"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
 
 [[package]]
 name = "concurrent-queue"
@@ -629,14 +733,25 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "derive_arbitrary"
+version = "1.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "67e77553c4162a157adbf834ebae5b415acbecbeafc7a74b0e886657506a7611"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.58",
+]
+
+[[package]]
 name = "digest"
 version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
  "block-buffer",
  "crypto-common",
@@ -663,34 +778,35 @@
  "redox_users",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "distribution-filename"
 version = "0.0.1"
-source = "git+https://github.com/astral-sh/uv.git?tag=0.1.31#7bcca28b12cd12a6fdf902ec8ae2c48630ba7356"
+source = "git+https://github.com/astral-sh/uv.git?tag=0.1.38#0b23caa18d7eb2f874d73e57b7b4bdf35e881a46"
 dependencies = [
  "pep440_rs",
  "platform-tags",
  "rkyv",
  "serde",
  "thiserror",
  "url",
  "uv-normalize",
 ]
 
 [[package]]
 name = "distribution-types"
 version = "0.0.1"
-source = "git+https://github.com/astral-sh/uv.git?tag=0.1.31#7bcca28b12cd12a6fdf902ec8ae2c48630ba7356"
+source = "git+https://github.com/astral-sh/uv.git?tag=0.1.38#0b23caa18d7eb2f874d73e57b7b4bdf35e881a46"
 dependencies = [
  "anyhow",
  "cache-key",
  "distribution-filename",
  "fs-err",
+ "git2",
  "itertools",
  "once_cell",
  "pep440_rs",
  "pep508_rs",
  "platform-tags",
  "pypi-types",
  "rkyv",
@@ -833,14 +949,20 @@
 checksum = "9564fc758e15025b46aa6643b1b77d047d1a56a1aea6e01002ac0c7026876213"
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
+name = "fs_extra"
+version = "1.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "42703706b716c37f96a77aea830392ad231f44c9e9a67872fa5548707e11b11c"
+
+[[package]]
 name = "funty"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e6d5a32815ae3f33302d95fdcb2ce17862f8c65363dcfd29360480ba1001fc9c"
 
 [[package]]
 name = "futures"
@@ -1004,33 +1126,14 @@
  "bstr",
  "log",
  "regex-automata",
  "regex-syntax",
 ]
 
 [[package]]
-name = "h2"
-version = "0.3.26"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "81fe527a889e1532da5c525686d96d4c2e74cdd345badf8dfef9f6b39dd5f5e8"
-dependencies = [
- "bytes",
- "fnv",
- "futures-core",
- "futures-sink",
- "futures-util",
- "http",
- "indexmap",
- "slab",
- "tokio",
- "tokio-util",
- "tracing",
-]
-
-[[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 dependencies = [
  "ahash",
 ]
@@ -1084,31 +1187,43 @@
 checksum = "6d1ad449764d627e22bfd7cd5e8868264fc9236e07c752972b4080cd351cb476"
 dependencies = [
  "utf8-width",
 ]
 
 [[package]]
 name = "http"
-version = "0.2.12"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "601cbb57e577e2f5ef5be8e7b83f0f63994f25aa94d673e54a92d5c516d101f1"
+checksum = "21b9ddb458710bc376481b842f5da65cdf31522de232c1ca8146abce2a358258"
 dependencies = [
  "bytes",
  "fnv",
  "itoa",
 ]
 
 [[package]]
 name = "http-body"
-version = "0.4.6"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1cac85db508abc24a2e48553ba12a996e87244a0395ce011e62b37158745d643"
+dependencies = [
+ "bytes",
+ "http",
+]
+
+[[package]]
+name = "http-body-util"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ceab25649e9960c0311ea418d17bee82c0dcec1bd053b5f9a66e265a693bed2"
+checksum = "0475f8b2ac86659c21b64320d5d653f9efe42acd2a4e560073ec61a155a34f1d"
 dependencies = [
  "bytes",
+ "futures-core",
  "http",
+ "http-body",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "http-content-range"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1117,55 +1232,67 @@
 [[package]]
 name = "httparse"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d897f394bad6a705d5f4104762e116a75639e470d80901eed05a860a95cb1904"
 
 [[package]]
-name = "httpdate"
-version = "1.0.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "df3b46402a9d5adb4c86a0cf463f42e19994e3ee891101b1841f30a545cb49a9"
-
-[[package]]
 name = "hyper"
-version = "0.14.28"
+version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf96e135eb83a2a8ddf766e426a841d8ddd7449d5f00d34ea02b41d2f19eef80"
+checksum = "fe575dd17d0862a9a33781c8c4696a55c320909004a67a00fb286ba8b1bc496d"
 dependencies = [
  "bytes",
  "futures-channel",
- "futures-core",
  "futures-util",
- "h2",
  "http",
  "http-body",
  "httparse",
- "httpdate",
  "itoa",
  "pin-project-lite",
- "socket2",
+ "smallvec",
  "tokio",
- "tower-service",
- "tracing",
  "want",
 ]
 
 [[package]]
 name = "hyper-rustls"
-version = "0.24.2"
+version = "0.26.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ec3efd23720e2049821a693cbc7e65ea87c72f1c58ff2f9522ff332b1491e590"
+checksum = "a0bea761b46ae2b24eb4aef630d8d1c398157b6fc29e6350ecf090a0b70c952c"
 dependencies = [
  "futures-util",
  "http",
  "hyper",
- "rustls",
+ "hyper-util",
+ "rustls 0.22.4",
+ "rustls-pki-types",
  "tokio",
  "tokio-rustls",
+ "tower-service",
+]
+
+[[package]]
+name = "hyper-util"
+version = "0.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca38ef113da30126bbff9cd1705f9273e15d45498615d138b0c20279ac7a76aa"
+dependencies = [
+ "bytes",
+ "futures-channel",
+ "futures-util",
+ "http",
+ "http-body",
+ "hyper",
+ "pin-project-lite",
+ "socket2",
+ "tokio",
+ "tower",
+ "tower-service",
+ "tracing",
 ]
 
 [[package]]
 name = "iana-time-zone"
 version = "0.1.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e7ffbb5a1b541ea2561f8c41c087286cc091e21e556a4f09a8f6cbf17b69b141"
@@ -1223,15 +1350,15 @@
  "hashbrown 0.14.3",
  "serde",
 ]
 
 [[package]]
 name = "install-wheel-rs"
 version = "0.0.1"
-source = "git+https://github.com/astral-sh/uv.git?tag=0.1.31#7bcca28b12cd12a6fdf902ec8ae2c48630ba7356"
+source = "git+https://github.com/astral-sh/uv.git?tag=0.1.38#0b23caa18d7eb2f874d73e57b7b4bdf35e881a46"
 dependencies = [
  "configparser",
  "csv",
  "data-encoding",
  "distribution-filename",
  "fs-err",
  "mailparse",
@@ -1314,14 +1441,26 @@
 checksum = "ca39ef0d69b18e6a2fd14c2f0a1d593200f4a4ed949b240b5917ab51fac754cb"
 dependencies = [
  "scopeguard",
  "winapi",
 ]
 
 [[package]]
+name = "lazy_static"
+version = "1.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
+
+[[package]]
+name = "lazycell"
+version = "1.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "830d08ce1d1d941e6b30645f1a0eb5643013d835ce3779a5fc208261dbe10f55"
+
+[[package]]
 name = "libc"
 version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "libgit2-sys"
@@ -1334,14 +1473,24 @@
  "libssh2-sys",
  "libz-sys",
  "openssl-sys",
  "pkg-config",
 ]
 
 [[package]]
+name = "libloading"
+version = "0.8.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0c2a198fb6b0eada2a8df47933734e6d35d350665a33a3593d7164fa52c75c19"
+dependencies = [
+ "cfg-if",
+ "windows-targets 0.52.5",
+]
+
+[[package]]
 name = "libredox"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c0ff37bd590ca25063e35af745c343cb7a0271906fb7b37e4813e8f79f00268d"
 dependencies = [
  "bitflags 2.5.0",
  "libc",
@@ -1403,14 +1552,24 @@
 dependencies = [
  "charset",
  "data-encoding",
  "quoted_printable",
 ]
 
 [[package]]
+name = "md-5"
+version = "0.10.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d89e7ee0cfbedfc4da3340218492196241d89eefb6dab27de5df917a6d2e78cf"
+dependencies = [
+ "cfg-if",
+ "digest",
+]
+
+[[package]]
 name = "memchr"
 version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memmap2"
@@ -1424,22 +1583,18 @@
 [[package]]
 name = "mime"
 version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
 
 [[package]]
-name = "mime_guess"
-version = "2.0.4"
+name = "minimal-lexical"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4192263c238a5f0d0c6bfd21f336a313a4ce1c450542449ca191bb657b4642ef"
-dependencies = [
- "mime",
- "unicase",
-]
+checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "miniz_oxide"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
@@ -1463,23 +1618,39 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "359f76430b20a79f9e20e115b3428614e654f04fab314482fc0fda0ebd3c6044"
 dependencies = [
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "mirai-annotations"
+version = "1.12.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c9be0862c1b3f26a88803c4a49de6889c10e608b3ee9344e6ef5b45fb37ad3d1"
+
+[[package]]
 name = "nanoid"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3ffa00dec017b5b1a8b7cf5e2c008bfda1aa7e0697ac1508b491fdf2622fb4d8"
 dependencies = [
  "rand",
 ]
 
 [[package]]
+name = "nom"
+version = "7.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
+dependencies = [
+ "memchr",
+ "minimal-lexical",
+]
+
+[[package]]
 name = "num-traits"
 version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
 dependencies = [
  "autocfg",
 ]
@@ -1502,15 +1673,15 @@
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "once-map"
 version = "0.0.1"
-source = "git+https://github.com/astral-sh/uv.git?tag=0.1.31#7bcca28b12cd12a6fdf902ec8ae2c48630ba7356"
+source = "git+https://github.com/astral-sh/uv.git?tag=0.1.38#0b23caa18d7eb2f874d73e57b7b4bdf35e881a46"
 dependencies = [
  "dashmap",
  "tokio",
 ]
 
 [[package]]
 name = "once_cell"
@@ -1605,35 +1776,53 @@
 [[package]]
 name = "paste"
 version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
 
 [[package]]
+name = "path-absolutize"
+version = "3.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e4af381fe79fa195b4909485d99f73a80792331df0625188e707854f0b3383f5"
+dependencies = [
+ "path-dedot",
+]
+
+[[package]]
+name = "path-dedot"
+version = "3.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "07ba0ad7e047712414213ff67533e6dd477af0a4e1d14fb52343e53d30ea9397"
+dependencies = [
+ "once_cell",
+]
+
+[[package]]
 name = "pathdiff"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8835116a5c179084a830efb3adc117ab007512b535bc1a21c991d3b32a6b44dd"
 
 [[package]]
 name = "pep440_rs"
 version = "0.5.0"
-source = "git+https://github.com/astral-sh/uv.git?tag=0.1.31#7bcca28b12cd12a6fdf902ec8ae2c48630ba7356"
+source = "git+https://github.com/astral-sh/uv.git?tag=0.1.38#0b23caa18d7eb2f874d73e57b7b4bdf35e881a46"
 dependencies = [
  "once_cell",
  "rkyv",
  "serde",
  "unicode-width",
  "unscanny",
 ]
 
 [[package]]
 name = "pep508_rs"
 version = "0.4.2"
-source = "git+https://github.com/astral-sh/uv.git?tag=0.1.31#7bcca28b12cd12a6fdf902ec8ae2c48630ba7356"
+source = "git+https://github.com/astral-sh/uv.git?tag=0.1.38#0b23caa18d7eb2f874d73e57b7b4bdf35e881a46"
 dependencies = [
  "derivative",
  "once_cell",
  "pep440_rs",
  "regex",
  "serde",
  "thiserror",
@@ -1696,28 +1885,38 @@
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "platform-tags"
 version = "0.0.1"
-source = "git+https://github.com/astral-sh/uv.git?tag=0.1.31#7bcca28b12cd12a6fdf902ec8ae2c48630ba7356"
+source = "git+https://github.com/astral-sh/uv.git?tag=0.1.38#0b23caa18d7eb2f874d73e57b7b4bdf35e881a46"
 dependencies = [
  "rustc-hash",
  "serde",
  "thiserror",
 ]
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
+name = "prettyplease"
+version = "0.2.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8d3928fb5db768cb86f891ff014f0144589297e3c6a1aba6ed7cecfdace270c7"
+dependencies = [
+ "proc-macro2",
+ "syn 2.0.58",
+]
+
+[[package]]
 name = "proc-macro2"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
@@ -1741,15 +1940,15 @@
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pypi-types"
 version = "0.0.1"
-source = "git+https://github.com/astral-sh/uv.git?tag=0.1.31#7bcca28b12cd12a6fdf902ec8ae2c48630ba7356"
+source = "git+https://github.com/astral-sh/uv.git?tag=0.1.38#0b23caa18d7eb2f874d73e57b7b4bdf35e881a46"
 dependencies = [
  "chrono",
  "indexmap",
  "mailparse",
  "once_cell",
  "pep440_rs",
  "pep508_rs",
@@ -1920,15 +2119,15 @@
 dependencies = [
  "bytecheck",
 ]
 
 [[package]]
 name = "requirements-txt"
 version = "0.0.1"
-source = "git+https://github.com/astral-sh/uv.git?tag=0.1.31#7bcca28b12cd12a6fdf902ec8ae2c48630ba7356"
+source = "git+https://github.com/astral-sh/uv.git?tag=0.1.38#0b23caa18d7eb2f874d73e57b7b4bdf35e881a46"
 dependencies = [
  "fs-err",
  "pep508_rs",
  "regex",
  "serde",
  "tracing",
  "unscanny",
@@ -1938,45 +2137,45 @@
  "uv-fs",
  "uv-normalize",
  "uv-warnings",
 ]
 
 [[package]]
 name = "reqwest"
-version = "0.11.27"
+version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd67538700a17451e7cba03ac727fb961abb7607553461627b97de0b89cf4a62"
+checksum = "566cafdd92868e0939d3fb961bd0dc25fcfaaed179291093b3d43e6b3150ea10"
 dependencies = [
  "async-compression",
- "base64 0.21.7",
+ "base64 0.22.0",
  "bytes",
- "encoding_rs",
+ "futures-channel",
  "futures-core",
  "futures-util",
- "h2",
  "http",
  "http-body",
+ "http-body-util",
  "hyper",
  "hyper-rustls",
+ "hyper-util",
  "ipnet",
  "js-sys",
  "log",
  "mime",
- "mime_guess",
  "once_cell",
  "percent-encoding",
  "pin-project-lite",
- "rustls",
+ "rustls 0.22.4",
  "rustls-native-certs",
  "rustls-pemfile",
+ "rustls-pki-types",
  "serde",
  "serde_json",
  "serde_urlencoded",
  "sync_wrapper",
- "system-configuration",
  "tokio",
  "tokio-rustls",
  "tokio-util",
  "tower-service",
  "url",
  "wasm-bindgen",
  "wasm-bindgen-futures",
@@ -1984,55 +2183,54 @@
  "web-sys",
  "webpki-roots",
  "winreg",
 ]
 
 [[package]]
 name = "reqwest-middleware"
-version = "0.2.5"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a735987236a8e238bf0296c7e351b999c188ccc11477f311b82b55c93984216"
+checksum = "0209efb52486ad88136190094ee214759ef7507068b27992256ed6610eb71a01"
 dependencies = [
  "anyhow",
  "async-trait",
  "http",
  "reqwest",
  "serde",
- "task-local-extensions",
  "thiserror",
+ "tower-service",
 ]
 
 [[package]]
 name = "reqwest-retry"
-version = "0.3.0"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9af20b65c2ee9746cc575acb6bd28a05ffc0d15e25c992a8f4462d8686aacb4f"
+checksum = "40f342894422862af74c50e1e9601cf0931accc9c6981e5eb413c46603b616b5"
 dependencies = [
  "anyhow",
  "async-trait",
  "chrono",
  "futures",
  "getrandom",
  "http",
  "hyper",
  "parking_lot",
  "reqwest",
  "reqwest-middleware",
  "retry-policies",
- "task-local-extensions",
  "tokio",
  "tracing",
  "wasm-timer",
 ]
 
 [[package]]
 name = "retry-policies"
-version = "0.2.1"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17dd00bff1d737c40dbcd47d4375281bf4c17933f9eef0a185fc7bacca23ecbd"
+checksum = "493b4243e32d6eedd29f9a398896e35c6943a123b55eec97dcaee98310d25810"
 dependencies = [
  "anyhow",
  "chrono",
  "rand",
 ]
 
 [[package]]
@@ -2077,28 +2275,28 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "rmp"
-version = "0.8.12"
+version = "0.8.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f9860a6cc38ed1da53456442089b4dfa35e7cedaa326df63017af88385e6b20"
+checksum = "228ed7c16fa39782c3b3468e974aec2795e9089153cd08ee2e9aefb3613334c4"
 dependencies = [
  "byteorder",
  "num-traits",
  "paste",
 ]
 
 [[package]]
 name = "rmp-serde"
-version = "1.1.2"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bffea85eea980d8a74453e5d02a8d93028f3c34725de143085a844ebe953258a"
+checksum = "938a142ab806f18b88a97b0dea523d39e0fd730a064b035726adcfc58a8a5188"
 dependencies = [
  "byteorder",
  "rmp",
  "serde",
 ]
 
 [[package]]
@@ -2133,52 +2331,79 @@
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.21.10"
+version = "0.22.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9d5a6813c0759e4609cd494e8e725babae6a2ca7b62a5536a13daaec6fcb7ba"
+checksum = "bf4ef73721ac7bcd79b2b315da7779d8fc09718c6b3d2d1b2d94850eb8c18432"
 dependencies = [
  "log",
  "ring",
+ "rustls-pki-types",
  "rustls-webpki",
- "sct",
+ "subtle",
+ "zeroize",
+]
+
+[[package]]
+name = "rustls"
+version = "0.23.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "afabcee0551bd1aa3e18e5adbf2c0544722014b899adb31bd186ec638d3da97e"
+dependencies = [
+ "aws-lc-rs",
+ "log",
+ "once_cell",
+ "rustls-pki-types",
+ "rustls-webpki",
+ "subtle",
+ "zeroize",
 ]
 
 [[package]]
 name = "rustls-native-certs"
-version = "0.6.3"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9aace74cb666635c918e9c12bc0d348266037aa8eb599b5cba565709a8dff00"
+checksum = "8f1fb85efa936c42c6d5fc28d2629bb51e4b2f4b8a5211e297d599cc5a093792"
 dependencies = [
  "openssl-probe",
  "rustls-pemfile",
+ "rustls-pki-types",
  "schannel",
  "security-framework",
 ]
 
 [[package]]
 name = "rustls-pemfile"
-version = "1.0.4"
+version = "2.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c74cae0a4cf6ccbbf5f359f08efdf8ee7e1dc532573bf0db71968cb56b1448c"
+checksum = "29993a25686778eb88d4189742cd713c9bce943bc54251a33509dc63cbacf73d"
 dependencies = [
- "base64 0.21.7",
+ "base64 0.22.0",
+ "rustls-pki-types",
 ]
 
 [[package]]
+name = "rustls-pki-types"
+version = "1.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "beb461507cee2c2ff151784c52762cf4d9ff6a61f3e80968600ed24fa837fa54"
+
+[[package]]
 name = "rustls-webpki"
-version = "0.101.7"
+version = "0.102.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8b6275d1ee7a1cd780b64aca7726599a1dbc893b1e64144529e55c3c2f745765"
+checksum = "f3bce581c0dd41bce533ce695a1437fa16a7ab5ac3ccfa99fe1a620a7885eabf"
 dependencies = [
+ "aws-lc-rs",
  "ring",
+ "rustls-pki-types",
  "untrusted",
 ]
 
 [[package]]
 name = "ryu"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2205,24 +2430,14 @@
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
-name = "sct"
-version = "0.7.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da046153aa2352493d6cb7da4b6e5c0c057d8a1d0a9aa8560baffdd945acd414"
-dependencies = [
- "ring",
- "untrusted",
-]
-
-[[package]]
 name = "seahash"
 version = "4.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1c107b6f4780854c8b126e228ea8869f4d7b71260f962fefb57b996b8959ba6b"
 
 [[package]]
 name = "security-framework"
@@ -2245,37 +2460,37 @@
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.58",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.115"
+version = "1.0.116"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
+checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -2324,14 +2539,20 @@
 [[package]]
 name = "shell-escape"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "45bb67a18fa91266cc7807181f62f9178a6873bfad7dc788c42e6430db40184f"
 
 [[package]]
+name = "shlex"
+version = "1.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0fda2ff0d084019ba4d7c6f371c95d8fd75ce3524c3cb8fb653a3023f6323e64"
+
+[[package]]
 name = "signal-hook-registry"
 version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
 dependencies = [
  "libc",
 ]
@@ -2430,50 +2651,20 @@
 checksum = "0b3a0d0aba8bf96a0e1ddfdc352fc53b3df7f39318c71854910c3c4b024ae52c"
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
-name = "system-configuration"
-version = "0.5.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba3a3adc5c275d719af8cb4272ea1c4a6d668a777f37e115f6d11ddbc1c8e0e7"
-dependencies = [
- "bitflags 1.3.2",
- "core-foundation",
- "system-configuration-sys",
-]
-
-[[package]]
-name = "system-configuration-sys"
-version = "0.5.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a75fb188eb626b924683e3b95e3a48e63551fcfb51949de2f06a9d91dbee93c9"
-dependencies = [
- "core-foundation-sys",
- "libc",
-]
-
-[[package]]
 name = "tap"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "55937e1799185b12863d447f42597ed69d9928686b8d88a1df17376a097d8369"
 
 [[package]]
-name = "task-local-extensions"
-version = "0.1.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba323866e5d033818e3240feeb9f7db2c4296674e4d9e16b97b7bf8f490434e8"
-dependencies = [
- "pin-utils",
-]
-
-[[package]]
 name = "tempfile"
 version = "3.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85b77fafb263dd9d05cbeac119526425676db3784113aa9295c88498cbf8bff1"
 dependencies = [
  "cfg-if",
  "fastrand",
@@ -2549,19 +2740,20 @@
  "proc-macro2",
  "quote",
  "syn 2.0.58",
 ]
 
 [[package]]
 name = "tokio-rustls"
-version = "0.24.1"
+version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c28327cf380ac148141087fbfb9de9d7bd4e84ab5d2c28fbc911d753de8a7081"
+checksum = "775e0c0f0adb3a2f22a00c4745d728b479985fc15ee7ca6a2608388c5569860f"
 dependencies = [
- "rustls",
+ "rustls 0.22.4",
+ "rustls-pki-types",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-stream"
 version = "0.1.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2634,25 +2826,48 @@
  "serde",
  "serde_spanned",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
+name = "tower"
+version = "0.4.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b8fa9be0de6cf49e536ce1851f987bd21a43b771b09473c3549a6c853db37c1c"
+dependencies = [
+ "futures-core",
+ "futures-util",
+ "pin-project",
+ "pin-project-lite",
+ "tokio",
+ "tower-layer",
+ "tower-service",
+ "tracing",
+]
+
+[[package]]
+name = "tower-layer"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c20c8dbed6283a09604c3e69b4b7eeb54e298b8a600d4d5ecb5ad39de609f1d0"
+
+[[package]]
 name = "tower-service"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6bc1c9ce2b5135ac7f93c72918fc37feb872bdc6a5533a8b85eb4b86bfdae52"
 
 [[package]]
 name = "tracing"
 version = "0.1.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c3523ab5a71916ccf420eebdf5521fcef02141234bbc0b8a49f2fdc4544364ef"
 dependencies = [
+ "log",
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
@@ -2683,23 +2898,14 @@
 [[package]]
 name = "typenum"
 version = "1.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "42ff0bf0c66b8238c6f3b578df37d0b7848e55df8577b3f74f92a69acceeb825"
 
 [[package]]
-name = "unicase"
-version = "2.7.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f7d2d4dafb69621809a81864c9c1b864479e1235c0dd4e199924b9742439ed89"
-dependencies = [
- "version_check",
-]
-
-[[package]]
 name = "unicode-bidi"
 version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08f95100a766bf4f8f28f90d77e0a5461bbdb219042e7679bebe79004fed8d75"
 
 [[package]]
 name = "unicode-ident"
@@ -2769,33 +2975,36 @@
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
 
 [[package]]
 name = "uv-auth"
 version = "0.0.1"
-source = "git+https://github.com/astral-sh/uv.git?tag=0.1.31#7bcca28b12cd12a6fdf902ec8ae2c48630ba7356"
+source = "git+https://github.com/astral-sh/uv.git?tag=0.1.38#0b23caa18d7eb2f874d73e57b7b4bdf35e881a46"
 dependencies = [
+ "anyhow",
  "async-trait",
  "base64 0.22.0",
+ "futures",
+ "http",
+ "once-map",
  "once_cell",
  "reqwest",
  "reqwest-middleware",
  "rust-netrc",
- "task-local-extensions",
- "thiserror",
+ "tokio",
  "tracing",
  "url",
  "urlencoding",
 ]
 
 [[package]]
 name = "uv-cache"
 version = "0.0.1"
-source = "git+https://github.com/astral-sh/uv.git?tag=0.1.31#7bcca28b12cd12a6fdf902ec8ae2c48630ba7356"
+source = "git+https://github.com/astral-sh/uv.git?tag=0.1.38#0b23caa18d7eb2f874d73e57b7b4bdf35e881a46"
 dependencies = [
  "cache-key",
  "cachedir",
  "directories",
  "distribution-types",
  "fs-err",
  "nanoid",
@@ -2810,15 +3019,15 @@
  "uv-normalize",
  "walkdir",
 ]
 
 [[package]]
 name = "uv-client"
 version = "0.0.1"
-source = "git+https://github.com/astral-sh/uv.git?tag=0.1.31#7bcca28b12cd12a6fdf902ec8ae2c48630ba7356"
+source = "git+https://github.com/astral-sh/uv.git?tag=0.1.38#0b23caa18d7eb2f874d73e57b7b4bdf35e881a46"
 dependencies = [
  "anyhow",
  "async-trait",
  "async_http_range_reader",
  "async_zip",
  "cache-key",
  "chrono",
@@ -2834,21 +3043,17 @@
  "platform-tags",
  "pypi-types",
  "reqwest",
  "reqwest-middleware",
  "reqwest-retry",
  "rkyv",
  "rmp-serde",
- "rustc-hash",
- "rustls",
- "rustls-native-certs",
  "serde",
  "serde_json",
  "sys-info",
- "task-local-extensions",
  "tempfile",
  "thiserror",
  "tl",
  "tokio",
  "tokio-util",
  "tracing",
  "url",
@@ -2856,35 +3061,34 @@
  "uv-auth",
  "uv-cache",
  "uv-configuration",
  "uv-fs",
  "uv-normalize",
  "uv-version",
  "uv-warnings",
- "webpki-roots",
 ]
 
 [[package]]
 name = "uv-configuration"
 version = "0.0.1"
-source = "git+https://github.com/astral-sh/uv.git?tag=0.1.31#7bcca28b12cd12a6fdf902ec8ae2c48630ba7356"
+source = "git+https://github.com/astral-sh/uv.git?tag=0.1.38#0b23caa18d7eb2f874d73e57b7b4bdf35e881a46"
 dependencies = [
  "anyhow",
- "distribution-types",
  "itertools",
  "pep508_rs",
+ "platform-tags",
  "rustc-hash",
- "uv-cache",
+ "uv-auth",
  "uv-normalize",
 ]
 
 [[package]]
 name = "uv-distribution"
 version = "0.0.1"
-source = "git+https://github.com/astral-sh/uv.git?tag=0.1.31#7bcca28b12cd12a6fdf902ec8ae2c48630ba7356"
+source = "git+https://github.com/astral-sh/uv.git?tag=0.1.38#0b23caa18d7eb2f874d73e57b7b4bdf35e881a46"
 dependencies = [
  "anyhow",
  "cache-key",
  "distribution-filename",
  "distribution-types",
  "fs-err",
  "futures",
@@ -2916,53 +3120,57 @@
  "uv-types",
  "zip",
 ]
 
 [[package]]
 name = "uv-extract"
 version = "0.0.1"
-source = "git+https://github.com/astral-sh/uv.git?tag=0.1.31#7bcca28b12cd12a6fdf902ec8ae2c48630ba7356"
+source = "git+https://github.com/astral-sh/uv.git?tag=0.1.38#0b23caa18d7eb2f874d73e57b7b4bdf35e881a46"
 dependencies = [
  "async-compression",
  "async_zip",
  "fs-err",
  "futures",
+ "md-5",
+ "pypi-types",
  "rayon",
  "rustc-hash",
+ "sha2",
  "thiserror",
  "tokio",
  "tokio-tar",
  "tokio-util",
  "tracing",
  "zip",
 ]
 
 [[package]]
 name = "uv-fs"
 version = "0.0.1"
-source = "git+https://github.com/astral-sh/uv.git?tag=0.1.31#7bcca28b12cd12a6fdf902ec8ae2c48630ba7356"
+source = "git+https://github.com/astral-sh/uv.git?tag=0.1.38#0b23caa18d7eb2f874d73e57b7b4bdf35e881a46"
 dependencies = [
  "backoff",
  "dunce",
  "encoding_rs_io",
  "fs-err",
  "fs2",
  "junction",
  "once_cell",
+ "path-absolutize",
  "tempfile",
  "tokio",
  "tracing",
  "urlencoding",
  "uv-warnings",
 ]
 
 [[package]]
 name = "uv-git"
 version = "0.0.1"
-source = "git+https://github.com/astral-sh/uv.git?tag=0.1.31#7bcca28b12cd12a6fdf902ec8ae2c48630ba7356"
+source = "git+https://github.com/astral-sh/uv.git?tag=0.1.38#0b23caa18d7eb2f874d73e57b7b4bdf35e881a46"
 dependencies = [
  "anyhow",
  "base64 0.22.0",
  "cache-key",
  "cargo-util",
  "fs-err",
  "git2",
@@ -2977,15 +3185,15 @@
  "url",
  "uv-fs",
 ]
 
 [[package]]
 name = "uv-installer"
 version = "0.0.1"
-source = "git+https://github.com/astral-sh/uv.git?tag=0.1.31#7bcca28b12cd12a6fdf902ec8ae2c48630ba7356"
+source = "git+https://github.com/astral-sh/uv.git?tag=0.1.38#0b23caa18d7eb2f874d73e57b7b4bdf35e881a46"
 dependencies = [
  "anyhow",
  "async-channel",
  "distribution-types",
  "fs-err",
  "futures",
  "install-wheel-rs",
@@ -3015,15 +3223,15 @@
  "uv-warnings",
  "walkdir",
 ]
 
 [[package]]
 name = "uv-interpreter"
 version = "0.0.1"
-source = "git+https://github.com/astral-sh/uv.git?tag=0.1.31#7bcca28b12cd12a6fdf902ec8ae2c48630ba7356"
+source = "git+https://github.com/astral-sh/uv.git?tag=0.1.38#0b23caa18d7eb2f874d73e57b7b4bdf35e881a46"
 dependencies = [
  "cache-key",
  "configparser",
  "fs-err",
  "install-wheel-rs",
  "once_cell",
  "pep440_rs",
@@ -3036,78 +3244,107 @@
  "serde",
  "serde_json",
  "tempfile",
  "thiserror",
  "tracing",
  "uv-cache",
  "uv-fs",
- "which",
+ "uv-toolchain",
+ "uv-warnings",
+ "which 6.0.1",
  "winapi",
 ]
 
 [[package]]
 name = "uv-normalize"
 version = "0.0.1"
-source = "git+https://github.com/astral-sh/uv.git?tag=0.1.31#7bcca28b12cd12a6fdf902ec8ae2c48630ba7356"
+source = "git+https://github.com/astral-sh/uv.git?tag=0.1.38#0b23caa18d7eb2f874d73e57b7b4bdf35e881a46"
 dependencies = [
  "rkyv",
  "serde",
 ]
 
 [[package]]
+name = "uv-toolchain"
+version = "0.1.0"
+source = "git+https://github.com/astral-sh/uv.git?tag=0.1.38#0b23caa18d7eb2f874d73e57b7b4bdf35e881a46"
+dependencies = [
+ "anyhow",
+ "fs-err",
+ "futures",
+ "once_cell",
+ "pep440_rs",
+ "pep508_rs",
+ "reqwest",
+ "reqwest-middleware",
+ "tempfile",
+ "thiserror",
+ "tokio-util",
+ "tracing",
+ "url",
+ "uv-client",
+ "uv-extract",
+ "uv-fs",
+]
+
+[[package]]
 name = "uv-types"
 version = "0.0.1"
-source = "git+https://github.com/astral-sh/uv.git?tag=0.1.31#7bcca28b12cd12a6fdf902ec8ae2c48630ba7356"
+source = "git+https://github.com/astral-sh/uv.git?tag=0.1.38#0b23caa18d7eb2f874d73e57b7b4bdf35e881a46"
 dependencies = [
  "anyhow",
  "distribution-types",
- "itertools",
  "once-map",
+ "pep440_rs",
  "pep508_rs",
+ "pypi-types",
+ "requirements-txt",
  "rustc-hash",
+ "thiserror",
+ "url",
  "uv-cache",
  "uv-configuration",
  "uv-interpreter",
  "uv-normalize",
 ]
 
 [[package]]
 name = "uv-version"
-version = "0.1.31"
-source = "git+https://github.com/astral-sh/uv.git?tag=0.1.31#7bcca28b12cd12a6fdf902ec8ae2c48630ba7356"
+version = "0.1.38"
+source = "git+https://github.com/astral-sh/uv.git?tag=0.1.38#0b23caa18d7eb2f874d73e57b7b4bdf35e881a46"
 
 [[package]]
 name = "uv-warnings"
 version = "0.0.1"
-source = "git+https://github.com/astral-sh/uv.git?tag=0.1.31#7bcca28b12cd12a6fdf902ec8ae2c48630ba7356"
+source = "git+https://github.com/astral-sh/uv.git?tag=0.1.38#0b23caa18d7eb2f874d73e57b7b4bdf35e881a46"
 dependencies = [
  "anstream",
  "once_cell",
  "owo-colors",
  "rustc-hash",
 ]
 
 [[package]]
 name = "uvx"
-version = "2.0.3"
+version = "2.0.5"
 dependencies = [
  "anstyle",
- "async_http_range_reader",
  "chrono",
  "clap",
  "clap_complete",
  "configparser",
  "directories",
  "home",
  "install-wheel-rs",
  "itertools",
  "owo-colors",
  "pep508_rs",
  "regex",
  "rmp-serde",
+ "rustls 0.23.5",
  "serde",
  "serde_json",
  "subprocess",
  "tempfile",
  "tokio",
  "uv-cache",
  "uv-installer",
@@ -3253,17 +3490,32 @@
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "webpki-roots"
-version = "0.25.4"
+version = "0.26.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5f20c57d8d7db6d3b86154206ae5d8fba62dd39573114de97c2cb0578251f8e1"
+checksum = "b3de34ae270483955a94f4b21bdaaeb83d508bb84a01435f393818edb0012009"
+dependencies = [
+ "rustls-pki-types",
+]
+
+[[package]]
+name = "which"
+version = "4.4.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87ba24419a2078cd2b0f2ede2691b6c66d8e47836da3b6db8265ebad47afbfc7"
+dependencies = [
+ "either",
+ "home",
+ "once_cell",
+ "rustix",
+]
 
 [[package]]
 name = "which"
 version = "6.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8211e4f58a2b2805adfbefbc07bab82958fc91e3836339b1ab7ae32465dce0d7"
 dependencies = [
@@ -3488,17 +3740,17 @@
 checksum = "f0c976aaaa0e1f90dbb21e9587cdaf1d9679a1cde8875c0d6bd83ab96a208352"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "winreg"
-version = "0.50.0"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "524e57b2c537c0f9b1e69f1965311ec12182b4122e45035b1508cd24d2adadb1"
+checksum = "a277a57398d4bfa075df44f501a17cfdf8542d224f0d36095a2adc7aee4ef0a5"
 dependencies = [
  "cfg-if",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "winsafe"
@@ -3523,19 +3775,26 @@
 dependencies = [
  "libc",
  "linux-raw-sys",
  "rustix",
 ]
 
 [[package]]
+name = "zeroize"
+version = "1.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
+
+[[package]]
 name = "zip"
-version = "0.6.6"
+version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "760394e246e4c28189f19d488c058bf16f564016aefac5d32bb1f3b51d5e9261"
+checksum = "f2655979068a1f8fa91cb9e8e5b9d3ee54d18e0ddc358f2f4a395afc0929a84b"
 dependencies = [
+ "arbitrary",
  "byteorder",
  "crc32fast",
  "crossbeam-utils",
  "flate2",
 ]
 
 [[package]]
```

### Comparing `uvx-2.0.3/README.md` & `uvx-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `uvx-2.0.3/src/animate.rs` & `uvx-2.0.5/src/animate.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.3/src/cli.rs` & `uvx-2.0.5/src/cli.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.3/src/cmd.rs` & `uvx-2.0.5/src/cmd.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.3/src/commands/completions.rs` & `uvx-2.0.5/src/commands/completions.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.3/src/commands/ensurepath.rs` & `uvx-2.0.5/src/commands/ensurepath.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.3/src/commands/inject.rs` & `uvx-2.0.5/src/commands/inject.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.3/src/commands/install.rs` & `uvx-2.0.5/src/commands/install.rs`

 * *Files 8% similar despite different names*

```diff
@@ -112,20 +112,25 @@
 ) -> Result<(), String> {
     let venv_root = venv.root();
 
     let symlinks = find_symlinks(requirement, &meta.installed_version, venv).await;
 
     let mut results = HashMap::new();
     for symlink in symlinks {
-        results.insert(
-            symlink.clone(),
-            create_symlink(&symlink, venv_root, force, binaries)
-                .await
-                .unwrap_or(false),
-        );
+        let result = create_symlink(&symlink, venv_root, force, binaries).await;
+
+        let success = match result {
+            Ok(_success) => _success,
+            Err(msg) => {
+                eprintln!("⚠️ {}", format!("{}", msg,).yellow());
+                false
+            },
+        };
+
+        results.insert(symlink.clone(), success);
     }
 
     meta.scripts = results;
     meta.save(venv_root).await?;
 
     Ok(())
 }
```

### Comparing `uvx-2.0.3/src/commands/list.rs` & `uvx-2.0.5/src/commands/list.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.3/src/commands/reinstall.rs` & `uvx-2.0.5/src/commands/reinstall.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.3/src/commands/reinstall_all.rs` & `uvx-2.0.5/src/commands/reinstall_all.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.3/src/commands/run.rs` & `uvx-2.0.5/src/commands/run.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.3/src/commands/runpip.rs` & `uvx-2.0.5/src/commands/runpip.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.3/src/commands/runpython.rs` & `uvx-2.0.5/src/commands/runpython.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.3/src/commands/runuv.rs` & `uvx-2.0.5/src/commands/runuv.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.3/src/commands/self_update.rs` & `uvx-2.0.5/src/commands/self_update.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.3/src/commands/uninject.rs` & `uvx-2.0.5/src/commands/uninject.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.3/src/commands/uninstall.rs` & `uvx-2.0.5/src/commands/uninstall.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.3/src/commands/uninstall_all.rs` & `uvx-2.0.5/src/commands/uninstall_all.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.3/src/commands/upgrade.rs` & `uvx-2.0.5/src/commands/upgrade.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.3/src/commands/upgrade_all.rs` & `uvx-2.0.5/src/commands/upgrade_all.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.3/src/helpers.rs` & `uvx-2.0.5/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.3/src/main.rs` & `uvx-2.0.5/src/main.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.3/src/metadata.rs` & `uvx-2.0.5/src/metadata.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.3/src/pip.rs` & `uvx-2.0.5/src/pip.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.3/src/symlinks.rs` & `uvx-2.0.5/src/symlinks.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.3/src/uv.rs` & `uvx-2.0.5/src/uv.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.3/src/venv.rs` & `uvx-2.0.5/src/venv.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.3/pyproject.toml` & `uvx-2.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uvx-2.0.3/PKG-INFO` & `uvx-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: uvx
-Version: 2.0.3
+Version: 2.0.5
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 4 - Beta
 Requires-Dist: uv
 Requires-Dist: pip
```

