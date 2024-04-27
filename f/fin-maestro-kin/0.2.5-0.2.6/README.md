# Comparing `tmp/fin_maestro_kin-0.2.5.tar.gz` & `tmp/fin_maestro_kin-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fin_maestro_kin-0.2.5.tar", max compression
+gzip compressed data, was "fin_maestro_kin-0.2.6.tar", max compression
```

## Comparing `fin_maestro_kin-0.2.5.tar` & `fin_maestro_kin-0.2.6.tar`

### file list

```diff
@@ -1,35 +1,17 @@
--rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.5/fin_maestro_kin/__init__.py
--rw-r--r--   0        0        0     1872 2024-04-20 19:23:53.441398 fin_maestro_kin-0.2.5/fin_maestro_kin/constants.py
--rw-r--r--   0        0        0     1025 2024-04-15 18:30:00.477406 fin_maestro_kin-0.2.5/fin_maestro_kin/main.py
--rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/__init__.py
--rw-r--r--   0        0        0      170 2024-03-23 08:46:49.868081 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0       18 2024-03-31 06:15:52.175723 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/__init__.py
--rw-r--r--   0        0        0      203 2024-03-31 06:41:27.749444 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/nse/__init__.py
--rw-r--r--   0        0        0      187 2024-03-23 08:47:13.994885 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/nse/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     9115 2024-04-15 18:39:26.059998 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/nse/__pycache__/helper.cpython-39.pyc
--rw-r--r--   0        0        0    13150 2024-04-15 18:33:51.983822 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/nse/__pycache__/nse_equities.cpython-39.pyc
--rw-r--r--   0        0        0     5973 2024-04-07 13:52:21.935537 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/nse/__pycache__/nse_indices.cpython-39.pyc
--rw-r--r--   0        0        0    12705 2024-04-15 18:39:19.947514 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/nse/helper.py
--rw-r--r--   0        0        0    19042 2024-04-15 18:33:45.624559 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/nse/nse_equities.py
--rw-r--r--   0        0        0     7634 2024-04-07 13:52:15.430589 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/nse/nse_indices.py
--rw-r--r--   0        0        0        0 2024-04-13 06:37:31.671927 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/screener/__init__.py
--rw-r--r--   0        0        0      192 2024-04-15 16:55:29.743148 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/screener/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3011 2024-04-19 20:03:28.320060 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/screener/__pycache__/helper.cpython-39.pyc
--rw-r--r--   0        0        0     8493 2024-04-19 20:04:53.435533 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/screener/__pycache__/screener_equities.cpython-39.pyc
--rw-r--r--   0        0        0     3209 2024-04-20 19:23:53.441398 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/screener/helper.py
--rw-r--r--   0        0        0    11704 2024-04-20 19:23:53.441398 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/screener/screener_equities.py
--rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/sentiment_analysis/__init__.py
--rw-r--r--   0        0        0      189 2024-03-17 10:59:01.312818 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/sentiment_analysis/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1358 2024-03-17 10:59:01.500759 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/sentiment_analysis/__pycache__/pcr_data.cpython-39.pyc
--rw-r--r--   0        0        0     2131 2024-03-17 10:59:01.344089 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/sentiment_analysis/__pycache__/sentiment_analysis.cpython-39.pyc
--rw-r--r--   0        0        0     1563 2024-02-10 16:25:56.398293 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/sentiment_analysis/pcr_data.py
--rw-r--r--   0        0        0     2109 2024-02-25 06:17:29.811861 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/sentiment_analysis/sentiment_analysis.py
--rw-r--r--   0        0        0        0 2024-02-10 15:38:47.413185 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/trend_detector/__init__.py
--rw-r--r--   0        0        0      185 2024-03-17 10:59:10.299081 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/trend_detector/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2006 2024-03-17 10:59:10.346263 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/trend_detector/__pycache__/trend_detector.cpython-39.pyc
--rw-r--r--   0        0        0     2074 2024-02-25 06:17:29.827487 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/trend_detector/trend_detector.py
--rw-r--r--   0        0        0     1090 2024-02-10 16:19:33.663653 fin_maestro_kin-0.2.5/LICENSE
--rw-r--r--   0        0        0      642 2024-04-20 19:24:48.839169 fin_maestro_kin-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     5347 2024-04-15 16:54:12.969094 fin_maestro_kin-0.2.5/README.md
--rw-r--r--   0        0        0     6235 1970-01-01 00:00:00.000000 fin_maestro_kin-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.6/fin_maestro_kin/__init__.py
+-rw-r--r--   0        0        0     1872 2024-04-26 21:46:47.948773 fin_maestro_kin-0.2.6/fin_maestro_kin/constants.py
+-rw-r--r--   0        0        0     1007 2024-04-27 07:19:02.530376 fin_maestro_kin-0.2.6/fin_maestro_kin/main.py
+-rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.6/fin_maestro_kin/modules/__init__.py
+-rw-r--r--   0        0        0       18 2024-03-31 06:15:52.175723 fin_maestro_kin-0.2.6/fin_maestro_kin/modules/data_toolkit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 22:03:36.979909 fin_maestro_kin-0.2.6/fin_maestro_kin/modules/data_toolkit/nse/__init__.py
+-rw-r--r--   0        0        0    42792 2024-04-26 22:09:51.476037 fin_maestro_kin-0.2.6/fin_maestro_kin/modules/data_toolkit/nse/nse_operations.py
+-rw-r--r--   0        0        0        0 2024-04-13 06:37:31.671927 fin_maestro_kin-0.2.6/fin_maestro_kin/modules/data_toolkit/screener/__init__.py
+-rw-r--r--   0        0        0     9242 2024-04-26 23:38:54.845857 fin_maestro_kin-0.2.6/fin_maestro_kin/modules/data_toolkit/screener/screener_equities.py
+-rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.6/fin_maestro_kin/modules/sentiment_analysis/__init__.py
+-rw-r--r--   0        0        0     3840 2024-04-27 07:12:00.425708 fin_maestro_kin-0.2.6/fin_maestro_kin/modules/sentiment_analysis/sentiment_analysis.py
+-rw-r--r--   0        0        0        0 2024-02-10 15:38:47.413185 fin_maestro_kin-0.2.6/fin_maestro_kin/modules/trend_detector/__init__.py
+-rw-r--r--   0        0        0     2263 2024-04-27 07:21:06.631998 fin_maestro_kin-0.2.6/fin_maestro_kin/modules/trend_detector/trend_detector.py
+-rw-r--r--   0        0        0     1090 2024-02-10 16:19:33.663653 fin_maestro_kin-0.2.6/LICENSE
+-rw-r--r--   0        0        0      614 2024-04-27 07:27:19.793888 fin_maestro_kin-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     5508 2024-04-26 18:16:29.525503 fin_maestro_kin-0.2.6/README.md
+-rw-r--r--   0        0        0     6369 1970-01-01 00:00:00.000000 fin_maestro_kin-0.2.6/PKG-INFO
```

### Comparing `fin_maestro_kin-0.2.5/fin_maestro_kin/constants.py` & `fin_maestro_kin-0.2.6/fin_maestro_kin/constants.py`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.5/fin_maestro_kin/modules/trend_detector/trend_detector.py` & `fin_maestro_kin-0.2.6/fin_maestro_kin/modules/trend_detector/trend_detector.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,55 +4,57 @@
 import matplotlib.pyplot as plt
 import matplotlib
 import io
 import datetime as dt
 import warnings
 
 warnings.filterwarnings("ignore")
-initial, end = dt.date.today() - dt.timedelta(days=374), dt.date.today()
 
-router = APIRouter(tags=["Trend Detector"])
 
+class TrendDetector:
+    def __init__(self):
+        self.router = APIRouter(tags=["Trend Detector"])
+        matplotlib.use('Agg')
+        plt.style.use('dark_background')
+
+    def register_routes(self, app):
+        self.router.add_api_route("/generate_plot", self.generate_plot, methods=["GET"])
+        app.include_router(self.router)
+
+    @staticmethod
+    def signals_generator(ticker, num_of_signals):
+        yf.pdr_override()
+        initial, end = dt.date.today() - dt.timedelta(days=374), dt.date.today()
+        df = yf.download(ticker, initial, end) 
+        closes = sorted(df.Close.tolist())
+        low, high = closes[num_of_signals], closes[-num_of_signals]
+
+        df['Signal'] = 0
+
+        df.loc[df['Adj Close'] > high, 'Signal'] = -1
+        df.loc[df['Adj Close'] < low, 'Signal'] = 1
+
+        long = df.loc[df['Signal'] == 1]
+        short = df.loc[df['Signal'] == -1]
+
+        fig = plt.figure()
+        fig.set_figwidth(12)
+        plt.plot(df.index, df['Adj Close'], color='white', label='Close Price')
+        plt.plot(long.index, df.loc[long.index]['Adj Close'], '^', markersize=10, color='g', label='Long/Buy')
+        plt.plot(short.index, df.loc[short.index]['Adj Close'], 'v', markersize=10, color='r', label='Short/Sell')
+        plt.ylabel('Closing Price')
+        plt.xlabel('Date')
+        plt.title(ticker)
+        plt.legend(loc='best')
+
+        return fig
+
+    async def generate_plot(self, ticker: str = Query(..., title="Ticker", description="Stock ticker symbol"),
+                            num_of_signals: int = Query(10, title="Num of Signals",
+                                                        description="Number of buy/sell signals to be plotted")):
+        fig = self.signals_generator(ticker, num_of_signals)
+
+        image_stream = io.BytesIO()
+        fig.savefig(image_stream, format="png")
+        image_stream.seek(0)
 
-#Example usage - http://127.0.0.1:8000/generate_plot?ticker=BSE.NS
-def signals_generator(ticker, num_of_signals):
-    matplotlib.use('Agg')
-    yf.pdr_override()
-    plt.style.use('dark_background')  # dark theme for plot
-
-    df = yf.download(ticker, initial, end)  # dataframe from yfinance for a specific ticker
-
-    closes = sorted(df.Close.tolist())
-    low, high = closes[num_of_signals], closes[-num_of_signals]
-
-    df['Signal'] = 0
-
-    df.loc[df['Adj Close'] > high, 'Signal'] = -1
-    df.loc[df['Adj Close'] < low, 'Signal'] = 1
-
-    long = df.loc[df['Signal'] == 1]
-    short = df.loc[df['Signal'] == -1]
-
-    fig = plt.figure()
-    fig.set_figwidth(12)
-    plt.plot(df.index, df['Adj Close'], color='white', label='Close Price')
-    plt.plot(long.index, df.loc[long.index]['Adj Close'], '^', markersize=10, color='g', label='Long/Buy')
-    plt.plot(short.index, df.loc[short.index]['Adj Close'], 'v', markersize=10, color='r', label='Short/Sell')
-    plt.ylabel('Closing Price')
-    plt.xlabel('Date')
-    plt.title(ticker)
-    plt.legend(loc='best')
-
-    return fig
-
-
-@router.get("/generate_plot",tags=["Trend Detector"])
-async def generate_plot(ticker: str = Query(..., title="Ticker", description="Stock ticker symbol"),
-                        num_of_signals: int = Query(10, title="Num of Signals", description="Number of buy/sell signals to be plotted")):
-    fig = signals_generator(ticker, num_of_signals)
-
-    # Convert the matplotlib figure to a PNG image
-    image_stream = io.BytesIO()
-    fig.savefig(image_stream, format="png")
-    image_stream.seek(0)
-
-    return StreamingResponse(content=image_stream, media_type="image/png")
+        return StreamingResponse(content=image_stream, media_type="image/png")
```

### Comparing `fin_maestro_kin-0.2.5/LICENSE` & `fin_maestro_kin-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.5/README.md` & `fin_maestro_kin-0.2.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 <p align="center">
-<img width="394" alt="image" src="https://github.com/devfinwiz/Fin-Maestro-Kin/assets/78873223/9a6e71e2-2867-49c5-b930-980a871bcb34">
+  <a href="https://fin-maestro-kin.apidog.io/"><img src="https://github.com/devfinwiz/Fin-Maestro-Kin/assets/78873223/eb0f030e-5c6c-4457-9713-97d0487ae59c" alt="Fin Maestro Kin"></a>
 </p>
-<div align="center">
+<p align="center" style="font-size: 20px;">
+    <em>Seamless Finance: Docker-Deployed APIs for Smart Investments.</em>
 
-</div>
 <h1 align="center">Fin-Maestro-Kin </h1>
 
-
 <p align="center">
-  <a href="https://www.codefactor.io/repository/github/devfinwiz/fin-maestro-kin">
-    <img src="https://img.shields.io/badge/CodeFactor-A-blue&?style=for-the-badge&color=blue">
+  <a href="https://github.com/devfinwiz/fin-maestro-kin/releases/latest">
+    <img src="https://img.shields.io/github/v/release/devfinwiz/fin-maestro-kin?style=for-the-badge">
   </a>
   <a href="">
-    <img src="https://img.shields.io/badge/Python-3.9.1-blue&?style=for-the-badge&color=blue">
+    <img src="https://img.shields.io/badge/Python-3.9.1-blue&?style=for-the-badge&color=brown">
   </a>
   <a href="https://github.com/devfinwiz/Fin-Maestro-Kin/blob/master/LICENSE">
     <img src="https://img.shields.io/github/license/devfinwiz/Fin-Maestro-Kin?color=purple&style=for-the-badge">
   </a>
-  <a href="https://github.com/devfinwiz/Fin-Maestro-Kin/commits/master">
-    <img src="https://img.shields.io/github/last-commit/devfinwiz/Fin-Maestro-Kin?color=yellow&style=for-the-badge">
-  </a>
   <a href="https://github.com/devfinwiz/Fin-Maestro-Kin/graphs/contributors">
     <img src="https://img.shields.io/github/contributors/devfinwiz/Fin-Maestro-Kin?color=indigo&style=for-the-badge">
   </a>
-  <a href="https://github.com/devfinwiz/Fin-Maestro-Kin/issues">
-    <img src="https://img.shields.io/github/issues-raw/devfinwiz/Fin-Maestro-Kin?color=indigo&style=for-the-badge">
+  <a href="https://www.codefactor.io/repository/github/devfinwiz/fin-maestro-kin">
+    <img src="https://www.codefactor.io/repository/github/devfinwiz/fin-maestro-kin/badge?style=for-the-badge&">
+  </a>
+  <a href="https://hub.docker.com/repository/docker/devfinwiz24/fin-maestro-kin/tags">
+    <img src="https://img.shields.io/docker/pulls/devfinwiz24/fin-maestro-kin?style=for-the-badge&logo=docker">
   </a>
 </p><br>
 
 
 | **Docker** | **Discussion** | **Bugs/Issues** | **Contribute** |
 | :---: | :---: | :---: | :---: |
 | [![Use](https://github.com/devfinwiz/Fin-Maestro-Kin/assets/78873223/5866ef40-3168-415b-b222-febb280f0248)](https://hub.docker.com/r/devfinwiz24/fin-maestro-kin) | [![meeting](https://user-images.githubusercontent.com/6128978/149935812-31266023-cc5b-4c98-a416-1d4cf8800c0c.png)](https://github.com/devfinwiz/Fin-Maestro-Kin/discussions) | [![warning](https://user-images.githubusercontent.com/6128978/149936142-04d7cf1c-5bc5-45c1-a8e4-015454a2de48.png)](https://github.com/devfinwiz/Fin-Maestro-Kin/issues/new/choose) | [![meeting](https://user-images.githubusercontent.com/6128978/149935812-31266023-cc5b-4c98-a416-1d4cf8800c0c.png)](https://github.com/devfinwiz/Fin-Maestro-Kin/fork) |
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
-                                    [image]
+                               _[_F_i_n_ _M_a_e_s_t_r_o_ _K_i_n_]
+         SSeeaammlleessss FFiinnaannccee:: DDoocckkeerr--DDeeppllooyyeedd AAPPIIss ffoorr SSmmaarrtt IInnvveessttmmeennttss..
                          ************ FFiinn--MMaaeessttrroo--KKiinn ************
-        _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_d_e_F_a_c_t_o_r_-_A_-_b_l_u_e_&_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
- _b_a_d_g_e_&_c_o_l_o_r_=_b_l_u_e_][https://img.shields.io/badge/Python-3.9.1-blue&?style=for-
-  the-badge&color=blue]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_d_e_v_f_i_n_w_i_z_/_F_i_n_-
- _M_a_e_s_t_r_o_-_K_i_n_?_c_o_l_o_r_=_p_u_r_p_l_e_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/
-_l_a_s_t_-_c_o_m_m_i_t_/_d_e_v_f_i_n_w_i_z_/_F_i_n_-_M_a_e_s_t_r_o_-_K_i_n_?_c_o_l_o_r_=_y_e_l_l_o_w_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/
-          _/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_c_o_n_t_r_i_b_u_t_o_r_s_/_d_e_v_f_i_n_w_i_z_/_F_i_n_-_M_a_e_s_t_r_o_-
-_K_i_n_?_c_o_l_o_r_=_i_n_d_i_g_o_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_i_s_s_u_e_s_-_r_a_w_/
-          _d_e_v_f_i_n_w_i_z_/_F_i_n_-_M_a_e_s_t_r_o_-_K_i_n_?_c_o_l_o_r_=_i_n_d_i_g_o_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]
+ _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_d_e_v_f_i_n_w_i_z_/_f_i_n_-_m_a_e_s_t_r_o_-_k_i_n_?_s_t_y_l_e_=_f_o_r_-
+   _t_h_e_-_b_a_d_g_e_][https://img.shields.io/badge/Python-3.9.1-blue&?style=for-the-
+badge&color=brown]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_d_e_v_f_i_n_w_i_z_/_F_i_n_-_M_a_e_s_t_r_o_-
+     _K_i_n_?_c_o_l_o_r_=_p_u_r_p_l_e_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/
+_c_o_n_t_r_i_b_u_t_o_r_s_/_d_e_v_f_i_n_w_i_z_/_F_i_n_-_M_a_e_s_t_r_o_-_K_i_n_?_c_o_l_o_r_=_i_n_d_i_g_o_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:
+       _/_/_w_w_w_._c_o_d_e_f_a_c_t_o_r_._i_o_/_r_e_p_o_s_i_t_o_r_y_/_g_i_t_h_u_b_/_d_e_v_f_i_n_w_i_z_/_f_i_n_-_m_a_e_s_t_r_o_-_k_i_n_/
+ _b_a_d_g_e_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_d_o_c_k_e_r_/_p_u_l_l_s_/_d_e_v_f_i_n_w_i_z_2_4_/
+               _f_i_n_-_m_a_e_s_t_r_o_-_k_i_n_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_=_d_o_c_k_e_r_]
 
 | **Docker** | **Discussion** | **Bugs/Issues** | **Contribute** | | :---: | :-
 --: | :---: | :---: | | [![Use](https://github.com/devfinwiz/Fin-Maestro-Kin/
 assets/78873223/5866ef40-3168-415b-b222-febb280f0248)](https://hub.docker.com/
 r/devfinwiz24/fin-maestro-kin) | [![meeting](https://user-
 images.githubusercontent.com/6128978/149935812-31266023-cc5b-4c98-a416-
 1d4cf8800c0c.png)](https://github.com/devfinwiz/Fin-Maestro-Kin/discussions) |
```

### Comparing `fin_maestro_kin-0.2.5/PKG-INFO` & `fin_maestro_kin-0.2.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: fin-maestro-kin
-Version: 0.2.5
-Summary: Where Data Meets FastAPI Brilliance with Fin-Maestro-Kin – Your All-in-One Finance API.
+Version: 0.2.6
+Summary: Seamless Finance: Docker Deployed APIs for Smart Investments.
 License: MIT
 Author: DEV_FINWIZ
 Author-email: devjuneja43@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -20,40 +20,39 @@
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: uvicorn (>=0.25.0,<0.26.0)
 Requires-Dist: yfinance (>=0.2.35,<0.3.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
-<img width="394" alt="image" src="https://github.com/devfinwiz/Fin-Maestro-Kin/assets/78873223/9a6e71e2-2867-49c5-b930-980a871bcb34">
+  <a href="https://fin-maestro-kin.apidog.io/"><img src="https://github.com/devfinwiz/Fin-Maestro-Kin/assets/78873223/eb0f030e-5c6c-4457-9713-97d0487ae59c" alt="Fin Maestro Kin"></a>
 </p>
-<div align="center">
+<p align="center" style="font-size: 20px;">
+    <em>Seamless Finance: Docker-Deployed APIs for Smart Investments.</em>
 
-</div>
 <h1 align="center">Fin-Maestro-Kin </h1>
 
-
 <p align="center">
-  <a href="https://www.codefactor.io/repository/github/devfinwiz/fin-maestro-kin">
-    <img src="https://img.shields.io/badge/CodeFactor-A-blue&?style=for-the-badge&color=blue">
+  <a href="https://github.com/devfinwiz/fin-maestro-kin/releases/latest">
+    <img src="https://img.shields.io/github/v/release/devfinwiz/fin-maestro-kin?style=for-the-badge">
   </a>
   <a href="">
-    <img src="https://img.shields.io/badge/Python-3.9.1-blue&?style=for-the-badge&color=blue">
+    <img src="https://img.shields.io/badge/Python-3.9.1-blue&?style=for-the-badge&color=brown">
   </a>
   <a href="https://github.com/devfinwiz/Fin-Maestro-Kin/blob/master/LICENSE">
     <img src="https://img.shields.io/github/license/devfinwiz/Fin-Maestro-Kin?color=purple&style=for-the-badge">
   </a>
-  <a href="https://github.com/devfinwiz/Fin-Maestro-Kin/commits/master">
-    <img src="https://img.shields.io/github/last-commit/devfinwiz/Fin-Maestro-Kin?color=yellow&style=for-the-badge">
-  </a>
   <a href="https://github.com/devfinwiz/Fin-Maestro-Kin/graphs/contributors">
     <img src="https://img.shields.io/github/contributors/devfinwiz/Fin-Maestro-Kin?color=indigo&style=for-the-badge">
   </a>
-  <a href="https://github.com/devfinwiz/Fin-Maestro-Kin/issues">
-    <img src="https://img.shields.io/github/issues-raw/devfinwiz/Fin-Maestro-Kin?color=indigo&style=for-the-badge">
+  <a href="https://www.codefactor.io/repository/github/devfinwiz/fin-maestro-kin">
+    <img src="https://www.codefactor.io/repository/github/devfinwiz/fin-maestro-kin/badge?style=for-the-badge&">
+  </a>
+  <a href="https://hub.docker.com/repository/docker/devfinwiz24/fin-maestro-kin/tags">
+    <img src="https://img.shields.io/docker/pulls/devfinwiz24/fin-maestro-kin?style=for-the-badge&logo=docker">
   </a>
 </p><br>
 
 
 | **Docker** | **Discussion** | **Bugs/Issues** | **Contribute** |
 | :---: | :---: | :---: | :---: |
 | [![Use](https://github.com/devfinwiz/Fin-Maestro-Kin/assets/78873223/5866ef40-3168-415b-b222-febb280f0248)](https://hub.docker.com/r/devfinwiz24/fin-maestro-kin) | [![meeting](https://user-images.githubusercontent.com/6128978/149935812-31266023-cc5b-4c98-a416-1d4cf8800c0c.png)](https://github.com/devfinwiz/Fin-Maestro-Kin/discussions) | [![warning](https://user-images.githubusercontent.com/6128978/149936142-04d7cf1c-5bc5-45c1-a8e4-015454a2de48.png)](https://github.com/devfinwiz/Fin-Maestro-Kin/issues/new/choose) | [![meeting](https://user-images.githubusercontent.com/6128978/149935812-31266023-cc5b-4c98-a416-1d4cf8800c0c.png)](https://github.com/devfinwiz/Fin-Maestro-Kin/fork) |
```

#### html2text {}

```diff
@@ -1,30 +1,31 @@
-Metadata-Version: 2.1 Name: fin-maestro-kin Version: 0.2.5 Summary: Where Data
-Meets FastAPI Brilliance with Fin-Maestro-Kin â Your All-in-One Finance API.
-License: MIT Author: DEV_FINWIZ Author-email: devjuneja43@gmail.com Requires-
-Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.12 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
-Requires-Dist: fastapi (>=0.109.0,<0.110.0) Requires-Dist: matplotlib
-(>=3.8.2,<4.0.0) Requires-Dist: numpy (>=1.26.3,<2.0.0) Requires-Dist: pandas
-(>=2.1.4,<3.0.0) Requires-Dist: pydantic (>=2.5.3,<3.0.0) Requires-Dist:
-requests (>=2.31.0,<3.0.0) Requires-Dist: uvicorn (>=0.25.0,<0.26.0) Requires-
-Dist: yfinance (>=0.2.35,<0.3.0) Description-Content-Type: text/markdown
-                                    [image]
+Metadata-Version: 2.1 Name: fin-maestro-kin Version: 0.2.6 Summary: Seamless
+Finance: Docker Deployed APIs for Smart Investments. License: MIT Author:
+DEV_FINWIZ Author-email: devjuneja43@gmail.com Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0) Requires-Dist: fastapi
+(>=0.109.0,<0.110.0) Requires-Dist: matplotlib (>=3.8.2,<4.0.0) Requires-Dist:
+numpy (>=1.26.3,<2.0.0) Requires-Dist: pandas (>=2.1.4,<3.0.0) Requires-Dist:
+pydantic (>=2.5.3,<3.0.0) Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-
+Dist: uvicorn (>=0.25.0,<0.26.0) Requires-Dist: yfinance (>=0.2.35,<0.3.0)
+Description-Content-Type: text/markdown
+                               _[_F_i_n_ _M_a_e_s_t_r_o_ _K_i_n_]
+         SSeeaammlleessss FFiinnaannccee:: DDoocckkeerr--DDeeppllooyyeedd AAPPIIss ffoorr SSmmaarrtt IInnvveessttmmeennttss..
                          ************ FFiinn--MMaaeessttrroo--KKiinn ************
-        _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_d_e_F_a_c_t_o_r_-_A_-_b_l_u_e_&_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
- _b_a_d_g_e_&_c_o_l_o_r_=_b_l_u_e_][https://img.shields.io/badge/Python-3.9.1-blue&?style=for-
-  the-badge&color=blue]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_d_e_v_f_i_n_w_i_z_/_F_i_n_-
- _M_a_e_s_t_r_o_-_K_i_n_?_c_o_l_o_r_=_p_u_r_p_l_e_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/
-_l_a_s_t_-_c_o_m_m_i_t_/_d_e_v_f_i_n_w_i_z_/_F_i_n_-_M_a_e_s_t_r_o_-_K_i_n_?_c_o_l_o_r_=_y_e_l_l_o_w_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/
-          _/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_c_o_n_t_r_i_b_u_t_o_r_s_/_d_e_v_f_i_n_w_i_z_/_F_i_n_-_M_a_e_s_t_r_o_-
-_K_i_n_?_c_o_l_o_r_=_i_n_d_i_g_o_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_i_s_s_u_e_s_-_r_a_w_/
-          _d_e_v_f_i_n_w_i_z_/_F_i_n_-_M_a_e_s_t_r_o_-_K_i_n_?_c_o_l_o_r_=_i_n_d_i_g_o_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]
+ _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_d_e_v_f_i_n_w_i_z_/_f_i_n_-_m_a_e_s_t_r_o_-_k_i_n_?_s_t_y_l_e_=_f_o_r_-
+   _t_h_e_-_b_a_d_g_e_][https://img.shields.io/badge/Python-3.9.1-blue&?style=for-the-
+badge&color=brown]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_d_e_v_f_i_n_w_i_z_/_F_i_n_-_M_a_e_s_t_r_o_-
+     _K_i_n_?_c_o_l_o_r_=_p_u_r_p_l_e_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/
+_c_o_n_t_r_i_b_u_t_o_r_s_/_d_e_v_f_i_n_w_i_z_/_F_i_n_-_M_a_e_s_t_r_o_-_K_i_n_?_c_o_l_o_r_=_i_n_d_i_g_o_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:
+       _/_/_w_w_w_._c_o_d_e_f_a_c_t_o_r_._i_o_/_r_e_p_o_s_i_t_o_r_y_/_g_i_t_h_u_b_/_d_e_v_f_i_n_w_i_z_/_f_i_n_-_m_a_e_s_t_r_o_-_k_i_n_/
+ _b_a_d_g_e_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_d_o_c_k_e_r_/_p_u_l_l_s_/_d_e_v_f_i_n_w_i_z_2_4_/
+               _f_i_n_-_m_a_e_s_t_r_o_-_k_i_n_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_=_d_o_c_k_e_r_]
 
 | **Docker** | **Discussion** | **Bugs/Issues** | **Contribute** | | :---: | :-
 --: | :---: | :---: | | [![Use](https://github.com/devfinwiz/Fin-Maestro-Kin/
 assets/78873223/5866ef40-3168-415b-b222-febb280f0248)](https://hub.docker.com/
 r/devfinwiz24/fin-maestro-kin) | [![meeting](https://user-
 images.githubusercontent.com/6128978/149935812-31266023-cc5b-4c98-a416-
 1d4cf8800c0c.png)](https://github.com/devfinwiz/Fin-Maestro-Kin/discussions) |
```

