# Comparing `tmp/PICNIK-0.1.8.tar.gz` & `tmp/pICNIK-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PICNIK-0.1.8.tar", max compression
+gzip compressed data, was "pICNIK-0.1.9.tar", max compression
```

## Comparing `PICNIK-0.1.8.tar` & `pICNIK-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0     1074 2021-09-25 21:35:05.028501 PICNIK-0.1.8/LICENSE
--rw-r--r--   0        0        0     3757 2022-03-04 06:36:33.169397 PICNIK-0.1.8/README.md
--rw-r--r--   0        0        0    84067 2022-03-18 19:25:47.981210 PICNIK-0.1.8/picnik.py
--rw-r--r--   0        0        0      695 2023-05-04 01:14:47.039371 PICNIK-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     4578 2023-05-04 01:14:51.749279 PICNIK-0.1.8/setup.py
--rw-r--r--   0        0        0     4676 2023-05-04 01:14:51.750071 PICNIK-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2021-09-25 21:35:05.028501 pICNIK-0.1.9/LICENSE
+-rw-r--r--   0        0        0     7119 2023-12-22 20:54:06.783196 pICNIK-0.1.9/README.md
+-rw-r--r--   0        0        0       36 2021-08-31 20:25:39.684072 pICNIK-0.1.9/picnik/__init__.py
+-rw-r--r--   0        0        0     2089 2023-12-22 19:11:21.761196 pICNIK-0.1.9/picnik/integration.py
+-rw-r--r--   0        0        0   100727 2023-12-22 20:55:22.795505 pICNIK-0.1.9/picnik/picnik.py
+-rw-r--r--   0        0        0     5339 2023-12-22 19:13:16.730121 pICNIK-0.1.9/picnik/rxn_models.py
+-rw-r--r--   0        0        0      723 2023-12-22 23:07:25.187317 pICNIK-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     8088 2023-12-22 23:11:25.646385 pICNIK-0.1.9/setup.py
+-rw-r--r--   0        0        0     8021 2023-12-22 23:11:25.647588 pICNIK-0.1.9/PKG-INFO
```

### Comparing `PICNIK-0.1.8/LICENSE` & `pICNIK-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PICNIK-0.1.8/picnik.py` & `pICNIK-0.1.9/picnik/picnik.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,46 @@
 #!/usr/bin/python3.7
 """
 This module has two classes: DataExtraction and ActivationEnergy. 
-DataExtraction reads csv files and creates pandas.DataFrames according 
-to the isoconversional principle. ActivationEnergy computes the activation
-energy with five implemented isoconversional methods: Friedman (Fr), 
-Ozawa-Flynn-Wall(OFW), Kissinger-Akahira-Sunos (KAS) and the method 
-developed by Vyazovkin (Vy, aVy).
+DataExtraction reads csv files and creates pandas.DataFrames according to the isoconversional principle. 
+ActivationEnergy computes the activation energy (E) with five implemented isoconversional methods: 
+Friedman (Fr), Ozawa-Flynn-Wall(OFW), Kissinger-Akahira-Sunos (KAS) and the method developed by Vyazovkin (Vy, aVy).
+Additionally, ActivationEnergy possesses methods to reconstruct de reaction model in its integral form, g(a),
+methods to compute the compensation effect parameters (a,b) and the pre-exponential factor (A), as well as methods
+to make model-free or model-based predictions.
 """
 #Dependencies
-import numpy as np
-import pandas as pd
-from   scipy.interpolate import interp1d
-from   scipy.optimize    import minimize_scalar
+import numpy as np                                                      # (1) numpy
+import pandas as pd                                                     # (2) pandas
+from   scipy.interpolate import interp1d                                # (3) scipy
+from   scipy.optimize    import minimize_scalar, fsolve, curve_fit      
 import scipy.special     as     sp
-import matplotlib.pyplot as plt
-from scipy.stats import linregress
+from scipy.stats import linregress, f                                   
 from scipy import integrate
-import derivative
-from scipy.optimize import fsolve
+import matplotlib.pyplot as plt                                         # (4) matplotlib
+import derivative                                                       # (5) derivtive
+import integration as integ                                             # (*) 
+import rxn_models                                                       # (*)
 
+plt.rcParams.update({'font.size': 16})
 
+"""
+For informationn about the depencies we refer the user to:
+    (1) https://numpy.org/doc/stable/
+        Harris, C.R., Millman, K.J., van der Walt, S.J. et al. Array programming with NumPy. Nature 585, 357–362 (2020). DOI: 10.1038/s41586-020-2649-2. (Publisher link).
+    (2) https://pandas.pydata.org/
+        Data structures for statistical computing in python, McKinney, Proceedings of the 9th Python in Science Conference, Volume 445, 2010.
+    (3) https://docs.scipy.org/doc/scipy/
+        Pauli Virtanen, Ralf Gommers, Travis E. Oliphant, Matt Haberland, Tyler Reddy, David Cournapeau, Evgeni Burovski, Pearu Peterson, Warren Weckesser, Jonathan Bright, Stéfan J. van der Walt, Matthew Brett, Joshua Wilson, K. Jarrod Millman, Nikolay Mayorov, Andrew R. J. Nelson, Eric Jones, Robert Kern, Eric Larson, CJ Carey, İlhan Polat, Yu Feng, Eric W. Moore, Jake VanderPlas, Denis Laxalde, Josef Perktold, Robert Cimrman, Ian Henriksen, E.A. Quintero, Charles R Harris, Anne M. Archibald, Antônio H. Ribeiro, Fabian Pedregosa, Paul van Mulbregt, and SciPy 1.0 Contributors. (2020) SciPy 1.0: Fundamental Algorithms for Scientific Computing in Python. Nature Methods, 17(3), 261-272.
+    (4) https://matplotlib.org/
+        J. D. Hunter, "Matplotlib: A 2D Graphics Environment", Computing in Science & Engineering, vol. 9, no. 3, pp. 90-95, 2007.
+    (5) https://derivative.readthedocs.io/en/latest/
+        Kaptanoglu et al., (2022). PySINDy: A comprehensive Python package for robust sparse system identification. Journal of Open Source Software, 7(69), 3994, https://doi.org/10.21105/joss.03994
+    (*) This module come along with the picnik package. https://github.com/ErickErock/pICNIK/ 
+"""
 #-----------------------------------------------------------------------------------------------------------
 class DataExtraction(object):
     """
     Extractor to manipulate raw data to create lists and Data Frames 
     that will be used to compute the Activation Energy.
     """
     def __init__(self):
@@ -45,24 +62,29 @@
         self.t              = []              #list off experimental time
         self.alpha          = []              #list of experimental conversion
         self.TempIsoDF      = pd.DataFrame()  #Isoconversional temperature DataFrame
         self.timeIsoDF      = pd.DataFrame()  #Isoconversional time DataFrame
         self.diffIsoDF      = pd.DataFrame()  #Isoconversional conversion rate DataFrame
         self.TempAdvIsoDF   = pd.DataFrame()  #Advanced isoconversional temperature DataFrame
         self.timeAdvIsoDF   = pd.DataFrame()  #Advanced isoconversional time DataFrame
+        self.diffAdvIsoDF   = pd.DataFrame()  #Advanced isoconversional conversion rate DataFrame
 #-----------------------------------------------------------------------------------------------------------    
     def read_files(self, flist, encoding='utf8'):
         """ 
         Reads each TGA file as a pandas DataFrame and calculates de heating rate 
         
         Parameters:    flist : list object containing the paths of the files to be used.
         
                        encoding : The available encodings for pandas.read_csv() method. Includes but not limited 
                                   to 'utf8', 'utf16','latin1'. For more information on the python standar encoding:
-                                  (https://docs.python.org/3/library/codecs.html#standard-encodings)
+                                  (https://docs.python.org/3/library/codecs.html#standard-encodings).
+
+        Returns:       Beta: Array of the fitted heating rates.
+                       
+                       T0: Array of experimental initial temperatures.
         """
     
         print("Files to be used: \n{}\n ".format(flist))
         DFlis         =   self.DFlis
         Beta          =   self.Beta
         BetaCorrCoeff =   self.BetaCC
         T0            =   self.T0            
@@ -99,41 +121,43 @@
                 #computes the heating rate
                 LR = linregress(DF[DF.columns[0]],                            
                                 DF[DF.columns[1]])
 
                 BetaCorrCoeff.append(LR.rvalue)
                 Beta.append(LR.slope)
                 DFlis.append(DF)
-
             except IndexError:
                 DF = pd.read_csv(item,  sep = ',', encoding = encoding)
-                T0.append(DF[DF.columns[1]][0]+273.15)
+                #stores the initial temperature of the ith experiment
+                T0.append(DF[DF.columns[1]][0]+273.15)                       
+                #computes the mass loss percentage
                 DF['%m'] = 100*(DF[DF.columns[2]]/DF[DF.columns[2]][0])
                 #creates a column for the temperature in Kelvin
                 DF['Temperature [K]'] = DF[DF.columns[1]] + 273.15      
-                #computes the differential thermogram with a Savitzki-Golay filter
-                dTdt = derivative.dxdt(DF[DF.columns[1]].values,
+                #computes the heating rate with a Savitzki-Golay filter
+                dTdt = derivative.dxdt(DF['Temperature [K]'].values,             
                                        DF[DF.columns[0]].values,
                                        kind="savitzky_golay", 
                                        order=3,
                                        left=0.5,
                                        right=0.5)
                 DF['dT/dt$'] = DF[DF.columns[0]]
-                DF['dT/dt$'] = dTdt
-                dwdt = derivative.dxdt(DF[DF.columns[2]].values,
-                                       DF[DF.columns[0]].values,
+                DF['dT/dt$'] = dTdt         
+                #computes the differential thermogram with a Savitzki-Golay filter                                    
+                dwdt = derivative.dxdt(DF[DF.columns[2]].values,             
+                                       DF[DF.columns[0]].values,          
                                        kind="savitzky_golay",
                                        order=3,
                                        left=0.5,
                                        right=0.5)
                 DF['dw/dt'] = DF[DF.columns[0]]
                 DF['dw/dt'] = dwdt 
                 
                 #computes the heating rate
-                LR = linregress(DF[DF.columns[0]],
+                LR = linregress(DF[DF.columns[0]],                            
                                 DF[DF.columns[1]])
 
                 BetaCorrCoeff.append(LR.rvalue)
                 Beta.append(LR.slope)
                 DFlis.append(DF)
 
         self.DFlis  = DFlis                     #List of the DataFrames constructed
@@ -189,15 +213,15 @@
         #In order to make the interpolation the x values must be strictly in ascending order.
         #The next block of code evaluates if the i-th value is bigger than the i-1-th, if so, 
         #the value is appended to the corresponding list. 
         for i in range(len(NDFl)):
             #The initial values are those of the lower limit of the temperature range.
             a = [NDFl[i]['alpha'].values[0]]
             Temp = [NDFl[i]['Temperature [K]'].values[0]]
-            time = [NDFl[i][DFlist[i].columns[0]].values[0]]
+            time = [NDFl[i][NDFl[i].columns[0]].values[0]]
             diff = [NDFl[i]['da/dt'].values[1]] 
             for j in range(len(NDFl[i]['alpha'].values)):
                 if NDFl[i]['alpha'].values[j] == a[-1]:
                     pass
                 #If the i-th value is bigger than the i-1-th
                 #its corresponding values of time, temperature 
                 #and conversion rate and itself are stored
@@ -221,28 +245,32 @@
         self.t         = t         #list of arrays of temperatures corresponding to a conversion value
         self.da_dt     = da_dt
 
         plt.style.use('tableau-colorblind10')
 
         markers = ["o","v","x","1","s","^","p","<","2",">"]
         #Plot of the thermograms showing the anaysis range.
-        for i in range(len(DFlist)):
-            plt.plot(DFlist[i]['Temperature [K]'].values[::40],           #Temperature in Kelvin
-                     DFlist[i]['%m'].values[::40],                        #mass loss percentage
+        fig, ax1 = plt.subplots(figsize=(12,9))
+
+        for i in range(len(NDFl)):
+            ax1.plot(NDFl[i]['Temperature [K]'].values[::40],           #Temperature in Kelvin
+                     NDFl[i]['alpha'].values[::40],                        #mass loss percentage
                      marker = markers[i],
+                     markersize=10,
                      linestyle = '--',
+                     linewidth=4,
                      label=r'$\beta=$'+str(np.round(self.Beta[i],decimals=2))+' K/min',
                      alpha=0.75)
-        plt.axvline(x=(T0),alpha=0.8,color='red',ls='--',lw=1.2)         #temperature lower limit
-        plt.axvline(x=(Tf),alpha=0.8,color='red',ls='--',lw=1.2)         #temperature upper limit
-        plt.ylabel('mass [%]')
-        plt.xlabel('Temperature [K]')
-        plt.xlim((T0-20),(Tf+20)) 
-        plt.legend(frameon=True)
-        plt.grid(True)
+        ax1.axvline(x=(T0),alpha=0.8,color='red',ls='--',lw=2.3)         #temperature lower limit
+        ax1.axvline(x=(Tf),alpha=0.8,color='red',ls='--',lw=2.3)         #temperature upper limit
+        ax1.set_ylabel(r'conversion ($\alpha$)')
+        ax1.set_xlabel('Temperature [K]')
+        ax1.set_xlim((T0-20),(Tf+20)) 
+        ax1.legend(frameon=True)
+        ax1.grid(True)
 
         plt.show()
 #-----------------------------------------------------------------------------------------------------------
     def Isoconversion(self, advanced = False, method='points', N = 1000, d_a = 0.001):    
         """
         Constructs the isoconversional DataFrames.
 
@@ -253,34 +281,34 @@
                                           True the conversion array can be constructed con the linspace 
                                           or arange functions of numpy. 'points' will call for linspace
                                           while 'step' will call for arange.
 
                                 N:        The number of points in the conversion array If method is set 
                                           to 'points'.
 
-                                d_a:      The size of the step from the i-th to the i+1-th value in the
-                                          conversion array If method is set to 'step'.
+                                d_a:      The step size between the i-th and the i+1-th value in the
+                                          conversion array if method is set to 'step'.
 
-        Returns:                pandas.DataFrame objects: Temperatures Dataframe, times DataFrame, conversion
-                                rates DataFrame. If advanced is to True it also returns a Temperatures and times
-                                DataFrames for the aadvanced method of Vyazovkin (aVy method in ActivationEnergy).                     
-               
+        Returns:                3 or 6 pandas.DataFrame objects: Temperatures Dataframe, times DataFrame, conversion
+                                rates DataFrame. If advanced set is to True it also returns an advanced version of each 
+                                DataFrameTemperatures and times for the advanced method of Vyazovkin (aVy method in ActivationEnergy).                           
         """
         
         alpha = self.alpha
         T     = self.T
         t     = self.t
         da_dt = self.da_dt
         Beta  = self.Beta
         
         TempIsoDF    = self.TempIsoDF      
         timeIsoDF    = self.timeIsoDF     
         diffIsoDF    = self.diffIsoDF      
         TempAdvIsoDF = self.TempAdvIsoDF   
-        timeAdvIsoDF = self.timeAdvIsoDF  
+        timeAdvIsoDF = self.timeAdvIsoDF
+        diffAdvIsoDF = self.diffAdvIsoDF  
         #The experimental set with the least points is selected as conversion 
         #array for the isoconversional coomputations because all the other data sets
         #have more points to interpolate a reliable function for the conversion array
         alps = np.array(alpha[-1])
         print(f'Creating Isoconversion DataFrames...')
         #The time, temperature and conversion rate values corresponding to conversion array
         #selected are pass atrightforward to the corresponding isoconversional DataFrame
@@ -348,27 +376,35 @@
                 TempAdvIsoDF['HR '+str(np.round(Beta[i], decimals = 1)) + ' K/min'] = np.round(inter_func(adv_alps), decimals = 4)
 
                 inter_func2 = interp1d(alpha[i], 
                                        t[i],
                                        kind='cubic', bounds_error=False, 
                                        fill_value="extrapolate")
                 timeAdvIsoDF['HR '+str(np.round(Beta[i], decimals = 1)) + ' K/min'] = np.round(inter_func2(adv_alps), decimals = 4)
+                
+                inter_func3 = interp1d(alpha[i], 
+                                       da_dt[i],
+                                       kind='cubic', bounds_error=False, 
+                                       fill_value="extrapolate")
+                diffAdvIsoDF['HR '+str(np.round(Beta[i], decimals = 1)) + ' K/min'] = np.round(inter_func2(adv_alps), decimals = 4)
             
             timeAdvIsoDF.index = adv_alps
             TempAdvIsoDF.index = adv_alps
+            diffAdvIsoDF.index = adv_alps
 
             self.TempAdvIsoDF = TempAdvIsoDF      #Isoconversional DataFrame of temperature for the advanced Vyazovkin method (aVy)
             self.timeAdvIsoDF = timeAdvIsoDF      #Isoconversional DataFrame of time for the advanced Vyazovkin method (aVy)
+            self.diffAdvIsoDF = diffAdvIsoDF      #Isoconversional DataFrame of conversion rate for the advanced Vyazovkin method (aVy)
             self.d_a          = d_a               #Size of the \Delta\alpha step
         else:
             pass
         
         print(f'Done')
 
-        return self.TempIsoDF, self.timeIsoDF, self.diffIsoDF, self.TempAdvIsoDF, self.timeAdvIsoDF
+        return self.TempIsoDF, self.timeIsoDF, self.diffIsoDF, self.TempAdvIsoDF, self.timeAdvIsoDF, self.diffAdvIsoDF
 #-----------------------------------------------------------------------------------------------------------        
     def get_beta(self):
         """
         Getter for the heating rates.
 
         Parameters:   None
 
@@ -583,19 +619,18 @@
                      self.da_dt[i],
                      label=str(np.round(self.Beta[i],decimals=1))+' K/min')
             plt.xlabel(self.DFlis[i].columns[0])
             plt.ylabel('$\alpha$')
             plt.legend()
         return plt.show()
 #-----------------------------------------------------------------------------------------------------------
-
 #-----------------------------------------------------------------------------------------------------------
 class ActivationEnergy(object):
     """
-	Uses the attributes of Dataextraction to compute activation energy values based on five methods: 
+	Uses the attributes of DataExtraction to compute activation energy values based on five methods: 
     Friedman, FOW, KAS, Vyazovkin and Advanced Vyazovkin. 
     """
     def __init__(self, Beta, T0, TempIsoDF=None, diffIsoDF=None, TempAdvIsoDF=None, timeAdvIsoDF=None):
         """
 		Constructor. Defines variables and the constant R=8.314 J/(mol K)
 
         Parameters:         Beta         : array object containing the values of heating 
@@ -1111,69 +1146,80 @@
         c = sup
         #Computation of the intagral defined in terms of the exponential integral
         #calculated with scipy.special
         J = a*(sp.expi(-a/c)-sp.expi(-a/b)) + c*np.exp(-a/c) - b*np.exp(-a/b)
 
         return J
 #-----------------------------------------------------------------------------------------------------------        
-    def J_time(self, E, row_i, col_i, method = 'trapezoid'):
+    def J_time(self, E, row_i, col_i, N=1, method='trapezoid',ti=None, tf=None, Beta=None, T_func=None, isothermal=False, isoT=0):
         """
         Time integral for the Advanced Vyazovkin Treatment. Considering a linear heating rate.
 
         Prameters:   E       : Float object. Value for the activation energy to evaluate the 
                                integral
 
                      row_i   : Index value for the row of conversion in the pandas DataFrame
                                containing the isoconversional times for evenly spaced conversion 
                                values.
  
                      col_i   : Index value for the column of heating rate in the pandas DataFrame 
                                containing the isoconversional times for evenly spaced conversion 
                                values.
 
-                     method  : Numerical integration method. Can be 'trapezoid', 'simpson' or 'quad'.
+                     method  : Numerical integration method. Can be 'trapezoid', 'simpson', 'romberg' or 'quad'.
                                The method corresponds to those implemented in the scipy.integrate
                                subpackage.
 
         Returns:     J_t     : Float. Value of the integral obtained by a numerical integration method. 
         """    
-        timeAdvIsoDF   = self.timeAdvIsoDF
-        #Heating rate for the computation
-        B  = self.Beta[col_i]
-        #Initial experimental temperature
-        T0 = self.T0[col_i]
-        #Time values associated to the lower limit of the
-        #Temperature range set with DataExtraction.Conversion
-        t0 = timeAdvIsoDF[timeAdvIsoDF.columns[col_i]][timeAdvIsoDF.index.values[row_i]]
-        #Time associated to the i-th conversion value
-        t  = timeAdvIsoDF[timeAdvIsoDF.columns[col_i]][timeAdvIsoDF.index.values[row_i+1]]
-        #Value for the Arrhenius exponential for the time t0 and energy E
-        y0 = np.exp(-E/(self.R*(T0+(B*t0))))
-        #Value for the Arrhenius exponential for the time t and energy E
-        y  = np.exp(-E/(self.R*(T0+(B*t))))
-            
+
+        def time_int(t,*args):
+            T0 = args[0]
+            B  = args[1]
+            E  = args[2]
+            if T_func == None:
+                T  = T0+(B*t)   
+            else:
+                T  = T_func(t)
+            return np.exp(-E/(self.R*(T)))
+       
+        if tf == None:
+            timeAdvIsoDF   = self.timeAdvIsoDF
+            #Heating rate for the computation
+            B  = self.Beta[col_i]
+            #Initial experimental temperature
+            T0 = self.T0[col_i]
+            t0 = timeAdvIsoDF[timeAdvIsoDF.columns[col_i]][timeAdvIsoDF.index.values[row_i]]
+            t  = timeAdvIsoDF[timeAdvIsoDF.columns[col_i]][timeAdvIsoDF.index.values[row_i+N]]
+        else:
+            t0 = ti
+            t  = tf
+            if isothermal == False:
+                T0 = np.mean(self.T0)
+                B  = Beta
+            else:
+                T0 = isoT
+                B = 0
         if method == 'trapezoid':
-            J_t = integrate.trapezoid(y=[y0,y],x=[t0,t])
+            J_t = integ.Trapezoid(time_int, t0, t, N, T0, B, E, Romberg=False)[0]
             return J_t
-            
         elif method == 'simpson':
-            J_t = integrate.simpson(y=[y0,y],x=[t0,t])
+            J_t = integ.Simpson(time_int, t0, t, N, T0, B, E)[0]
             return J_t
-            
         elif method == 'quad':
-            def time_int(t,T0,B,E):
-                return np.exp(-E/(self.R*(T0+(B*t))))
-            
             J_t = integrate.quad(time_int,t0,t,args=(T0,B,E))[0]
             return J_t
+        elif method == 'romberg':
+            J_t = integ.Romberg(time_int, t0, t, N, T0, B, E)[0]
+            return J_t
         else:
             raise ValueError('method not recognized')
 
 #-----------------------------------------------------------------------------------------------------------        
-    def adv_omega(self,E, row, var = 'time', method='trapezoid'):
+    def adv_omega(self,E, row, var = 'time', N = 1, method='trapezoid'):
         """
         Function to minimize according to the advanced Vyazovkin treatment:
 
         \Omega(Ea) = \sum_{i}^{n}\sum_{j}^{n-1}{[{J(E,T(t_{i}))]}/[B_{i}{J(E,T(t_{j}))}]}
 
         Parameters:   E       : Float object. Value for the activation energy to evaluate 
                                 the integral
@@ -1209,22 +1255,23 @@
             O = np.array(np.sum((omega_i)))
             return O
   
         elif var == 'time':
             I_B = np.array([self.J_time(E,
                                         row,
                                         i,
+                                        N,
                                         method) 
                             for i in range(len(timeAdvIsoDF.columns))])
             #Double sum
             omega_i = np.array([I_B[k]*((np.sum(1/(I_B)))-(1/I_B[k])) for k in range(len(Beta))])
             O = np.array(np.sum((omega_i)))
             return O        
 #-----------------------------------------------------------------------------------------------------------
-    def visualize_advomega(self,row,var='time',bounds=(1,300),N=1000, method='trapezoid'):
+    def visualize_advomega(self,row,var='time',bounds=(1,300),n=1000, N = 1, method='trapezoid'):
         """
         Method to visualize adv_omega function. 
 
         Parameters:   row     : Index value for the row of conversion in the pandas DataFrame
                                 containing the isoconversional times or temperatures.
                      
                       var     : The variable to perform the integral with, it can be either
@@ -1245,27 +1292,27 @@
         #Temperature DataFrame
         TempAdvIsoDF = self.TempAdvIsoDF
         #time DataFrame
         timeAdvIsoDF = self.timeAdvIsoDF
         #Heating Rates
         Beta         = self.Beta
         #Activation energy (independent variable) array
-        E = np.linspace(bounds[0], bounds[1], N)
+        E = np.linspace(bounds[0], bounds[1], n)
         #Evaluation of \Omega(E)
-        O = np.array([float(self.adv_omega(E[i],row,var,method)) for i in range(len(E))])
+        O = np.array([float(self.adv_omega(E[i],row,var,N,method)) for i in range(len(E))])
         plt.style.use('seaborn-whitegrid')
         plt.plot(E,O,color='teal',label=r'$\alpha$ = '+str(np.round(timeAdvIsoDF.index[row],decimals=3)))
         plt.ylabel(r'$\Omega\left(E_{\alpha}\right)$')
         plt.xlabel(r'$E_{\alpha}$')
         plt.legend()
         plt.grid(True)
 
         return plt.show()
 #-----------------------------------------------------------------------------------------------------------        
-    def variance_aVy(self, E, row_i, var = 'time', method = 'trapezoid'):
+    def variance_aVy(self, E, row_i, var = 'time', N=1, method = 'trapezoid'):
         """
         Method to calculate the variance of the activation energy E obtained with the Vyazovkin 
         treatment. The variance is computed as:
 
         S^{2}(E) = {1}/{n(n-1)}\sum_{i}^{n}\sum_{j}^{n-1}{[{J(E,T(t_{i}))]}/[{J(E,T(t_{j}))}]-1}^{2}
 
         Parameters:     E      : The activation energy value used to calculate 
@@ -1286,29 +1333,29 @@
 
         --------------------------------------------------------------------------------------------
         Reference:     Vyazovkin, S., & Wight, C. A. (2000). Estimating realistic confidence intervals 
                        for the activation energy determined from thermoanalytical measurements. 
                        Analytical chemistry, 72(14), 3171-3175.
         """
         #Total number of addends
-        N = len(self.Beta)*(len(self.Beta)-1)
+        n = len(self.Beta)*(len(self.Beta)-1)
         #Selection of the integral based on parameter "var"
         if var == 'time':
             #lower limit 
             inf = self.timeAdvIsoDF.index.values[row_i] 
             #upper limit
             sup = self.timeAdvIsoDF.index.values[row_i+1]
             #initial temperature
             T0  = self.T0
             #time integrals into a list comprehension        
-            J = np.array([self.J_time(E, row_i, i, method) for i in range(len(self.Beta))])     
+            J = np.array([self.J_time(E, row_i, i, N,method) for i in range(len(self.Beta))])     
             #Each value to be compared with one (s-1) to compute the variance
             s = np.array([J[i]/J for i in range(len(J))])
             
-            return np.sum((s-1)**2)/N
+            return np.sum((s-1)**2)/n
             
         elif var == 'Temperature':
             #lower limit
             inf = self.TempAdvIsoDF.index.values[row_i] 
             #upper limit
             sup = self.TempAdvIsoDF.index.values[row_i+1]
         
@@ -1316,33 +1363,33 @@
             J = [self.J_Temp(E, 
                             self.TempAdvIsoDF[self.TempAdvIsoDF.columns[i]][inf], 
                             self.TempAdvIsoDF[self.TempAdvIsoDF.columns[i]][sup]) 
                  for i in range(len(self.Beta))]
             #Each value to be compared with one (s-1) to compute the variance
             s = np.array([J[i]/J for i in range(len(J))])
             
-            return np.sum((s-1)**2)/N
+            return np.sum((s-1)**2)/n
 
         else:
             raise ValueError('variable not valid')
 
 #-----------------------------------------------------------------------------------------------------------        
-    def psi_aVy(self, E, row_i, var = 'time', method = 'trapezoid'):
+    def psi_aVy(self, E, row_i, var = 'time', N = 1, p =0.95, method = 'trapezoid'):
         """
         Method to calculate the F distribution to minimize for the Vyazovkin method.
         The distribution is computed as: 
 
         \Psi(E) = S^{2}(E)/S^{2}_{min}
 
         Parameters:     E      : The activation energy value used to calculate 
                                  the value of omega.
 
                         row_i  : index value for the row of conversion in the
                                  pandas DataFrame containing the isoconversional
-                                 temperatures.         
+                                 times or temperatures.         
 
                         bounds : Tuple object containing the lower and upper limit values 
                                  for E, to evaluate the variance.
 
                         var    : The variable to perform the integral with, it can be either
                                 'time' or 'Temperature'
 
@@ -1354,50 +1401,49 @@
                                  and upper confidence limits for E.  
         --------------------------------------------------------------------------------------------
         
         Reference:     Vyazovkin, S., & Wight, C. A. (2000). Estimating realistic confidence intervals 
                        for the activation energy determined from thermoanalytical measurements. 
                        Analytical chemistry, 72(14), 3171-3175.
         """         
-        #F values for a 95% confidence interval for (n-1) and (n-1) degreees of freedom
-        F      = [161.4, 19.00, 9.277, 6.388, 5.050, 4.284, 3.787, 3.438, 3.179,2.978,2.687]
-        #F value for the n-1 degrees of freedom
-        #Subtracts 1 to n (len(B)) because of degrees of freedom and 1 because of python indexation
-        f      = F[len(self.Beta)-1-1]
+        #F values for a p% confidence interval for (n-1) and (n-1) degreees of freedom
+        n1, n2 = len(self.Beta)*(len(self.Beta)-1)-1, len(self.Beta)*(len(self.Beta)-1)-1
+        F = f.ppf(p,n1,n2)
+            
         #Quadrature method from parameter "method"              
         method = method
         #Psi evaluation interval
-        E_p    = np.linspace(1,E+50,50)  #intervalo para evaluar Psi
+        E_p    = np.linspace(1,E+150,150)  #intervalo para evaluar Psi
         #'True' value of the activation energy in kJ/mol for a given conversion (row_i)
         E_min  = E
         #Variance of the 'True' activation energy 
-        s_min  = self.variance_aVy(E_min, row_i,var, method) 
+        s_min  = self.variance_aVy(E_min, row_i,var, N,method) 
         #Variance of the activation energy array E_p 
-        s      = np.array([self.variance_aVy(E_p[i], row_i, var, method) for i in range(len(E_p))])
+        s      = np.array([self.variance_aVy(E_p[i], row_i, var, N,method) for i in range(len(E_p))])
         
         #Psi function moved towards negative values (f-1) in order 
         #to set the confidence limits such that \psy = 0 for those values
-        Psy_to_cero = (s/s_min)-f-1
+        Psy_to_cero = (s/s_min)-F
         
         #Interpolation function of \Psy vs E to find the roots
         #which are the confidence limits
         inter_func = interp1d(E_p,
                               Psy_to_cero, 
                               kind='cubic',  
                               bounds_error=False, 
                               fill_value="extrapolate")
         #Finding the confidence limits
         zeros = np.array([fsolve(inter_func, E-150)[0],
                           fsolve(inter_func, E+150)[0]])
         
-        error = np.mean(np.array([abs(E-zeros[0]), abs(E-zeros[1])]))
+        error = abs(zeros[1] - zeros[0])/2
 
-        return error 
+        return error, Psy_to_cero, E_p 
 #-----------------------------------------------------------------------------------------------------------            
-    def error_aVy(self, E, var = 'time', method = 'trapezoid'):
+    def error_aVy(self, E, var = 'time', N = 1, p =0.95, method = 'trapezoid'):
         """
         Method to calculate the distribution to minimize for the Vyazovkin method.
 
         Parameters:     bounds   : Tuple object containing the lower and upper limit values 
                                    for E, to evaluate adv_omega.
 
                         var    : The variable to perform the integral with, it can be either
@@ -1407,21 +1453,21 @@
                                  or 'quad'. The method correspond to those implemented in 
                                  the scipy.integrate subpackage. Default 'trapezoid'.
 
         Returns:        error_aVy : Array of error values associated to the array of activation 
                                     energies obtained by the Vyazovkin method.  
         """ 
         method = method
-        error_aVy = np.array([self.psi_aVy(E[i], i, var=var, method=method) for i in range(len(E))])
 
-        return error_aVy  
+        error_aVy = np.array([self.psi_aVy(E[i], i, var=var, N=N, p=p, method=method)[0] for i in range(len(E))])
 
+        return error_aVy  
 
 #-----------------------------------------------------------------------------------------------------------
-    def aVy(self,bounds, var='time', method='trapezoid'):
+    def aVy(self,bounds, var='time', N = 1, p= 0.95, method='trapezoid', strat = 'min'):
         """
         Method to compute the Activation Energy based on the Advanced Vyazovkin treatment.
         \Omega(E_{\alpha})= min[ sum_{i}^{n}\sum_{j}^{n-1}[J(E,T_{i})]/[J(E,T_{j})] ]
 
         Parameters:   bounds : Tuple object containing the lower limit and the upper 
                                limit values of E, for evaluating omega.
 
@@ -1447,21 +1493,49 @@
                       account for variation in the activation energy, Journal of Computational
                       Chemistry 22 (2) (2001) 178–183.
         """
 
         timeAdvIsoDF = self.timeAdvIsoDF
         Beta         = self.Beta
         print(f'Advanced Vyazovkin method: Computing activation energies...')
-        #Computing and minimization of \Omega(E) for the conversion values in the isoconversional DataFrame    
-        E_aVy        = [minimize_scalar(self.adv_omega,bounds=bounds,args=(k,var,method), method = 'bounded').x 
-                        for k in range(len(timeAdvIsoDF.index)-1)]
+        
+        if strat == 'min':
+            E_aVy    = [minimize_scalar(self.adv_omega,bounds=bounds,args=(m,var,N,method), method = 'bounded').x 
+                        for m in range(len(timeAdvIsoDF.index)-N)]
+
+            error   = self.error_aVy(E_aVy, var=var, N=N, p=p, method=method)
+
+        elif strat == 'quad_fit':
+            E_aVy = []
+            error = []
+            def quadratic(x,*args):
+                A = args[0]
+                B = args[1]
+                C = args[2]
+                return (A*(x**2))+(B*x) + C
+
+            E = np.linspace(bounds[0], bounds[1], 500)
+            for r in range(len(timeAdvIsoDF.index)-N):
+                O = self.adv_omega(E, r, var = var, N = N, method=method) 
+                popt, pcov = curve_fit(quadratic, E, O, p0=[1,1,1])
+                
+                print(popt)
+                E_min = -popt[1]/(2*popt[0])
+                E_aVy.append(E_min)
+
+                perr = np.sqrt(np.diag(pcov))
+                m = perr[1]/(2*popt[0])
+                n = perr[0]*(popt[1]/(2*(popt[0]**2)))
+                E_err= np.sqrt(m**2 + n**2)        
+                error.append(E_err)
+            error = np.array(error)
 
         E_aVy   = np.array(E_aVy)
-
-        error   = self.error_aVy(E_aVy, var, method)
+        
+        
 
         self.E_aVy =  (E_aVy, error)
         print(f'Done.')
         return self.E_aVy
 #-----------------------------------------------------------------------------------------------------------
     def T_prom(self,TempIsoDF):
         """
@@ -1479,15 +1553,15 @@
             Ti = np.mean(TempIsoDF.iloc[i].values)
             T_prom.append(Ti)
         T_prom = np.array(T_prom)
         
         return T_prom
 #-----------------------------------------------------------------------------------------------------------
 
-    def export_Ea(self, E_Fr=False, E_OFW=False, E_KAS=False, E_Vy=False, E_aVy=False, file_t="xlsx" ):
+    def export_Ea(self, E_Fr=False, E_OFW=False, E_KAS=False, E_Vy=False, E_aVy=False, N = 1, file_t="xlsx" ):
         """
         Method to export activation energy values and their uncertainty calculated as either a csv or xlsx file.
          
         Parameters:    E_Fr     : tuple of activation energies and its uncertainty obtained by de Friedman method.
 
                        E_OFW    : tuple of activation energies and its uncertainty obtained by de OFW method.
 
@@ -1521,24 +1595,24 @@
             ad_col = ['alpha',                       #Conversion
                       'Temperature [K]',             #Temperature
                       'adv.Vyazovkin [kJ/mol]',      #Activation energies in kJ/mol
                       'aVy_error [kJ/mol]']          #Associated error in kJ/mol
             #pandas.DataFrame to save the advanced Vyazovking method results
             adv_DF = pd.DataFrame([],columns = ad_col)
             #Conversion values for the isoconversional evaluations
-            adv_alps = TempAdvIsoDF.index.values[1:]
+            adv_alps = TempAdvIsoDF.index.values[N:]
             #Mean values for temperature at isoconversional values
             adv_Temp = self.T_prom(TempAdvIsoDF)
             #Filling the columns with thier corresponding values
             adv_DF[ad_col[0]] = adv_alps             
-            adv_DF[ad_col[1]] = adv_Temp[1:]
+            adv_DF[ad_col[1]] = adv_Temp[N:]
             adv_DF[ad_col[2]] = aVy[0]
             adv_DF[ad_col[3]] = aVy[1]
         
-            print(TempAdvIsoDF, adv_DF)
+            #print(TempAdvIsoDF, adv_DF)
 
         else:
             pass
 
         #Conversion values for the isoconversional evaluations
         alps     = TempIsoDF.index.values
         #Mean values for temperature at isoconversional values
@@ -1604,17 +1678,23 @@
             DF_Nrgy['Vyazovkin [kJ/mol]'] = E_Vy[0]        #Activation energies in kJ/mol
             DF_Nrgy['Vy_error [kJ/mol]']=E_Vy[1]           #Associated error in kJ/mol
         else:
             pass        
 
 
         #For methods Fr, KAS, OFW and Vy
-        name1 = 'Activation_Energies_Results.'
+        if E_Fr == False and E_OFW == False and E_KAS == False and E_Vy == False:
+            pass
+        else:   
+            name1 = input('Input file name for the Fr, OFW, KAS and/or Vy results:' )
         #For method aVy
-        name2 = 'Advanced_Vyazovkin_Results.'
+        if E_aVy == False:
+            pass
+        else:
+            name2 = input('Input file name for the adv.Vy results:')
 
         #The format of the file is set with the parameter "file_t"
         if(file_t=='xlsx'):
             
             if len(columns) == 2:
                 pass
             #else, create the corresponding file
@@ -1650,56 +1730,308 @@
             if aVy == self.E_aVy:
                 adv_DF.to_csv((name2+'csv'), 
                                encoding='utf8', 
                                sep=',',
                                index=False)
             else:
                 pass
-            print('Results saved as {0} and {1}'.format(name1,name2)) 
+            print('Results exported') 
         else:
             raise ValueError("File type not recognized")
 
         print(f'Done.')        
 #-----------------------------------------------------------------------------------------------------------        
-    def prediction(self, E = None, B = 1, T0 = 298.15, Tf=1298.15):
+    def prediction(self,E, B, isoT = None, T_init=None,T_func = None, alpha=0, N=1, method='trapezoid', bounds = (5,5)):
         """
-        Experimental method. May raise error or give unreliable results.
+        Method to compute a model-free prediction based on the integral isoconversional principle: $g(\alpha)=constant$ which implies 
+        an equality between teperature integrals to reach a given conversion: $J[E_alpha,T(t)_i] = J[E_alpha,T(t)_j]$
+        where $T(t)_i and T(t)_j$ are two different temperature programs
+
+        Parameters:         E       :    Activation energy array
 
+                            B       :    Heating rate for a linear temperature program; T(t) = T0 +Bt
+                             
+                            isoT    :    Temperature for a constant temperature program (isothermal); T = isoT = constant
 
+                            T_init  :    Initial temperature for the linear temperature program (T0). 
+                                         The default value is an average of the experimental initial temperatures.
 
+                            T_func  :    A custom program temperature; T = T(t)
 
+                            alpha   :    This parameter determines the starting point in the time domain for the temperature 
+                                         integral. The default value (alpha = 0) sets the initial time to an averge of the 
+                                         experimental initial times. Otherwise the initial time equals zero.
 
-        Method to calculate a kinetic prediction, based on an isoconversional 
-        activation energy
+                            N       :    Data blocks for the numerical integration (see J_time).
 
-        Parameters:   E  : numpy array of the activation energy values to use for
-                           the prediction.
+                            method  :    Numerical integration method. For more information see integration.py (help(picnik.integ)).
 
+                            bounds  :    As the computation of the time required to reach a given conversion involves a minimization
+                                         procedure this parameters sets the bounds in the time domain where the minimum would be reasonable
+                                         to be found.
+
+        Returns:            a_prime :    Conversion array
+
+                            T_prime :    Temperature array corresponding to the temperature program which the prediction is made for
+
+                            t_prime :    Predicted time to reach each converssion value in the a_prime array
+        -----------------------------------------------------------------------------------------------------------------------------------
+        References:         Granado, L., & Sbirrazzuoli, N. (2021). Isoconversional computations for nonisothermal kinetic predictions. Thermochimica Acta, 697, 178859. 
+
+        """
+        def j(t,Ei,col,row):
+            
+            J0  = self.J_time(Ei,
+                              row,
+                              col,
+                              N=N,
+                              method=method)
+            if isoT != None:
+                Ji  = self.J_time(Ei,
+                                  row,
+                                  col,
+                                  N=N,
+                                  method=method,
+                                  ti = t_prime[row],
+                                  tf = t,
+                                  Beta = B,
+                                  isothermal =True, 
+                                  isoT = isoT)
+            else:
+                if T_func == None:
+                    Ji  = self.J_time(Ei,
+                                      row,
+                                      col,
+                                      N=N,
+                                      method=method,
+                                      ti = t_prime[row],
+                                      tf = t,
+                                      Beta = B)
+                else:
+                    Ji  = self.J_time(Ei,
+                                      row,
+                                      col,
+                                      N=N,
+                                      method=method,
+                                      ti = t_prime[row],
+                                      tf = t,
+                                      Beta = B,
+                                      T_func = T_func)
+            return (Ji-J0)**2
+        
+        def J(t,Ei,row):
+            J = []
+            for b in range(len(Beta)):
+                J.append(j(t,Ei,b,row))
+            J = np.sum(np.array(J))
+            return J
+
+
+        Beta = self.Beta
+        T0   = self.T0
+        tDF  = self.timeAdvIsoDF
+        
+        if T_init == None:
+            T_i = np.mean(T0)
+        else:
+            T_i = T_init
+    
+        if alpha != 0:
+            tDF = tDF.loc[tDF.index.values <= alpha]
+            tj_init = 0
+        else: 
+            t0_int = interp1d(Beta,
+                          tDF.iloc[0].values[0:len(Beta)],
+                          fill_value='extrapolate')
+            tj_init = t0_int(B)
+    
+        t_prime = [tj_init]
+        print('Beginning simulation at : ',tj_init,' min')
+        for i in range(len(tDF.index)-N):
+            tm = minimize_scalar(J,args=(E[i],i),bounds=((t_prime[i]-bounds[0]),(t_prime[i]+bounds[0])), method = 'bounded').x
+            t_prime.append(tm)
+            
+        t_prime = np.array(t_prime)
+        a_prime = tDF.index.values
+        if isoT != None:
+            T_prime = isoT
+        else:
+            if T_func == None:
+                T_prime = T_i + (B*t_prime)
+            else:
+                T_prime = np.array([T_func(t_prime[i]) for i in range(len(t_prime))]) 
+        return (a_prime, T_prime, t_prime)
+#----------------------------------------------------------------
+
+    def compensation_effect(self, E, B, f_alpha = None):
+        """
+        Experimental method. May raise error or give unreliable results.
+        Parameters:   f_alpha  : List of functions to iterate. 
+                                 By default the function will iterate over all the functions
+                                 on the rxn_models.py file 
                       B  : Float. Value of the heating rate for the prediction.
+                      E  : numpy array containing the values of activation energy.
+        Returns:      a  : 
+                      b  : 
+        """
+        if B not in self.Beta:
+            # seria mejor mandar una excepcion?
+            print("not in the experimental heating rates")
+            return
+        Beta = list(self.Beta)
+        index = Beta.index(B)
+        column = self.TempIsoDF.columns[index]
+        self.TempIsoDF = self.TempIsoDF.loc[(self.TempIsoDF.index > 0.005) & (self.TempIsoDF.index < 0.995)]
+        self.diffIsoDF = self.diffIsoDF.loc[(self.diffIsoDF.index > 0.005) & (self.diffIsoDF.index < 0.995)]
+        x = self.TempIsoDF[column]
+        y = self.diffIsoDF[column]
+        alpha = self.TempIsoDF.index.values
+        # f_alpha: iterator
+        if f_alpha is None:
+            f_alpha = filter(callable, list(rxn_models.__dict__.values()))
+
+        AVals = []
+        EVals = []
+        def g(xaux,A,E):
+            return A*np.exp(-E/(self.R*xaux))*f(alpha)
+
+        for f in f_alpha:
+            try:   
+                popt, pcov = curve_fit(g, x, y)
+                AVals += [popt[0]]
+                EVals += [popt[1]]
+            except RuntimeError:
+                pass
+
+        LR = linregress(EVals,np.log(AVals))
+        a = LR.slope
+        b = LR.intercept
+        ln_A = (a*E) + b
+        return ln_A, a,b, np.array(AVals), np.array(EVals)
 
-                      T0 : Float. Initial temperature, in Kelvin, for the prediction.
+#---------------------------------------------------------------
+    def reconstruction(self,E, A, col, N=1):
+        """ 
+        Method to numericaly reconstruct the reaction model in its integral expression, $g(\alpha)$ 
+        The reconstructions is computed as $g(\alpha)=\sum_{i}g(alpha_{i})$
 
-                      Tf : Float. Final temperature, in Kelvin, for the prediction.
+        Parameters:     E   :   Activation energy array.
+                        
+                        A   :   Pre-exponential factor array.
 
-        Returns:      a  : numpy array containing the predicted conversion values.
+                        col :   The index for the experimental heating rate, B, assossiated to the temperatures 
+                                to be used for the temperature integral
 
-                      T  : numpy array cppntaining the temperature values corresponding 
-                           to the predicted conversion.
+                        N   :   Data blocks for the numerical integration (see J_time).
 
-                      t  : numpy array cppntaining the time values corresponding to the 
-                           predicted conversion.
+
+        Returns:        g   :   Numerical values (not an analystical function) of the integral reaction model
+                                of the process under study
         """
-        b      = np.exp(self.Fr_b)
-        a_pred = [0]
-        T      = np.linspace(T0,Tf,len(b))
-        t      =  (T-T0)/B
-        dt     =  t[1]-t[0]
-        for i in range(len(b)-1):
-            a = a_pred[i] + b[i]*np.exp(-(E[i]/(self.R*(T0+B*t[i]))))*dt
-            a_pred.append(a)
+        g = []
+        g_tmp = []
+        for i in range(len(E)-N):
+            J   = self.J_time(E[i],i,col,N=N,Beta=self.Beta[col])
+            g_i = A[i]*J
+            g_tmp.append(g_i)
+            g.append(np.sum(np.array(g_tmp)))
+        
+        return np.array(g)
+
+#---------------------------------------------------------------
+    def t_isothermal(self, E, A, T0, col, g_a=None, alpha=None, isoconv=False, N=1):
+        """
+        Method to compute isothermal, model-based or model-free, predictions. 
+        Note that the ActivationEnergy.prediction( method also computes isothermal prediction which may be more accurate.
+
+        Parameters:         E       :   Activation energy array.
+                            
+                            A       :   Pre-exponential factor array.
+
+                            T0      :   Temperature of the system in Kelvin.
+
+                            col     :   The index for the experimental heating rate, B, assossiated to the temperatures 
+                                        to be used for the temperature integral
+
+                            g_a     :   This parameter may be one of two types: The first one is an numpy.array-type object as
+                                        the one obtained with the ActivationEnergy.reconstruction method. The second one is 
+                                        one of the functions defined in rxn_model.py which may be summoned as picnik.rxn_models.MOD,
+                                        where MOD is one of the following codes: A2, A3, A4, D1, D2, D3, F1, P2, P2_3, P3, P4, R2 or R3.
+
+                            alpha   :   Conversion array. 
+                                
+                            isoconv :   Boolean. If True overrides the g_a options and the method computes the time required to reach a 
+                                        given conversion value (from the 'alpha' array) based on the isoconversional principle.
+
+                            N       :   Data blocks for the numerical integration (see J_time).
+
+
+        Returns:            t_p     :   Predicted time required to reach each the conversion values in the 'alpha' array. 
+        """
+        if type(g_a) == np.ndarray:
+            G = interp1d(alpha[:-1:],g_a,fill_value='extrapolate')
+            m = G(alpha)
+            E0=np.mean(E)
+            A0=np.mean(A)
+            n = A0*np.exp(-E0/(self.R*T0))
+            return m/n
+
+        elif type(g_a) == type(rxn_models.A2):
+            m=g_a(alpha,integral=True)
+            E0=np.mean(E)
+            A0=np.mean(A)
+            n = A0*np.exp(-E0/(self.R*T0))
+            return m/n
+
+        else: pass
+        
+        if isoconv == True:
+            t_p = []
+            t_tmp = []
+            for i in range(len(E)-N):
+                J   = self.J_time(E[i],i,col,N=N,Beta=self.Beta[col])
+                t_i = J/(np.exp(-E[i]/(self.R*T0)))
+                t_tmp.append(t_i)
+                tp = np.sum(np.array(t_tmp))
+                t_p.append(tp)
+            return np.array(t_p)
+#---------------------------------------------------------------
+    def export_prediction(self, time, Temp, alpha, name="prediction.csv" ):
+        """
+        Method to export the kinetic prediction.
+
+        Parameters:     time    : Time array.
+
+                        Temp    : Temperature array.
+
+                        alpha   : Conversion array.
+
+                        name    : File name in .csv format.
+
+        Returns:    None. A file will be created according to the working path or path specified in `name`.
+        """
+        predDF = pd.DataFrame({'time':time,
+                               'Temperature':Temp,
+                               'conversion':alpha})
+        predDF.to_csv(name,index=False)
+#---------------------------------------------------------------
+    def export_kinetic_triplet(self, E, ln_A, g_a, name="kinetic_triplet.csv" ):
+        """
+        Method to export the kinetic prediction.
+
+        Parameters:     time    : Activation energy array.
+
+                        Temp    : Natural logarithm of pre-exponential factor array.
+
+                        g_a     : Model reaction array.
+
+                        name    : File name in .csv format.
+
+        Returns:    None. A file will be created according to the working path or path specified in `name`.
+        """
+        kinDF = pd.DataFrame({'E':E,
+                               'ln_A':ln_A,
+                               'g(alpha)':g_a})
+        kinDF.to_csv(name,index=False)
 
-        a_pred      = np.array(a_pred)
-        self.a_pred = a_pred
-       
-        return (self.a_pred, T, t)
```

