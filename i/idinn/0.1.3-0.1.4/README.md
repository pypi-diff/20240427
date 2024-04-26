# Comparing `tmp/idinn-0.1.3.tar.gz` & `tmp/idinn-0.1.4.tar.gz`

## Comparing `idinn-0.1.3.tar` & `idinn-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 idinn-0.1.3/.readthedocs.yaml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 idinn-0.1.3/requirements.txt
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/Makefile
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/conf.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/make.bat
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/requirements.txt
--rw-r--r--   0        0        0   453134 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/_static/optimization_schematic.png
--rw-r--r--   0        0        0   243113 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/_static/youtube.png
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/get_started/get_started.rst
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/get_started/installation.rst
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/joss/paper.bib
--rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/joss/paper.md
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/tutorials/api.rst
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/tutorials/benchmark.rst
--rw-r--r--   0        0        0     6428 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/tutorials/dual.rst
--rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/tutorials/single.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/tutorials/transfer.rst
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/understand/dynamics.rst
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/understand/optimization.rst
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/understand/order.rst
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/understand/straight.rst
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 idinn-0.1.3/src/idinn/__init__.py
--rw-r--r--   0        0        0    23534 2020-02-02 00:00:00.000000 idinn-0.1.3/src/idinn/controller.py
--rw-r--r--   0        0        0    11952 2020-02-02 00:00:00.000000 idinn-0.1.3/src/idinn/sourcing_model.py
--rw-r--r--   0        0        0     4717 2020-02-02 00:00:00.000000 idinn-0.1.3/tests/test_controller.py
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 idinn-0.1.3/tests/test_sourcing_model.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 idinn-0.1.3/.gitignore
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 idinn-0.1.3/LICENSE
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 idinn-0.1.3/README.md
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 idinn-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 idinn-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 idinn-0.1.4/.readthedocs.yaml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 idinn-0.1.4/requirements.txt
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/Makefile
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/conf.py
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/make.bat
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/requirements.txt
+-rw-r--r--   0        0        0   453134 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/_static/optimization_schematic.png
+-rw-r--r--   0        0        0   243113 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/_static/youtube.png
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/get_started/get_started.rst
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/get_started/installation.rst
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/joss/paper.bib
+-rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/joss/paper.md
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/tutorials/api.rst
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/tutorials/benchmark.rst
+-rw-r--r--   0        0        0     6539 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/tutorials/dual.rst
+-rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/tutorials/single.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/tutorials/transfer.rst
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/understand/dynamics.rst
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/understand/optimization.rst
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/understand/order.rst
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 idinn-0.1.4/docs/understand/straight.rst
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 idinn-0.1.4/src/idinn/__init__.py
+-rw-r--r--   0        0        0    23534 2020-02-02 00:00:00.000000 idinn-0.1.4/src/idinn/controller.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 idinn-0.1.4/src/idinn/demand.py
+-rw-r--r--   0        0        0    10273 2020-02-02 00:00:00.000000 idinn-0.1.4/src/idinn/sourcing_model.py
+-rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 idinn-0.1.4/tests/test_controller.py
+-rw-r--r--   0        0        0     7757 2020-02-02 00:00:00.000000 idinn-0.1.4/tests/test_sourcing_model.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 idinn-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 idinn-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 idinn-0.1.4/README.md
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 idinn-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 idinn-0.1.4/PKG-INFO
```

### Comparing `idinn-0.1.3/.readthedocs.yaml` & `idinn-0.1.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `idinn-0.1.3/docs/Makefile` & `idinn-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `idinn-0.1.3/docs/conf.py` & `idinn-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `idinn-0.1.3/docs/index.rst` & `idinn-0.1.4/docs/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ######################################################
 idinn: Inventory-Dynamics Control with Neural Networks
 ######################################################
 
 ..  youtube:: hUBfTWV6tWQ
    :width: 100%
 
-`idinn` implements **i**nventory **d**ynamics–**i**nformed **n**eural **n**etworks for solving single-sourcing and dual-sourcing problems. Neural network controllers and inventory dynamics are implemented into customizable objects with PyTorch backend to enable users to find the optimal neural controllers for the user-specified inventory systems.
+`idinn` implements inventory dynamics–informed neural networks for solving single-sourcing and dual-sourcing problems. Neural network controllers and inventory dynamics are implemented into customizable objects with PyTorch backend to enable users to find the optimal neural controllers for the user-specified inventory systems.
 
 Example Usage
 =============
 
 .. code-block:: python
 
    import torch
@@ -56,11 +56,17 @@
 .. toctree::
    :hidden:
    :maxdepth: 1
    :caption: Tutorials
 
    tutorials/single
    tutorials/dual
+
+.. toctree::
+   :hidden:
+   :maxdepth: 1
+   :caption: References
+
    tutorials/api
```

### Comparing `idinn-0.1.3/docs/make.bat` & `idinn-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `idinn-0.1.3/docs/_static/optimization_schematic.png` & `idinn-0.1.4/docs/_static/optimization_schematic.png`

 * *Files identical despite different names*

### Comparing `idinn-0.1.3/docs/_static/youtube.png` & `idinn-0.1.4/docs/_static/youtube.png`

 * *Files identical despite different names*

### Comparing `idinn-0.1.3/docs/get_started/get_started.rst` & `idinn-0.1.4/docs/get_started/get_started.rst`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
    # Initialize the sourcing model
    sourcing_model = SingleSourcingModel(
       lead_time=0,
       holding_cost=5,
       shortage_cost=495,
       batch_size=32,
       init_inventory=10,
-      demand_distribuion="uniform",
+      demand_distribution="uniform",
       demand_low=1,
       demand_high=4
    )
 
 Afterwards, initialize a controller that is compatible with the chosen sourcing model. In the above single-sourcing example, the relevant controller is :class:`SingleSourcingNeuralController`.
 
 .. code-block:: python
```

### Comparing `idinn-0.1.3/docs/get_started/installation.rst` & `idinn-0.1.4/docs/get_started/installation.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 ************
 Installation
 ************
 
-Install `idinn`
-===============
-
 Requirements
 ============
 
 The basic usage of `idinn` requires a working `Python`_ and `PyTorch`_ installation. If plotting simulation result of a controller is needed, `matplotlib`_ should also be installed. We recommend using the following versions for maximum compability:
 
 * Python_     ``>= 3.8``
 * PyTorch_    ``>= 2.0``
```

### Comparing `idinn-0.1.3/docs/joss/paper.bib` & `idinn-0.1.4/docs/joss/paper.bib`

 * *Files identical despite different names*

### Comparing `idinn-0.1.3/docs/joss/paper.md` & `idinn-0.1.4/docs/joss/paper.md`

 * *Files identical despite different names*

### Comparing `idinn-0.1.3/docs/tutorials/dual.rst` & `idinn-0.1.4/docs/tutorials/dual.rst`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 ==================================================
 
 Dual-sourcing problems are similar to single-sourcing problems but are more intricate. In a dual-sourcing problem, a company has two potential suppliers for a product, each offering varying lead times (the duration for orders to arrive) and order costs (the expense of placing an order). The challenge lies in the company's decision-making process: determining which supplier to engage for each product to minimize costs given stochastic demand. We can solve dual-sourcing problems with `idinn` in a way similar to the approaches describes described in :doc:`/get_started/get_started` and :doc:`/tutorials/single`.
 
 Initialization
 --------------
 
-To address dual-sourcing problems, we employ two main classes: `DualSourcingModel` and `DualSourcingNeuralController`, responsible for setting up the sourcing model and its corresponding controller. In this tutorial, we adopt a dual-sourcing model with specific parameters: regular order lead time and expedited order lead time both set to 0, regular order cost, :math:`c^r`, at 0, expedited order cost, :math:`c^e`, at 20, initial inventory of 6, and a batch size of 256. Additionally, the holding cost, :math:`h`, is 5, while the shortage cost, :math:`s`, is 495. Demand is generated from a uniform distribution with interval :math:`[0, 4]`. Notice that both the `demand_low` and `demand_low` parameter are inclusive (closed bracket). Hence, the generated demand will never exceed 4. In our code, the sourcing model is initialized as follows.
+To address dual-sourcing problems, we employ two main classes: (i) `DualSourcingModel` and (ii) `DualSourcingNeuralController`, responsible for setting up the sourcing model and its corresponding controller. In this tutorial, we examine a dual-sourcing model characterized by the following parameters: the regular order lead time is 2; the expedited order lead time is 0; the regular order cost, :math:`c^r`, is 0; the expedited order cost, :math:`c^e`, is 20; and the initial inventory is 6. Additionally, the holding cost, :math:`h`, and the shortage cost, :math:`b`, are 5 and 495, respectively. Demand is generated from a discrete uniform distribution with interval :math:`[1, 4]`. Notice that both the `demand_low` and `demand_low` parameters are inclusive. In this example, we use a batch size of 256. 
+
+In `idinn`, the sourcing model is initialized as follows.
 
 .. code-block:: python
     
    import torch
    from idinn.sourcing_model import DualSourcingModel
    from idinn.controller import DualSourcingNeuralController
 
@@ -19,45 +21,45 @@
         expedited_lead_time=0,
         regular_order_cost=0,
         expedited_order_cost=20,
         holding_cost=5,
         shortage_cost=495,
         batch_size=256,
         init_inventory=6,
-        demand_distribuion="uniform",
+        demand_distribution="uniform",
         demand_low=1,
         demand_high=4
     )
 
 The cost at period :math:`t`, :math:`c_t`, is
 
 .. math::
 
-   c_t = c^r q^r_t + c^e q^e_t + h \cdot \max(0, I_t) + s \cdot \max(0, - I_t)\,,
+   c_t = c^r q^r_t + c^e q^e_t + h \max(0, I_t) + b \max(0, - I_t)\,,
 
-where :math:`I_t` is the inventory level at period :math:`t`, :math:`q^r_t` is the regular order sent at period :math:`t`, :math:`q^e_t` is the expedited order sent at period :math:`t`. The higher the holding cost, the more costly it is to keep the inventory (when the inventory level is positive). The higher the shortage cost, the more costly it is to run out of stock (when the inventory level is negative). The higher the regular or expedited order costs, the more costly it is to send the respective orders. The cost can be calculated using the `get_cost` method of the sourcing model.
+where :math:`I_t` is the inventory level at the end of period :math:`t`, :math:`q^r_t` is the regular order placed at period :math:`t`, and :math:`q^e_t` is the expedited order placed at period :math:`t`. The higher the holding cost, the more costly it is to keep the inventory (when the inventory level is positive). The higher the shortage cost, the more costly it is to run out of stock (when the inventory level is negative). The higher the regular or expedited order costs, the more costly it is to place the respective orders. The cost can be calculated using the `get_total_cost` method of the sourcing model.
 
 .. code-block:: python
     
-   dual_sourcing_model.get_cost(regular_q=0, expedited_q=0)
+   dual_sourcing_model.get_total_cost(regular_q=0, expedited_q=0)
 
 In our example, this function should return 30 for each sample since the initial inventory is 6, the holding cost is 5, and there is neither a regular nor expedited order. We have 256 samples in this case, as we specified a batch size of 256.
 
-For dual-sourcing problems, we initialize the neural network controller using the `DualSourcingNeuralController` class. In this tutorial, we use a simple neural network with 6 hidden layers and 128, 64, 32, 16, 8, 4 neurons, respectively. The activation function is `torch.nn.CELU(alpha=1)`. The neural network controller is initialized as follows.
+For dual-sourcing problems, we initialize the neural network controller using the `DualSourcingNeuralController` class. In this tutorial, we use a simple neural network with 6 hidden layers. The numbers of neurons in each layer are 128, 64, 32, 16, 8, and 4, respectively. The activation function is `torch.nn.CELU(alpha=1)`. The neural network controller is initialized as follows.
 
 .. code-block:: python
 
     dual_controller = DualSourcingNeuralController(
         hidden_layers=[128, 64, 32, 16, 8, 4], activation=torch.nn.CELU(alpha=1)
     )
 
 Training
 --------
 
-Although the neural network controller has not been trained yet, we can still utilize it to calculate the total cost if we apply this controller for 100 periods alongside our previously specified sourcing model.
+Although the neural network controller has not been trained yet, we can still compute the total cost associated with its order policy. To do so, we integrate it with our previously specified sourcing model and run simulations for 100 periods.
 
 .. code-block:: python
 
     dual_controller.get_total_cost(sourcing_model=dual_sourcing_model, sourcing_periods=100)
 
 Unsurprisingly, the performance is poor because we are only using the untrained neural network in which the weights are just (pseudo) random numbers. We can train the neural network controller using the `train` method, in which the training data is generated from the given sourcing model. To better monitor the training process, we specify the `tensorboard_writer` parameter to log both the training loss and validation loss. For reproducibility, we also specify the seed of the underlying random number generator using the  `seed` parameter.
 
@@ -76,18 +78,18 @@
 
 After training, we can use the trained neural network controller to calculate the total cost for 100 periods with our previously specified sourcing model. The total cost should be significantly lower than the cost associated with the untrained model.
 
 .. code-block:: python
     
     dual_controller.get_total_cost(sourcing_model=dual_sourcing_model, sourcing_periods=100)
 
-Simulation, Plotting and Order Calculation
+Simulation, Plotting, and Order Calculation
 ------------------------------------------
 
-We can also inspect how the controller performs in the specified sourcing environment by (i) plotting the inventory and order histories and (ii) calculating optimal orders.
+We can also inspect how the controller performs in the specified sourcing environment by (i) plotting the inventory and order histories, and (ii) calculating optimal orders.
 
 .. code-block:: python
 
     # Simulate and plot the results
     dual_controller.plot(sourcing_model=dual_sourcing_model, sourcing_periods=100)
     # Calculate the optimal order quantity for applications
     regular_q, expedited_q = dual_controller.forward(
```

### Comparing `idinn-0.1.3/docs/tutorials/single.rst` & `idinn-0.1.4/docs/tutorials/single.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,89 +2,91 @@
 ====================================================
 
 Single-sourcing problems are inventory management problems where only one delivery option exists. The overall objective in single-sourcing and related inventory management problems is for companies to identify the optimal order quantities to minimize costs given stochastic demand. This problem can be addressed using `idinn`. As illustrated in the :doc:`/get_started/get_started` section, we first initialize the sourcing model and its associated neural network controller. Subsequently, we train the neural network controller using data generated from the sourcing model. Finally, we can use the trained neural network controller to compute optimal order quantities.
 
 Initialization
 --------------
 
-Since we deal with the single-sourcing problem, we use the `SingleSourcingModel` class to initialize the sourcing model. In this tutorial, let us pick a single sourcing model which has a lead time of 0, i.e. the order arrives immediately after it is placed, an initial inventory of 10 and a batch size of 32. The holding cost, :math:`h`, is 5 and the shortage cost, :math:`s`, is 495. The demand is generated from a uniform distribution with interval :math:`[0, 4]`. Notice that both the `demand_low` and `demand_low` parameter are inclusive (closed bracket). Hence, the generated demand will never exceed 4. In our code, the sourcing model is initialized as follows.
+Since we deal with the single-sourcing problem, we use the `SingleSourcingModel` class to initialize the sourcing model. In this tutorial, let us pick a single sourcing model which has a lead time of 0 (i.e., the order arrives immediately after it is placed) and an initial inventory of 10. The holding cost, :math:`h`, and the shortage cost, :math:`b`, are 5 and 495, respectively. The demand is generated from a discrete uniform distribution with support :math:`[1, 4]`. Notice that both the `demand_low` and `demand_low` parameters are inclusive. In this example, we use a batch size of 32.
+
+In `idinn`, the sourcing model is initialized as follows.
 
 .. code-block:: python
     
    import torch
    from idinn.sourcing_model import SingleSourcingModel
    from idinn.controller import SingleSourcingNeuralController
 
    single_sourcing_model = SingleSourcingModel(
       lead_time=0,
       holding_cost=5,
       shortage_cost=495,
       batch_size=32,
       init_inventory=10,
-      demand_distribuion="uniform",
+      demand_distribution="uniform",
       demand_low=1,
       demand_high=4
    )
 
 The cost at period :math:`t`, :math:`c_t`, is
 
 .. math::
 
-   c_t = h \cdot \max(0, I_t) + s \cdot \max(0, - I_t)\,,
+   c_t = h \max(0, I_t) + b \max(0, - I_t)\,,
 
-where :math:`I_t` is the inventory level at period :math:`t`. The higher the holding cost, the more costly it is to keep the inventory (when the inventory level is positive). The higher the shortage cost, the more costly it is to run out of stock (when the inventory level is negative). The cost can be calculated using the `get_cost` method of the sourcing model.
+where :math:`I_t` is the inventory level at the end of period :math:`t`. The higher the holding cost, the more costly it is to keep the inventory (when the inventory level is positive). The higher the shortage cost, the more costly it is to run out of stock (when the inventory level is negative). The cost can be calculated using the `get_total_cost` method of the sourcing model.
 
 .. code-block:: python
     
-   single_sourcing_model.get_cost()
+   single_sourcing_model.get_total_cost()
 
 In our example, this function should return 50 for each sample since the initial inventory is 10 and the holding cost is 5. We have 32 samples in this case, as we specified a batch size of 32.
 
 For single-sourcing problems, we initialize the neural network controller using the `SingleSourcingNeuralController` class. In this tutorial, we use a simple neural network with 1 hidden layer and 2 neurons. The activation function is `torch.nn.CELU(alpha=1)`. The neural network controller is initialized as follows.
 
 .. code-block:: python
 
     single_controller = SingleSourcingNeuralController(
         hidden_layers=[2], activation=torch.nn.CELU(alpha=1)
     )
 
 Training
 --------
 
-Although the neural network controller has not been trained yet, we can still utilize it to calculate the total cost if we apply this controller for 100 periods alongside our previously specified sourcing model.
+Although the neural network controller has not been trained yet, we can still compute the total cost associated with its order policy. To do so, we integrate it with our previously specified sourcing model and run simulations for 100 periods.
 
 .. code-block:: python
     
     single_controller.get_total_cost(sourcing_model=single_sourcing_model, sourcing_periods=100)
 
 Unsurprisingly, the performance is poor because we are only using the untrained neural network in which the weights are just (pseudo) random numbers. We can train the neural network controller using the `train` method, in which the training data is generated from the given sourcing model. To better monitor the training process, we specify the `tensorboard_writer` parameter to log both the training loss and validation loss. For reproducibility, we also specify the seed of the underlying random number generator using the `seed` parameter.
 
 .. code-block:: python
 
     from torch.utils.tensorboard import SummaryWriter
 
     single_controller.train(
-        sourcing_model=sourcing_model,
+        sourcing_model=single_sourcing_model,
         sourcing_periods=50,
         validation_sourcing_periods=1000,
         epochs=5000,
         seed=1,
         tensorboard_writer=SummaryWriter()
     )
 
 After training, we can use the trained neural network controller to calculate the total cost for 100 periods with our previously specified sourcing model. The total cost should be significantly lower than the cost associated with the untrained model.
 
 .. code-block:: python
 
     single_controller.get_total_cost(sourcing_model=single_sourcing_model, sourcing_periods=100)
 
-Simulation, Plotting and Order Calculation
+Simulation, Plotting, and Order Calculation
 ------------------------------------------
 
-We can also inspect how the controller performs in the specified sourcing environment by (i) plotting the inventory and order histories and (ii) calculating optimal orders.
+We can also inspect how the controller performs in the specified sourcing environment by (i) plotting the inventory and order histories, and (ii) calculating optimal orders.
 
 .. code-block:: python
 
     # Simulate and plot the results
     single_controller.plot(sourcing_model=single_sourcing_model, sourcing_periods=100)
     # Calculate the optimal order quantity for applications
     single_controller.forward(current_inventory=10, past_orders=[1, 5])
```

### Comparing `idinn-0.1.3/src/idinn/controller.py` & `idinn-0.1.4/src/idinn/controller.py`

 * *Files identical despite different names*

### Comparing `idinn-0.1.3/src/idinn/sourcing_model.py` & `idinn-0.1.4/src/idinn/sourcing_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,37 @@
 import torch
+from .demand import UniformDemand
 
 
 class BaseSourcingModel:
     def __init__(
         self,
         holding_cost,
         shortage_cost,
         init_inventory,
         batch_size,
         lead_time=None,
         regular_lead_time=None,
         expedited_lead_time=None,
         regular_order_cost=None,
         expedited_order_cost=None,
-        demand=None,
-        demand_distribuion="uniform",
-        demand_low=1,
-        demand_high=4,
+        demand_generator=UniformDemand(low=1, high=4),
     ):
         self.holding_cost = holding_cost
         self.shortage_cost = shortage_cost
         self.init_inventory = torch.tensor(
             [init_inventory], requires_grad=True, dtype=torch.float
         )
         self.batch_size = batch_size
         self.lead_time = lead_time
         self.regular_lead_time = regular_lead_time
         self.expedited_lead_time = expedited_lead_time
         self.regular_order_cost = regular_order_cost
         self.expedited_order_cost = expedited_order_cost
-
-        if demand is not None:
-            self.demand_iterator = iter(demand)
-        elif demand_distribuion is not None:
-            if demand_distribuion == "uniform":
-                self.demand_iterator = torch.distributions.Uniform(
-                    low=demand_low, high=demand_high + 1
-                )
-            else:
-                raise ValueError("Only `uniform` distribution is supported.")
-        else:
-            raise ValueError("`demand` or `demand_distribution` must be provided.")
+        self.demand_generator = demand_generator
         self.reset()
 
     def reset(
         self,
         batch_size=None,
     ):
         if batch_size is not None and self.batch_size != batch_size:
@@ -87,48 +74,24 @@
 
     def get_current_inventory(self):
         # Keep dim when slicing past_inventories
         # https://stackoverflow.com/questions/57237352/why-does-torch-slice-lose-dimension
         # https://discuss.pytorch.org/t/solved-simple-question-about-keep-dim-when-slicing-the-tensor/9280
         return self.past_inventories[:, [-1]]
 
-    def generate_demand(self):
-        """
-        Generate demands depending on the type of demand_iterator.
-        """
-        if isinstance(self.demand_iterator, torch.distributions.Uniform):
-            current_demand = self.demand_iterator.sample((self.batch_size, 1)).int()
-        else:
-            try:
-                current_demand = next(self.demand_iterator)
-            except StopIteration:
-                raise ValueError(
-                    "`demand` is not long enough for the overall sourcing periods."
-                )
-            # Ensure demand is a tensor of non-negative integers and the shape conforms to (batch_size,1)
-            if not isinstance(current_demand, torch.Tensor):
-                current_demand = (
-                    torch.tensor(current_demand).int().repeat(self.batch_size, 1)
-                )
-                current_demand = torch.clamp(current_demand, min=0)
-        return current_demand
-
 
 class SingleSourcingModel(BaseSourcingModel):
     def __init__(
         self,
         lead_time,
         holding_cost,
         shortage_cost,
         init_inventory,
         batch_size=1,
-        demand=None,
-        demand_distribuion="uniform",
-        demand_low=1,
-        demand_high=4,
+        demand_generator=UniformDemand(low=1, high=4),
     ):
         """
         Parameters
         ----------
         lead_time : float
             The lead time for orders.
         holding_cost : float
@@ -137,31 +100,28 @@
             The cost of inventory shortage.
         init_inventory : float
             The initial inventory.
         batch_size : int, optional
             The batch size for orders. default is 1.
         demand : Iterable, torch.Tensor, np.array, or pd.Series, optional
             The array for outputting values of demands.
-        demand_distribuion : str, default is `uniform`.
+        demand_distribution : str, default is `uniform`.
             Distribution for generated demands when `demand` is not specified.
         demand_low : int, default is 1.
             Lower inclusive bound for generated demands when `demand` is not specified.
         demand_high : int, default is 4.
             Higher inclusive bound for generated demands when `demand` is not specified.
         """
         super().__init__(
             lead_time=lead_time,
             holding_cost=holding_cost,
             shortage_cost=shortage_cost,
             init_inventory=init_inventory,
             batch_size=batch_size,
-            demand=demand,
-            demand_distribuion=demand_distribuion,
-            demand_low=demand_low,
-            demand_high=demand_high,
+            demand_generator=demand_generator,
         )
 
     def get_lead_time(self):
         return self.lead_time
 
     def get_past_orders(self):
         return self.past_orders
@@ -186,15 +146,15 @@
         if seed is not None:
             torch.manual_seed(seed)
         # Current orders are added to past_orders
         self.past_orders = torch.cat([self.past_orders, q], dim=1)
         # Past orders arrived
         arrived_order = self.past_orders[:, [-1 - self.lead_time]]
         # Generate current demand
-        current_demand = self.generate_demand()
+        current_demand = self.demand_generator.sample(self.batch_size)
         # Update inventory
         current_inventory = (
             self.get_current_inventory() + arrived_order - current_demand
         )
         # Current inventories are added to past_inventories
         self.past_inventories = torch.cat(
             [self.past_inventories, current_inventory], dim=1
@@ -208,18 +168,15 @@
         expedited_lead_time,
         regular_order_cost,
         expedited_order_cost,
         holding_cost,
         shortage_cost,
         init_inventory,
         batch_size=1,
-        demand=None,
-        demand_distribuion="uniform",
-        demand_low=1,
-        demand_high=4,
+        demand_generator=UniformDemand(low=1, high=4),
     ):
         """
         Parameters
         ----------
         regular_lead_time : float
             The lead time for regular orders.
         expedited_lead_time : float
@@ -234,15 +191,15 @@
             The cost of shortage.
         init_inventory : float
             The initial inventory.
         batch_size : int, default is 1
             The batch size for orders.
         demand : Iterable, torch.Tensor, np.array, or pd.Series, optional
             The array for outputting values of demands.
-        demand_distribuion : str, default is `uniform`.
+        demand_distribution : str, default is `uniform`.
             Distribution for generated demand when `demand` is not specified.
         demand_low : int, default is 1.
             Lower bound for generated demand when `demand` is not specified.
         demand_high : int, default is 4.
             Higher bound for generated demand when `demand` is not specified.
         """
         super().__init__(
@@ -250,18 +207,15 @@
             expedited_lead_time=expedited_lead_time,
             regular_order_cost=regular_order_cost,
             expedited_order_cost=expedited_order_cost,
             holding_cost=holding_cost,
             shortage_cost=shortage_cost,
             init_inventory=init_inventory,
             batch_size=batch_size,
-            demand=demand,
-            demand_distribuion=demand_distribuion,
-            demand_low=demand_low,
-            demand_high=demand_high,
+            demand_generator=demand_generator,
         )
 
     def get_past_regular_orders(self):
         return self.past_regular_orders
 
     def get_past_expedited_orders(self):
         return self.past_expedited_orders
@@ -286,15 +240,15 @@
         Orders items to the inventory and update the inventory with generated demands.
 
         Parameters
         ----------
         regular_q : int, or torch.Tensor
             The quantity of items to order from the regular supplier.
         expedited_q : int, or torch.Tensor
-            The quantity of items to order from the expedited supplier.    
+            The quantity of items to order from the expedited supplier.
         seed : int, optional
             Random seed for reproducibility.
         """
         if seed is not None:
             torch.manual_seed(seed)
         if not isinstance(regular_q, torch.Tensor):
             regular_q = torch.tensor([[regular_q]])
@@ -313,15 +267,15 @@
             :, [-1 - self.regular_lead_time]
         ]
         # Past expedited orders arrived
         arrived_expedited_orders = self.past_expedited_orders[
             :, [-1 - self.expedited_lead_time]
         ]
         # Generate current demand
-        current_demand = self.generate_demand()
+        current_demand = self.demand_generator.sample(self.batch_size)
         # Update inventory
         current_inventory = (
             self.get_current_inventory()
             + arrived_expedited_orders
             + arrived_regular_orders
             - current_demand
         )
```

### Comparing `idinn-0.1.3/tests/test_controller.py` & `idinn-0.1.4/tests/test_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,14 @@
 def single_sourcing_model():
     return SingleSourcingModel(
         lead_time=2,
         holding_cost=0.5,
         shortage_cost=1,
         init_inventory=10,
         batch_size=1,
-        demand_distribuion="uniform",
-        demand_low=1,
-        demand_high=4
     )
 
 @pytest.fixture
 def single_sourcing_controller():
     single_sourcing_controller = SingleSourcingNeuralController(
         hidden_layers = [4, 2],
         activation = torch.nn.ReLU()
@@ -59,17 +56,14 @@
         expedited_lead_time=1,
         regular_order_cost=0,
         expedited_order_cost=20,
         holding_cost=0.5,
         shortage_cost=1,
         init_inventory=10,
         batch_size=1,
-        demand_distribuion="uniform",
-        demand_low=1,
-        demand_high=4
     )
 
 @pytest.fixture
 def dual_sourcing_controller():
     dual_sourcing_controller = DualSourcingNeuralController(
         hidden_layers = [4, 2],
         activation = torch.nn.ReLU()
```

### Comparing `idinn-0.1.3/tests/test_sourcing_model.py` & `idinn-0.1.4/tests/test_sourcing_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import torch
 import pytest
 from idinn.sourcing_model import SingleSourcingModel, DualSourcingModel
+from idinn.demand import CustomDemand
 
 
 @pytest.fixture
 def single_sourcing_model():
     """
     Single sourcing model at default state.
     """
@@ -64,82 +65,82 @@
 def test_single_sourcing_model_get_cost(single_sourcing_model: SingleSourcingModel):
     assert torch.all(
         torch.eq(single_sourcing_model.get_cost(), torch.tensor([[5.0], [5.0], [5.0]]))
     )
 
 
 @pytest.fixture
-def single_sourcing_model_fixed_demand():
+def single_sourcing_model_custom_demand():
     """
     Single sourcing model with fixed demand at 1.
     """
     return SingleSourcingModel(
         lead_time=1,
         holding_cost=0.5,
         shortage_cost=1,
         init_inventory=10,
         batch_size=3,
-        demand=[1, 1, 1, 1, 1],
+        demand_generator=CustomDemand([1, 1, 1, 1, 1]),
     )
 
 
 def test_single_sourcing_model_order(
-    single_sourcing_model_fixed_demand: SingleSourcingModel,
+    single_sourcing_model_custom_demand: SingleSourcingModel,
 ):
-    single_sourcing_model_fixed_demand.order(torch.tensor([[1.0], [2.0], [3.0]]))
+    single_sourcing_model_custom_demand.order(torch.tensor([[1.0], [2.0], [3.0]]))
     assert torch.all(
         torch.eq(
-            single_sourcing_model_fixed_demand.get_past_orders(),
+            single_sourcing_model_custom_demand.get_past_orders(),
             torch.cat([torch.zeros(3, 2), torch.tensor([[1.0], [2.0], [3.0]])], dim=1),
         )
     )
     assert torch.all(
         torch.eq(
-            single_sourcing_model_fixed_demand.get_past_inventories(),
+            single_sourcing_model_custom_demand.get_past_inventories(),
             torch.cat(
                 [
                     torch.tensor([10.0]).repeat(3, 2),
                     torch.tensor([[9.0], [9.0], [9.0]]),
                 ],
                 dim=1,
             ),
         )
     )
     assert torch.all(
         torch.eq(
-            single_sourcing_model_fixed_demand.get_current_inventory(),
+            single_sourcing_model_custom_demand.get_current_inventory(),
             torch.tensor([[9.0], [9.0], [9.0]]),
         )
     )
     assert torch.all(
         torch.eq(
-            single_sourcing_model_fixed_demand.get_cost(),
+            single_sourcing_model_custom_demand.get_cost(),
             torch.tensor([[4.5], [4.5], [4.5]]),
         )
     )
 
-    single_sourcing_model_fixed_demand.order(torch.tensor([[1.0], [2.0], [3.0]]))
+    single_sourcing_model_custom_demand.order(torch.tensor([[1.0], [2.0], [3.0]]))
     assert torch.all(
         torch.eq(
-            single_sourcing_model_fixed_demand.get_past_orders(),
+            single_sourcing_model_custom_demand.get_past_orders(),
             torch.cat(
                 [torch.zeros(3, 2), torch.tensor([[1.0, 1.0], [2.0, 2.0], [3.0, 3.0]])],
                 dim=1,
             ),
         )
     )
     assert torch.all(
         torch.eq(
-            single_sourcing_model_fixed_demand.get_current_inventory(),
+            single_sourcing_model_custom_demand.get_current_inventory(),
             torch.tensor([[9.0], [10.0], [11.0]]),
         )
     )
     assert torch.all(
         torch.eq(
-            single_sourcing_model_fixed_demand.get_cost(),
+            single_sourcing_model_custom_demand.get_cost(),
             torch.tensor([[4.5], [5.0], [5.5]]),
         )
     )
 
 
 @pytest.fixture
 def dual_sourcing_model():
@@ -219,67 +220,67 @@
         torch.eq(
             dual_sourcing_model.get_cost(0, 0), torch.tensor([[5.0], [5.0], [5.0]])
         )
     )
 
 
 @pytest.fixture
-def dual_sourcing_model_fixed_demand():
+def dual_sourcing_model_custom_demand():
     """
     Dual sourcing model with fixed demand at 1.
     """
     return DualSourcingModel(
         regular_lead_time=1,
         expedited_lead_time=0,
         regular_order_cost=0,
         expedited_order_cost=20,
         holding_cost=0.5,
         shortage_cost=1,
         init_inventory=10,
         batch_size=3,
-        demand=[1, 1, 1, 1, 1],
+        demand_generator=CustomDemand([1, 1, 1, 1, 1]),
     )
 
 
 def test_dual_sourcing_model_order(
-    dual_sourcing_model_fixed_demand: DualSourcingModel,
+    dual_sourcing_model_custom_demand: DualSourcingModel,
 ):
-    dual_sourcing_model_fixed_demand.order(
+    dual_sourcing_model_custom_demand.order(
         regular_q=torch.tensor([[1.0], [2.0], [3.0]]),
         expedited_q=torch.tensor([[4.0], [5.0], [6.0]]),
     )
     assert torch.all(
         torch.eq(
-            dual_sourcing_model_fixed_demand.get_past_regular_orders(),
+            dual_sourcing_model_custom_demand.get_past_regular_orders(),
             torch.cat([torch.zeros(3, 2), torch.tensor([[1.0], [2.0], [3.0]])], dim=1),
         )
     )
     assert torch.all(
         torch.eq(
-            dual_sourcing_model_fixed_demand.get_past_expedited_orders(),
+            dual_sourcing_model_custom_demand.get_past_expedited_orders(),
             torch.cat([torch.zeros(3, 2), torch.tensor([[4.0], [5.0], [6.0]])], dim=1),
         )
     )
     assert torch.all(
         torch.eq(
-            dual_sourcing_model_fixed_demand.get_past_inventories(),
+            dual_sourcing_model_custom_demand.get_past_inventories(),
             torch.cat(
                 [
                     torch.tensor([10.0]).repeat(3, 2),
                     torch.tensor([[13.0], [14.0], [15.0]]),
                 ],
                 dim=1,
             ),
         )
     )
     assert torch.all(
         torch.eq(
-            dual_sourcing_model_fixed_demand.get_current_inventory(),
+            dual_sourcing_model_custom_demand.get_current_inventory(),
             torch.tensor([[13.0], [14.0], [15.0]]),
         )
     )
     assert torch.all(
         torch.eq(
-            dual_sourcing_model_fixed_demand.get_cost(regular_q=0, expedited_q=1),
+            dual_sourcing_model_custom_demand.get_cost(regular_q=0, expedited_q=1),
             torch.tensor([[26.5], [27.0], [27.5]]),
         )
     )
```

### Comparing `idinn-0.1.3/.gitignore` & `idinn-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `idinn-0.1.3/LICENSE` & `idinn-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `idinn-0.1.3/README.md` & `idinn-0.1.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 # Initialize the sourcing model and the neural controller
 sourcing_model = SingleSourcingModel(
     lead_time=0,
     holding_cost=5,
     shortage_cost=495,
     batch_size=32,
     init_inventory=10,
-    demand_distribuion="uniform",
+    demand_distribution="uniform",
     demand_low=1,
     demand_high=4
 )
 controller = SingleFullyConnectedNeuralController(
     hidden_layers=[2],
     activation=torch.nn.CELU(alpha=1)
 )
```

### Comparing `idinn-0.1.3/pyproject.toml` & `idinn-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -15,17 +15,14 @@
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 dependencies = ["numpy", "matplotlib", "torch>=2.0"]
 dynamic = ["version"]
 
-[project.optional-dependencies]
-dynamic-programming = ["numba"]
-
 [project.urls]
 Homepage = "https://gitlab.com/ComputationalScience/idinn"
 Documentation = "https://inventory-optimization.readthedocs.io"
 Issues = "https://gitlab.com/ComputationalScience/idinn/-/issues"
 
 [build-system]
 requires = ["hatchling"]
```

### Comparing `idinn-0.1.3/PKG-INFO` & `idinn-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: idinn
-Version: 0.1.3
+Version: 0.1.4
 Summary: Inventory dynamics–informed neural networks for solving single-sourcing and dual-sourcing problems.
 Project-URL: Homepage, https://gitlab.com/ComputationalScience/idinn
 Project-URL: Documentation, https://inventory-optimization.readthedocs.io
 Project-URL: Issues, https://gitlab.com/ComputationalScience/idinn/-/issues
 Author-email: Jiawei Li <sud.concept0x@icloud.com>, Thomas Asikis <thomas.asikis@uzh.ch>, Ioannis Fragkos <fragkos@rsm.nl>, Lucas Boettcher <l.boettcher@fs.de>
 License: MIT License
         
@@ -32,16 +32,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: torch>=2.0
-Provides-Extra: dynamic-programming
-Requires-Dist: numba; extra == 'dynamic-programming'
 Description-Content-Type: text/markdown
 
 # idinn: Inventory-Dynamics Control with Neural Networks
 
 [<img src="https://gitlab.com/ComputationalScience/idinn/-/raw/main/docs/_static/youtube.png" align="center" width="60%" size="auto" alt="youtube">](https://www.youtube.com/watch?v=hUBfTWV6tWQ)
 
 `idinn` implements **i**nventory **d**ynamics–**i**nformed **n**eural **n**etworks for solving single-sourcing and dual-sourcing problems. Neural network controllers and inventory dynamics are implemented into customizable objects with PyTorch backend to enable users to find the optimal neural controllers for the user-specified inventory systems.
@@ -72,15 +70,15 @@
 # Initialize the sourcing model and the neural controller
 sourcing_model = SingleSourcingModel(
     lead_time=0,
     holding_cost=5,
     shortage_cost=495,
     batch_size=32,
     init_inventory=10,
-    demand_distribuion="uniform",
+    demand_distribution="uniform",
     demand_low=1,
     demand_high=4
 )
 controller = SingleFullyConnectedNeuralController(
     hidden_layers=[2],
     activation=torch.nn.CELU(alpha=1)
 )
```

