# Comparing `tmp/dwdhandler-0.2.0.tar.gz` & `tmp/dwdhandler-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwdhandler-0.2.0.tar", last modified: Sat Mar 23 11:59:14 2024, max compression
+gzip compressed data, was "dwdhandler-0.2.1.tar", last modified: Sat Apr 27 17:13:52 2024, max compression
```

## Comparing `dwdhandler-0.2.0.tar` & `dwdhandler-0.2.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-03-23 11:59:14.625586 dwdhandler-0.2.0/
--rw-rw-r--   0 tobias    (1000) tobias    (1000)    35148 2024-03-21 19:39:06.000000 dwdhandler-0.2.0/LICENSE
--rw-r--r--   0 tobias    (1000) tobias    (1000)     1196 2024-03-23 11:59:14.625586 dwdhandler-0.2.0/PKG-INFO
--rw-rw-r--   0 tobias    (1000) tobias    (1000)      478 2024-03-23 11:22:42.000000 dwdhandler-0.2.0/README.md
--rw-rw-r--   0 tobias    (1000) tobias    (1000)      103 2021-06-08 15:54:47.000000 dwdhandler-0.2.0/pyproject.toml
--rw-rw-r--   0 tobias    (1000) tobias    (1000)      762 2024-03-23 11:59:14.625586 dwdhandler-0.2.0/setup.cfg
-drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-03-23 11:59:14.621586 dwdhandler-0.2.0/src/
-drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-03-23 11:59:14.621586 dwdhandler-0.2.0/src/dwdhandler/
--rw-rw-r--   0 tobias    (1000) tobias    (1000)      167 2023-03-19 15:20:19.000000 dwdhandler-0.2.0/src/dwdhandler/__init__.py
-drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-03-23 11:59:14.621586 dwdhandler-0.2.0/src/dwdhandler/calculation/
--rw-rw-r--   0 tobias    (1000) tobias    (1000)        0 2022-02-21 20:37:50.000000 dwdhandler-0.2.0/src/dwdhandler/calculation/__init__.py
--rw-rw-r--   0 tobias    (1000) tobias    (1000)    22878 2023-10-23 18:15:18.000000 dwdhandler-0.2.0/src/dwdhandler/calculation/calc_stats.py
--rw-rw-r--   0 tobias    (1000) tobias    (1000)     5010 2023-08-17 16:59:09.000000 dwdhandler-0.2.0/src/dwdhandler/calculation/return_period.py
-drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-03-23 11:59:14.621586 dwdhandler-0.2.0/src/dwdhandler/constants/
--rw-rw-r--   0 tobias    (1000) tobias    (1000)        0 2021-06-08 15:54:47.000000 dwdhandler-0.2.0/src/dwdhandler/constants/__init__.py
--rw-rw-r--   0 tobias    (1000) tobias    (1000)     1719 2023-07-01 10:06:00.000000 dwdhandler-0.2.0/src/dwdhandler/constants/constpar.py
--rw-rw-r--   0 tobias    (1000) tobias    (1000)     6062 2023-07-02 12:20:04.000000 dwdhandler-0.2.0/src/dwdhandler/constants/filedata.py
--rw-rw-r--   0 tobias    (1000) tobias    (1000)      542 2022-01-22 16:29:40.000000 dwdhandler-0.2.0/src/dwdhandler/constants/serverdata.py
--rw-rw-r--   0 tobias    (1000) tobias    (1000)    44023 2024-03-23 11:08:12.000000 dwdhandler-0.2.0/src/dwdhandler/dow_handler.py
-drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-03-23 11:59:14.621586 dwdhandler-0.2.0/src/dwdhandler/helper/
--rw-rw-r--   0 tobias    (1000) tobias    (1000)        0 2021-06-08 15:54:47.000000 dwdhandler-0.2.0/src/dwdhandler/helper/__init__.py
--rw-rw-r--   0 tobias    (1000) tobias    (1000)     1447 2023-06-05 18:14:27.000000 dwdhandler-0.2.0/src/dwdhandler/helper/ftp.py
--rw-rw-r--   0 tobias    (1000) tobias    (1000)    21509 2023-11-05 15:19:44.000000 dwdhandler-0.2.0/src/dwdhandler/helper/hfunctions.py
-drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-03-23 11:59:14.621586 dwdhandler-0.2.0/src/dwdhandler/plotting/
--rw-rw-r--   0 tobias    (1000) tobias    (1000)        0 2021-12-04 10:40:07.000000 dwdhandler-0.2.0/src/dwdhandler/plotting/__init__.py
--rw-rw-r--   0 tobias    (1000) tobias    (1000)   104972 2024-02-16 22:09:09.000000 dwdhandler-0.2.0/src/dwdhandler/plotting/plotconstr.py
-drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-03-23 11:59:14.625586 dwdhandler-0.2.0/src/dwdhandler.egg-info/
--rw-r--r--   0 tobias    (1000) tobias    (1000)     1196 2024-03-23 11:59:14.000000 dwdhandler-0.2.0/src/dwdhandler.egg-info/PKG-INFO
--rw-rw-r--   0 tobias    (1000) tobias    (1000)      735 2024-03-23 11:59:14.000000 dwdhandler-0.2.0/src/dwdhandler.egg-info/SOURCES.txt
--rw-rw-r--   0 tobias    (1000) tobias    (1000)        1 2024-03-23 11:59:14.000000 dwdhandler-0.2.0/src/dwdhandler.egg-info/dependency_links.txt
--rw-rw-r--   0 tobias    (1000) tobias    (1000)       62 2024-03-23 11:59:14.000000 dwdhandler-0.2.0/src/dwdhandler.egg-info/requires.txt
--rw-rw-r--   0 tobias    (1000) tobias    (1000)       11 2024-03-23 11:59:14.000000 dwdhandler-0.2.0/src/dwdhandler.egg-info/top_level.txt
+drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-04-27 17:13:52.155254 dwdhandler-0.2.1/
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)    35148 2024-03-21 19:39:06.000000 dwdhandler-0.2.1/LICENSE
+-rw-r--r--   0 tobias    (1000) tobias    (1000)    41886 2024-04-27 17:13:52.155254 dwdhandler-0.2.1/PKG-INFO
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)      478 2024-03-23 11:22:42.000000 dwdhandler-0.2.1/README.md
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)      968 2024-04-27 17:12:45.000000 dwdhandler-0.2.1/pyproject.toml
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)      751 2024-04-27 17:13:52.155254 dwdhandler-0.2.1/setup.cfg
+drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-04-27 17:13:52.151254 dwdhandler-0.2.1/src/
+drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-04-27 17:13:52.151254 dwdhandler-0.2.1/src/dwdhandler/
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)      196 2024-04-27 12:45:25.000000 dwdhandler-0.2.1/src/dwdhandler/__init__.py
+drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-04-27 17:13:52.151254 dwdhandler-0.2.1/src/dwdhandler/calculation/
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)        0 2022-02-21 20:37:50.000000 dwdhandler-0.2.1/src/dwdhandler/calculation/__init__.py
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)    22878 2023-10-23 18:15:18.000000 dwdhandler-0.2.1/src/dwdhandler/calculation/calc_stats.py
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)     1550 2024-04-22 11:36:15.000000 dwdhandler-0.2.1/src/dwdhandler/calculation/geo.py
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)     5010 2023-08-17 16:59:09.000000 dwdhandler-0.2.1/src/dwdhandler/calculation/return_period.py
+drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-04-27 17:13:52.155254 dwdhandler-0.2.1/src/dwdhandler/constants/
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)        0 2021-06-08 15:54:47.000000 dwdhandler-0.2.1/src/dwdhandler/constants/__init__.py
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)     1742 2024-03-24 17:56:23.000000 dwdhandler-0.2.1/src/dwdhandler/constants/constpar.py
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)     6062 2023-07-02 12:20:04.000000 dwdhandler-0.2.1/src/dwdhandler/constants/filedata.py
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)      542 2022-01-22 16:29:40.000000 dwdhandler-0.2.1/src/dwdhandler/constants/serverdata.py
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)    44023 2024-03-23 11:08:12.000000 dwdhandler-0.2.1/src/dwdhandler/dow_handler.py
+drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-04-27 17:13:52.155254 dwdhandler-0.2.1/src/dwdhandler/helper/
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)        0 2021-06-08 15:54:47.000000 dwdhandler-0.2.1/src/dwdhandler/helper/__init__.py
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)     1447 2023-06-05 18:14:27.000000 dwdhandler-0.2.1/src/dwdhandler/helper/ftp.py
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)    20327 2024-04-27 12:41:53.000000 dwdhandler-0.2.1/src/dwdhandler/helper/hfunctions.py
+drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-04-27 17:13:52.155254 dwdhandler-0.2.1/src/dwdhandler/plotting/
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)        0 2021-12-04 10:40:07.000000 dwdhandler-0.2.1/src/dwdhandler/plotting/__init__.py
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)   105384 2024-03-30 13:14:30.000000 dwdhandler-0.2.1/src/dwdhandler/plotting/plotconstr.py
+drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-04-27 17:13:52.155254 dwdhandler-0.2.1/src/dwdhandler.egg-info/
+-rw-r--r--   0 tobias    (1000) tobias    (1000)    41886 2024-04-27 17:13:52.000000 dwdhandler-0.2.1/src/dwdhandler.egg-info/PKG-INFO
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)      769 2024-04-27 17:13:52.000000 dwdhandler-0.2.1/src/dwdhandler.egg-info/SOURCES.txt
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)        1 2024-04-27 17:13:52.000000 dwdhandler-0.2.1/src/dwdhandler.egg-info/dependency_links.txt
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)       83 2024-04-27 17:13:52.000000 dwdhandler-0.2.1/src/dwdhandler.egg-info/requires.txt
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)       11 2024-04-27 17:13:52.000000 dwdhandler-0.2.1/src/dwdhandler.egg-info/top_level.txt
```

### Comparing `dwdhandler-0.2.0/LICENSE` & `dwdhandler-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dwdhandler-0.2.0/setup.cfg` & `dwdhandler-0.2.1/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dwdhandler
-version = 0.2.0
+version = 0.2.1
 author = Tobias Schad
 author_email = tobias.schad@googlemail.com
 description = Package to handle data from German Weather Service and some simple plotting routines
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GPL version 3
 url = https://github.com/MrTscha/dwdhandler
@@ -18,15 +18,14 @@
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	numpy
 	pandas
-	pysqlite3
 	seaborn
 	matplotlib
 	folium
 	plotly
 	scipy
 
 [options.packages.find]
```

### Comparing `dwdhandler-0.2.0/src/dwdhandler/calculation/calc_stats.py` & `dwdhandler-0.2.1/src/dwdhandler/calculation/calc_stats.py`

 * *Files identical despite different names*

### Comparing `dwdhandler-0.2.0/src/dwdhandler/calculation/return_period.py` & `dwdhandler-0.2.1/src/dwdhandler/calculation/return_period.py`

 * *Files identical despite different names*

### Comparing `dwdhandler-0.2.0/src/dwdhandler/constants/constpar.py` & `dwdhandler-0.2.1/src/dwdhandler/constants/constpar.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 FILLVALUE = -999
 ASCIIRASCRS = 'epsg:31467'
 STATIONNAMEID = 'STATIONS_ID'
 DATENAMESTAT = 'MESS_DATUM' # Name of time variable of station data
 DATENAMESTATEND = 'MESS_DATUM_ENDE'
 STATIONNAMEQUAL = 'QN'
 
+RADIUSEARTH = 6371000
+
 RASTERFACTDICT = {
     'air_temperature_max':0.1,
     'air_temperature_mean':0.1,
     'air_temperature_min':0.1,
     'evapo_p':0.1,
     'evapo_r':0.1
 }
```

### Comparing `dwdhandler-0.2.0/src/dwdhandler/constants/filedata.py` & `dwdhandler-0.2.1/src/dwdhandler/constants/filedata.py`

 * *Files identical despite different names*

### Comparing `dwdhandler-0.2.0/src/dwdhandler/constants/serverdata.py` & `dwdhandler-0.2.1/src/dwdhandler/constants/serverdata.py`

 * *Files identical despite different names*

### Comparing `dwdhandler-0.2.0/src/dwdhandler/dow_handler.py` & `dwdhandler-0.2.1/src/dwdhandler/dow_handler.py`

 * *Files identical despite different names*

### Comparing `dwdhandler-0.2.0/src/dwdhandler/helper/ftp.py` & `dwdhandler-0.2.1/src/dwdhandler/helper/ftp.py`

 * *Files identical despite different names*

### Comparing `dwdhandler-0.2.0/src/dwdhandler/helper/hfunctions.py` & `dwdhandler-0.2.1/src/dwdhandler/helper/hfunctions.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,45 +27,45 @@
     if not exists(dir_in):
         makedirs(dir_in)
 
 def read_station_list(dir_in,file_in,debug=False):
     """ Reads DWD station list metadata """
 
     if(debug):
-        print("Open file {} and read station list".format(dir_in+file_in))                                
+        print("Open file {} and read station list".format(dir_in+file_in))
 
-    check_file_encoding(dir_in,file_in)                                                        
+    check_file_encoding(dir_in,file_in)
 
-    input_file = open(dir_in+file_in,"r")                                                           
+    input_file = open(dir_in+file_in,"r")
 
-    lines = input_file.readlines()                                                                                
+    lines = input_file.readlines()
 
     i = 0
 
     station_list = {}
 
-    for line in lines:                                                                                            
+    for line in lines:
         if(i == 0):
-            header = line.split()                                                                                 
-        elif(i > 1): # skip second line...                                                                        
+            header = line.split()
+        elif(i > 1): # skip second line...
             station_key = line[0:5]
-            year, month, day = extract_yyyymmdd(line[6:14])                                                       
-            b_date      = datetime.datetime(int(year), int(month), int(day))                                      
-            year, month, day = extract_yyyymmdd(line[15:23])
-            e_date      = datetime.datetime(int(year), int(month), int(day))                                      
-            height      = line[34:38].replace(" ","")
-            height      = np.float(height)                                                                        
-            lat         = float(line[43:50])                                                                      
-            lon         = float(line[53:60])                                                                      
-            name        = line[61:141].rstrip()                                                                   
-            state       = line[142:180].rstrip()                                                                  
-            station_list[station_key] = {'von':b_date,'bis':e_date,                                               
-                                     'hoehe':height,'lat':lat,'lon':lon,                                          
-                                     'name':name,'bundesland':state}                                              
-        i += 1                                                                                                    
+            year, month, day = extract_yyyymmdd(line[21:30])
+            b_date      = datetime.datetime(int(year), int(month), int(day))
+            year, month, day = extract_yyyymmdd(line[30:38])
+            e_date      = datetime.datetime(int(year), int(month), int(day))
+            height      = line[49:53].replace(" ","")
+            height      = np.float(height)
+            lat         = float(line[58:65])
+            lon         = float(line[68:75])
+            name        = line[76:156].rstrip()
+            state       = line[157:204].rstrip()
+            station_list[station_key] = {'von':b_date,'bis':e_date,
+                                     'hoehe':height,'lat':lat,'lon':lon,
+                                     'name':name,'bundesland':state}
+        i += 1
 
     if(debug):
         print("{} stations read".format(i-2))                                                                     
         #print(station_list)                                                                                      
 
     return pd.DataFrame(station_list).T
```

### Comparing `dwdhandler-0.2.0/src/dwdhandler/plotting/plotconstr.py` & `dwdhandler-0.2.1/src/dwdhandler/plotting/plotconstr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1226,24 +1226,29 @@
         #tmp_arr[4:] = moving_average(temp,5)
         tmp_arr[move_avg-1:] = moving_average(temp,move_avg)
         tmp_arr = np.ma.masked_where(tmp_arr == -999.,tmp_arr)
         ax.plot_date(date_arr,tmp_arr,'-',color='tomato',label=f'Gleitendes Mittel ({move_avg}j)')
         handles, labels = ax.get_legend_handles_labels()
         ax.legend(handles, labels,loc='upper left',fontsize=fs_legend)
         ax.set_xticks([])
-        ax.set_xlim(date_arr[0],date_arr[-1])
+        year_diff = 2
+        xstart = datetime(date_arr[0].year-year_diff,date_arr[0].month, date_arr[0].day)
+        xend   = datetime(date_arr[-1].year+year_diff,date_arr[-1].month, date_arr[-1].day)
+        #ax.set_xlim(date_arr[0],date_arr[-1])
+        ax.set_xlim(xstart, xend)
         ax.set_ylabel('[$^\circ C$]',fontsize=fsyl_size)
         ax = axs[0,1]
         var_t = 'air_temperature_mean'
         ptypet = 'dev'
         cmap = self.cmap_dict[var_t][ptypet]
         norm_size = [self.vminmax_dict_regavgyear[var_t][ptypet]['vmin'],self.vminmax_dict_regavgyear[var_t][ptypet]['vmax']]
         normalize = self.make_stripe_plot(date_arr,temp_dev,ax,cmap,norm_size,lretnorm=True)
         ax.set_xticks([])
-        ax.set_xlim(date_arr[0],date_arr[-1])
+        #ax.set_xlim(date_arr[0],date_arr[-1])
+        ax.set_xlim(xstart, xend)
 
         cax, _ = mpl.colorbar.make_axes(ax,shrink=0.65,fraction=0.03,pad=0.04,anchor=(2.0,0.5))
         cbar   = mpl.colorbar.ColorbarBase(cax,cmap=cmap,norm=normalize,extend='both')
         cbar.set_label(self.unit_dict[var_t],fontsize=fs_cbar)
 
         # plot precipitation
         ax = axs[1,0]
@@ -1252,26 +1257,28 @@
         #tmp_arr[4:] = moving_average(prec,5)
         tmp_arr[move_avg-1:] = moving_average(prec,move_avg)
         tmp_arr = np.ma.masked_where(tmp_arr == -999.,tmp_arr)
         ax.plot_date(date_arr,tmp_arr,'-',color='royalblue',label=f'Gleitendes Mittel ({move_avg}j)')
         handles, labels = ax.get_legend_handles_labels()
         ax.legend(handles, labels,loc='upper left',fontsize=fs_legend)
         ax.set_xticks([])
-        ax.set_xlim(date_arr[0],date_arr[-1])
+        #ax.set_xlim(date_arr[0],date_arr[-1])
+        ax.set_xlim(xstart, xend)
         ax.set_ylabel('[mm]',fontsize=fsyl_size)
         ax = axs[1,1]
         var_t = 'precipitation'
         ptypet = 'per'
         cmap = self.cmap_dict[var_t][ptypet]
         norm_size = [self.vminmax_dict_regavgyear[var_t][ptypet]['vmin'],self.vminmax_dict_regavgyear[var_t][ptypet]['vmax']]
         # calculate percental deviation
         prec_perc = (1.0 + (prec_dev/prec))*100.0
         normalize = self.make_stripe_plot(date_arr,prec_perc,ax,cmap,norm_size,lretnorm=True)
         ax.set_xticks([])
-        ax.set_xlim(date_arr[0],date_arr[-1])
+        #ax.set_xlim(date_arr[0],date_arr[-1])
+        ax.set_xlim(xstart, xend)
 
         cax, _ = mpl.colorbar.make_axes(ax,shrink=0.65,fraction=0.03,pad=0.04,anchor=(2.0,0.5))
         cbar   = mpl.colorbar.ColorbarBase(cax,cmap=cmap,norm=normalize,extend='both')
         cbar.set_label('%',fontsize=fs_cbar)
 
         # plot sunshine duration
         ax = axs[2,0]
@@ -1282,15 +1289,16 @@
         #print(sd)
         tmp_arr = np.ma.masked_where(tmp_arr == -999.,tmp_arr)
         # to avoid error message replace mask with nan
         tmp_arr = tmp_arr.filled(np.nan)
         ax.plot_date(date_arr,tmp_arr,'-',color='orange',label=f'Gleitendes Mittel ({move_avg}j)')
         handles, labels = ax.get_legend_handles_labels()
         ax.legend(handles, labels,loc='upper left',fontsize=fs_legend)
-        ax.set_xlim(date_arr[0],date_arr[-1])
+        #ax.set_xlim(date_arr[0],date_arr[-1])
+        ax.set_xlim(xstart, xend)
         ax.tick_params(axis='x', labelrotation=45)
         ax.set_ylabel('[h]',fontsize=fsyl_size)
 
         ax = axs[2,1]
         var_t = 'sunshine_duration'
         ptypet = 'per'
         cmap = self.cmap_dict[var_t][ptypet]
@@ -1298,15 +1306,16 @@
         cmap = self.get_continuous_cmap(hex_list)
         norm_size = [self.vminmax_dict_regavgyear[var_t][ptypet]['vmin'],self.vminmax_dict_regavgyear[var_t][ptypet]['vmax']]
         # calculate percental deviation
         sd_perc = (1.0 + (sd_dev/sd))*100.0
         # to avoid error message replace mask with nan
         sd_perc = sd_perc.filled(np.nan)
         normalize = self.make_stripe_plot(date_arr,sd_perc,ax,cmap,norm_size,lretnorm=True)
-        ax.set_xlim(date_arr[0],date_arr[-1])
+        #ax.set_xlim(date_arr[0],date_arr[-1])
+        ax.set_xlim(xstart, xend)
         ax.tick_params(axis='x', labelrotation=45)
 
         cax, _ = mpl.colorbar.make_axes(ax,shrink=0.65,fraction=0.03,pad=0.04,anchor=(2.0,0.5))
         cbar   = mpl.colorbar.ColorbarBase(cax,cmap=cmap,norm=normalize,extend='both')
         cbar.set_label('%',fontsize=fs_cbar)
 
         if(title is not None):
@@ -1912,15 +1921,15 @@
                          var_plot,
                          df_clim_daily,
                          clim_period,
                          df_climstats=None,
                          date_index=None,
                          year_in=None,
                          title=None,
-                         returnJson=False,
+                         returnJson=True,
                          filename=None
                         ):
         """Plots timeseries of actual year
            with given min/max and percentiles
         Arguments:
             df_in: DataFrame with timeseries data
             var_plot: Variable to plot
```

### Comparing `dwdhandler-0.2.0/src/dwdhandler.egg-info/SOURCES.txt` & `dwdhandler-0.2.1/src/dwdhandler.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/dwdhandler.egg-info/PKG-INFO
 src/dwdhandler.egg-info/SOURCES.txt
 src/dwdhandler.egg-info/dependency_links.txt
 src/dwdhandler.egg-info/requires.txt
 src/dwdhandler.egg-info/top_level.txt
 src/dwdhandler/calculation/__init__.py
 src/dwdhandler/calculation/calc_stats.py
+src/dwdhandler/calculation/geo.py
 src/dwdhandler/calculation/return_period.py
 src/dwdhandler/constants/__init__.py
 src/dwdhandler/constants/constpar.py
 src/dwdhandler/constants/filedata.py
 src/dwdhandler/constants/serverdata.py
 src/dwdhandler/helper/__init__.py
 src/dwdhandler/helper/ftp.py
```

