# Comparing `tmp/bihyung-0.1.1.tar.gz` & `tmp/bihyung-0.1.2.tar.gz`

## Comparing `bihyung-0.1.1.tar` & `bihyung-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0     1001      127      898 2024-04-27 01:18:58.000000 bihyung-0.1.1/llm-daemon/Cargo.toml
--rw-r--r--   0     1001      127      220 2024-04-27 01:18:58.000000 bihyung-0.1.1/llm-daemon/README.md
--rw-r--r--   0     1001      127     2984 2024-04-27 01:18:58.000000 bihyung-0.1.1/llm-daemon/benches/port_open.rs
--rw-r--r--   0     1001      127     1023 2024-04-27 01:18:58.000000 bihyung-0.1.1/llm-daemon/src/daemon_trait.rs
--rw-r--r--   0     1001      127      429 2024-04-27 01:18:58.000000 bihyung-0.1.1/llm-daemon/src/lib.rs
--rw-r--r--   0     1001      127     6884 2024-04-27 01:18:58.000000 bihyung-0.1.1/llm-daemon/src/llama_daemon/daemon2.rs
--rw-r--r--   0     1001      127     1102 2024-04-27 01:18:58.000000 bihyung-0.1.1/llm-daemon/src/llama_daemon/mod.rs
--rw-r--r--   0     1001      127      950 2024-04-27 01:18:58.000000 bihyung-0.1.1/llm-daemon/src/mlc_daemon/bootstrap.rs
--rw-r--r--   0     1001      127    10739 2024-04-27 01:18:58.000000 bihyung-0.1.1/llm-daemon/src/mlc_daemon/daemon2.rs
--rw-r--r--   0     1001      127       96 2024-04-27 01:18:58.000000 bihyung-0.1.1/llm-daemon/src/mlc_daemon/mod.rs
--rw-r--r--   0     1001      127     8476 2024-04-27 01:18:58.000000 bihyung-0.1.1/llm-daemon/src/proxy.rs
--rw-r--r--   0     1001      127     3934 2024-04-27 01:18:58.000000 bihyung-0.1.1/llm-daemon/src/test_client.rs
--rw-r--r--   0     1001      127       62 2024-04-27 01:18:58.000000 bihyung-0.1.1/llm-daemon/tests/simple_test.rs
--rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 bihyung-0.1.1/bihyung/Cargo.toml
--rw-r--r--   0     1001      127      686 2024-04-27 01:18:58.000000 bihyung-0.1.1/bihyung/.gitignore
--rw-r--r--   0     1001      127     4038 2024-04-27 01:18:58.000000 bihyung-0.1.1/bihyung/src/lib.rs
--rw-r--r--   0     1001      127    50605 2024-04-27 01:18:58.000000 bihyung-0.1.1/Cargo.lock
--rw-r--r--   0        0        0      268 1970-01-01 00:00:00.000000 bihyung-0.1.1/Cargo.toml
--rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 bihyung-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      256 1970-01-01 00:00:00.000000 bihyung-0.1.1/PKG-INFO
+-rw-r--r--   0     1001      127      925 2024-04-27 02:29:22.000000 bihyung-0.1.2/llm-daemon/Cargo.toml
+-rw-r--r--   0     1001      127      220 2024-04-27 02:29:22.000000 bihyung-0.1.2/llm-daemon/README.md
+-rw-r--r--   0     1001      127     2984 2024-04-27 02:29:22.000000 bihyung-0.1.2/llm-daemon/benches/port_open.rs
+-rw-r--r--   0     1001      127     1023 2024-04-27 02:29:22.000000 bihyung-0.1.2/llm-daemon/src/daemon_trait.rs
+-rw-r--r--   0     1001      127      429 2024-04-27 02:29:22.000000 bihyung-0.1.2/llm-daemon/src/lib.rs
+-rw-r--r--   0     1001      127     7133 2024-04-27 02:29:22.000000 bihyung-0.1.2/llm-daemon/src/llama_daemon/daemon2.rs
+-rw-r--r--   0     1001      127     1102 2024-04-27 02:29:22.000000 bihyung-0.1.2/llm-daemon/src/llama_daemon/mod.rs
+-rw-r--r--   0     1001      127      950 2024-04-27 02:29:22.000000 bihyung-0.1.2/llm-daemon/src/mlc_daemon/bootstrap.rs
+-rw-r--r--   0     1001      127    10694 2024-04-27 02:29:22.000000 bihyung-0.1.2/llm-daemon/src/mlc_daemon/daemon2.rs
+-rw-r--r--   0     1001      127       96 2024-04-27 02:29:22.000000 bihyung-0.1.2/llm-daemon/src/mlc_daemon/mod.rs
+-rw-r--r--   0     1001      127     8476 2024-04-27 02:29:22.000000 bihyung-0.1.2/llm-daemon/src/proxy.rs
+-rw-r--r--   0     1001      127     3934 2024-04-27 02:29:22.000000 bihyung-0.1.2/llm-daemon/src/test_client.rs
+-rw-r--r--   0     1001      127       62 2024-04-27 02:29:22.000000 bihyung-0.1.2/llm-daemon/tests/simple_test.rs
+-rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 bihyung-0.1.2/bihyung/Cargo.toml
+-rw-r--r--   0     1001      127      686 2024-04-27 02:29:22.000000 bihyung-0.1.2/bihyung/.gitignore
+-rw-r--r--   0     1001      127     4056 2024-04-27 02:29:22.000000 bihyung-0.1.2/bihyung/src/lib.rs
+-rw-r--r--   0     1001      127    50437 2024-04-27 02:29:22.000000 bihyung-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0      268 1970-01-01 00:00:00.000000 bihyung-0.1.2/Cargo.toml
+-rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 bihyung-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      256 1970-01-01 00:00:00.000000 bihyung-0.1.2/PKG-INFO
```

### Comparing `bihyung-0.1.1/llm-daemon/Cargo.toml` & `bihyung-0.1.2/llm-daemon/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "llm-daemon"
-version = "0.1.1"
+version = "0.1.2"
 edition = "2021"
 license = "GPL-3.0-only"
 keywords = ["llm"]
 description = "LLM as a daemon"
 homepage = "https://github.com/blmarket/llm-daemon"
 repository = "https://github.com/blmarket/llm-daemon"
 readme = "README.md"
@@ -19,14 +19,15 @@
 serde_json = { workspace = true }
 futures = "0.3"
 hyper = { version = "1", features = ["full"] }
 hyper-util = { version = "0.1", features = ["full"] }
 reqwest = { version = "0.12", default-features = false, features = ["json", "rustls-tls"] }
 tempfile = "3"
 url = "2"
+tracing-subscriber = "0.3"
 
 [dev-dependencies]
 tracing-test = "0.2"
 criterion = "0.5"
 
 [features]
 default = ["llama-daemon", "mlc-daemon"]
```

### Comparing `bihyung-0.1.1/llm-daemon/benches/port_open.rs` & `bihyung-0.1.2/llm-daemon/benches/port_open.rs`

 * *Files identical despite different names*

### Comparing `bihyung-0.1.1/llm-daemon/src/daemon_trait.rs` & `bihyung-0.1.2/llm-daemon/src/daemon_trait.rs`

 * *Files identical despite different names*

### Comparing `bihyung-0.1.1/llm-daemon/src/llama_daemon/daemon2.rs` & `bihyung-0.1.2/llm-daemon/src/llama_daemon/daemon2.rs`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 use tokio::io::AsyncWriteExt as _;
 use tokio::net::{UnixListener, UnixStream};
 use tokio::process::Command;
 use tokio::runtime::Builder as RuntimeBuilder;
 use tokio::select;
 use tokio::signal::unix::{signal, SignalKind};
 use tracing::{debug, error, info, trace, warn};
+use tracing_subscriber::util::SubscriberInitExt;
 
 use crate::daemon_trait::LlmConfig;
 use crate::LlmDaemon;
 
 pub struct LlamaConfig {
     pub server_path: PathBuf,
     pub model_path: PathBuf,
@@ -93,14 +94,18 @@
                 if res.is_err() {
                     eprintln!(
                         "Maybe another daemon is already running: {:?}",
                         res.err()
                     );
                     exit(0)
                 }
+                let _guard = tracing_subscriber::FmtSubscriber::builder()
+                    .compact()
+                    .with_max_level(tracing::Level::TRACE)
+                    .set_default();
                 let runtime = RuntimeBuilder::new_current_thread()
                     .enable_time()
                     .enable_io()
                     .build()
                     .expect("failed to create runtime");
                 runtime.block_on(async {
                     let mut cmd = Command::new(self.config.server_path.clone())
```

### Comparing `bihyung-0.1.1/llm-daemon/src/llama_daemon/mod.rs` & `bihyung-0.1.2/llm-daemon/src/llama_daemon/mod.rs`

 * *Files identical despite different names*

### Comparing `bihyung-0.1.1/llm-daemon/src/mlc_daemon/bootstrap.rs` & `bihyung-0.1.2/llm-daemon/src/mlc_daemon/bootstrap.rs`

 * *Files identical despite different names*

### Comparing `bihyung-0.1.1/llm-daemon/src/mlc_daemon/daemon2.rs` & `bihyung-0.1.2/llm-daemon/src/mlc_daemon/daemon2.rs`

 * *Files 2% similar despite different names*

```diff
@@ -140,29 +140,29 @@
 
                     let _ = std::io::stdout().write_all(format!("child: {:?}\n", cmd.id()).as_bytes());
 
                     let listener =
                         UnixListener::bind(&config.sock_file).expect("Failed to open socket");
                     let mut sigterms =
                         signal(SignalKind::terminate()).expect("failed to add SIGTERM handler");
-                    let _ = std::io::stdout().write_all(format!("Starting loop\n").as_bytes());
+                    let _ = std::io::stdout().write_all("Starting loop\n".as_bytes());
                     let _ = std::io::stdout().flush();
                     loop {
                         select! {
                            _ = sigterms.recv() => {
-                               let _ = std::io::stdout().write_all(format!("Got SIGTERM, closing\n").as_bytes());
+                               let _ = std::io::stdout().write_all("Got SIGTERM, closing\n".as_bytes());
                                break;
                            },
                            exit_status = cmd.wait() => {
                                let _ = std::io::stdout().write_all(format!("Child got closed: {:?}\n", exit_status).as_bytes());
                                break;
                            },
                            res = listener.accept() => {
                                let Ok((mut stream, _)) = res else {
-                                   let _ = std::io::stdout().write_all(format!("Failed to accept a socket, closing\n").as_bytes());
+                                   let _ = std::io::stdout().write_all("Failed to accept a socket, closing\n".as_bytes());
                                    break;
                                };
                                let mut buf = [0u8; 32];
                                loop {
                                    let _ = stream.readable().await;
                                    match stream.try_read(&mut buf) {
                                         Ok(sz) => {
@@ -177,28 +177,28 @@
                                             break;
                                         }
                                     }
                                }
                                let _ = stream.shutdown().await;
                            },
                            _ = tokio::time::sleep(Duration::from_secs(2)) => {
-                               let _ = std::io::stdout().write_all(format!("No activitiy for 10 seconds, closing...\n").as_bytes());
+                               let _ = std::io::stdout().write_all("No activitiy for 10 seconds, closing...\n".as_bytes());
                                break;
                            },
                         }
                     }
                     // Child might be already killed, so ignore the error
                     let _ = std::io::stdout().write_all(format!("Closing child: {:?}\n", cmd.id()).as_bytes());
                     cmd.kill().await.ok();
                     // To make sure temp_dir is alive until here
                     drop(temp_dir);
                 });
                 std::fs::remove_file(&config.sock_file).ok();
                 let _ = std::io::stdout()
-                    .write_all(format!("Server closed\n").as_bytes());
+                    .write_all("Server closed\n".as_bytes());
                 exit(0)
             },
             daemonize::Outcome::Parent(res) => {
                 res.expect("parent should have no problem");
             },
         }
         Ok(())
```

### Comparing `bihyung-0.1.1/llm-daemon/src/proxy.rs` & `bihyung-0.1.2/llm-daemon/src/proxy.rs`

 * *Files identical despite different names*

### Comparing `bihyung-0.1.1/llm-daemon/src/test_client.rs` & `bihyung-0.1.2/llm-daemon/src/test_client.rs`

 * *Files identical despite different names*

### Comparing `bihyung-0.1.1/bihyung/.gitignore` & `bihyung-0.1.2/bihyung/.gitignore`

 * *Files identical despite different names*

### Comparing `bihyung-0.1.1/bihyung/src/lib.rs` & `bihyung-0.1.2/bihyung/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -150,21 +150,21 @@
         self.endpoint.clone()
     }
 }
 
 /// A Python module implemented in Rust.
 #[pymodule]
 fn bihyung(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
-    // TODO: Allow user to change log level, for debugging?
-    let subscriber = tracing_subscriber::FmtSubscriber::builder()
-        .with_max_level(tracing::Level::WARN)
-        .finish();
+    // // TODO: Allow user to change log level, for debugging?
+    // let subscriber = tracing_subscriber::FmtSubscriber::builder()
+    //     .with_max_level(tracing::Level::WARN)
+    //     .finish();
 
-    tracing::subscriber::set_global_default(subscriber)
-        .expect("failed to config logging");
+    // tracing::subscriber::set_global_default(subscriber)
+    //     .expect("failed to config logging");
     info!("This will be logged to stdout");
     m.add_class::<Generator>()?;
     m.add_class::<LlamaDaemon>()?;
     m.add_class::<MlcDaemon>()?;
     m.add_class::<ProxyDaemon>()?;
     Ok(())
 }
```

### Comparing `bihyung-0.1.1/Cargo.lock` & `bihyung-0.1.2/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -135,34 +135,28 @@
 name = "base64"
 version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9475866fec1451be56a3c2400fd081ff546538961565ccb5b7142cbd22bc7a51"
 
 [[package]]
 name = "bihyung"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "enum_dispatch",
  "llm-daemon",
  "pyo3",
  "pyo3-asyncio",
  "tokio",
  "tracing",
  "tracing-subscriber",
  "url",
 ]
 
 [[package]]
 name = "bitflags"
-version = "1.3.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
-
-[[package]]
-name = "bitflags"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "bumpalo"
 version = "3.16.0"
@@ -179,17 +173,17 @@
 name = "cast"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "37b2a672a2cb129a2e41c10b1224bb368f9f37a2b16b612598138befd7b37eb5"
 
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
 
@@ -716,38 +710,39 @@
 name = "linux-raw-sys"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
 
 [[package]]
 name = "llm-daemon"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "anyhow",
  "axum",
  "criterion",
  "daemonize",
  "futures",
  "hyper",
  "hyper-util",
  "reqwest",
  "serde",
  "serde_json",
  "tempfile",
  "tokio",
  "tracing",
+ "tracing-subscriber",
  "tracing-test",
  "url",
 ]
 
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
 name = "log"
@@ -865,33 +860,33 @@
 name = "overload"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
 
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
- "windows-targets 0.48.5",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
@@ -1074,19 +1069,19 @@
 dependencies = [
  "crossbeam-deque",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
 ]
 
 [[package]]
 name = "regex"
 version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
@@ -1189,19 +1184,19 @@
 name = "rustc-demangle"
 version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
 
 [[package]]
 name = "rustix"
-version = "0.38.32"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
- "bitflags 2.5.0",
+ "bitflags",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
@@ -1226,23 +1221,23 @@
 dependencies = [
  "base64",
  "rustls-pki-types",
 ]
 
 [[package]]
 name = "rustls-pki-types"
-version = "1.4.1"
+version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ecd36cc4259e3e4514335c4a138c6b43171a8d61d8f5c9348f9fc7529416f247"
+checksum = "beb461507cee2c2ff151784c52762cf4d9ff6a61f3e80968600ed24fa837fa54"
 
 [[package]]
 name = "rustls-webpki"
-version = "0.102.2"
+version = "0.102.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "faaa0a62740bedb9b2ef5afa303da42764c012f743917351dc9a237ea1663610"
+checksum = "f3bce581c0dd41bce533ce695a1437fa16a7ab5ac3ccfa99fe1a620a7885eabf"
 dependencies = [
  "ring",
  "rustls-pki-types",
  "untrusted",
 ]
 
 [[package]]
@@ -1332,17 +1327,17 @@
 checksum = "f40ca3c46823713e0d4209592e8d6e826aa57e928f09752619fc696c499637f6"
 dependencies = [
  "lazy_static",
 ]
 
 [[package]]
 name = "signal-hook-registry"
-version = "1.4.1"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
+checksum = "a9e9e0b4211b72e7b8b6e85c807d36c212bdb33ea8587f7569562a84df5465b1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "slab"
 version = "0.4.9"
@@ -1815,19 +1810,19 @@
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
 name = "winapi-util"
-version = "0.1.6"
+version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
+checksum = "4d4cc384e1e73b93bafa6fb4f1df8c41695c8a91cf9c4c64358067d15a7b6c6b"
 dependencies = [
- "winapi",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
```

