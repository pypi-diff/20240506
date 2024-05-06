# Comparing `tmp/optihood-0.0.0.tar.gz` & `tmp/optihood-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optihood-0.0.0.tar", last modified: Thu May  2 13:13:42 2024, max compression
+gzip compressed data, was "optihood-0.0.1.tar", last modified: Mon May  6 13:58:42 2024, max compression
```

## Comparing `optihood-0.0.0.tar` & `optihood-0.0.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 13:13:42.328322 optihood-0.0.0/
--rw-rw-rw-   0        0        0    22157 2024-05-02 13:13:42.327320 optihood-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    18865 2024-03-14 07:57:37.000000 optihood-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 13:13:42.292330 optihood-0.0.0/optihood/
--rw-rw-rw-   0        0        0        0 2023-11-08 10:47:08.000000 optihood-0.0.0/optihood/__init__.py
--rw-rw-rw-   0        0        0    39587 2024-03-08 12:54:46.000000 optihood-0.0.0/optihood/buildings.py
--rw-rw-rw-   0        0        0     5183 2023-11-08 10:47:08.000000 optihood-0.0.0/optihood/combined_prod.py
--rw-rw-rw-   0        0        0    10793 2024-03-08 12:46:51.000000 optihood-0.0.0/optihood/constraints.py
--rw-rw-rw-   0        0        0    30677 2024-03-08 12:31:48.000000 optihood-0.0.0/optihood/converters.py
--rw-rw-rw-   0        0        0    84574 2024-03-20 12:27:13.000000 optihood-0.0.0/optihood/energy_network.py
--rw-rw-rw-   0        0        0    29364 2023-11-08 10:47:08.000000 optihood-0.0.0/optihood/labelDict.py
--rw-rw-rw-   0        0        0     2007 2023-11-08 10:47:08.000000 optihood-0.0.0/optihood/links.py
--rw-rw-rw-   0        0        0    62970 2023-11-08 10:47:08.000000 optihood-0.0.0/optihood/plot_functions.py
--rw-rw-rw-   0        0        0    13127 2023-11-08 10:47:08.000000 optihood-0.0.0/optihood/plot_sankey.py
--rw-rw-rw-   0        0        0    12745 2023-11-08 10:47:08.000000 optihood-0.0.0/optihood/sinks.py
--rw-rw-rw-   0        0        0     4160 2023-11-08 10:47:08.000000 optihood-0.0.0/optihood/sources.py
--rw-rw-rw-   0        0        0     4532 2023-11-08 10:47:08.000000 optihood-0.0.0/optihood/storages.py
-drwxrwxrwx   0        0        0        0 2024-05-02 13:13:42.325320 optihood-0.0.0/optihood.egg-info/
--rw-rw-rw-   0        0        0    22157 2024-05-02 13:13:41.000000 optihood-0.0.0/optihood.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      470 2024-05-02 13:13:42.000000 optihood-0.0.0/optihood.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 13:13:41.000000 optihood-0.0.0/optihood.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      136 2024-05-02 13:13:41.000000 optihood-0.0.0/optihood.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-02 13:13:41.000000 optihood-0.0.0/optihood.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 13:13:42.328322 optihood-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      985 2024-05-02 12:31:36.000000 optihood-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:58:42.592208 optihood-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-06 13:58:29.000000 optihood-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19021 2024-05-06 13:58:42.592208 optihood-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18517 2024-05-06 13:58:29.000000 optihood-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:58:42.592208 optihood-0.0.1/optihood/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:58:29.000000 optihood-0.0.1/optihood/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38937 2024-05-06 13:58:29.000000 optihood-0.0.1/optihood/buildings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-06 13:58:29.000000 optihood-0.0.1/optihood/combined_prod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10542 2024-05-06 13:58:29.000000 optihood-0.0.1/optihood/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30062 2024-05-06 13:58:29.000000 optihood-0.0.1/optihood/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83359 2024-05-06 13:58:29.000000 optihood-0.0.1/optihood/energy_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28731 2024-05-06 13:58:29.000000 optihood-0.0.1/optihood/labelDict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-06 13:58:29.000000 optihood-0.0.1/optihood/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61778 2024-05-06 13:58:29.000000 optihood-0.0.1/optihood/plot_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-05-06 13:58:29.000000 optihood-0.0.1/optihood/plot_sankey.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12458 2024-05-06 13:58:29.000000 optihood-0.0.1/optihood/sinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-06 13:58:29.000000 optihood-0.0.1/optihood/sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-05-06 13:58:29.000000 optihood-0.0.1/optihood/storages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:58:42.592208 optihood-0.0.1/optihood.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19021 2024-05-06 13:58:42.000000 optihood-0.0.1/optihood.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-06 13:58:42.000000 optihood-0.0.1/optihood.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 13:58:42.000000 optihood-0.0.1/optihood.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-06 13:58:42.000000 optihood-0.0.1/optihood.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 13:58:42.000000 optihood-0.0.1/optihood.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 13:58:42.592208 optihood-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-06 13:58:29.000000 optihood-0.0.1/setup.py
```

### Comparing `optihood-0.0.0/PKG-INFO` & `optihood-0.0.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,363 +1,366 @@
-Metadata-Version: 2.1
-Name: optihood
-Version: 0.0.0
-Summary: optihood optimization framework
-Home-page: https://optihood.readthedocs.io
-Author: Institute for Solar Technology (SPF), OST Rapperswil
-Author-email: neha.dimri@ost.ch
-License: UNKNOWN
-Description: # optihood: energy modelling and optimization framework
-        
-        optihood provides a complete python-based framework to **OPTI**mize the investment in alternative energy
-        technologies (heat pump, solar thermal, PV, etc.) as well as the operation of available energy resources (natural gas,
-        sun, grid electricity, etc.) for decentralized energy networks on a neighbour**HOOD**-scale. It is designed to facilitate 
-        the researchers and energy planners in optimizing an energy neighbourhood in terms of cost and/or environmental criteria. 
-        It enables the users to perform both single-objective and multi-objective optimization and analysis. The energy model and 
-        it's associated parameters can be defined easily using an excel file. Additionally, a variety of plotting methods are 
-        defined for easy and fast result visualization.
-        
-        ## Documentation
-        The documentation can be found on https://optihood.readthedocs.io/.
-        
-        ## Prerequisites
-        In order to use optihood, the following prerequisites are needed on your machine:
-        
-        - [Python 3.9](https://www.python.org/downloads/) is installed.
-        - Git is installed
-        - An active [Github](https://github.com/) account to clone the repo.
-        - A solver is installed. [Gurobi solver](https://www.gurobi.com/resource/parallelism-linear-mixed-integer-programming/)
-        is recommended, although other solvers like CBC, GLPK, Cplex could also be used.
-        
-        ## Installation
-        
-        As of now, optihood is available as an open source code and needs to be installed from source. Please follow the
-        instructions mentioned below to complete the installation. The commands given below are suited for the Windows platform
-        and should be run from within the optihood directory in a Command Prompt. For other platforms, similar alternative
-        commands could be used.
-        
-        1. Clone the optihood repo to a folder called 'optihood' on your local machine:
-            ```commandline
-            git clone https://github.com/SPF-OST/OptiHood.git
-            ```
-        2. All the next commands should be run from within the optihood folder. Create a virtual environment and activate it:
-            ```commandline
-            py -3.9 -m venv venv
-            venv\Scripts\activate
-            ```    
-        3. Install the requirements into the created virtual environment:
-            ```commandline
-            pip install wheel
-            pip install -r requirements.txt
-            ```
-        
-        
-            It might be required to install C++ build tools. To do that, click on the link that appears with the error message and follow the instructions (it is the lapack package that is missing). In order to be able to 
-            install the missing package, it is required to have a complete Visual Studio instance and installing it with the "Desktop development with C++" workload.
-           
-        4.  Verify the installation of the oemof package and the solver by running the installation test in your virtual environment:
-            ```commandline
-            oemof_installation_test
-            ```
-        
-            
-            If the installation is successful a message similar to the following would display (the installed solver would be marked as working):
-            ```commandline
-            *****************************
-            Solver installed with oemof
-            cbc: not working
-            glpk: not working
-            gurobi: working
-            cplex: not working
-            
-            *****************************
-            oemof successfully installed.
-            *****************************
-            ```
-        5.  To test whether the installation worked well, you could run a [basic example](https://github.com/SPF-OST/OptiHood/tree/main/data/examples/).
-        
-        ## Defining an energy network
-        
-        Optihood offers a several functionalities to define an energy network, optimize it and visualize the results, which
-        provides the user with a complete framework for optimization without the need to code by hand. 
-        
-        An energy network can be defined as an object of the EnergyNetworkIndiv class or the EnergyNetworkGroup class. This
-        object then acts as the primary container for the model. The EnergyNetworkClass is the main parent class, from which 
-        two child classes EnergyNetworkIndiv and EnergyNetworkGroup are inherited. Either EnergyNetworkIndiv class or 
-        EnergyNetworkGroup class could be used to define an energy network. The choice mainly depends on whether the buildings 
-        are linked together (electrically and/or thermally) or not.
-        
-        If the buildings within an energy network do not share electricity and/or heat, EnergyNetworkIndiv class is used:
-        
-            import EnergyNetworkIndiv
-            network = EnergyNetworkIndiv(dateTimeIndex, tSH=35, tDHW=55)
-            
-        Otherwise, if the buildings are expected to share energy (electrical and/or heat), EnergyNetworkGroup class is used:
-        
-            import EnergyNetworkGroup
-            network = EnergyNetworkGroup(dateTimeIndex, tSH=35, tDHW=55)
-            
-        The first parameter to be passed in both the cases is a Datetime index. This parameter gives the time range for an
-        optimization model. The Datetime index could be defined using date_range() in pandas:
-        
-            import pandas as pd
-            dateTimeIndex = pd.date_range('2021-01-01 00:00:00', '2021-12-31 23:00:00', freq="60min")
-            
-        The second and the third parameters tSH and tDHW define the temperatures for space heating and domestic hot water
-        production, respectively.
-        
-        Once the 'network' object has been created, the next step then is to build the model from an input excel file which
-        defines different components which constitute the model, how they are connected and their associated parameters:
-        
-            network.setFromExcel(inputExcelFilePath, numberOfBuildings, clusterSize, opt)
-            
-        'inputExcelFilePath' gives the path of the excel input file. 'numberofBuildings' is an integer parameter specifying the
-        number of buildings defined in the excel file. The last two parameters clusterSize and opt are optional. The 'opt'
-        parameter could be either 'costs' (default value) or 'env' depending on which criteria should be optimized. The
-        'clusterSize' parameter is used to provide a selected number of days which could be assumed representative of the entire
-        time range. For example: two typical days could be selected to model the entire year, which could represent two clusters
-        summer and winter. This would improve the optimization speed. If not given during the function call, the default value
-        of the clusterSize parameter assumes no day clusters.
-        
-        ## Input Excel File
-        
-        The input excel file is used to define an optimization model and set the model parameters. Each sheet of this excel file
-        is structured to defin different components, such as buses, storages and transformers, their respective parameters,
-        connections between these components and the building to which they belong.
-        
-        The input excel file typically has 9-10 sheets, each defining a different component type of the model.
-        
-        ### buses
-        This excel sheet defines the buses used in the energy network. Buses define the connections between different
-        components. Each row of this excel sheet represents a bus node in the model.
-        
-        - **label** (string):
-            label name of the bus. Should be unique for each building i.e. different buildings could have the same label for two
-            buses but for one building the buses should not have duplicate labels.
-        
-        - **active** (0 or 1):
-            If set to 1 then the corresponding bus is active, otherwise (if 0) then the bus is inactive in the model. Could be
-            used to optimize different scenarios with different buses without the need to re-construct the base excel file.
-        
-        - **excess** (0 or 1):
-            If set to 1 then the corresponding bus has the possibility of having an excess flow unbalanced to the demand. An
-            additional sink node is automatically added in this case to accept this excess flow. If set to 0 then the bus cannot
-            have an excess flow.
-        
-        - **excess costs** (float):
-            The associated cost of excess flow from a bus. Relevant only if **excess** is set to 1. Could be negative to denote
-            monetary gains such as in case of PV feed-in.
-        
-        - **building** (integer):
-            Building number to which the bus belongs. Should be unique for each building.
-        
-        ### commodity_sources
-        This sheet defines the different commodity sources which serve as an energy input to the model. The parameters **label**,
-        **active** and **building** are analogous to the parameters described earlier for buses.
-        
-        - **to** (string):
-            Label of bus to which the energy from the commodity source flows. The corresponding bus label should exist in
-            the buses sheet.
-        
-        - **variable costs** (float):
-            Cost per kW of the commodity source.
-        
-        - **CO2 impact** (float):
-            CO2 impact per kW of the commodity source.
-        
-        ### demand
-        The nodes related to the energy demand i.e. sink are defined in this sheet. The parameters **label**, **active** and
-        **building** are analogous to the parameters described earlier for buses.
-        
-        - **from** (string):
-            Label of the bus from which the energy flows to the demand node. The corresponding bus label should exist in
-            the buses sheet.
-        
-        - **fixed** (0 or 1):
-            If set to 1, the energy demand profiles are fixed and a path to the demand profiles should then be given in the
-            csv_data sheet of the input excel file. If set to 0, the optimizer will select the demand profiles for optimum
-            operation (a total annual demand profile could be given in this case). At the present development stage only fixed
-            demands are accepted.
-        
-        - **nominal value** (float):
-            The demand profiles series should be normalized values. this parameter then defines the maximum demand with which
-            the normalized series is multiplied to obtain the actual demand profile series. If set to 1, then the given demand
-            profile series is taken as it is (not normalized).
-        
-        ### transformers
-        The nodes related to the energy conversion units (or transformers) such as CHP, heat pump, etc. are given in this excel
-        sheet. The parameters **label**, **active** and **building** are analogous to the parameters described earlier for buses.
-        
-        - **from** (string):
-            Label of bus from which the energy flows to the transformer node. The corresponding bus label should exist in
-            the buses sheet.
-        
-        - **to** (strings separated by comma):
-            Label of the bus(es) to which the energy flows from the transformer node. Different bus labels should be separated
-            by a comma (,), for example: Bus1, Bus2, Bus3. The bus label(s) should exist in the buses sheet.
-        
-        - **efficiency** (float values separated by comma):
-            Conversion efficiency from input to the output(s) of the transformer node. Efficiencies should be separated by
-            a comma (,) in the case with more than one outputs (i.e. when more than one buses are listed under **to**).
-        
-        - **capacity_DHW** (float):
-            Maximum capacity limit for domestic hot water (DHW) production from the transformer unit in kW. Could be left blank
-            if the parameter is not relevant to a transformer (for example if a transformer does not produce DHW)
-        
-        - **capacity_SH** (float):
-            Maximum capacity limit for space heat (SH) production from the transformer unit in kW. Could be left blank if the
-            parameter is not relevant to a transformer (for example if a transformer does not produce SH)
-        
-        - **capacity_el** (float):
-            Maximum capacity limit for electricity production from the transformer unit in kW. Could be left blank if the
-            parameter is not relevant to a transformer (for example if a transformer does not produce electricity). Note for CHP
-            this parameter acts as the main capacity against which optimization is performed.
-        
-        - **capacity_min** (float):
-            Minimum capacity to be installed in kW for an investment in the transformer unit.
-        
-        - **lifetime** (non-negative integer):
-            Lifetime of the node in years.
-        
-        - **invest_base** (float):
-            Base investment cost of the node.
-        
-        - **invest_cap** (float):
-            Investment cost per unit installed capacity (i.e. per kW) of the node.
-        
-        - **maintenance** (float):
-            Maintenance cost of the node. Given as a percentage of the base investment cost **invest_base**. For example:
-            if the investment cost is to be taken as 5% of **invest_base**, then the value of **maintenance** field should be 0.05.
-            Set as 0 if this cost is to be ignored.
-        
-        - **installation** (float):
-            Installation cost of the node. Given as a percentage of the base investment cost **invest_base**. For example:
-            if the Installation cost is to be taken as 15% of **invest_base**, then **installation** field should be 0.15. Set
-            as 0 if this cost is to be ignored.
-        
-        - **planification** (float):
-            Cost associated with planning. Given as a percentage of the base investment cost **invest_base**. For example:
-            if the planning cost is 5% of **invest_base**, then **planification** should be 0.05. Set as 0 if this cost is to be
-            ignored.
-        
-        - **heat_impact** (float):
-            Environmental impact for heat production. Set as 0 if there is no impact due to heat production.
-        
-        - **elec_impact** (float):
-            Environmental impact for electricity production. Set as 0 if there is no impact due to electricity production.
-        
-        - **impact_cap** (float):
-            Environmental impact per unit installed capacity i.e. per kW of the node. Set as 0 if there is no impact per
-            installed capacity of the node.
-        
-        ### solar
-        This excel sheet defines the parameters related to the solar components such as solar thermal collector and PV panels.
-        The parameters **label**, **active** and **building** are analogous to the parameters described earlier for buses.
-        **from** and **to** parameters have been previously defined for commodity sources and demand sheets, respectively, while
-        the cost and environmental impact paramaters are described under transformers sheet.
-        
-        - **connect** (string):
-            Label of the bus which connects a solar collector to the model. This bus allows excess heat production from the solar
-            collector. A node for heat sink is created automatically. The given bus label should exist in the buses sheet. This
-            parameter is irrelevant for PV.
-        
-        - **electrical_consumption** (float):
-            Electrical consumption of the solar component. Given as a percentage fraction of the energy produced. 0.02 means
-            the electrical consumption is 2% of the energy is produced.
-        
-        - **peripheral_losses** (float):
-            Peripheral losses of the solar component. Given as a percentage fraction of the energy produced. 0.05 means 5% of
-            the energy produced is lost to the surrounding environment.
-        
-        - **latitude** (float):
-            Latitude of the geographical location where the solar collector/panel is placed. Given in degrees.
-        
-        - **longitude** (float):
-            Longitude of the geographical location where the solar collector/panel is placed. Given in degrees.
-        
-        - **tilt** (float):
-            Tilt angle of the solar collector/panel. Given in degrees.
-        
-        - **azimuth** (float):
-            Azimuth angle of the solar collector/panel. Given in degrees.
-        
-        - **eta_0**, **a_1** and **a_2** (float):
-            Efficiency parameters of the solar thermal collector. Solar thermal collector is linearized using the pre-calculations
-            given in [oemof-thermal](https://oemof-thermal.readthedocs.io/en/latest/solar_thermal_collector.html).
-        
-        - **temp_collector_inlet** (float):
-            Inlet fluid temperature of the solar thermal collector. Given in degree C.
-        
-        - **delta_temp_n** (float):
-            Temperature difference between the inlet fluid and the mean fluid temperature in case of solar collector. For PV,
-            this parameter denotes the temperature difference between the solar cells and the ambient.
-        
-        - **capacity_max** (float):
-            Maximum capacity limit in kW.
-        
-        - **capacity_min** (float):
-            Minimum possible capacity in kW for the installation of solar collector/panel.
-        
-        ### storages
-        This excel sheet defines the parameters related to the energy storage units such as battery and hot water tank. **label**,
-        **active** and **building** have been defined previously for buses excel sheet. A description of **from** and **to** has
-        been given in commodity sources and demand sheets, respectively. The cost and environmental impact parameters are
-        described in the transformers sheet section. **capacity_min** and **capacity_max** are described in the solar excel sheet
-        section.
-        
-        - **efficiency inflow** (float):
-            Charging efficiency of battery. This parameter is not relevant for thermal storages.
-        
-        - **efficiency outflow** (float):
-            Discharging efficiency of battery. This parameter is not relevant for thermal storages.
-        
-        - **initial capacity** (float):
-            initial capacity of the storage. This parameter is expressed as a fraction of the total storage capacity. 0 means storage is initially 
-            assumed to be empty, 1 denotes that the storage is 100% full initially, while 0.5 means the storage is at 50% capacity initially.
-        
-        - **capacity loss** (float):
-            Losses from battery storage. This parameter is not relevant for thermal storages.
-        
-        ### stratified_storage
-        This excel sheet defines the parameters relevant to stratified thermal storage. The pre-calculations given in [oemof-thermal](https://oemof-thermal.readthedocs.io/en/latest/stratified_thermal_storage.html)
-        have been used to linearize the thermal hot water storage. The parameter names used here are similar to the parameters
-        defined in oemof-thermal.
-        
-        ### links
-        This excel sheet defines the parameters for electricity and space heating links. The buildings could share electricity
-        production and/or space heat production. Links allow this sharing to be possible. **label** and **active** have been
-        defined already for buses excel sheet. **invest_base** and **invest_cap** parameters (defined in the transformers sheet
-        section) are only relevant for space heating links in the present stage of development.
-        
-        - **buildingA** (integer):
-            Building number of the first building of the link. This should match with the values typically given in the
-            **building** parameter in the other excel sheets.
-        
-        - **buildingB** (integer):
-            Building number of the second building of the link. This should match with the values typically given in the
-            **building** parameter in the other excel sheets.
-        
-        - **efficiency from A to B** (integer):
-            Efficiency of energy transfer over the link from **buildingA** to **buildingB**.
-        
-        - **efficiency from B to A** (integer):
-            Efficiency of energy transfer over the link from **buildingB** to **buildingA**.
-        
-        ### csv_data
-        The paths to CSV files containing demand profiles, weather data and electricity impact data are to be given in this
-        excel sheet. **INFO** gives further information about each row.
-        
-        ### grid_connection
-        This excel sheet should not be modified by the users. It defines the separation of the flows from electricity grid and
-        the produced electricity flows to make sure that the grid electricity is not stored in batteries.
-        
-        
-        ## Collaborators
-        
-        SPF/OST & HEIG-VD
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: ==3.9
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: optihood
+Version: 0.0.1
+Summary: optihood optimization framework
+Home-page: https://optihood.readthedocs.io
+Author: Institute for Solar Technology (SPF), OST Rapperswil
+Author-email: neha.dimri@ost.ch
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# optihood: energy modelling and optimization framework
+
+optihood provides a complete python-based framework to **OPTI**mize the investment in alternative energy
+technologies (heat pump, solar thermal, PV, etc.) as well as the operation of available energy resources (natural gas,
+sun, grid electricity, etc.) for decentralized energy networks on a neighbour**HOOD**-scale. It is designed to facilitate 
+the researchers and energy planners in optimizing an energy neighbourhood in terms of cost and/or environmental criteria. 
+It enables the users to perform both single-objective and multi-objective optimization and analysis. The energy model and 
+it's associated parameters can be defined easily using an excel file. Additionally, a variety of plotting methods are 
+defined for easy and fast result visualization.
+
+## Documentation
+The documentation can be found on https://optihood.readthedocs.io/.
+
+## Prerequisites
+In order to use optihood, the following prerequisites are needed on your machine:
+
+- [Python 3.9](https://www.python.org/downloads/) is installed.
+- Git is installed
+- An active [Github](https://github.com/) account to clone the repo.
+- A solver is installed. [Gurobi solver](https://www.gurobi.com/resource/parallelism-linear-mixed-integer-programming/)
+is recommended, although other solvers like CBC, GLPK, Cplex could also be used.
+
+## Installation
+
+As of now, optihood is available as an open source code and needs to be installed from source. Please follow the
+instructions mentioned below to complete the installation. The commands given below are suited for the Windows platform
+and should be run from within the optihood directory in a Command Prompt. For other platforms, similar alternative
+commands could be used.
+
+1. Clone the optihood repo to a folder called 'optihood' on your local machine:
+    ```commandline
+    git clone https://github.com/SPF-OST/OptiHood.git
+    ```
+2. All the next commands should be run from within the optihood folder. Create a virtual environment and activate it:
+    ```commandline
+    py -3.9 -m venv venv
+    venv\Scripts\activate
+    ```    
+3. Install the requirements into the created virtual environment:
+    ```commandline
+    pip install wheel
+    pip install -r requirements.txt
+    ```
+
+
+    It might be required to install C++ build tools. To do that, click on the link that appears with the error message and follow the instructions (it is the lapack package that is missing). In order to be able to 
+    install the missing package, it is required to have a complete Visual Studio instance and installing it with the "Desktop development with C++" workload.
+   
+4.  Verify the installation of the oemof package and the solver by running the installation test in your virtual environment:
+    ```commandline
+    oemof_installation_test
+    ```
+
+    
+    If the installation is successful a message similar to the following would display (the installed solver would be marked as working):
+    ```commandline
+    *****************************
+    Solver installed with oemof
+    cbc: not working
+    glpk: not working
+    gurobi: working
+    cplex: not working
+    
+    *****************************
+    oemof successfully installed.
+    *****************************
+    ```
+5.  To test whether the installation worked well, you could run a [basic example](https://github.com/SPF-OST/OptiHood/tree/main/data/examples/).
+
+## Defining an energy network
+
+Optihood offers a several functionalities to define an energy network, optimize it and visualize the results, which
+provides the user with a complete framework for optimization without the need to code by hand. 
+
+An energy network can be defined as an object of the EnergyNetworkIndiv class or the EnergyNetworkGroup class. This
+object then acts as the primary container for the model. The EnergyNetworkClass is the main parent class, from which 
+two child classes EnergyNetworkIndiv and EnergyNetworkGroup are inherited. Either EnergyNetworkIndiv class or 
+EnergyNetworkGroup class could be used to define an energy network. The choice mainly depends on whether the buildings 
+are linked together (electrically and/or thermally) or not.
+
+If the buildings within an energy network do not share electricity and/or heat, EnergyNetworkIndiv class is used:
+
+    import EnergyNetworkIndiv
+    network = EnergyNetworkIndiv(dateTimeIndex, tSH=35, tDHW=55)
+    
+Otherwise, if the buildings are expected to share energy (electrical and/or heat), EnergyNetworkGroup class is used:
+
+    import EnergyNetworkGroup
+    network = EnergyNetworkGroup(dateTimeIndex, tSH=35, tDHW=55)
+    
+The first parameter to be passed in both the cases is a Datetime index. This parameter gives the time range for an
+optimization model. The Datetime index could be defined using date_range() in pandas:
+
+    import pandas as pd
+    dateTimeIndex = pd.date_range('2021-01-01 00:00:00', '2021-12-31 23:00:00', freq="60min")
+    
+The second and the third parameters tSH and tDHW define the temperatures for space heating and domestic hot water
+production, respectively.
+
+Once the 'network' object has been created, the next step then is to build the model from an input excel file which
+defines different components which constitute the model, how they are connected and their associated parameters:
+
+    network.setFromExcel(inputExcelFilePath, numberOfBuildings, clusterSize, opt)
+    
+'inputExcelFilePath' gives the path of the excel input file. 'numberofBuildings' is an integer parameter specifying the
+number of buildings defined in the excel file. The last two parameters clusterSize and opt are optional. The 'opt'
+parameter could be either 'costs' (default value) or 'env' depending on which criteria should be optimized. The
+'clusterSize' parameter is used to provide a selected number of days which could be assumed representative of the entire
+time range. For example: two typical days could be selected to model the entire year, which could represent two clusters
+summer and winter. This would improve the optimization speed. If not given during the function call, the default value
+of the clusterSize parameter assumes no day clusters.
+
+## Input Excel File
+
+The input excel file is used to define an optimization model and set the model parameters. Each sheet of this excel file
+is structured to defin different components, such as buses, storages and transformers, their respective parameters,
+connections between these components and the building to which they belong.
+
+The input excel file typically has 9-10 sheets, each defining a different component type of the model.
+
+### buses
+This excel sheet defines the buses used in the energy network. Buses define the connections between different
+components. Each row of this excel sheet represents a bus node in the model.
+
+- **label** (string):
+    label name of the bus. Should be unique for each building i.e. different buildings could have the same label for two
+    buses but for one building the buses should not have duplicate labels.
+
+- **active** (0 or 1):
+    If set to 1 then the corresponding bus is active, otherwise (if 0) then the bus is inactive in the model. Could be
+    used to optimize different scenarios with different buses without the need to re-construct the base excel file.
+
+- **excess** (0 or 1):
+    If set to 1 then the corresponding bus has the possibility of having an excess flow unbalanced to the demand. An
+    additional sink node is automatically added in this case to accept this excess flow. If set to 0 then the bus cannot
+    have an excess flow.
+
+- **excess costs** (float):
+    The associated cost of excess flow from a bus. Relevant only if **excess** is set to 1. Could be negative to denote
+    monetary gains such as in case of PV feed-in.
+
+- **building** (integer):
+    Building number to which the bus belongs. Should be unique for each building.
+
+### commodity_sources
+This sheet defines the different commodity sources which serve as an energy input to the model. The parameters **label**,
+**active** and **building** are analogous to the parameters described earlier for buses.
+
+- **to** (string):
+    Label of bus to which the energy from the commodity source flows. The corresponding bus label should exist in
+    the buses sheet.
+
+- **variable costs** (float):
+    Cost per kW of the commodity source.
+
+- **CO2 impact** (float):
+    CO2 impact per kW of the commodity source.
+
+### demand
+The nodes related to the energy demand i.e. sink are defined in this sheet. The parameters **label**, **active** and
+**building** are analogous to the parameters described earlier for buses.
+
+- **from** (string):
+    Label of the bus from which the energy flows to the demand node. The corresponding bus label should exist in
+    the buses sheet.
+
+- **fixed** (0 or 1):
+    If set to 1, the energy demand profiles are fixed and a path to the demand profiles should then be given in the
+    csv_data sheet of the input excel file. If set to 0, the optimizer will select the demand profiles for optimum
+    operation (a total annual demand profile could be given in this case). At the present development stage only fixed
+    demands are accepted.
+
+- **nominal value** (float):
+    The demand profiles series should be normalized values. this parameter then defines the maximum demand with which
+    the normalized series is multiplied to obtain the actual demand profile series. If set to 1, then the given demand
+    profile series is taken as it is (not normalized).
+
+### transformers
+The nodes related to the energy conversion units (or transformers) such as CHP, heat pump, etc. are given in this excel
+sheet. The parameters **label**, **active** and **building** are analogous to the parameters described earlier for buses.
+
+- **from** (string):
+    Label of bus from which the energy flows to the transformer node. The corresponding bus label should exist in
+    the buses sheet.
+
+- **to** (strings separated by comma):
+    Label of the bus(es) to which the energy flows from the transformer node. Different bus labels should be separated
+    by a comma (,), for example: Bus1, Bus2, Bus3. The bus label(s) should exist in the buses sheet.
+
+- **efficiency** (float values separated by comma):
+    Conversion efficiency from input to the output(s) of the transformer node. Efficiencies should be separated by
+    a comma (,) in the case with more than one outputs (i.e. when more than one buses are listed under **to**).
+
+- **capacity_DHW** (float):
+    Maximum capacity limit for domestic hot water (DHW) production from the transformer unit in kW. Could be left blank
+    if the parameter is not relevant to a transformer (for example if a transformer does not produce DHW)
+
+- **capacity_SH** (float):
+    Maximum capacity limit for space heat (SH) production from the transformer unit in kW. Could be left blank if the
+    parameter is not relevant to a transformer (for example if a transformer does not produce SH)
+
+- **capacity_el** (float):
+    Maximum capacity limit for electricity production from the transformer unit in kW. Could be left blank if the
+    parameter is not relevant to a transformer (for example if a transformer does not produce electricity). Note for CHP
+    this parameter acts as the main capacity against which optimization is performed.
+
+- **capacity_min** (float):
+    Minimum capacity to be installed in kW for an investment in the transformer unit.
+
+- **lifetime** (non-negative integer):
+    Lifetime of the node in years.
+
+- **invest_base** (float):
+    Base investment cost of the node.
+
+- **invest_cap** (float):
+    Investment cost per unit installed capacity (i.e. per kW) of the node.
+
+- **maintenance** (float):
+    Maintenance cost of the node. Given as a percentage of the base investment cost **invest_base**. For example:
+    if the investment cost is to be taken as 5% of **invest_base**, then the value of **maintenance** field should be 0.05.
+    Set as 0 if this cost is to be ignored.
+
+- **installation** (float):
+    Installation cost of the node. Given as a percentage of the base investment cost **invest_base**. For example:
+    if the Installation cost is to be taken as 15% of **invest_base**, then **installation** field should be 0.15. Set
+    as 0 if this cost is to be ignored.
+
+- **planification** (float):
+    Cost associated with planning. Given as a percentage of the base investment cost **invest_base**. For example:
+    if the planning cost is 5% of **invest_base**, then **planification** should be 0.05. Set as 0 if this cost is to be
+    ignored.
+
+- **heat_impact** (float):
+    Environmental impact for heat production. Set as 0 if there is no impact due to heat production.
+
+- **elec_impact** (float):
+    Environmental impact for electricity production. Set as 0 if there is no impact due to electricity production.
+
+- **impact_cap** (float):
+    Environmental impact per unit installed capacity i.e. per kW of the node. Set as 0 if there is no impact per
+    installed capacity of the node.
+
+### solar
+This excel sheet defines the parameters related to the solar components such as solar thermal collector and PV panels.
+The parameters **label**, **active** and **building** are analogous to the parameters described earlier for buses.
+**from** and **to** parameters have been previously defined for commodity sources and demand sheets, respectively, while
+the cost and environmental impact paramaters are described under transformers sheet.
+
+- **connect** (string):
+    Label of the bus which connects a solar collector to the model. This bus allows excess heat production from the solar
+    collector. A node for heat sink is created automatically. The given bus label should exist in the buses sheet. This
+    parameter is irrelevant for PV.
+
+- **electrical_consumption** (float):
+    Electrical consumption of the solar component. Given as a percentage fraction of the energy produced. 0.02 means
+    the electrical consumption is 2% of the energy is produced.
+
+- **peripheral_losses** (float):
+    Peripheral losses of the solar component. Given as a percentage fraction of the energy produced. 0.05 means 5% of
+    the energy produced is lost to the surrounding environment.
+
+- **latitude** (float):
+    Latitude of the geographical location where the solar collector/panel is placed. Given in degrees.
+
+- **longitude** (float):
+    Longitude of the geographical location where the solar collector/panel is placed. Given in degrees.
+
+- **tilt** (float):
+    Tilt angle of the solar collector/panel. Given in degrees.
+
+- **azimuth** (float):
+    Azimuth angle of the solar collector/panel. Given in degrees.
+
+- **eta_0**, **a_1** and **a_2** (float):
+    Efficiency parameters of the solar thermal collector. Solar thermal collector is linearized using the pre-calculations
+    given in [oemof-thermal](https://oemof-thermal.readthedocs.io/en/latest/solar_thermal_collector.html).
+
+- **temp_collector_inlet** (float):
+    Inlet fluid temperature of the solar thermal collector. Given in degree C.
+
+- **delta_temp_n** (float):
+    Temperature difference between the inlet fluid and the mean fluid temperature in case of solar collector. For PV,
+    this parameter denotes the temperature difference between the solar cells and the ambient.
+
+- **capacity_max** (float):
+    Maximum capacity limit in kW.
+
+- **capacity_min** (float):
+    Minimum possible capacity in kW for the installation of solar collector/panel.
+
+### storages
+This excel sheet defines the parameters related to the energy storage units such as battery and hot water tank. **label**,
+**active** and **building** have been defined previously for buses excel sheet. A description of **from** and **to** has
+been given in commodity sources and demand sheets, respectively. The cost and environmental impact parameters are
+described in the transformers sheet section. **capacity_min** and **capacity_max** are described in the solar excel sheet
+section.
+
+- **efficiency inflow** (float):
+    Charging efficiency of battery. This parameter is not relevant for thermal storages.
+
+- **efficiency outflow** (float):
+    Discharging efficiency of battery. This parameter is not relevant for thermal storages.
+
+- **initial capacity** (float):
+    initial capacity of the storage. This parameter is expressed as a fraction of the total storage capacity. 0 means storage is initially 
+    assumed to be empty, 1 denotes that the storage is 100% full initially, while 0.5 means the storage is at 50% capacity initially.
+
+- **capacity loss** (float):
+    Losses from battery storage. This parameter is not relevant for thermal storages.
+
+### stratified_storage
+This excel sheet defines the parameters relevant to stratified thermal storage. The pre-calculations given in [oemof-thermal](https://oemof-thermal.readthedocs.io/en/latest/stratified_thermal_storage.html)
+have been used to linearize the thermal hot water storage. The parameter names used here are similar to the parameters
+defined in oemof-thermal.
+
+### links
+This excel sheet defines the parameters for electricity and space heating links. The buildings could share electricity
+production and/or space heat production. Links allow this sharing to be possible. **label** and **active** have been
+defined already for buses excel sheet. **invest_base** and **invest_cap** parameters (defined in the transformers sheet
+section) are only relevant for space heating links in the present stage of development.
+
+- **buildingA** (integer):
+    Building number of the first building of the link. This should match with the values typically given in the
+    **building** parameter in the other excel sheets.
+
+- **buildingB** (integer):
+    Building number of the second building of the link. This should match with the values typically given in the
+    **building** parameter in the other excel sheets.
+
+- **efficiency from A to B** (integer):
+    Efficiency of energy transfer over the link from **buildingA** to **buildingB**.
+
+- **efficiency from B to A** (integer):
+    Efficiency of energy transfer over the link from **buildingB** to **buildingA**.
+
+### csv_data
+The paths to CSV files containing demand profiles, weather data and electricity impact data are to be given in this
+excel sheet. **INFO** gives further information about each row.
+
+### grid_connection
+This excel sheet should not be modified by the users. It defines the separation of the flows from electricity grid and
+the produced electricity flows to make sure that the grid electricity is not stored in batteries.
+
+
+## Collaborators
+
+SPF/OST & HEIG-VD
+
+
```

### Comparing `optihood-0.0.0/README.md` & `optihood-0.0.1/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,348 +1,348 @@
-# optihood: energy modelling and optimization framework
-
-optihood provides a complete python-based framework to **OPTI**mize the investment in alternative energy
-technologies (heat pump, solar thermal, PV, etc.) as well as the operation of available energy resources (natural gas,
-sun, grid electricity, etc.) for decentralized energy networks on a neighbour**HOOD**-scale. It is designed to facilitate 
-the researchers and energy planners in optimizing an energy neighbourhood in terms of cost and/or environmental criteria. 
-It enables the users to perform both single-objective and multi-objective optimization and analysis. The energy model and 
-it's associated parameters can be defined easily using an excel file. Additionally, a variety of plotting methods are 
-defined for easy and fast result visualization.
-
-## Documentation
-The documentation can be found on https://optihood.readthedocs.io/.
-
-## Prerequisites
-In order to use optihood, the following prerequisites are needed on your machine:
-
-- [Python 3.9](https://www.python.org/downloads/) is installed.
-- Git is installed
-- An active [Github](https://github.com/) account to clone the repo.
-- A solver is installed. [Gurobi solver](https://www.gurobi.com/resource/parallelism-linear-mixed-integer-programming/)
-is recommended, although other solvers like CBC, GLPK, Cplex could also be used.
-
-## Installation
-
-As of now, optihood is available as an open source code and needs to be installed from source. Please follow the
-instructions mentioned below to complete the installation. The commands given below are suited for the Windows platform
-and should be run from within the optihood directory in a Command Prompt. For other platforms, similar alternative
-commands could be used.
-
-1. Clone the optihood repo to a folder called 'optihood' on your local machine:
-    ```commandline
-    git clone https://github.com/SPF-OST/OptiHood.git
-    ```
-2. All the next commands should be run from within the optihood folder. Create a virtual environment and activate it:
-    ```commandline
-    py -3.9 -m venv venv
-    venv\Scripts\activate
-    ```    
-3. Install the requirements into the created virtual environment:
-    ```commandline
-    pip install wheel
-    pip install -r requirements.txt
-    ```
-
-
-    It might be required to install C++ build tools. To do that, click on the link that appears with the error message and follow the instructions (it is the lapack package that is missing). In order to be able to 
-    install the missing package, it is required to have a complete Visual Studio instance and installing it with the "Desktop development with C++" workload.
-   
-4.  Verify the installation of the oemof package and the solver by running the installation test in your virtual environment:
-    ```commandline
-    oemof_installation_test
-    ```
-
-    
-    If the installation is successful a message similar to the following would display (the installed solver would be marked as working):
-    ```commandline
-    *****************************
-    Solver installed with oemof
-    cbc: not working
-    glpk: not working
-    gurobi: working
-    cplex: not working
-    
-    *****************************
-    oemof successfully installed.
-    *****************************
-    ```
-5.  To test whether the installation worked well, you could run a [basic example](https://github.com/SPF-OST/OptiHood/tree/main/data/examples/).
-
-## Defining an energy network
-
-Optihood offers a several functionalities to define an energy network, optimize it and visualize the results, which
-provides the user with a complete framework for optimization without the need to code by hand. 
-
-An energy network can be defined as an object of the EnergyNetworkIndiv class or the EnergyNetworkGroup class. This
-object then acts as the primary container for the model. The EnergyNetworkClass is the main parent class, from which 
-two child classes EnergyNetworkIndiv and EnergyNetworkGroup are inherited. Either EnergyNetworkIndiv class or 
-EnergyNetworkGroup class could be used to define an energy network. The choice mainly depends on whether the buildings 
-are linked together (electrically and/or thermally) or not.
-
-If the buildings within an energy network do not share electricity and/or heat, EnergyNetworkIndiv class is used:
-
-    import EnergyNetworkIndiv
-    network = EnergyNetworkIndiv(dateTimeIndex, tSH=35, tDHW=55)
-    
-Otherwise, if the buildings are expected to share energy (electrical and/or heat), EnergyNetworkGroup class is used:
-
-    import EnergyNetworkGroup
-    network = EnergyNetworkGroup(dateTimeIndex, tSH=35, tDHW=55)
-    
-The first parameter to be passed in both the cases is a Datetime index. This parameter gives the time range for an
-optimization model. The Datetime index could be defined using date_range() in pandas:
-
-    import pandas as pd
-    dateTimeIndex = pd.date_range('2021-01-01 00:00:00', '2021-12-31 23:00:00', freq="60min")
-    
-The second and the third parameters tSH and tDHW define the temperatures for space heating and domestic hot water
-production, respectively.
-
-Once the 'network' object has been created, the next step then is to build the model from an input excel file which
-defines different components which constitute the model, how they are connected and their associated parameters:
-
-    network.setFromExcel(inputExcelFilePath, numberOfBuildings, clusterSize, opt)
-    
-'inputExcelFilePath' gives the path of the excel input file. 'numberofBuildings' is an integer parameter specifying the
-number of buildings defined in the excel file. The last two parameters clusterSize and opt are optional. The 'opt'
-parameter could be either 'costs' (default value) or 'env' depending on which criteria should be optimized. The
-'clusterSize' parameter is used to provide a selected number of days which could be assumed representative of the entire
-time range. For example: two typical days could be selected to model the entire year, which could represent two clusters
-summer and winter. This would improve the optimization speed. If not given during the function call, the default value
-of the clusterSize parameter assumes no day clusters.
-
-## Input Excel File
-
-The input excel file is used to define an optimization model and set the model parameters. Each sheet of this excel file
-is structured to defin different components, such as buses, storages and transformers, their respective parameters,
-connections between these components and the building to which they belong.
-
-The input excel file typically has 9-10 sheets, each defining a different component type of the model.
-
-### buses
-This excel sheet defines the buses used in the energy network. Buses define the connections between different
-components. Each row of this excel sheet represents a bus node in the model.
-
-- **label** (string):
-    label name of the bus. Should be unique for each building i.e. different buildings could have the same label for two
-    buses but for one building the buses should not have duplicate labels.
-
-- **active** (0 or 1):
-    If set to 1 then the corresponding bus is active, otherwise (if 0) then the bus is inactive in the model. Could be
-    used to optimize different scenarios with different buses without the need to re-construct the base excel file.
-
-- **excess** (0 or 1):
-    If set to 1 then the corresponding bus has the possibility of having an excess flow unbalanced to the demand. An
-    additional sink node is automatically added in this case to accept this excess flow. If set to 0 then the bus cannot
-    have an excess flow.
-
-- **excess costs** (float):
-    The associated cost of excess flow from a bus. Relevant only if **excess** is set to 1. Could be negative to denote
-    monetary gains such as in case of PV feed-in.
-
-- **building** (integer):
-    Building number to which the bus belongs. Should be unique for each building.
-
-### commodity_sources
-This sheet defines the different commodity sources which serve as an energy input to the model. The parameters **label**,
-**active** and **building** are analogous to the parameters described earlier for buses.
-
-- **to** (string):
-    Label of bus to which the energy from the commodity source flows. The corresponding bus label should exist in
-    the buses sheet.
-
-- **variable costs** (float):
-    Cost per kW of the commodity source.
-
-- **CO2 impact** (float):
-    CO2 impact per kW of the commodity source.
-
-### demand
-The nodes related to the energy demand i.e. sink are defined in this sheet. The parameters **label**, **active** and
-**building** are analogous to the parameters described earlier for buses.
-
-- **from** (string):
-    Label of the bus from which the energy flows to the demand node. The corresponding bus label should exist in
-    the buses sheet.
-
-- **fixed** (0 or 1):
-    If set to 1, the energy demand profiles are fixed and a path to the demand profiles should then be given in the
-    csv_data sheet of the input excel file. If set to 0, the optimizer will select the demand profiles for optimum
-    operation (a total annual demand profile could be given in this case). At the present development stage only fixed
-    demands are accepted.
-
-- **nominal value** (float):
-    The demand profiles series should be normalized values. this parameter then defines the maximum demand with which
-    the normalized series is multiplied to obtain the actual demand profile series. If set to 1, then the given demand
-    profile series is taken as it is (not normalized).
-
-### transformers
-The nodes related to the energy conversion units (or transformers) such as CHP, heat pump, etc. are given in this excel
-sheet. The parameters **label**, **active** and **building** are analogous to the parameters described earlier for buses.
-
-- **from** (string):
-    Label of bus from which the energy flows to the transformer node. The corresponding bus label should exist in
-    the buses sheet.
-
-- **to** (strings separated by comma):
-    Label of the bus(es) to which the energy flows from the transformer node. Different bus labels should be separated
-    by a comma (,), for example: Bus1, Bus2, Bus3. The bus label(s) should exist in the buses sheet.
-
-- **efficiency** (float values separated by comma):
-    Conversion efficiency from input to the output(s) of the transformer node. Efficiencies should be separated by
-    a comma (,) in the case with more than one outputs (i.e. when more than one buses are listed under **to**).
-
-- **capacity_DHW** (float):
-    Maximum capacity limit for domestic hot water (DHW) production from the transformer unit in kW. Could be left blank
-    if the parameter is not relevant to a transformer (for example if a transformer does not produce DHW)
-
-- **capacity_SH** (float):
-    Maximum capacity limit for space heat (SH) production from the transformer unit in kW. Could be left blank if the
-    parameter is not relevant to a transformer (for example if a transformer does not produce SH)
-
-- **capacity_el** (float):
-    Maximum capacity limit for electricity production from the transformer unit in kW. Could be left blank if the
-    parameter is not relevant to a transformer (for example if a transformer does not produce electricity). Note for CHP
-    this parameter acts as the main capacity against which optimization is performed.
-
-- **capacity_min** (float):
-    Minimum capacity to be installed in kW for an investment in the transformer unit.
-
-- **lifetime** (non-negative integer):
-    Lifetime of the node in years.
-
-- **invest_base** (float):
-    Base investment cost of the node.
-
-- **invest_cap** (float):
-    Investment cost per unit installed capacity (i.e. per kW) of the node.
-
-- **maintenance** (float):
-    Maintenance cost of the node. Given as a percentage of the base investment cost **invest_base**. For example:
-    if the investment cost is to be taken as 5% of **invest_base**, then the value of **maintenance** field should be 0.05.
-    Set as 0 if this cost is to be ignored.
-
-- **installation** (float):
-    Installation cost of the node. Given as a percentage of the base investment cost **invest_base**. For example:
-    if the Installation cost is to be taken as 15% of **invest_base**, then **installation** field should be 0.15. Set
-    as 0 if this cost is to be ignored.
-
-- **planification** (float):
-    Cost associated with planning. Given as a percentage of the base investment cost **invest_base**. For example:
-    if the planning cost is 5% of **invest_base**, then **planification** should be 0.05. Set as 0 if this cost is to be
-    ignored.
-
-- **heat_impact** (float):
-    Environmental impact for heat production. Set as 0 if there is no impact due to heat production.
-
-- **elec_impact** (float):
-    Environmental impact for electricity production. Set as 0 if there is no impact due to electricity production.
-
-- **impact_cap** (float):
-    Environmental impact per unit installed capacity i.e. per kW of the node. Set as 0 if there is no impact per
-    installed capacity of the node.
-
-### solar
-This excel sheet defines the parameters related to the solar components such as solar thermal collector and PV panels.
-The parameters **label**, **active** and **building** are analogous to the parameters described earlier for buses.
-**from** and **to** parameters have been previously defined for commodity sources and demand sheets, respectively, while
-the cost and environmental impact paramaters are described under transformers sheet.
-
-- **connect** (string):
-    Label of the bus which connects a solar collector to the model. This bus allows excess heat production from the solar
-    collector. A node for heat sink is created automatically. The given bus label should exist in the buses sheet. This
-    parameter is irrelevant for PV.
-
-- **electrical_consumption** (float):
-    Electrical consumption of the solar component. Given as a percentage fraction of the energy produced. 0.02 means
-    the electrical consumption is 2% of the energy is produced.
-
-- **peripheral_losses** (float):
-    Peripheral losses of the solar component. Given as a percentage fraction of the energy produced. 0.05 means 5% of
-    the energy produced is lost to the surrounding environment.
-
-- **latitude** (float):
-    Latitude of the geographical location where the solar collector/panel is placed. Given in degrees.
-
-- **longitude** (float):
-    Longitude of the geographical location where the solar collector/panel is placed. Given in degrees.
-
-- **tilt** (float):
-    Tilt angle of the solar collector/panel. Given in degrees.
-
-- **azimuth** (float):
-    Azimuth angle of the solar collector/panel. Given in degrees.
-
-- **eta_0**, **a_1** and **a_2** (float):
-    Efficiency parameters of the solar thermal collector. Solar thermal collector is linearized using the pre-calculations
-    given in [oemof-thermal](https://oemof-thermal.readthedocs.io/en/latest/solar_thermal_collector.html).
-
-- **temp_collector_inlet** (float):
-    Inlet fluid temperature of the solar thermal collector. Given in degree C.
-
-- **delta_temp_n** (float):
-    Temperature difference between the inlet fluid and the mean fluid temperature in case of solar collector. For PV,
-    this parameter denotes the temperature difference between the solar cells and the ambient.
-
-- **capacity_max** (float):
-    Maximum capacity limit in kW.
-
-- **capacity_min** (float):
-    Minimum possible capacity in kW for the installation of solar collector/panel.
-
-### storages
-This excel sheet defines the parameters related to the energy storage units such as battery and hot water tank. **label**,
-**active** and **building** have been defined previously for buses excel sheet. A description of **from** and **to** has
-been given in commodity sources and demand sheets, respectively. The cost and environmental impact parameters are
-described in the transformers sheet section. **capacity_min** and **capacity_max** are described in the solar excel sheet
-section.
-
-- **efficiency inflow** (float):
-    Charging efficiency of battery. This parameter is not relevant for thermal storages.
-
-- **efficiency outflow** (float):
-    Discharging efficiency of battery. This parameter is not relevant for thermal storages.
-
-- **initial capacity** (float):
-    initial capacity of the storage. This parameter is expressed as a fraction of the total storage capacity. 0 means storage is initially 
-    assumed to be empty, 1 denotes that the storage is 100% full initially, while 0.5 means the storage is at 50% capacity initially.
-
-- **capacity loss** (float):
-    Losses from battery storage. This parameter is not relevant for thermal storages.
-
-### stratified_storage
-This excel sheet defines the parameters relevant to stratified thermal storage. The pre-calculations given in [oemof-thermal](https://oemof-thermal.readthedocs.io/en/latest/stratified_thermal_storage.html)
-have been used to linearize the thermal hot water storage. The parameter names used here are similar to the parameters
-defined in oemof-thermal.
-
-### links
-This excel sheet defines the parameters for electricity and space heating links. The buildings could share electricity
-production and/or space heat production. Links allow this sharing to be possible. **label** and **active** have been
-defined already for buses excel sheet. **invest_base** and **invest_cap** parameters (defined in the transformers sheet
-section) are only relevant for space heating links in the present stage of development.
-
-- **buildingA** (integer):
-    Building number of the first building of the link. This should match with the values typically given in the
-    **building** parameter in the other excel sheets.
-
-- **buildingB** (integer):
-    Building number of the second building of the link. This should match with the values typically given in the
-    **building** parameter in the other excel sheets.
-
-- **efficiency from A to B** (integer):
-    Efficiency of energy transfer over the link from **buildingA** to **buildingB**.
-
-- **efficiency from B to A** (integer):
-    Efficiency of energy transfer over the link from **buildingB** to **buildingA**.
-
-### csv_data
-The paths to CSV files containing demand profiles, weather data and electricity impact data are to be given in this
-excel sheet. **INFO** gives further information about each row.
-
-### grid_connection
-This excel sheet should not be modified by the users. It defines the separation of the flows from electricity grid and
-the produced electricity flows to make sure that the grid electricity is not stored in batteries.
-
-
-## Collaborators
-
-SPF/OST & HEIG-VD
+# optihood: energy modelling and optimization framework
+
+optihood provides a complete python-based framework to **OPTI**mize the investment in alternative energy
+technologies (heat pump, solar thermal, PV, etc.) as well as the operation of available energy resources (natural gas,
+sun, grid electricity, etc.) for decentralized energy networks on a neighbour**HOOD**-scale. It is designed to facilitate 
+the researchers and energy planners in optimizing an energy neighbourhood in terms of cost and/or environmental criteria. 
+It enables the users to perform both single-objective and multi-objective optimization and analysis. The energy model and 
+it's associated parameters can be defined easily using an excel file. Additionally, a variety of plotting methods are 
+defined for easy and fast result visualization.
+
+## Documentation
+The documentation can be found on https://optihood.readthedocs.io/.
+
+## Prerequisites
+In order to use optihood, the following prerequisites are needed on your machine:
+
+- [Python 3.9](https://www.python.org/downloads/) is installed.
+- Git is installed
+- An active [Github](https://github.com/) account to clone the repo.
+- A solver is installed. [Gurobi solver](https://www.gurobi.com/resource/parallelism-linear-mixed-integer-programming/)
+is recommended, although other solvers like CBC, GLPK, Cplex could also be used.
+
+## Installation
+
+As of now, optihood is available as an open source code and needs to be installed from source. Please follow the
+instructions mentioned below to complete the installation. The commands given below are suited for the Windows platform
+and should be run from within the optihood directory in a Command Prompt. For other platforms, similar alternative
+commands could be used.
+
+1. Clone the optihood repo to a folder called 'optihood' on your local machine:
+    ```commandline
+    git clone https://github.com/SPF-OST/OptiHood.git
+    ```
+2. All the next commands should be run from within the optihood folder. Create a virtual environment and activate it:
+    ```commandline
+    py -3.9 -m venv venv
+    venv\Scripts\activate
+    ```    
+3. Install the requirements into the created virtual environment:
+    ```commandline
+    pip install wheel
+    pip install -r requirements.txt
+    ```
+
+
+    It might be required to install C++ build tools. To do that, click on the link that appears with the error message and follow the instructions (it is the lapack package that is missing). In order to be able to 
+    install the missing package, it is required to have a complete Visual Studio instance and installing it with the "Desktop development with C++" workload.
+   
+4.  Verify the installation of the oemof package and the solver by running the installation test in your virtual environment:
+    ```commandline
+    oemof_installation_test
+    ```
+
+    
+    If the installation is successful a message similar to the following would display (the installed solver would be marked as working):
+    ```commandline
+    *****************************
+    Solver installed with oemof
+    cbc: not working
+    glpk: not working
+    gurobi: working
+    cplex: not working
+    
+    *****************************
+    oemof successfully installed.
+    *****************************
+    ```
+5.  To test whether the installation worked well, you could run a [basic example](https://github.com/SPF-OST/OptiHood/tree/main/data/examples/).
+
+## Defining an energy network
+
+Optihood offers a several functionalities to define an energy network, optimize it and visualize the results, which
+provides the user with a complete framework for optimization without the need to code by hand. 
+
+An energy network can be defined as an object of the EnergyNetworkIndiv class or the EnergyNetworkGroup class. This
+object then acts as the primary container for the model. The EnergyNetworkClass is the main parent class, from which 
+two child classes EnergyNetworkIndiv and EnergyNetworkGroup are inherited. Either EnergyNetworkIndiv class or 
+EnergyNetworkGroup class could be used to define an energy network. The choice mainly depends on whether the buildings 
+are linked together (electrically and/or thermally) or not.
+
+If the buildings within an energy network do not share electricity and/or heat, EnergyNetworkIndiv class is used:
+
+    import EnergyNetworkIndiv
+    network = EnergyNetworkIndiv(dateTimeIndex, tSH=35, tDHW=55)
+    
+Otherwise, if the buildings are expected to share energy (electrical and/or heat), EnergyNetworkGroup class is used:
+
+    import EnergyNetworkGroup
+    network = EnergyNetworkGroup(dateTimeIndex, tSH=35, tDHW=55)
+    
+The first parameter to be passed in both the cases is a Datetime index. This parameter gives the time range for an
+optimization model. The Datetime index could be defined using date_range() in pandas:
+
+    import pandas as pd
+    dateTimeIndex = pd.date_range('2021-01-01 00:00:00', '2021-12-31 23:00:00', freq="60min")
+    
+The second and the third parameters tSH and tDHW define the temperatures for space heating and domestic hot water
+production, respectively.
+
+Once the 'network' object has been created, the next step then is to build the model from an input excel file which
+defines different components which constitute the model, how they are connected and their associated parameters:
+
+    network.setFromExcel(inputExcelFilePath, numberOfBuildings, clusterSize, opt)
+    
+'inputExcelFilePath' gives the path of the excel input file. 'numberofBuildings' is an integer parameter specifying the
+number of buildings defined in the excel file. The last two parameters clusterSize and opt are optional. The 'opt'
+parameter could be either 'costs' (default value) or 'env' depending on which criteria should be optimized. The
+'clusterSize' parameter is used to provide a selected number of days which could be assumed representative of the entire
+time range. For example: two typical days could be selected to model the entire year, which could represent two clusters
+summer and winter. This would improve the optimization speed. If not given during the function call, the default value
+of the clusterSize parameter assumes no day clusters.
+
+## Input Excel File
+
+The input excel file is used to define an optimization model and set the model parameters. Each sheet of this excel file
+is structured to defin different components, such as buses, storages and transformers, their respective parameters,
+connections between these components and the building to which they belong.
+
+The input excel file typically has 9-10 sheets, each defining a different component type of the model.
+
+### buses
+This excel sheet defines the buses used in the energy network. Buses define the connections between different
+components. Each row of this excel sheet represents a bus node in the model.
+
+- **label** (string):
+    label name of the bus. Should be unique for each building i.e. different buildings could have the same label for two
+    buses but for one building the buses should not have duplicate labels.
+
+- **active** (0 or 1):
+    If set to 1 then the corresponding bus is active, otherwise (if 0) then the bus is inactive in the model. Could be
+    used to optimize different scenarios with different buses without the need to re-construct the base excel file.
+
+- **excess** (0 or 1):
+    If set to 1 then the corresponding bus has the possibility of having an excess flow unbalanced to the demand. An
+    additional sink node is automatically added in this case to accept this excess flow. If set to 0 then the bus cannot
+    have an excess flow.
+
+- **excess costs** (float):
+    The associated cost of excess flow from a bus. Relevant only if **excess** is set to 1. Could be negative to denote
+    monetary gains such as in case of PV feed-in.
+
+- **building** (integer):
+    Building number to which the bus belongs. Should be unique for each building.
+
+### commodity_sources
+This sheet defines the different commodity sources which serve as an energy input to the model. The parameters **label**,
+**active** and **building** are analogous to the parameters described earlier for buses.
+
+- **to** (string):
+    Label of bus to which the energy from the commodity source flows. The corresponding bus label should exist in
+    the buses sheet.
+
+- **variable costs** (float):
+    Cost per kW of the commodity source.
+
+- **CO2 impact** (float):
+    CO2 impact per kW of the commodity source.
+
+### demand
+The nodes related to the energy demand i.e. sink are defined in this sheet. The parameters **label**, **active** and
+**building** are analogous to the parameters described earlier for buses.
+
+- **from** (string):
+    Label of the bus from which the energy flows to the demand node. The corresponding bus label should exist in
+    the buses sheet.
+
+- **fixed** (0 or 1):
+    If set to 1, the energy demand profiles are fixed and a path to the demand profiles should then be given in the
+    csv_data sheet of the input excel file. If set to 0, the optimizer will select the demand profiles for optimum
+    operation (a total annual demand profile could be given in this case). At the present development stage only fixed
+    demands are accepted.
+
+- **nominal value** (float):
+    The demand profiles series should be normalized values. this parameter then defines the maximum demand with which
+    the normalized series is multiplied to obtain the actual demand profile series. If set to 1, then the given demand
+    profile series is taken as it is (not normalized).
+
+### transformers
+The nodes related to the energy conversion units (or transformers) such as CHP, heat pump, etc. are given in this excel
+sheet. The parameters **label**, **active** and **building** are analogous to the parameters described earlier for buses.
+
+- **from** (string):
+    Label of bus from which the energy flows to the transformer node. The corresponding bus label should exist in
+    the buses sheet.
+
+- **to** (strings separated by comma):
+    Label of the bus(es) to which the energy flows from the transformer node. Different bus labels should be separated
+    by a comma (,), for example: Bus1, Bus2, Bus3. The bus label(s) should exist in the buses sheet.
+
+- **efficiency** (float values separated by comma):
+    Conversion efficiency from input to the output(s) of the transformer node. Efficiencies should be separated by
+    a comma (,) in the case with more than one outputs (i.e. when more than one buses are listed under **to**).
+
+- **capacity_DHW** (float):
+    Maximum capacity limit for domestic hot water (DHW) production from the transformer unit in kW. Could be left blank
+    if the parameter is not relevant to a transformer (for example if a transformer does not produce DHW)
+
+- **capacity_SH** (float):
+    Maximum capacity limit for space heat (SH) production from the transformer unit in kW. Could be left blank if the
+    parameter is not relevant to a transformer (for example if a transformer does not produce SH)
+
+- **capacity_el** (float):
+    Maximum capacity limit for electricity production from the transformer unit in kW. Could be left blank if the
+    parameter is not relevant to a transformer (for example if a transformer does not produce electricity). Note for CHP
+    this parameter acts as the main capacity against which optimization is performed.
+
+- **capacity_min** (float):
+    Minimum capacity to be installed in kW for an investment in the transformer unit.
+
+- **lifetime** (non-negative integer):
+    Lifetime of the node in years.
+
+- **invest_base** (float):
+    Base investment cost of the node.
+
+- **invest_cap** (float):
+    Investment cost per unit installed capacity (i.e. per kW) of the node.
+
+- **maintenance** (float):
+    Maintenance cost of the node. Given as a percentage of the base investment cost **invest_base**. For example:
+    if the investment cost is to be taken as 5% of **invest_base**, then the value of **maintenance** field should be 0.05.
+    Set as 0 if this cost is to be ignored.
+
+- **installation** (float):
+    Installation cost of the node. Given as a percentage of the base investment cost **invest_base**. For example:
+    if the Installation cost is to be taken as 15% of **invest_base**, then **installation** field should be 0.15. Set
+    as 0 if this cost is to be ignored.
+
+- **planification** (float):
+    Cost associated with planning. Given as a percentage of the base investment cost **invest_base**. For example:
+    if the planning cost is 5% of **invest_base**, then **planification** should be 0.05. Set as 0 if this cost is to be
+    ignored.
+
+- **heat_impact** (float):
+    Environmental impact for heat production. Set as 0 if there is no impact due to heat production.
+
+- **elec_impact** (float):
+    Environmental impact for electricity production. Set as 0 if there is no impact due to electricity production.
+
+- **impact_cap** (float):
+    Environmental impact per unit installed capacity i.e. per kW of the node. Set as 0 if there is no impact per
+    installed capacity of the node.
+
+### solar
+This excel sheet defines the parameters related to the solar components such as solar thermal collector and PV panels.
+The parameters **label**, **active** and **building** are analogous to the parameters described earlier for buses.
+**from** and **to** parameters have been previously defined for commodity sources and demand sheets, respectively, while
+the cost and environmental impact paramaters are described under transformers sheet.
+
+- **connect** (string):
+    Label of the bus which connects a solar collector to the model. This bus allows excess heat production from the solar
+    collector. A node for heat sink is created automatically. The given bus label should exist in the buses sheet. This
+    parameter is irrelevant for PV.
+
+- **electrical_consumption** (float):
+    Electrical consumption of the solar component. Given as a percentage fraction of the energy produced. 0.02 means
+    the electrical consumption is 2% of the energy is produced.
+
+- **peripheral_losses** (float):
+    Peripheral losses of the solar component. Given as a percentage fraction of the energy produced. 0.05 means 5% of
+    the energy produced is lost to the surrounding environment.
+
+- **latitude** (float):
+    Latitude of the geographical location where the solar collector/panel is placed. Given in degrees.
+
+- **longitude** (float):
+    Longitude of the geographical location where the solar collector/panel is placed. Given in degrees.
+
+- **tilt** (float):
+    Tilt angle of the solar collector/panel. Given in degrees.
+
+- **azimuth** (float):
+    Azimuth angle of the solar collector/panel. Given in degrees.
+
+- **eta_0**, **a_1** and **a_2** (float):
+    Efficiency parameters of the solar thermal collector. Solar thermal collector is linearized using the pre-calculations
+    given in [oemof-thermal](https://oemof-thermal.readthedocs.io/en/latest/solar_thermal_collector.html).
+
+- **temp_collector_inlet** (float):
+    Inlet fluid temperature of the solar thermal collector. Given in degree C.
+
+- **delta_temp_n** (float):
+    Temperature difference between the inlet fluid and the mean fluid temperature in case of solar collector. For PV,
+    this parameter denotes the temperature difference between the solar cells and the ambient.
+
+- **capacity_max** (float):
+    Maximum capacity limit in kW.
+
+- **capacity_min** (float):
+    Minimum possible capacity in kW for the installation of solar collector/panel.
+
+### storages
+This excel sheet defines the parameters related to the energy storage units such as battery and hot water tank. **label**,
+**active** and **building** have been defined previously for buses excel sheet. A description of **from** and **to** has
+been given in commodity sources and demand sheets, respectively. The cost and environmental impact parameters are
+described in the transformers sheet section. **capacity_min** and **capacity_max** are described in the solar excel sheet
+section.
+
+- **efficiency inflow** (float):
+    Charging efficiency of battery. This parameter is not relevant for thermal storages.
+
+- **efficiency outflow** (float):
+    Discharging efficiency of battery. This parameter is not relevant for thermal storages.
+
+- **initial capacity** (float):
+    initial capacity of the storage. This parameter is expressed as a fraction of the total storage capacity. 0 means storage is initially 
+    assumed to be empty, 1 denotes that the storage is 100% full initially, while 0.5 means the storage is at 50% capacity initially.
+
+- **capacity loss** (float):
+    Losses from battery storage. This parameter is not relevant for thermal storages.
+
+### stratified_storage
+This excel sheet defines the parameters relevant to stratified thermal storage. The pre-calculations given in [oemof-thermal](https://oemof-thermal.readthedocs.io/en/latest/stratified_thermal_storage.html)
+have been used to linearize the thermal hot water storage. The parameter names used here are similar to the parameters
+defined in oemof-thermal.
+
+### links
+This excel sheet defines the parameters for electricity and space heating links. The buildings could share electricity
+production and/or space heat production. Links allow this sharing to be possible. **label** and **active** have been
+defined already for buses excel sheet. **invest_base** and **invest_cap** parameters (defined in the transformers sheet
+section) are only relevant for space heating links in the present stage of development.
+
+- **buildingA** (integer):
+    Building number of the first building of the link. This should match with the values typically given in the
+    **building** parameter in the other excel sheets.
+
+- **buildingB** (integer):
+    Building number of the second building of the link. This should match with the values typically given in the
+    **building** parameter in the other excel sheets.
+
+- **efficiency from A to B** (integer):
+    Efficiency of energy transfer over the link from **buildingA** to **buildingB**.
+
+- **efficiency from B to A** (integer):
+    Efficiency of energy transfer over the link from **buildingB** to **buildingA**.
+
+### csv_data
+The paths to CSV files containing demand profiles, weather data and electricity impact data are to be given in this
+excel sheet. **INFO** gives further information about each row.
+
+### grid_connection
+This excel sheet should not be modified by the users. It defines the separation of the flows from electricity grid and
+the produced electricity flows to make sure that the grid electricity is not stored in batteries.
+
+
+## Collaborators
+
+SPF/OST & HEIG-VD
```

### Comparing `optihood-0.0.0/optihood/buildings.py` & `optihood-0.0.1/optihood/buildings.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,651 +1,651 @@
-import numpy as np
-import oemof.solph as solph
-import pandas as pd
-from oemof.tools import logger
-from oemof.tools import economics
-import logging
-from optihood.converters import *
-from optihood.sources import PV
-from optihood.storages import ElectricalStorage, ThermalStorage
-from optihood.sinks import SinkRCModel
-
-intRate = 0.05
-
-class Building:
-    def __init__(self, label):
-        self.__nodesList = []
-        self.__inputs = []
-        self.__technologies = []
-        self.__costParam = {}
-        self.__envParam = {}
-        self.__busDict = {}
-        self.__buildingLabel = label
-        self.__linkBuses = ["electricityBus", "electricityInBus", "domesticHotWaterBus", "dhwDemandBus", "spaceHeatingBus", "shDemandBus"]
-
-    def getBuildingLabel(self):
-        return self.__buildingLabel
-
-    def getNodesList(self):
-        return self.__nodesList
-
-    def getBusDict(self):
-        return self.__busDict
-
-    def getInputs(self):
-        return self.__inputs
-
-    def getTechnologies(self):
-        return self.__technologies
-
-    def getCostParam(self):
-        return self.__costParam
-
-    def getEnvParam(self):
-        return self.__envParam
-
-    def addBus(self, data, opt, mergeLinkBuses, electricityImpact, clusterSize, includeCarbonBenefits):
-        # Create Bus objects from buses table
-        for i, b in data.iterrows():
-            if b["active"]:
-                if mergeLinkBuses and b["label"] in self.__linkBuses:
-                    label = b["label"]
-                else:
-                    label = b["label"] + '__' + self.__buildingLabel
-
-                if not mergeLinkBuses or (mergeLinkBuses and (self.__buildingLabel=='Building1' or label not in self.__linkBuses)):
-                    bus = solph.Bus(label=label)
-                    self.__nodesList.append(bus)
-                    self.__busDict[label] = bus
-                    if opt=='costs':
-                        if not clusterSize: varcost=float(b["excess costs"])
-                        else:
-                            varcost = None
-                            for d in clusterSize:
-                                temp = pd.Series(np.tile([float(b["excess costs"])*clusterSize[d]], 24))
-                                if varcost is not None:
-                                    varcost = varcost.append(temp, ignore_index=True)
-                                else:
-                                    varcost = temp
-                    elif opt=='env' and includeCarbonBenefits:varcost=-electricityImpact['impact']
-                    else: varcost=0
-                    if b["excess"]:
-                        self.__nodesList.append(
-                            solph.Sink(
-                                label="excess"+label,
-                                inputs={
-                                    self.__busDict[label]: solph.Flow(
-                                        variable_costs=varcost
-                                    )}))
-                        # add the excess production cost to self.__costParam
-                        self.__costParam["excess"+label] = float(b["excess costs"])
-        if mergeLinkBuses and self.__buildingLabel=='Building1':
-            return self.__busDict
-
-    def addToBusDict(self, busDictBuilding1):
-        for label in self.__linkBuses:
-            self.__busDict[label] = busDictBuilding1[label]
-
-    def addPV(self, data, data_timeseries, opt, dispatchMode):
-        # Create Source objects from table 'commodity sources'
-        for i, s in data.iterrows():
-            if opt == "costs":
-                epc=self._calculateInvest(s)[0]
-                base=self._calculateInvest(s)[1]
-                env_capa=float(s["impact_cap"]) / float(s["lifetime"])
-                env_flow=float(s["elec_impact"])
-                varc=0 # variable cost is only passed for environmental optimization if there are emissions per kWh of energy produced from the unit
-
-                envParam = [0, float(s["elec_impact"]), float(s["impact_cap"]) / float(s["lifetime"])]
-
-            elif opt == "env":
-                epc = float(s["impact_cap"]) / float(s["lifetime"])
-                base = 0
-                env_capa = float(s["impact_cap"]) / float(s["lifetime"])
-                env_flow = float(s["elec_impact"])
-                varc = float(s["elec_impact"]) # variable cost is only passed for environmental optimization if there are emissions per kWh of energy produced from the unit
-
-                envParam = [0, float(s["elec_impact"]), float(s["impact_cap"]) / float(s["lifetime"])]
-
-            # If roof area and zenith do not exist in the excel file
-            if 'roof_area' not in s.keys():
-                s["roof_area"] = np.nan
-            if 'zenith_angle' not in s.keys():
-                s["zenith_angle"] = np.nan
-            if 'efficiency' not in s.keys():
-                s["efficiency"] = np.nan
-
-            self.__nodesList.append(PV(s["label"], self.__buildingLabel,
-                                       self.__busDict[s["to"] + '__' + self.__buildingLabel],
-                                       float(s["peripheral_losses"]), float(s["latitude"]), float(s["longitude"]),
-                                       float(s["tilt"]), float(s["efficiency"]), s["roof_area"],
-                                       s["zenith_angle"], s["azimuth"],
-                                       data_timeseries['gls'],
-                                       data_timeseries['str.diffus'],
-                                       data_timeseries['tre200h0'], float(s["capacity_min"]), float(s["capacity_max"]),
-                                       epc, base, env_capa, env_flow, varc, dispatchMode))
-
-            self.__envParam[s["label"] + '__' + self.__buildingLabel] = envParam
-
-            self.__costParam[s["label"] + '__' + self.__buildingLabel] = [self._calculateInvest(s)[0],
-                                                                          self._calculateInvest(s)[1]]
-            self.__technologies.append(
-                [s["to"] + '__' + self.__buildingLabel, s["label"] + '__' + self.__buildingLabel])
-
-    def addSolar(self, data, data_timeseries, opt, mergeLinkBuses, dispatchMode):
-        # Create Source objects from table 'commodity sources'
-        for i, s in data.iterrows():
-            if mergeLinkBuses and s["from"] in self.__linkBuses:
-                inputBusLabel = s["from"]
-            else:
-                inputBusLabel = s["from"] + '__' + self.__buildingLabel
-
-            if opt == "costs":
-                epc=self._calculateInvest(s)[0]
-                base=self._calculateInvest(s)[1]
-                env_capa=float(s["impact_cap"]) / float(s["lifetime"])
-                env_flow=float(s["heat_impact"])
-                varc=0 # variable cost is only passed for environmental optimization if there are emissions per kWh of energy produced from the unit
-
-                envParam = [env_flow, 0, env_capa]
-
-            elif opt == "env":
-                epc=float(s["impact_cap"]) / float(s["lifetime"])
-                base=0
-                env_capa= float(s["impact_cap"]) / float(s["lifetime"])
-                env_flow=float(s["heat_impact"])
-                varc= float(s["heat_impact"]) # variable cost is only passed for environmental optimization if there are emissions per kWh of energy produced from the unit
-
-                envParam = [env_flow, 0, env_capa]
-
-            # If roof area and zenith do not exist in the excel file
-            if 'roof_area' not in s.keys():
-                s["roof_area"] = np.nan
-            if 'zenith_angle' not in s.keys():
-                s["zenith_angle"] = np.nan
-            collector=SolarCollector(s["label"], self.__buildingLabel,
-                                                   self.__busDict[inputBusLabel],
-                                                   self.__busDict[s["to"] + '__' + self.__buildingLabel],
-                                                   self.__busDict[s["connect"]+ '__' + self.__buildingLabel],
-                                                   float(s["electrical_consumption"]), float(s["peripheral_losses"]), float(s["latitude"]),
-                                                   float(s["longitude"]), float(s["tilt"]), s["roof_area"],
-                                                   s["zenith_angle"], float(s["azimuth"]),
-                                                   float(s["eta_0"]), float(s["a_1"]), float(s["a_2"]), float(s["temp_collector_inlet"]),
-                                                   float(s["delta_temp_n"]), data_timeseries['gls'], data_timeseries['str.diffus'],
-                                                    data_timeseries['tre200h0'], float(s["capacity_min"]), float(s["capacity_max"]),
-                                                   epc, base, env_capa, env_flow, varc, dispatchMode)
-            self.__nodesList.append(collector.getSolar("source"))
-            self.__nodesList.append(collector.getSolar("transformer"))
-            self.__nodesList.append(collector.getSolar("sink"))
-
-            self.__envParam["heat_"+s["label"] + '__' + self.__buildingLabel] = envParam
-
-            self.__costParam["heat_"+s["label"] + '__' + self.__buildingLabel] = [self._calculateInvest(s)[0],
-                                                                          self._calculateInvest(s)[1]]
-            self.__technologies.append(
-                [s["to"] + '__' + self.__buildingLabel, s["label"] + '__' + self.__buildingLabel])
-
-    def addPVT(self, data, data_timeseries, opt, mergeLinkBuses, dispatchMode):
-        # Create Source objects from table 'commodity sources'
-        for i, s in data.iterrows():
-            if s["active"]:
-                if mergeLinkBuses and s["from"] in self.__linkBuses:
-                    inputBusLabel = s["from"]
-                else:
-                    inputBusLabel = s["from"] + '__' + self.__buildingLabel
-
-                outputBuses = [self.__busDict[s["to"].split(",")[0] + '__' + self.__buildingLabel],
-                               self.__busDict[s["to"].split(",")[1] + '__' + self.__buildingLabel],
-                               self.__busDict[s["to"].split(",")[2] + '__' + self.__buildingLabel]]
-                connectBuses = [self.__busDict[s["connect"].split(",")[0] + '__' + self.__buildingLabel],
-                               self.__busDict[s["connect"].split(",")[1] + '__' + self.__buildingLabel]]
-                if opt == "costs":
-                    epc = self._calculateInvest(s)[0]
-                    base = self._calculateInvest(s)[1]
-                    env_capa = float(s["impact_cap"]) / float(s["lifetime"])
-                    env_flow = float(s["heat_impact"])
-                    varc = 0  # variable cost is only passed for environmental optimization if there are emissions per kWh of energy produced from the unit
-
-                    envParam = [env_flow, 0, env_capa]
-
-                elif opt == "env":
-                    epc = float(s["impact_cap"]) / float(s["lifetime"])
-                    base = 0
-                    env_capa = float(s["impact_cap"]) / float(s["lifetime"])
-                    env_flow = float(s["heat_impact"])
-                    varc = float(s[
-                                     "heat_impact"])  # variable cost is only passed for environmental optimization if there are emissions per kWh of energy produced from the unit
-
-                    envParam = [env_flow, 0, env_capa]
-
-                # If roof area does not exist in the excel file
-                if 'roof_area' not in s.keys():
-                    s["roof_area"] = np.nan
-                else:
-                    s["roof_area"] = float(s["roof_area"])
-                pvtcollector = PVT(s["label"], self.__buildingLabel,
-                                                       self.__busDict[inputBusLabel],
-                                                       outputBuses,
-                                                       connectBuses,
-                                                       float(s["electrical_consumption"]), float(s["peripheral_losses"]), float(s["latitude"]),
-                                                       float(s["longitude"]), float(s["tilt"]), s["roof_area"],
-                                                       float(s["zenith_angle"]), float(s["azimuth"]),
-                                                       float(s["eta_0"]), float(s["a_1"]), float(s["a_2"]), float(s["temp_collector_inlet"]),data_timeseries['tre200h0'],
-                                                       float(s["delta_temp_n"]), data_timeseries['gls'], data_timeseries['str.diffus'], float(s["capacity_min"]), float(s["capacity_max"]),
-                                                       epc, base, env_capa, env_flow, varc, dispatchMode,
-                                                        float(s["pv_efficiency"]))
-                nodes = [pvtcollector.getPVT("el_source")]
-                for t in ["heat_source", "heat_transformer", "excess_heat_sink"]:
-                    nodes.append(pvtcollector.getPVT(t))
-                for x in nodes:
-                    self.__nodesList.append(x)
-
-
-                self.__envParam['heatSourceSH_' + s['label'] + '__' + self.__buildingLabel] = envParam
-                self.__envParam['heatSourceDHW_' + s['label'] + '__' + self.__buildingLabel] = [env_flow, 0, 0]
-                self.__costParam['heatSourceSH_' + s['label'] + '__' + self.__buildingLabel] = [self._calculateInvest(s)[0],
-                                                                                            self._calculateInvest(s)[1]]
-                self.__costParam['heatSourceDHW_' + s['label'] + '__' + self.__buildingLabel] = [0, 0]
-
-                self.__technologies.append(
-                    [outputBuses[0], s["label"] + 'SH__' + self.__buildingLabel])
-                self.__technologies.append(
-                    [outputBuses[1], s["label"] + 'DHW__' + self.__buildingLabel])
-
-    def addGridSeparation(self, dataGridSeparation, mergeLinkBuses):
-        if not dataGridSeparation.empty:
-            for i, gs in dataGridSeparation.iterrows():
-                if mergeLinkBuses:
-                    if gs["label"] in ['gridElectricity','electricitySource','shSource']:
-                        label = gs["label"]+'__'+self.__buildingLabel
-                    else:
-                        label = gs["label"]
-                    if gs["from"] in self.__linkBuses:
-                        inputBusLabel = gs["from"]
-                    else:
-                        inputBusLabel = gs["from"]+'__'+self.__buildingLabel
-                    if gs["to"] in self.__linkBuses:
-                        outputBusLabel = gs["to"]
-                    else:
-                        outputBusLabel = gs["to"]+'__'+self.__buildingLabel
-                else:
-                    label = gs["label"]+'__'+self.__buildingLabel
-                    inputBusLabel = gs["from"]+'__'+self.__buildingLabel
-                    outputBusLabel = gs["to"] + '__' + self.__buildingLabel
-
-                if (self.__buildingLabel in label) or (mergeLinkBuses and self.__buildingLabel=='Building1'):
-                    self.__nodesList.append(solph.Transformer(label=label,
-                                                              inputs={self.__busDict[inputBusLabel]: solph.Flow()},
-                                                              outputs={self.__busDict[outputBusLabel]: solph.Flow()},
-                                                      conversion_factors={self.__busDict[outputBusLabel]: float(gs["efficiency"])}))
-
-    def addSource(self, data, data_elimpact, data_elcost, data_natGascost, data_natGasImpact, opt):
-        # Create Source objects from table 'commodity sources'
-
-        for i, cs in data.iterrows():
-            if cs["active"]:
-                sourceLabel = cs["label"]+'__' + self.__buildingLabel
-                outputBusLabel = cs["to"] + '__' + self.__buildingLabel
-                # variable costs = (if opt == "costs") : cs["variable costs"]
-                #                  (if opt == "env") and ('electricity' in cs["label"]): data_elec["impact"]
-                #                  (if opt == "env") and ('electricity' not in cs["label"]): cs["CO2 impact"]
-                # env_per_flow = (if 'electricity' in cs["label"]) : data_elec["impact"]
-                #                 (if 'electricity' not in cs["label"]) : cs["CO2 impact"]
-                # self.__envParam is assigned the value data_elec["impact"] or cs["CO2 impact"] depending on whether ('electricity' is in cs["label"]) or not
-                if opt == "costs":
-                    if 'electricity' in cs["label"]:
-                        varCosts = data_elcost["cost"]
-                    elif 'naturalGas' in cs['label']:
-                        varCosts = data_natGascost["cost"]
-                    else:
-                        varCosts = float(cs["variable costs"])
-                elif 'electricity' in cs["label"]:
-                    varCosts = data_elimpact["impact"]
-                elif 'naturalGas' in cs["label"]:
-                    varCosts = data_natGasImpact["impact"]
-                else:
-                    varCosts = float(cs["CO2 impact"])
-
-                if 'electricity' in cs["label"]:
-                    envImpactPerFlow = data_elimpact["impact"]
-                    envParameter = data_elimpact["impact"]
-                    costParameter = data_elcost["cost"]
-                elif 'naturalGas' in cs['label']:
-                    envImpactPerFlow = data_natGasImpact["impact"]
-                    envParameter = data_natGasImpact["impact"]
-                    costParameter = data_natGascost["cost"]
-                else:
-                    envImpactPerFlow = float(cs["CO2 impact"])
-                    envParameter = float(cs["CO2 impact"])
-                    costParameter = float(cs["variable costs"])
-                    # add the inputs (natural gas, wood, etc...) to self.__inputs
-                    self.__inputs.append([sourceLabel, outputBusLabel])
-
-                self.__nodesList.append(solph.Source(
-                    label=sourceLabel,
-                    outputs={self.__busDict[outputBusLabel]: solph.Flow(
-                            variable_costs=varCosts,
-                            env_per_flow=envImpactPerFlow,
-                        )}))
-
-                # set environment and cost parameters
-                self.__envParam[sourceLabel] = envParameter
-                self.__costParam[sourceLabel] = costParameter
-
-    def addSink(self, data, timeseries, buildingModelParams, mergeLinkBuses):
-        # Create Sink objects with fixed time series from 'demand' table
-        for i, de in data.iterrows():
-            if de["active"]:
-                sinkLabel = de["label"]+'__'+self.__buildingLabel
-                if mergeLinkBuses and de["from"] in self.__linkBuses:
-                    inputBusLabel = de["from"]
-                else:
-                    inputBusLabel = de["from"]+'__'+self.__buildingLabel
-
-                if de["building model"] == 'Yes':   # Should a building model be used?
-                    # Only valid for SH demands at the moment
-                    # create sink
-                    self.__nodesList.append(
-                        SinkRCModel(
-                            tAmbient=buildingModelParams['tAmb'].values,
-                            totalIrradiationHorizontal=buildingModelParams['IrrH'].values,
-                            heatGainOccupants=buildingModelParams['Qocc'].values,
-                            label=sinkLabel,
-                            inputs={self.__busDict[inputBusLabel]: solph.Flow()},
-                        )
-                    )
-                else:
-                    # set static inflow values, if any
-                    inflow_args = {"nominal_value": float(de["nominal value"])}
-                    # get time series for node and parameter
-                    for col in timeseries.columns.values:
-                        if col == de["label"]:
-                            inflow_args["fix"] = timeseries[col]
-                    # create sink
-                    self.__nodesList.append(
-                        solph.Sink(
-                            label=sinkLabel,
-                            inputs={self.__busDict[inputBusLabel]: solph.Flow(**inflow_args)},
-                        )
-                    )
-
-    def _addHeatPump(self, data, temperatureDHW, temperatureSH, temperatureAmb, opt, mergeLinkBuses, dispatchMode):
-        hpSHLabel = data["label"] + '__' + self.__buildingLabel
-        if mergeLinkBuses and data["from"] in self.__linkBuses:
-            inputBusLabel = data["from"]
-        else:
-            inputBusLabel = data["from"] + '__' + self.__buildingLabel
-        outputSHBusLabel = data["to"].split(",")[0] + '__' + self.__buildingLabel
-        outputDHWBusLabel = data["to"].split(",")[1] + '__' + self.__buildingLabel
-        envImpactPerCapacity = float(data["impact_cap"]) / float(data["lifetime"])
-        if data["capacity_min"] == 'x':
-            capacityMinSH = float(data["capacity_SH"])
-        else:
-            capacityMinSH = float(data["capacity_min"])
-
-        heatPump = HeatPumpLinear(self.__buildingLabel, temperatureDHW, temperatureSH, temperatureAmb,
-                                  self.__busDict[inputBusLabel],
-                                  self.__busDict[outputSHBusLabel],
-                                  self.__busDict[outputDHWBusLabel],
-                                  capacityMinSH, float(data["capacity_SH"]),float(data["efficiency"]),
-                                  self._calculateInvest(data)[0] * (opt == "costs") + envImpactPerCapacity*(opt == "env"),
-                                  self._calculateInvest(data)[1] * (opt == "costs"),
-                                  float(data["heat_impact"]) * (opt == "env"),
-                                  float(data["heat_impact"]), envImpactPerCapacity, dispatchMode)
-
-        self.__nodesList.append(heatPump.getHP("sh"))
-
-        # set technologies, environment and cost parameters
-        self.__technologies.append([outputDHWBusLabel, hpSHLabel])
-        self.__technologies.append([outputSHBusLabel, hpSHLabel])
-
-        self.__costParam[hpSHLabel] = [self._calculateInvest(data)[0], self._calculateInvest(data)[1]]
-
-        self.__envParam[hpSHLabel] = [float(data["heat_impact"]), 0, envImpactPerCapacity]
-
-    def _addGeothemalHeatPump(self, data, temperatureDHW, temperatureSH, temperatureAmb, opt, mergeLinkBuses, dispatchMode):
-        gwhpSHLabel = data["label"] + '__' + self.__buildingLabel
-        if mergeLinkBuses and data["from"] in self.__linkBuses:
-            inputBusLabel = data["from"]
-        else:
-            inputBusLabel = data["from"] + '__' + self.__buildingLabel
-        outputSHBusLabel = data["to"].split(",")[0] + '__' + self.__buildingLabel
-        outputDHWBusLabel = data["to"].split(",")[1] + '__' + self.__buildingLabel
-        envImpactPerCapacity = float(data["impact_cap"]) / float(data["lifetime"])
-        if data["capacity_min"] == 'x':
-            capacityMinSH = float(data["capacity_SH"])
-        else:
-            capacityMinSH = float(data["capacity_min"])
-        geothermalheatPump = GeothermalHeatPumpLinear(self.__buildingLabel, temperatureDHW, temperatureSH, temperatureAmb,
-                                  self.__busDict[inputBusLabel],
-                                  self.__busDict[outputSHBusLabel],
-                                  self.__busDict[outputDHWBusLabel],
-                                  capacityMinSH, float(data["capacity_SH"]),float(data["efficiency"]),
-                                  self._calculateInvest(data)[0] * (opt == "costs") + envImpactPerCapacity*(opt == "env"),
-                                  self._calculateInvest(data)[1] * (opt == "costs"),
-                                  float(data["heat_impact"]) * (opt == "env"),
-                                  float(data["heat_impact"]), envImpactPerCapacity, dispatchMode)
-
-        self.__nodesList.append(geothermalheatPump.getHP("sh"))
-
-        # set technologies, environment and cost parameters
-        self.__technologies.append([outputDHWBusLabel, gwhpSHLabel])
-        self.__technologies.append([outputSHBusLabel, gwhpSHLabel])
-
-        self.__costParam[gwhpSHLabel] = [self._calculateInvest(data)[0], self._calculateInvest(data)[1]]
-
-        self.__envParam[gwhpSHLabel] = [float(data["heat_impact"]), 0, envImpactPerCapacity]
-
-    def _addGeothemalHeatPumpSplit(self, data, temperatureDHW, temperatureSH, temperatureAmb, opt, mergeLinkBuses, dispatchMode):
-        gwhpDHWLabel = data["label"][0:4] + str(temperatureDHW) + '__' + self.__buildingLabel
-        gwhpSHLabel = data["label"][0:4] + str(temperatureSH) + '__' + self.__buildingLabel
-        if mergeLinkBuses and data["from"] in self.__linkBuses:
-            inputBusLabel = data["from"]
-        else:
-            inputBusLabel = data["from"] + '__' + self.__buildingLabel
-        outputSHBusLabel = data["to"].split(",")[0] + '__' + self.__buildingLabel
-        outputDHWBusLabel = data["to"].split(",")[1] + '__' + self.__buildingLabel
-        envImpactPerCapacity = float(data["impact_cap"]) / float(data["lifetime"])
-        capacityDHW = float(data["capacity_DHW"])
-        capacitySH = float(data["capacity_SH"])
-        if data["capacity_min"] == 'x':
-            capacityMinSH = capacitySH
-            capacityMinDHW = capacityDHW
-        else:
-            capacityMinSH = capacityMinDHW = float(data["capacity_min"])
-
-        geothermalheatPumpSH = GeothermalHeatPumpLinearSingleUse(self.__buildingLabel, temperatureSH, temperatureAmb,
-                                  self.__busDict[inputBusLabel],
-                                  self.__busDict[outputSHBusLabel],
-                                  capacityMinSH, capacitySH,
-                                  self._calculateInvest(data)[0] * (opt == "costs") + envImpactPerCapacity*(opt == "env"),
-                                  self._calculateInvest(data)[1] * (opt == "costs"),
-                                  float(data["heat_impact"]) * (opt == "env"),
-                                  float(data["heat_impact"]), envImpactPerCapacity, dispatchMode)
-        geothermalheatPumpDHW = GeothermalHeatPumpLinearSingleUse(self.__buildingLabel, temperatureDHW,
-                                                        temperatureAmb,
-                                                        self.__busDict[inputBusLabel],
-                                                        self.__busDict[outputDHWBusLabel],
-                                                        capacityMinDHW, capacityDHW,
-                                                        self._calculateInvest(data)[0] * (
-                                                                    opt == "costs") + envImpactPerCapacity * (
-                                                                    opt == "env"),
-                                                        self._calculateInvest(data)[1] * (opt == "costs"),
-                                                        float(data["heat_impact"]) * (opt == "env"),
-                                                        float(data["heat_impact"]), envImpactPerCapacity, dispatchMode)
-
-        self.__nodesList.append(geothermalheatPumpSH.getHP("sh"))
-        self.__nodesList.append(geothermalheatPumpDHW.getHP("sh"))
-
-        # set technologies, environment and cost parameters
-        self.__technologies.append([outputDHWBusLabel, gwhpDHWLabel])
-        self.__technologies.append([outputSHBusLabel, gwhpSHLabel])
-
-        self.__costParam[gwhpSHLabel] = [self._calculateInvest(data)[0], self._calculateInvest(data)[1]]
-        self.__costParam[gwhpDHWLabel] = [self._calculateInvest(data)[0], self._calculateInvest(data)[1]]
-
-        self.__envParam[gwhpSHLabel] = [float(data["heat_impact"]), 0, envImpactPerCapacity]
-        self.__envParam[gwhpDHWLabel] = [float(data["heat_impact"]), 0, envImpactPerCapacity]
-
-    def _addCHP(self, data, timesteps, opt, dispatchMode):
-        chpSHLabel = data["label"] + '__' + self.__buildingLabel
-        inputBusLabel = data["from"] + '__' + self.__buildingLabel
-        outputElBusLabel = data["to"].split(",")[0] + '__' + self.__buildingLabel
-        outputSHBusLabel = data["to"].split(",")[1] + '__' + self.__buildingLabel
-        outputDHWBusLabel = data["to"].split(",")[2] + '__' + self.__buildingLabel
-        elEfficiency = float(data["efficiency"].split(",")[0])
-        shEfficiency = float(data["efficiency"].split(",")[1])
-        dhwEfficiency = float(data["efficiency"].split(",")[2])
-        envImpactPerCapacity = float(data["impact_cap"]) / float(data["lifetime"])
-        if data["capacity_min"] == 'x':
-            capacityMinSH = float(data["capacity_SH"])
-        else:
-            capacityMinSH = float(data["capacity_min"])
-        chp = CHP(self.__buildingLabel, self.__busDict[inputBusLabel],
-                  self.__busDict[outputElBusLabel],
-                  self.__busDict[outputSHBusLabel],
-                  self.__busDict[outputDHWBusLabel],
-                  elEfficiency, shEfficiency,
-                  dhwEfficiency, capacityMinSH,
-                  float(data["capacity_SH"]),
-                  self._calculateInvest(data)[0] * (opt == "costs") + envImpactPerCapacity * (opt == "env"),
-                  self._calculateInvest(data)[1] * (opt == "costs"), float(data["elec_impact"]) * (opt == "env"),
-                  float(data["heat_impact"]) * (opt == "env"),
-                  float(data["elec_impact"]), float(data["heat_impact"]), envImpactPerCapacity, timesteps, dispatchMode)
-
-        self.__nodesList.append(chp.getCHP("sh"))
-
-        # set technologies, environment and cost parameters
-        self.__technologies.append([outputElBusLabel, chpSHLabel])
-        self.__technologies.append([outputSHBusLabel, chpSHLabel])
-        self.__technologies.append([outputDHWBusLabel, chpSHLabel])
-
-        self.__costParam[chpSHLabel] = [self._calculateInvest(data)[0], self._calculateInvest(data)[1]]
-
-        self.__envParam[chpSHLabel] = [float(data["heat_impact"]), float(data["elec_impact"]), envImpactPerCapacity]
-
-    def _addGasBoiler(self, data, opt, dispatchMode):
-        gasBoilLabel = data["label"] + '__' + self.__buildingLabel
-        inputBusLabel = data["from"] + '__' + self.__buildingLabel
-        outputSHBusLabel = data["to"].split(",")[0] + '__' + self.__buildingLabel
-        outputDHWBusLabel = data["to"].split(",")[1] + '__' + self.__buildingLabel
-        shEfficiency = float(data["efficiency"].split(",")[0])
-        dhwEfficiency = float(data["efficiency"].split(",")[1])
-        envImpactPerCapacity = float(data["impact_cap"]) / float(data["lifetime"])
-        if data["capacity_min"] == 'x':
-            capacityMinSH = float(data["capacity_SH"])
-        else:
-            capacityMinSH = float(data["capacity_min"])
-
-        self.__nodesList.append(GasBoiler(self.__buildingLabel, self.__busDict[inputBusLabel],
-                  self.__busDict[outputSHBusLabel], self.__busDict[outputDHWBusLabel],
-                  shEfficiency, dhwEfficiency, capacityMinSH, float(data["capacity_SH"]),
-                  self._calculateInvest(data)[0] * (opt == "costs") + envImpactPerCapacity * (opt == "env"),
-                  self._calculateInvest(data)[1] * (opt == "costs"), float(data["heat_impact"]) * (opt == "env"), float(data["heat_impact"]), envImpactPerCapacity, dispatchMode))
-
-        # set technologies, environment and cost parameters
-        self.__technologies.append([outputSHBusLabel, gasBoilLabel])
-        self.__technologies.append([outputDHWBusLabel, gasBoilLabel])
-
-        self.__costParam[gasBoilLabel] = [self._calculateInvest(data)[0], self._calculateInvest(data)[1]]
-
-        self.__envParam[gasBoilLabel] = [float(data["heat_impact"]), 0, envImpactPerCapacity]
-
-    def _addElectricRod(self, data, opt, mergeLinkBuses, dispatchMode):
-        elRodLabel = data["label"] + '__' + self.__buildingLabel
-        if mergeLinkBuses and data["from"] in self.__linkBuses:
-            inputBusLabel = data["from"]
-        else:
-            inputBusLabel = data["from"] + '__' + self.__buildingLabel
-        outputSHBusLabel = data["to"].split(",")[0] + '__' + self.__buildingLabel
-        outputDHWBusLabel = data["to"].split(",")[1] + '__' + self.__buildingLabel
-        efficiency = float(data["efficiency"])
-        envImpactPerCapacity = float(data["impact_cap"]) / float(data["lifetime"])
-        if data["capacity_min"] == 'x':
-            capacityMinSH = float(data["capacity_SH"])
-        else:
-            capacityMinSH = float(data["capacity_min"])
-
-        self.__nodesList.append(ElectricRod(self.__buildingLabel, self.__busDict[inputBusLabel],
-                                          self.__busDict[outputSHBusLabel], self.__busDict[outputDHWBusLabel],
-                                          efficiency, capacityMinSH, float(data["capacity_SH"]),
-                                          self._calculateInvest(data)[0] * (opt == "costs") + envImpactPerCapacity * (
-                                                      opt == "env"),
-                                          self._calculateInvest(data)[1] * (opt == "costs"),
-                                          float(data["heat_impact"]) * (opt == "env"), float(data["heat_impact"]),
-                                          envImpactPerCapacity, dispatchMode))
-
-        # set technologies, environment and cost parameters
-        self.__technologies.append([outputSHBusLabel, elRodLabel])
-        self.__technologies.append([outputDHWBusLabel, elRodLabel])
-
-        self.__costParam[elRodLabel] = [self._calculateInvest(data)[0], self._calculateInvest(data)[1]]
-
-        self.__envParam[elRodLabel] = [float(data["heat_impact"]), 0, envImpactPerCapacity]
-
-    def addTransformer(self, data, temperatureDHW, temperatureSH, temperatureAmb, temperatureGround, opt, mergeLinkBuses, dispatchMode):
-        for i, t in data.iterrows():
-            if t["active"]:
-                if t["label"] == "HP":
-                    self._addHeatPump(t, temperatureDHW, temperatureSH, temperatureAmb, opt, mergeLinkBuses, dispatchMode)
-                elif t["label"] == "GWHP":
-                    self._addGeothemalHeatPump(t, temperatureDHW, temperatureSH, temperatureGround, opt, mergeLinkBuses, dispatchMode)
-                elif t["label"] == "GWHP split":
-                    self._addGeothemalHeatPumpSplit(t, temperatureDHW, temperatureSH, temperatureGround, opt, mergeLinkBuses, dispatchMode)
-                elif t["label"] == "CHP":
-                    self._addCHP(t, len(temperatureAmb), opt, dispatchMode)
-                elif t["label"] == "GasBoiler":
-                    self._addGasBoiler(t, opt, dispatchMode)
-                elif t["label"] == "ElectricRod":
-                    self._addElectricRod(t, opt, mergeLinkBuses, dispatchMode)
-                else:
-                    logging.warning("Transformer label not identified...")
-
-    def addStorage(self, data, stratifiedStorageParams, opt, mergeLinkBuses, dispatchMode):
-        for i, s in data.iterrows():
-            if s["active"]:
-                storageLabel = s["label"]+'__'+self.__buildingLabel
-                if mergeLinkBuses and s["from"] in self.__linkBuses:
-                    inputBusLabel = s["from"]
-                else:
-                    inputBusLabel = s["from"]+'__'+self.__buildingLabel
-                if mergeLinkBuses and s["to"] in self.__linkBuses:
-                    outputBusLabel = s["to"]
-                else:
-                    outputBusLabel = s["to"]+'__'+self.__buildingLabel
-                envImpactPerCapacity = float(s["impact_cap"]) / float(s["lifetime"])         # annualized value
-                # set technologies, environment and cost parameters
-                self.__costParam[storageLabel] = [self._calculateInvest(s)[0], self._calculateInvest(s)[1]]
-                self.__envParam[storageLabel] = [float(s["heat_impact"]), float(s["elec_impact"]), envImpactPerCapacity]
-                self.__technologies.append([outputBusLabel, storageLabel])
-
-                if s["label"] == "electricalStorage":
-                    self.__nodesList.append(ElectricalStorage(self.__buildingLabel, self.__busDict[inputBusLabel],
-                                                              self.__busDict[outputBusLabel], float(s["capacity loss"]),
-                                                            float(s["initial capacity"]), float(s["efficiency inflow"]),
-                                                            float(s["efficiency outflow"]), float(s["capacity min"]),
-                                                            float(s["capacity max"]),
-                                                            self._calculateInvest(s)[0]*(opt == "costs") + envImpactPerCapacity*(opt == "env"),
-                                                            self._calculateInvest(s)[1]*(opt == "costs"),
-                                                            float(s["elec_impact"])*(opt == "env"),
-                                                            float(s["elec_impact"]), envImpactPerCapacity, dispatchMode))
-
-                elif s["label"] == "dhwStorage" or s["label"] == "shStorage":
-                    ts = ThermalStorage(storageLabel, s["label"],
-                                                           stratifiedStorageParams, self.__busDict[inputBusLabel],
-                                                           self.__busDict[outputBusLabel],
-                                                        float(s["initial capacity"]), float(s["capacity min"]),
-                                                        float(s["capacity max"]),
-                                                        self._calculateInvest(s)[0]*(opt == "costs") + envImpactPerCapacity*(opt == "env"),
-                                                        self._calculateInvest(s)[1]*(opt == "costs"), float(s["heat_impact"])*(opt == "env"),
-                                                        float(s["heat_impact"]), envImpactPerCapacity, dispatchMode)
-                    self.__nodesList.append(ts.getStorage())
-                else:
-                    logging.warning("Storage label not identified")
-
-    def _calculateInvest(self, data):
-        # Calculate the CAPEX and the part of the OPEX not related to energy flows (maintenance)
-        c = data["installation"] + data["planification"] + 1
-        m = data["maintenance"]
-        perCapacity = m * data["invest_cap"] + economics.annuity(c * data["invest_cap"], data["lifetime"], intRate)
-        base = m * data["invest_base"] + economics.annuity(c * data["invest_base"], data["lifetime"], intRate)
+import numpy as np
+import oemof.solph as solph
+import pandas as pd
+from oemof.tools import logger
+from oemof.tools import economics
+import logging
+from optihood.converters import *
+from optihood.sources import PV
+from optihood.storages import ElectricalStorage, ThermalStorage
+from optihood.sinks import SinkRCModel
+
+intRate = 0.05
+
+class Building:
+    def __init__(self, label):
+        self.__nodesList = []
+        self.__inputs = []
+        self.__technologies = []
+        self.__costParam = {}
+        self.__envParam = {}
+        self.__busDict = {}
+        self.__buildingLabel = label
+        self.__linkBuses = ["electricityBus", "electricityInBus", "domesticHotWaterBus", "dhwDemandBus", "spaceHeatingBus", "shDemandBus"]
+
+    def getBuildingLabel(self):
+        return self.__buildingLabel
+
+    def getNodesList(self):
+        return self.__nodesList
+
+    def getBusDict(self):
+        return self.__busDict
+
+    def getInputs(self):
+        return self.__inputs
+
+    def getTechnologies(self):
+        return self.__technologies
+
+    def getCostParam(self):
+        return self.__costParam
+
+    def getEnvParam(self):
+        return self.__envParam
+
+    def addBus(self, data, opt, mergeLinkBuses, electricityImpact, clusterSize, includeCarbonBenefits):
+        # Create Bus objects from buses table
+        for i, b in data.iterrows():
+            if b["active"]:
+                if mergeLinkBuses and b["label"] in self.__linkBuses:
+                    label = b["label"]
+                else:
+                    label = b["label"] + '__' + self.__buildingLabel
+
+                if not mergeLinkBuses or (mergeLinkBuses and (self.__buildingLabel=='Building1' or label not in self.__linkBuses)):
+                    bus = solph.Bus(label=label)
+                    self.__nodesList.append(bus)
+                    self.__busDict[label] = bus
+                    if opt=='costs':
+                        if not clusterSize: varcost=float(b["excess costs"])
+                        else:
+                            varcost = None
+                            for d in clusterSize:
+                                temp = pd.Series(np.tile([float(b["excess costs"])*clusterSize[d]], 24))
+                                if varcost is not None:
+                                    varcost = varcost.append(temp, ignore_index=True)
+                                else:
+                                    varcost = temp
+                    elif opt=='env' and includeCarbonBenefits:varcost=-electricityImpact['impact']
+                    else: varcost=0
+                    if b["excess"]:
+                        self.__nodesList.append(
+                            solph.Sink(
+                                label="excess"+label,
+                                inputs={
+                                    self.__busDict[label]: solph.Flow(
+                                        variable_costs=varcost
+                                    )}))
+                        # add the excess production cost to self.__costParam
+                        self.__costParam["excess"+label] = float(b["excess costs"])
+        if mergeLinkBuses and self.__buildingLabel=='Building1':
+            return self.__busDict
+
+    def addToBusDict(self, busDictBuilding1):
+        for label in self.__linkBuses:
+            self.__busDict[label] = busDictBuilding1[label]
+
+    def addPV(self, data, data_timeseries, opt, dispatchMode):
+        # Create Source objects from table 'commodity sources'
+        for i, s in data.iterrows():
+            if opt == "costs":
+                epc=self._calculateInvest(s)[0]
+                base=self._calculateInvest(s)[1]
+                env_capa=float(s["impact_cap"]) / float(s["lifetime"])
+                env_flow=float(s["elec_impact"])
+                varc=0 # variable cost is only passed for environmental optimization if there are emissions per kWh of energy produced from the unit
+
+                envParam = [0, float(s["elec_impact"]), float(s["impact_cap"]) / float(s["lifetime"])]
+
+            elif opt == "env":
+                epc = float(s["impact_cap"]) / float(s["lifetime"])
+                base = 0
+                env_capa = float(s["impact_cap"]) / float(s["lifetime"])
+                env_flow = float(s["elec_impact"])
+                varc = float(s["elec_impact"]) # variable cost is only passed for environmental optimization if there are emissions per kWh of energy produced from the unit
+
+                envParam = [0, float(s["elec_impact"]), float(s["impact_cap"]) / float(s["lifetime"])]
+
+            # If roof area and zenith do not exist in the excel file
+            if 'roof_area' not in s.keys():
+                s["roof_area"] = np.nan
+            if 'zenith_angle' not in s.keys():
+                s["zenith_angle"] = np.nan
+            if 'efficiency' not in s.keys():
+                s["efficiency"] = np.nan
+
+            self.__nodesList.append(PV(s["label"], self.__buildingLabel,
+                                       self.__busDict[s["to"] + '__' + self.__buildingLabel],
+                                       float(s["peripheral_losses"]), float(s["latitude"]), float(s["longitude"]),
+                                       float(s["tilt"]), float(s["efficiency"]), s["roof_area"],
+                                       s["zenith_angle"], s["azimuth"],
+                                       data_timeseries['gls'],
+                                       data_timeseries['str.diffus'],
+                                       data_timeseries['tre200h0'], float(s["capacity_min"]), float(s["capacity_max"]),
+                                       epc, base, env_capa, env_flow, varc, dispatchMode))
+
+            self.__envParam[s["label"] + '__' + self.__buildingLabel] = envParam
+
+            self.__costParam[s["label"] + '__' + self.__buildingLabel] = [self._calculateInvest(s)[0],
+                                                                          self._calculateInvest(s)[1]]
+            self.__technologies.append(
+                [s["to"] + '__' + self.__buildingLabel, s["label"] + '__' + self.__buildingLabel])
+
+    def addSolar(self, data, data_timeseries, opt, mergeLinkBuses, dispatchMode):
+        # Create Source objects from table 'commodity sources'
+        for i, s in data.iterrows():
+            if mergeLinkBuses and s["from"] in self.__linkBuses:
+                inputBusLabel = s["from"]
+            else:
+                inputBusLabel = s["from"] + '__' + self.__buildingLabel
+
+            if opt == "costs":
+                epc=self._calculateInvest(s)[0]
+                base=self._calculateInvest(s)[1]
+                env_capa=float(s["impact_cap"]) / float(s["lifetime"])
+                env_flow=float(s["heat_impact"])
+                varc=0 # variable cost is only passed for environmental optimization if there are emissions per kWh of energy produced from the unit
+
+                envParam = [env_flow, 0, env_capa]
+
+            elif opt == "env":
+                epc=float(s["impact_cap"]) / float(s["lifetime"])
+                base=0
+                env_capa= float(s["impact_cap"]) / float(s["lifetime"])
+                env_flow=float(s["heat_impact"])
+                varc= float(s["heat_impact"]) # variable cost is only passed for environmental optimization if there are emissions per kWh of energy produced from the unit
+
+                envParam = [env_flow, 0, env_capa]
+
+            # If roof area and zenith do not exist in the excel file
+            if 'roof_area' not in s.keys():
+                s["roof_area"] = np.nan
+            if 'zenith_angle' not in s.keys():
+                s["zenith_angle"] = np.nan
+            collector=SolarCollector(s["label"], self.__buildingLabel,
+                                                   self.__busDict[inputBusLabel],
+                                                   self.__busDict[s["to"] + '__' + self.__buildingLabel],
+                                                   self.__busDict[s["connect"]+ '__' + self.__buildingLabel],
+                                                   float(s["electrical_consumption"]), float(s["peripheral_losses"]), float(s["latitude"]),
+                                                   float(s["longitude"]), float(s["tilt"]), s["roof_area"],
+                                                   s["zenith_angle"], float(s["azimuth"]),
+                                                   float(s["eta_0"]), float(s["a_1"]), float(s["a_2"]), float(s["temp_collector_inlet"]),
+                                                   float(s["delta_temp_n"]), data_timeseries['gls'], data_timeseries['str.diffus'],
+                                                    data_timeseries['tre200h0'], float(s["capacity_min"]), float(s["capacity_max"]),
+                                                   epc, base, env_capa, env_flow, varc, dispatchMode)
+            self.__nodesList.append(collector.getSolar("source"))
+            self.__nodesList.append(collector.getSolar("transformer"))
+            self.__nodesList.append(collector.getSolar("sink"))
+
+            self.__envParam["heat_"+s["label"] + '__' + self.__buildingLabel] = envParam
+
+            self.__costParam["heat_"+s["label"] + '__' + self.__buildingLabel] = [self._calculateInvest(s)[0],
+                                                                          self._calculateInvest(s)[1]]
+            self.__technologies.append(
+                [s["to"] + '__' + self.__buildingLabel, s["label"] + '__' + self.__buildingLabel])
+
+    def addPVT(self, data, data_timeseries, opt, mergeLinkBuses, dispatchMode):
+        # Create Source objects from table 'commodity sources'
+        for i, s in data.iterrows():
+            if s["active"]:
+                if mergeLinkBuses and s["from"] in self.__linkBuses:
+                    inputBusLabel = s["from"]
+                else:
+                    inputBusLabel = s["from"] + '__' + self.__buildingLabel
+
+                outputBuses = [self.__busDict[s["to"].split(",")[0] + '__' + self.__buildingLabel],
+                               self.__busDict[s["to"].split(",")[1] + '__' + self.__buildingLabel],
+                               self.__busDict[s["to"].split(",")[2] + '__' + self.__buildingLabel]]
+                connectBuses = [self.__busDict[s["connect"].split(",")[0] + '__' + self.__buildingLabel],
+                               self.__busDict[s["connect"].split(",")[1] + '__' + self.__buildingLabel]]
+                if opt == "costs":
+                    epc = self._calculateInvest(s)[0]
+                    base = self._calculateInvest(s)[1]
+                    env_capa = float(s["impact_cap"]) / float(s["lifetime"])
+                    env_flow = float(s["heat_impact"])
+                    varc = 0  # variable cost is only passed for environmental optimization if there are emissions per kWh of energy produced from the unit
+
+                    envParam = [env_flow, 0, env_capa]
+
+                elif opt == "env":
+                    epc = float(s["impact_cap"]) / float(s["lifetime"])
+                    base = 0
+                    env_capa = float(s["impact_cap"]) / float(s["lifetime"])
+                    env_flow = float(s["heat_impact"])
+                    varc = float(s[
+                                     "heat_impact"])  # variable cost is only passed for environmental optimization if there are emissions per kWh of energy produced from the unit
+
+                    envParam = [env_flow, 0, env_capa]
+
+                # If roof area does not exist in the excel file
+                if 'roof_area' not in s.keys():
+                    s["roof_area"] = np.nan
+                else:
+                    s["roof_area"] = float(s["roof_area"])
+                pvtcollector = PVT(s["label"], self.__buildingLabel,
+                                                       self.__busDict[inputBusLabel],
+                                                       outputBuses,
+                                                       connectBuses,
+                                                       float(s["electrical_consumption"]), float(s["peripheral_losses"]), float(s["latitude"]),
+                                                       float(s["longitude"]), float(s["tilt"]), s["roof_area"],
+                                                       float(s["zenith_angle"]), float(s["azimuth"]),
+                                                       float(s["eta_0"]), float(s["a_1"]), float(s["a_2"]), float(s["temp_collector_inlet"]),data_timeseries['tre200h0'],
+                                                       float(s["delta_temp_n"]), data_timeseries['gls'], data_timeseries['str.diffus'], float(s["capacity_min"]), float(s["capacity_max"]),
+                                                       epc, base, env_capa, env_flow, varc, dispatchMode,
+                                                        float(s["pv_efficiency"]))
+                nodes = [pvtcollector.getPVT("el_source")]
+                for t in ["heat_source", "heat_transformer", "excess_heat_sink"]:
+                    nodes.append(pvtcollector.getPVT(t))
+                for x in nodes:
+                    self.__nodesList.append(x)
+
+
+                self.__envParam['heatSourceSH_' + s['label'] + '__' + self.__buildingLabel] = envParam
+                self.__envParam['heatSourceDHW_' + s['label'] + '__' + self.__buildingLabel] = [env_flow, 0, 0]
+                self.__costParam['heatSourceSH_' + s['label'] + '__' + self.__buildingLabel] = [self._calculateInvest(s)[0],
+                                                                                            self._calculateInvest(s)[1]]
+                self.__costParam['heatSourceDHW_' + s['label'] + '__' + self.__buildingLabel] = [0, 0]
+
+                self.__technologies.append(
+                    [outputBuses[0], s["label"] + 'SH__' + self.__buildingLabel])
+                self.__technologies.append(
+                    [outputBuses[1], s["label"] + 'DHW__' + self.__buildingLabel])
+
+    def addGridSeparation(self, dataGridSeparation, mergeLinkBuses):
+        if not dataGridSeparation.empty:
+            for i, gs in dataGridSeparation.iterrows():
+                if mergeLinkBuses:
+                    if gs["label"] in ['gridElectricity','electricitySource','shSource']:
+                        label = gs["label"]+'__'+self.__buildingLabel
+                    else:
+                        label = gs["label"]
+                    if gs["from"] in self.__linkBuses:
+                        inputBusLabel = gs["from"]
+                    else:
+                        inputBusLabel = gs["from"]+'__'+self.__buildingLabel
+                    if gs["to"] in self.__linkBuses:
+                        outputBusLabel = gs["to"]
+                    else:
+                        outputBusLabel = gs["to"]+'__'+self.__buildingLabel
+                else:
+                    label = gs["label"]+'__'+self.__buildingLabel
+                    inputBusLabel = gs["from"]+'__'+self.__buildingLabel
+                    outputBusLabel = gs["to"] + '__' + self.__buildingLabel
+
+                if (self.__buildingLabel in label) or (mergeLinkBuses and self.__buildingLabel=='Building1'):
+                    self.__nodesList.append(solph.Transformer(label=label,
+                                                              inputs={self.__busDict[inputBusLabel]: solph.Flow()},
+                                                              outputs={self.__busDict[outputBusLabel]: solph.Flow()},
+                                                      conversion_factors={self.__busDict[outputBusLabel]: float(gs["efficiency"])}))
+
+    def addSource(self, data, data_elimpact, data_elcost, data_natGascost, data_natGasImpact, opt):
+        # Create Source objects from table 'commodity sources'
+
+        for i, cs in data.iterrows():
+            if cs["active"]:
+                sourceLabel = cs["label"]+'__' + self.__buildingLabel
+                outputBusLabel = cs["to"] + '__' + self.__buildingLabel
+                # variable costs = (if opt == "costs") : cs["variable costs"]
+                #                  (if opt == "env") and ('electricity' in cs["label"]): data_elec["impact"]
+                #                  (if opt == "env") and ('electricity' not in cs["label"]): cs["CO2 impact"]
+                # env_per_flow = (if 'electricity' in cs["label"]) : data_elec["impact"]
+                #                 (if 'electricity' not in cs["label"]) : cs["CO2 impact"]
+                # self.__envParam is assigned the value data_elec["impact"] or cs["CO2 impact"] depending on whether ('electricity' is in cs["label"]) or not
+                if opt == "costs":
+                    if 'electricity' in cs["label"]:
+                        varCosts = data_elcost["cost"]
+                    elif 'naturalGas' in cs['label']:
+                        varCosts = data_natGascost["cost"]
+                    else:
+                        varCosts = float(cs["variable costs"])
+                elif 'electricity' in cs["label"]:
+                    varCosts = data_elimpact["impact"]
+                elif 'naturalGas' in cs["label"]:
+                    varCosts = data_natGasImpact["impact"]
+                else:
+                    varCosts = float(cs["CO2 impact"])
+
+                if 'electricity' in cs["label"]:
+                    envImpactPerFlow = data_elimpact["impact"]
+                    envParameter = data_elimpact["impact"]
+                    costParameter = data_elcost["cost"]
+                elif 'naturalGas' in cs['label']:
+                    envImpactPerFlow = data_natGasImpact["impact"]
+                    envParameter = data_natGasImpact["impact"]
+                    costParameter = data_natGascost["cost"]
+                else:
+                    envImpactPerFlow = float(cs["CO2 impact"])
+                    envParameter = float(cs["CO2 impact"])
+                    costParameter = float(cs["variable costs"])
+                    # add the inputs (natural gas, wood, etc...) to self.__inputs
+                    self.__inputs.append([sourceLabel, outputBusLabel])
+
+                self.__nodesList.append(solph.Source(
+                    label=sourceLabel,
+                    outputs={self.__busDict[outputBusLabel]: solph.Flow(
+                            variable_costs=varCosts,
+                            env_per_flow=envImpactPerFlow,
+                        )}))
+
+                # set environment and cost parameters
+                self.__envParam[sourceLabel] = envParameter
+                self.__costParam[sourceLabel] = costParameter
+
+    def addSink(self, data, timeseries, buildingModelParams, mergeLinkBuses):
+        # Create Sink objects with fixed time series from 'demand' table
+        for i, de in data.iterrows():
+            if de["active"]:
+                sinkLabel = de["label"]+'__'+self.__buildingLabel
+                if mergeLinkBuses and de["from"] in self.__linkBuses:
+                    inputBusLabel = de["from"]
+                else:
+                    inputBusLabel = de["from"]+'__'+self.__buildingLabel
+
+                if de["building model"] == 'Yes':   # Should a building model be used?
+                    # Only valid for SH demands at the moment
+                    # create sink
+                    self.__nodesList.append(
+                        SinkRCModel(
+                            tAmbient=buildingModelParams['tAmb'].values,
+                            totalIrradiationHorizontal=buildingModelParams['IrrH'].values,
+                            heatGainOccupants=buildingModelParams['Qocc'].values,
+                            label=sinkLabel,
+                            inputs={self.__busDict[inputBusLabel]: solph.Flow()},
+                        )
+                    )
+                else:
+                    # set static inflow values, if any
+                    inflow_args = {"nominal_value": float(de["nominal value"])}
+                    # get time series for node and parameter
+                    for col in timeseries.columns.values:
+                        if col == de["label"]:
+                            inflow_args["fix"] = timeseries[col]
+                    # create sink
+                    self.__nodesList.append(
+                        solph.Sink(
+                            label=sinkLabel,
+                            inputs={self.__busDict[inputBusLabel]: solph.Flow(**inflow_args)},
+                        )
+                    )
+
+    def _addHeatPump(self, data, temperatureDHW, temperatureSH, temperatureAmb, opt, mergeLinkBuses, dispatchMode):
+        hpSHLabel = data["label"] + '__' + self.__buildingLabel
+        if mergeLinkBuses and data["from"] in self.__linkBuses:
+            inputBusLabel = data["from"]
+        else:
+            inputBusLabel = data["from"] + '__' + self.__buildingLabel
+        outputSHBusLabel = data["to"].split(",")[0] + '__' + self.__buildingLabel
+        outputDHWBusLabel = data["to"].split(",")[1] + '__' + self.__buildingLabel
+        envImpactPerCapacity = float(data["impact_cap"]) / float(data["lifetime"])
+        if data["capacity_min"] == 'x':
+            capacityMinSH = float(data["capacity_SH"])
+        else:
+            capacityMinSH = float(data["capacity_min"])
+
+        heatPump = HeatPumpLinear(self.__buildingLabel, temperatureDHW, temperatureSH, temperatureAmb,
+                                  self.__busDict[inputBusLabel],
+                                  self.__busDict[outputSHBusLabel],
+                                  self.__busDict[outputDHWBusLabel],
+                                  capacityMinSH, float(data["capacity_SH"]),float(data["efficiency"]),
+                                  self._calculateInvest(data)[0] * (opt == "costs") + envImpactPerCapacity*(opt == "env"),
+                                  self._calculateInvest(data)[1] * (opt == "costs"),
+                                  float(data["heat_impact"]) * (opt == "env"),
+                                  float(data["heat_impact"]), envImpactPerCapacity, dispatchMode)
+
+        self.__nodesList.append(heatPump.getHP("sh"))
+
+        # set technologies, environment and cost parameters
+        self.__technologies.append([outputDHWBusLabel, hpSHLabel])
+        self.__technologies.append([outputSHBusLabel, hpSHLabel])
+
+        self.__costParam[hpSHLabel] = [self._calculateInvest(data)[0], self._calculateInvest(data)[1]]
+
+        self.__envParam[hpSHLabel] = [float(data["heat_impact"]), 0, envImpactPerCapacity]
+
+    def _addGeothemalHeatPump(self, data, temperatureDHW, temperatureSH, temperatureAmb, opt, mergeLinkBuses, dispatchMode):
+        gwhpSHLabel = data["label"] + '__' + self.__buildingLabel
+        if mergeLinkBuses and data["from"] in self.__linkBuses:
+            inputBusLabel = data["from"]
+        else:
+            inputBusLabel = data["from"] + '__' + self.__buildingLabel
+        outputSHBusLabel = data["to"].split(",")[0] + '__' + self.__buildingLabel
+        outputDHWBusLabel = data["to"].split(",")[1] + '__' + self.__buildingLabel
+        envImpactPerCapacity = float(data["impact_cap"]) / float(data["lifetime"])
+        if data["capacity_min"] == 'x':
+            capacityMinSH = float(data["capacity_SH"])
+        else:
+            capacityMinSH = float(data["capacity_min"])
+        geothermalheatPump = GeothermalHeatPumpLinear(self.__buildingLabel, temperatureDHW, temperatureSH, temperatureAmb,
+                                  self.__busDict[inputBusLabel],
+                                  self.__busDict[outputSHBusLabel],
+                                  self.__busDict[outputDHWBusLabel],
+                                  capacityMinSH, float(data["capacity_SH"]),float(data["efficiency"]),
+                                  self._calculateInvest(data)[0] * (opt == "costs") + envImpactPerCapacity*(opt == "env"),
+                                  self._calculateInvest(data)[1] * (opt == "costs"),
+                                  float(data["heat_impact"]) * (opt == "env"),
+                                  float(data["heat_impact"]), envImpactPerCapacity, dispatchMode)
+
+        self.__nodesList.append(geothermalheatPump.getHP("sh"))
+
+        # set technologies, environment and cost parameters
+        self.__technologies.append([outputDHWBusLabel, gwhpSHLabel])
+        self.__technologies.append([outputSHBusLabel, gwhpSHLabel])
+
+        self.__costParam[gwhpSHLabel] = [self._calculateInvest(data)[0], self._calculateInvest(data)[1]]
+
+        self.__envParam[gwhpSHLabel] = [float(data["heat_impact"]), 0, envImpactPerCapacity]
+
+    def _addGeothemalHeatPumpSplit(self, data, temperatureDHW, temperatureSH, temperatureAmb, opt, mergeLinkBuses, dispatchMode):
+        gwhpDHWLabel = data["label"][0:4] + str(temperatureDHW) + '__' + self.__buildingLabel
+        gwhpSHLabel = data["label"][0:4] + str(temperatureSH) + '__' + self.__buildingLabel
+        if mergeLinkBuses and data["from"] in self.__linkBuses:
+            inputBusLabel = data["from"]
+        else:
+            inputBusLabel = data["from"] + '__' + self.__buildingLabel
+        outputSHBusLabel = data["to"].split(",")[0] + '__' + self.__buildingLabel
+        outputDHWBusLabel = data["to"].split(",")[1] + '__' + self.__buildingLabel
+        envImpactPerCapacity = float(data["impact_cap"]) / float(data["lifetime"])
+        capacityDHW = float(data["capacity_DHW"])
+        capacitySH = float(data["capacity_SH"])
+        if data["capacity_min"] == 'x':
+            capacityMinSH = capacitySH
+            capacityMinDHW = capacityDHW
+        else:
+            capacityMinSH = capacityMinDHW = float(data["capacity_min"])
+
+        geothermalheatPumpSH = GeothermalHeatPumpLinearSingleUse(self.__buildingLabel, temperatureSH, temperatureAmb,
+                                  self.__busDict[inputBusLabel],
+                                  self.__busDict[outputSHBusLabel],
+                                  capacityMinSH, capacitySH,
+                                  self._calculateInvest(data)[0] * (opt == "costs") + envImpactPerCapacity*(opt == "env"),
+                                  self._calculateInvest(data)[1] * (opt == "costs"),
+                                  float(data["heat_impact"]) * (opt == "env"),
+                                  float(data["heat_impact"]), envImpactPerCapacity, dispatchMode)
+        geothermalheatPumpDHW = GeothermalHeatPumpLinearSingleUse(self.__buildingLabel, temperatureDHW,
+                                                        temperatureAmb,
+                                                        self.__busDict[inputBusLabel],
+                                                        self.__busDict[outputDHWBusLabel],
+                                                        capacityMinDHW, capacityDHW,
+                                                        self._calculateInvest(data)[0] * (
+                                                                    opt == "costs") + envImpactPerCapacity * (
+                                                                    opt == "env"),
+                                                        self._calculateInvest(data)[1] * (opt == "costs"),
+                                                        float(data["heat_impact"]) * (opt == "env"),
+                                                        float(data["heat_impact"]), envImpactPerCapacity, dispatchMode)
+
+        self.__nodesList.append(geothermalheatPumpSH.getHP("sh"))
+        self.__nodesList.append(geothermalheatPumpDHW.getHP("sh"))
+
+        # set technologies, environment and cost parameters
+        self.__technologies.append([outputDHWBusLabel, gwhpDHWLabel])
+        self.__technologies.append([outputSHBusLabel, gwhpSHLabel])
+
+        self.__costParam[gwhpSHLabel] = [self._calculateInvest(data)[0], self._calculateInvest(data)[1]]
+        self.__costParam[gwhpDHWLabel] = [self._calculateInvest(data)[0], self._calculateInvest(data)[1]]
+
+        self.__envParam[gwhpSHLabel] = [float(data["heat_impact"]), 0, envImpactPerCapacity]
+        self.__envParam[gwhpDHWLabel] = [float(data["heat_impact"]), 0, envImpactPerCapacity]
+
+    def _addCHP(self, data, timesteps, opt, dispatchMode):
+        chpSHLabel = data["label"] + '__' + self.__buildingLabel
+        inputBusLabel = data["from"] + '__' + self.__buildingLabel
+        outputElBusLabel = data["to"].split(",")[0] + '__' + self.__buildingLabel
+        outputSHBusLabel = data["to"].split(",")[1] + '__' + self.__buildingLabel
+        outputDHWBusLabel = data["to"].split(",")[2] + '__' + self.__buildingLabel
+        elEfficiency = float(data["efficiency"].split(",")[0])
+        shEfficiency = float(data["efficiency"].split(",")[1])
+        dhwEfficiency = float(data["efficiency"].split(",")[2])
+        envImpactPerCapacity = float(data["impact_cap"]) / float(data["lifetime"])
+        if data["capacity_min"] == 'x':
+            capacityMinSH = float(data["capacity_SH"])
+        else:
+            capacityMinSH = float(data["capacity_min"])
+        chp = CHP(self.__buildingLabel, self.__busDict[inputBusLabel],
+                  self.__busDict[outputElBusLabel],
+                  self.__busDict[outputSHBusLabel],
+                  self.__busDict[outputDHWBusLabel],
+                  elEfficiency, shEfficiency,
+                  dhwEfficiency, capacityMinSH,
+                  float(data["capacity_SH"]),
+                  self._calculateInvest(data)[0] * (opt == "costs") + envImpactPerCapacity * (opt == "env"),
+                  self._calculateInvest(data)[1] * (opt == "costs"), float(data["elec_impact"]) * (opt == "env"),
+                  float(data["heat_impact"]) * (opt == "env"),
+                  float(data["elec_impact"]), float(data["heat_impact"]), envImpactPerCapacity, timesteps, dispatchMode)
+
+        self.__nodesList.append(chp.getCHP("sh"))
+
+        # set technologies, environment and cost parameters
+        self.__technologies.append([outputElBusLabel, chpSHLabel])
+        self.__technologies.append([outputSHBusLabel, chpSHLabel])
+        self.__technologies.append([outputDHWBusLabel, chpSHLabel])
+
+        self.__costParam[chpSHLabel] = [self._calculateInvest(data)[0], self._calculateInvest(data)[1]]
+
+        self.__envParam[chpSHLabel] = [float(data["heat_impact"]), float(data["elec_impact"]), envImpactPerCapacity]
+
+    def _addGasBoiler(self, data, opt, dispatchMode):
+        gasBoilLabel = data["label"] + '__' + self.__buildingLabel
+        inputBusLabel = data["from"] + '__' + self.__buildingLabel
+        outputSHBusLabel = data["to"].split(",")[0] + '__' + self.__buildingLabel
+        outputDHWBusLabel = data["to"].split(",")[1] + '__' + self.__buildingLabel
+        shEfficiency = float(data["efficiency"].split(",")[0])
+        dhwEfficiency = float(data["efficiency"].split(",")[1])
+        envImpactPerCapacity = float(data["impact_cap"]) / float(data["lifetime"])
+        if data["capacity_min"] == 'x':
+            capacityMinSH = float(data["capacity_SH"])
+        else:
+            capacityMinSH = float(data["capacity_min"])
+
+        self.__nodesList.append(GasBoiler(self.__buildingLabel, self.__busDict[inputBusLabel],
+                  self.__busDict[outputSHBusLabel], self.__busDict[outputDHWBusLabel],
+                  shEfficiency, dhwEfficiency, capacityMinSH, float(data["capacity_SH"]),
+                  self._calculateInvest(data)[0] * (opt == "costs") + envImpactPerCapacity * (opt == "env"),
+                  self._calculateInvest(data)[1] * (opt == "costs"), float(data["heat_impact"]) * (opt == "env"), float(data["heat_impact"]), envImpactPerCapacity, dispatchMode))
+
+        # set technologies, environment and cost parameters
+        self.__technologies.append([outputSHBusLabel, gasBoilLabel])
+        self.__technologies.append([outputDHWBusLabel, gasBoilLabel])
+
+        self.__costParam[gasBoilLabel] = [self._calculateInvest(data)[0], self._calculateInvest(data)[1]]
+
+        self.__envParam[gasBoilLabel] = [float(data["heat_impact"]), 0, envImpactPerCapacity]
+
+    def _addElectricRod(self, data, opt, mergeLinkBuses, dispatchMode):
+        elRodLabel = data["label"] + '__' + self.__buildingLabel
+        if mergeLinkBuses and data["from"] in self.__linkBuses:
+            inputBusLabel = data["from"]
+        else:
+            inputBusLabel = data["from"] + '__' + self.__buildingLabel
+        outputSHBusLabel = data["to"].split(",")[0] + '__' + self.__buildingLabel
+        outputDHWBusLabel = data["to"].split(",")[1] + '__' + self.__buildingLabel
+        efficiency = float(data["efficiency"])
+        envImpactPerCapacity = float(data["impact_cap"]) / float(data["lifetime"])
+        if data["capacity_min"] == 'x':
+            capacityMinSH = float(data["capacity_SH"])
+        else:
+            capacityMinSH = float(data["capacity_min"])
+
+        self.__nodesList.append(ElectricRod(self.__buildingLabel, self.__busDict[inputBusLabel],
+                                          self.__busDict[outputSHBusLabel], self.__busDict[outputDHWBusLabel],
+                                          efficiency, capacityMinSH, float(data["capacity_SH"]),
+                                          self._calculateInvest(data)[0] * (opt == "costs") + envImpactPerCapacity * (
+                                                      opt == "env"),
+                                          self._calculateInvest(data)[1] * (opt == "costs"),
+                                          float(data["heat_impact"]) * (opt == "env"), float(data["heat_impact"]),
+                                          envImpactPerCapacity, dispatchMode))
+
+        # set technologies, environment and cost parameters
+        self.__technologies.append([outputSHBusLabel, elRodLabel])
+        self.__technologies.append([outputDHWBusLabel, elRodLabel])
+
+        self.__costParam[elRodLabel] = [self._calculateInvest(data)[0], self._calculateInvest(data)[1]]
+
+        self.__envParam[elRodLabel] = [float(data["heat_impact"]), 0, envImpactPerCapacity]
+
+    def addTransformer(self, data, temperatureDHW, temperatureSH, temperatureAmb, temperatureGround, opt, mergeLinkBuses, dispatchMode):
+        for i, t in data.iterrows():
+            if t["active"]:
+                if t["label"] == "HP":
+                    self._addHeatPump(t, temperatureDHW, temperatureSH, temperatureAmb, opt, mergeLinkBuses, dispatchMode)
+                elif t["label"] == "GWHP":
+                    self._addGeothemalHeatPump(t, temperatureDHW, temperatureSH, temperatureGround, opt, mergeLinkBuses, dispatchMode)
+                elif t["label"] == "GWHP split":
+                    self._addGeothemalHeatPumpSplit(t, temperatureDHW, temperatureSH, temperatureGround, opt, mergeLinkBuses, dispatchMode)
+                elif t["label"] == "CHP":
+                    self._addCHP(t, len(temperatureAmb), opt, dispatchMode)
+                elif t["label"] == "GasBoiler":
+                    self._addGasBoiler(t, opt, dispatchMode)
+                elif t["label"] == "ElectricRod":
+                    self._addElectricRod(t, opt, mergeLinkBuses, dispatchMode)
+                else:
+                    logging.warning("Transformer label not identified...")
+
+    def addStorage(self, data, stratifiedStorageParams, opt, mergeLinkBuses, dispatchMode):
+        for i, s in data.iterrows():
+            if s["active"]:
+                storageLabel = s["label"]+'__'+self.__buildingLabel
+                if mergeLinkBuses and s["from"] in self.__linkBuses:
+                    inputBusLabel = s["from"]
+                else:
+                    inputBusLabel = s["from"]+'__'+self.__buildingLabel
+                if mergeLinkBuses and s["to"] in self.__linkBuses:
+                    outputBusLabel = s["to"]
+                else:
+                    outputBusLabel = s["to"]+'__'+self.__buildingLabel
+                envImpactPerCapacity = float(s["impact_cap"]) / float(s["lifetime"])         # annualized value
+                # set technologies, environment and cost parameters
+                self.__costParam[storageLabel] = [self._calculateInvest(s)[0], self._calculateInvest(s)[1]]
+                self.__envParam[storageLabel] = [float(s["heat_impact"]), float(s["elec_impact"]), envImpactPerCapacity]
+                self.__technologies.append([outputBusLabel, storageLabel])
+
+                if s["label"] == "electricalStorage":
+                    self.__nodesList.append(ElectricalStorage(self.__buildingLabel, self.__busDict[inputBusLabel],
+                                                              self.__busDict[outputBusLabel], float(s["capacity loss"]),
+                                                            float(s["initial capacity"]), float(s["efficiency inflow"]),
+                                                            float(s["efficiency outflow"]), float(s["capacity min"]),
+                                                            float(s["capacity max"]),
+                                                            self._calculateInvest(s)[0]*(opt == "costs") + envImpactPerCapacity*(opt == "env"),
+                                                            self._calculateInvest(s)[1]*(opt == "costs"),
+                                                            float(s["elec_impact"])*(opt == "env"),
+                                                            float(s["elec_impact"]), envImpactPerCapacity, dispatchMode))
+
+                elif s["label"] == "dhwStorage" or s["label"] == "shStorage":
+                    ts = ThermalStorage(storageLabel, s["label"],
+                                                           stratifiedStorageParams, self.__busDict[inputBusLabel],
+                                                           self.__busDict[outputBusLabel],
+                                                        float(s["initial capacity"]), float(s["capacity min"]),
+                                                        float(s["capacity max"]),
+                                                        self._calculateInvest(s)[0]*(opt == "costs") + envImpactPerCapacity*(opt == "env"),
+                                                        self._calculateInvest(s)[1]*(opt == "costs"), float(s["heat_impact"])*(opt == "env"),
+                                                        float(s["heat_impact"]), envImpactPerCapacity, dispatchMode)
+                    self.__nodesList.append(ts.getStorage())
+                else:
+                    logging.warning("Storage label not identified")
+
+    def _calculateInvest(self, data):
+        # Calculate the CAPEX and the part of the OPEX not related to energy flows (maintenance)
+        c = data["installation"] + data["planification"] + 1
+        m = data["maintenance"]
+        perCapacity = m * data["invest_cap"] + economics.annuity(c * data["invest_cap"], data["lifetime"], intRate)
+        base = m * data["invest_base"] + economics.annuity(c * data["invest_base"], data["lifetime"], intRate)
         return perCapacity, base
```

### Comparing `optihood-0.0.0/optihood/combined_prod.py` & `optihood-0.0.1/optihood/combined_prod.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,151 +1,151 @@
-from pyomo.core.base.block import SimpleBlock
-from pyomo.environ import BuildAction
-from pyomo.environ import Constraint
-
-from oemof.solph import network as solph_network
-from oemof.solph.plumbing import sequence as solph_sequence
-
-
-class CombinedTransformer(solph_network.Transformer):
-    r"""
-    A transformer able to produce both SH and DHW in the same timestep
-    Pelec_in = Qsh/efficiencySH + Qdhw/efficiencyDHW
-    """
-
-    def __init__(self, efficiencies, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.efficiency = {
-            k: solph_sequence(v)
-            for k, v in efficiencies.items()
-        }
-
-    def constraint_group(self):
-        return CombinedTransformerBlock
-
-
-class CombinedTransformerBlock(SimpleBlock):
-    r"""Block for the linear relation of nodes
-    """
-
-    CONSTRAINT_GROUP = True
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-    def _create(self, group=None):
-        """Creates the linear constraint
-        """
-        if group is None:
-            return None
-
-        m = self.parent_block()
-
-        for n in group:
-            n.inflow = list(n.inputs)[0]
-            n.flowSH = [k for k, v in n.efficiency.items()][0]
-            n.flowDHW = [k for k, v in n.efficiency.items()][1]
-            n.outputSH = [o for o in n.outputs if n.flowSH == o][0]
-            n.outputDHW = [o for o in n.outputs if n.flowDHW == o][0]
-            n.efficiency_sq = (
-                n.efficiency[n.outputSH],
-                n.efficiency[n.outputDHW]
-            )
-
-        def _input_output_relation_rule(block):
-            """Connection between input and outputs."""
-            for t in m.TIMESTEPS:
-                for g in group:
-                    lhs = m.flow[g.inflow, g, t]
-                    rhs = (m.flow[g, g.outputSH, t] / g.efficiency_sq[0][t]
-                           + m.flow[g, g.outputDHW, t] / g.efficiency_sq[1][t])
-                    block.input_output_relation.add((g, t), (lhs == rhs))
-
-        self.input_output_relation = Constraint(
-            group, m.TIMESTEPS, noruleinit=True
-        )
-        self.input_output_relation_build = BuildAction(
-            rule=_input_output_relation_rule
-        )
-
-
-class CombinedCHP(solph_network.Transformer):
-    r"""
-    A CHP able to produce both SH and DHW in the same timestep
-    Pelec_in = Qsh/efficiencySH + Qdhw/efficiencyDHW
-             = Pelec_out/efficiencyEl
-    """
-
-    def __init__(self, efficiencies, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.efficiency = {
-            k: solph_sequence(v)
-            for k, v in efficiencies.items()
-        }
-
-    def constraint_group(self):
-        return CombinedCHPBlock
-
-
-class CombinedCHPBlock(SimpleBlock):
-    r"""Block for the linear relation of nodes
-    """
-
-    CONSTRAINT_GROUP = True
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-    def _create(self, group=None):
-        """Creates the linear constraint
-        """
-        if group is None:
-            return None
-
-        m = self.parent_block()
-
-        for n in group:
-            n.inflow = list(n.inputs)[0]
-            n.flowSH = [k for k, v in n.efficiency.items()][0]
-            n.flowDHW = [k for k, v in n.efficiency.items()][1]
-            n.flowEl = [k for k, v in n.efficiency.items()][2]
-            n.outputSH = [o for o in n.outputs if n.flowSH == o][0]
-            n.outputDHW = [o for o in n.outputs if n.flowDHW == o][0]
-            n.outputEl = [o for o in n.outputs if n.flowEl == o][0]
-            n.efficiency_sq = (
-                n.efficiency[n.outputSH],
-                n.efficiency[n.outputDHW],
-                n.efficiency[n.outputEl]
-            )
-
-        def _input_heat_relation_rule(block):
-            """Connection between input and heat outputs."""
-            for t in m.TIMESTEPS:
-                for g in group:
-                    lhs = m.flow[g.inflow, g, t]
-                    rhs = (
-                        m.flow[g, g.outputSH, t] / g.efficiency_sq[0][t]
-                        + m.flow[g, g.outputDHW, t] / g.efficiency_sq[1][t]
-                    )
-                    block.input_heat_relation.add((g, t), (lhs == rhs))
-
-        self.input_heat_relation = Constraint(
-            group, m.TIMESTEPS, noruleinit=True
-        )
-        self.input_heat_relation_build = BuildAction(
-            rule=_input_heat_relation_rule
-        )
-
-        def _input_elec_relation_rule(block):
-            """Connection between input and elec output."""
-            for t in m.TIMESTEPS:
-                for g in group:
-                    lhs = m.flow[g.inflow, g, t]
-                    rhs = (m.flow[g, g.outputEl, t] / g.efficiency_sq[2][t])
-                    block.input_elec_relation.add((g, t), (lhs == rhs))
-
-        self.input_elec_relation = Constraint(
-            group, m.TIMESTEPS, noruleinit=True
-        )
-        self.input_elec_relation_build = BuildAction(
-            rule=_input_elec_relation_rule
+from pyomo.core.base.block import SimpleBlock
+from pyomo.environ import BuildAction
+from pyomo.environ import Constraint
+
+from oemof.solph import network as solph_network
+from oemof.solph.plumbing import sequence as solph_sequence
+
+
+class CombinedTransformer(solph_network.Transformer):
+    r"""
+    A transformer able to produce both SH and DHW in the same timestep
+    Pelec_in = Qsh/efficiencySH + Qdhw/efficiencyDHW
+    """
+
+    def __init__(self, efficiencies, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.efficiency = {
+            k: solph_sequence(v)
+            for k, v in efficiencies.items()
+        }
+
+    def constraint_group(self):
+        return CombinedTransformerBlock
+
+
+class CombinedTransformerBlock(SimpleBlock):
+    r"""Block for the linear relation of nodes
+    """
+
+    CONSTRAINT_GROUP = True
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def _create(self, group=None):
+        """Creates the linear constraint
+        """
+        if group is None:
+            return None
+
+        m = self.parent_block()
+
+        for n in group:
+            n.inflow = list(n.inputs)[0]
+            n.flowSH = [k for k, v in n.efficiency.items()][0]
+            n.flowDHW = [k for k, v in n.efficiency.items()][1]
+            n.outputSH = [o for o in n.outputs if n.flowSH == o][0]
+            n.outputDHW = [o for o in n.outputs if n.flowDHW == o][0]
+            n.efficiency_sq = (
+                n.efficiency[n.outputSH],
+                n.efficiency[n.outputDHW]
+            )
+
+        def _input_output_relation_rule(block):
+            """Connection between input and outputs."""
+            for t in m.TIMESTEPS:
+                for g in group:
+                    lhs = m.flow[g.inflow, g, t]
+                    rhs = (m.flow[g, g.outputSH, t] / g.efficiency_sq[0][t]
+                           + m.flow[g, g.outputDHW, t] / g.efficiency_sq[1][t])
+                    block.input_output_relation.add((g, t), (lhs == rhs))
+
+        self.input_output_relation = Constraint(
+            group, m.TIMESTEPS, noruleinit=True
+        )
+        self.input_output_relation_build = BuildAction(
+            rule=_input_output_relation_rule
+        )
+
+
+class CombinedCHP(solph_network.Transformer):
+    r"""
+    A CHP able to produce both SH and DHW in the same timestep
+    Pelec_in = Qsh/efficiencySH + Qdhw/efficiencyDHW
+             = Pelec_out/efficiencyEl
+    """
+
+    def __init__(self, efficiencies, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.efficiency = {
+            k: solph_sequence(v)
+            for k, v in efficiencies.items()
+        }
+
+    def constraint_group(self):
+        return CombinedCHPBlock
+
+
+class CombinedCHPBlock(SimpleBlock):
+    r"""Block for the linear relation of nodes
+    """
+
+    CONSTRAINT_GROUP = True
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def _create(self, group=None):
+        """Creates the linear constraint
+        """
+        if group is None:
+            return None
+
+        m = self.parent_block()
+
+        for n in group:
+            n.inflow = list(n.inputs)[0]
+            n.flowSH = [k for k, v in n.efficiency.items()][0]
+            n.flowDHW = [k for k, v in n.efficiency.items()][1]
+            n.flowEl = [k for k, v in n.efficiency.items()][2]
+            n.outputSH = [o for o in n.outputs if n.flowSH == o][0]
+            n.outputDHW = [o for o in n.outputs if n.flowDHW == o][0]
+            n.outputEl = [o for o in n.outputs if n.flowEl == o][0]
+            n.efficiency_sq = (
+                n.efficiency[n.outputSH],
+                n.efficiency[n.outputDHW],
+                n.efficiency[n.outputEl]
+            )
+
+        def _input_heat_relation_rule(block):
+            """Connection between input and heat outputs."""
+            for t in m.TIMESTEPS:
+                for g in group:
+                    lhs = m.flow[g.inflow, g, t]
+                    rhs = (
+                        m.flow[g, g.outputSH, t] / g.efficiency_sq[0][t]
+                        + m.flow[g, g.outputDHW, t] / g.efficiency_sq[1][t]
+                    )
+                    block.input_heat_relation.add((g, t), (lhs == rhs))
+
+        self.input_heat_relation = Constraint(
+            group, m.TIMESTEPS, noruleinit=True
+        )
+        self.input_heat_relation_build = BuildAction(
+            rule=_input_heat_relation_rule
+        )
+
+        def _input_elec_relation_rule(block):
+            """Connection between input and elec output."""
+            for t in m.TIMESTEPS:
+                for g in group:
+                    lhs = m.flow[g.inflow, g, t]
+                    rhs = (m.flow[g, g.outputEl, t] / g.efficiency_sq[2][t])
+                    block.input_elec_relation.add((g, t), (lhs == rhs))
+
+        self.input_elec_relation = Constraint(
+            group, m.TIMESTEPS, noruleinit=True
+        )
+        self.input_elec_relation_build = BuildAction(
+            rule=_input_elec_relation_rule
         )
```

### Comparing `optihood-0.0.0/optihood/constraints.py` & `optihood-0.0.1/optihood/constraints.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,252 +1,252 @@
-from pyomo import environ as pyo
-from oemof.solph.plumbing import sequence
-from math import pi
-
-def dailySHStorageConstraint(om):
-    """
-    Function to limit the SH storage capacity to 2 days
-    :param om: optimization model
-    :return: om: optimization model
-    """
-    for s in om.NODES:
-        if "shStorage" in s.label:
-            constr = s.label.replace("__Building","") + "_constraint_"
-            for t in om.TIMESTEPS:
-                if t % 48 == 0 and t!=0:
-                    setattr(
-                        om,
-                        constr + str(t),
-                        pyo.Constraint(expr=(om.GenericInvestmentStorageBlock.storage_content[s, t] == 0)),
-                    )
-
-    return om
-
-def connectInvestmentRule(om):
-    """Constraint to equate the investment objects of all the output flows of a Link"""
-
-    elLinkOutputFlows = [(i, o) for (i, o) in om.flows if (i.label == "electricityLink" or i.label == "elLink")]
-    shLinkOutputFlows = [(i, o) for (i, o) in om.flows if i.label == "shLink"]
-    dhwLinkOutputFlows = [(i, o) for (i, o) in om.flows if i.label == "dhwLink"]
-
-    if elLinkOutputFlows:
-        first = om.InvestmentFlow.invest[next(iter(elLinkOutputFlows))]
-        for (i, o) in elLinkOutputFlows:
-            expr = (first == om.InvestmentFlow.invest[i, o])
-            setattr(
-                om,
-                "elLinkConstr_" + o.label,
-                pyo.Constraint(expr=expr),
-            )
-
-    if shLinkOutputFlows:
-        first = om.InvestmentFlow.invest[next(iter(shLinkOutputFlows))]
-        for (i, o) in shLinkOutputFlows:
-            expr = (first == om.InvestmentFlow.invest[i, o])
-            setattr(
-                om,
-                "shLinkConstr_" + o.label,
-                pyo.Constraint(expr=expr),
-            )
-
-    if dhwLinkOutputFlows:
-        first = om.InvestmentFlow.invest[next(iter(dhwLinkOutputFlows))]
-        for (i, o) in dhwLinkOutputFlows:
-            expr = (first == om.InvestmentFlow.invest[i, o])
-            setattr(
-                om,
-                "dhwLinkConstr_" + o.label,
-                pyo.Constraint(expr=expr),
-            )
-
-    return om
-
-
-def environmentalImpactlimit(om, keyword1, keyword2, limit=None):
-    """
-    Based on: oemof.solph.constraints.emission_limit
-    Function to limit the environmental impacts during the multi-objective optimization
-    :param om: model
-    :param keyword1: keyword for environmental impacts per flow, placed in a solph.Flow() object
-    :param keyword2: keyword for environmental impacts per capacity installed, placed in a solph.Investment() object
-    :param limit: limit not to be reached
-    :return:
-    """
-    flows = {}
-    transformerFlowCapacityDict = {}
-    storageCapacityDict = {}
-    for (i, o) in om.flows:
-        if hasattr(om.flows[i, o], keyword1):
-            flows[(i, o)] = om.flows[i, o]
-        if hasattr(om.flows[i, o].investment, keyword2):
-            transformerFlowCapacityDict[(i, o)] = om.flows[i, o].investment
-
-    for x in om.GenericInvestmentStorageBlock.INVESTSTORAGES:
-        if hasattr(x.investment, keyword2):
-            storageCapacityDict[x] = om.GenericInvestmentStorageBlock.invest[x]
-
-    envImpact = "totalEnvironmentalImpact"
-
-    setattr(
-        om,
-        envImpact,
-        pyo.Expression(
-            expr=sum(
-            # Environmental inpact of input flows
-                om.flow[inflow, outflow, t]
-                * om.timeincrement[t]
-                * sequence(getattr(flows[inflow, outflow], keyword1))[t]
-                for (inflow, outflow) in flows
-                for t in om.TIMESTEPS
-            )
-            # fix Environmental impact per transformer capacity
-            + sum(om.InvestmentFlow.invest[inflow, outflow] * getattr(transformerFlowCapacityDict[inflow, outflow], keyword2)
-            for (inflow, outflow) in transformerFlowCapacityDict)
-            # fix Environmental impact per storage capacity
-            + sum(om.GenericInvestmentStorageBlock.invest[x] * getattr(x.investment, keyword2) for x in storageCapacityDict)
-        ),
-    )
-    setattr(
-        om,
-        envImpact + "_constraint",
-        pyo.Constraint(expr=(getattr(om, envImpact) <= limit)),
-    )
-    return om, flows, transformerFlowCapacityDict, storageCapacityDict
-
-
-def roof_area_limit(model, keyword1, keyword2, nb):
-    r"""
-    Based on: oemof.solph.constraints.additional_investment_flow_limit
-    Constraint to limit the capacity of solar panels installed considering the roof area available
-    Parameters
-    ----------
-    model : oemof.solph.Model
-        Model to which constraints are added.
-    keyword1 : attribute to consider
-        Coefficient representing the area used by one unit of capacity of a solar panel
-    keyword2 : attribute to consider
-        Total roof area available for panels.
-    nb : int
-        Number of buildings in the neighbourhood
-
-    Note
-    ----
-    The Investment attribute of the considered (Investment-)flows requires an
-    attribute named like keyword!
-    """
-
-    for b in range(1, nb+1):
-        limit = 0
-        invest_flows = {}
-        for (i, o) in model.flows:
-            if str(b) in str(i):
-                if hasattr(model.flows[i, o].investment, keyword1):
-                    invest_flows[(i, o)] = model.flows[i, o].investment
-                    limit = getattr(model.flows[i, o].investment, keyword2)
-
-        limit_name = "invest_limit_" + keyword1 + "_building" + str(b)
-
-        setattr(
-            model,
-            limit_name,
-            pyo.Expression(
-                expr=sum(
-                    model.InvestmentFlow.invest[inflow, outflow]
-                    * getattr(invest_flows[inflow, outflow], keyword1)
-                    for (inflow, outflow) in invest_flows
-                )
-            ),
-        )
-
-        setattr(
-            model,
-            limit_name + "_constraint",
-            pyo.Constraint(expr=(getattr(model, limit_name) <= limit)),
-        )
-
-
-    return model
-
-def electricRodCapacityConstaint(om, numBuildings):
-    """constraint to set the total capacity of electric rod equal to sum of total capacity selected for HP"""
-    electricRodInputFlows = [(i, o) for (i, o) in om.flows if ("ElectricRod" in o.label)]
-    airHeatPumpInputFlows = [(i, o) for (i, o) in om.flows if ("HP" in o.label and "CHP" not in o.label and "GWHP" not in o.label)]
-    groundHeatPumpInputFlows = [(i, o) for (i, o) in om.flows if ("GWHP" in o.label and not any([c.isdigit() for c in o.label.split("__")[0]]))]
-    groundHeatPumpOutFlows = [(i, o) for (i, o) in om.flows if ("GWHP" in i.label and any([c.isdigit() for c in i.label.split("__")[0]]))]     # for splitted GSHPs
-
-    elRodCapacityTotal = 0
-    airHeatPumpCapacityTotal = 0
-    groundHeatPumpCapacityTotal = 0
-
-    for b in range(1,numBuildings+1):
-        elRodCapacity = [om.InvestmentFlow.invest[i, o] for (i, o) in electricRodInputFlows if ((f'__Building{b}') in o.label)]
-        airHeatPumpCapacity = [om.InvestmentFlow.invest[i, o] for (i, o) in airHeatPumpInputFlows if ((f'__Building{b}') in o.label)]
-        if groundHeatPumpInputFlows:
-            groundHeatPumpCapacity = [om.InvestmentFlow.invest[i, o] for (i, o) in groundHeatPumpInputFlows if ((f'__Building{b}') in o.label)]
-        else:
-            groundHeatPumpCapacity = [om.InvestmentFlow.invest[i, o] for (i, o) in groundHeatPumpOutFlows if ((f'__Building{b}') in i.label)]
-        if elRodCapacity:
-            elRodCapacity = elRodCapacity[0]
-            airHeatPumpCapacity = airHeatPumpCapacity[0] if airHeatPumpCapacity else 0
-            if groundHeatPumpInputFlows:
-                groundHeatPumpCapacity = groundHeatPumpCapacity[0] if groundHeatPumpCapacity else 0
-            else:
-                groundHeatPumpCapacity = groundHeatPumpCapacity[0] + groundHeatPumpCapacity[1] if groundHeatPumpCapacity else 0
-            elRodCapacityTotal = elRodCapacityTotal + elRodCapacity
-            airHeatPumpCapacityTotal = airHeatPumpCapacityTotal + airHeatPumpCapacity
-            groundHeatPumpCapacityTotal = groundHeatPumpCapacityTotal + groundHeatPumpCapacity
-
-    expr = (elRodCapacityTotal <= (airHeatPumpCapacityTotal + groundHeatPumpCapacityTotal))
-    setattr(
-        om,
-        "electricRodSizeConstr",
-        pyo.Constraint(expr=expr),
-    )
-    return om
-
-def totalPVCapacityConstraint(om, numBuildings):
-    pvOutFlows = [(i, o) for (i, o) in om.flows if ("pv" in i.label)]
-    pvCapacityTotal = 0
-    for b in range(1,numBuildings+1):
-        pvCapacity = [om.InvestmentFlow.invest[i, o] for (i, o) in pvOutFlows if ((f'__Building{b}') in o.label)]
-        if pvCapacity:
-            pvCapacity = pvCapacity[0]
-            pvCapacityTotal = pvCapacityTotal + pvCapacity
-    expr = (pvCapacityTotal <= 205)
-    setattr(
-        om,
-        "PVSizeConstr",
-        pyo.Constraint(expr=expr),
-    )
-    return om
-
-def PVTElectricalThermalCapacityConstraint(om, numBuildings):
-    pvtElOutFlows = [(i, o) for (i, o) in om.flows if ("elSource_pvt" in i.label)]
-    pvtShOutFlows = [(i, o) for (i, o) in om.flows if ("heatSource_SHpvt" in i.label)]
-    pvtDhwOutFlows = [(i, o) for (i, o) in om.flows if ("heatSource_DHWpvt" in i.label)]
-    for b in range(1, numBuildings + 1):
-        elCapacity = [om.InvestmentFlow.invest[i, o] for (i, o) in pvtElOutFlows if ((f'__Building{b}') in o.label)]
-        shCapacity = [om.InvestmentFlow.invest[i, o] for (i, o) in pvtShOutFlows if ((f'__Building{b}') in o.label)]
-        dhwCapacity = [om.InvestmentFlow.invest[i, o] for (i, o) in pvtDhwOutFlows if ((f'__Building{b}') in o.label)]
-        areaUnitCapEl = [getattr(om.flows[i, o].investment, 'space_el') for (i, o) in pvtElOutFlows if ((f'__Building{b}') in o.label)]
-        areaUnitCapSh = [getattr(om.flows[i, o].investment, 'space') for (i, o) in pvtShOutFlows if ((f'__Building{b}') in o.label)]
-        if elCapacity or shCapacity:
-            elCapacity = elCapacity[0]
-            shCapacity = shCapacity[0]
-            dhwCapacity = dhwCapacity[0]
-            areaUnitCapEl = areaUnitCapEl[0]
-            areaUnitCapSh = areaUnitCapSh[0]
-            expr = (elCapacity*areaUnitCapEl == shCapacity*areaUnitCapSh)
-            setattr(
-                om,
-                "PVTSizeConstrElTh_B"+str(b),
-                pyo.Constraint(expr=expr),
-            )
-            expr = (dhwCapacity == shCapacity)
-            setattr(
-                om,
-                "PVTSizeConstrDhwSh_B" + str(b),
-                pyo.Constraint(expr=expr),
-            )
-
-
+from pyomo import environ as pyo
+from oemof.solph.plumbing import sequence
+from math import pi
+
+def dailySHStorageConstraint(om):
+    """
+    Function to limit the SH storage capacity to 2 days
+    :param om: optimization model
+    :return: om: optimization model
+    """
+    for s in om.NODES:
+        if "shStorage" in s.label:
+            constr = s.label.replace("__Building","") + "_constraint_"
+            for t in om.TIMESTEPS:
+                if t % 48 == 0 and t!=0:
+                    setattr(
+                        om,
+                        constr + str(t),
+                        pyo.Constraint(expr=(om.GenericInvestmentStorageBlock.storage_content[s, t] == 0)),
+                    )
+
+    return om
+
+def connectInvestmentRule(om):
+    """Constraint to equate the investment objects of all the output flows of a Link"""
+
+    elLinkOutputFlows = [(i, o) for (i, o) in om.flows if (i.label == "electricityLink" or i.label == "elLink")]
+    shLinkOutputFlows = [(i, o) for (i, o) in om.flows if i.label == "shLink"]
+    dhwLinkOutputFlows = [(i, o) for (i, o) in om.flows if i.label == "dhwLink"]
+
+    if elLinkOutputFlows:
+        first = om.InvestmentFlow.invest[next(iter(elLinkOutputFlows))]
+        for (i, o) in elLinkOutputFlows:
+            expr = (first == om.InvestmentFlow.invest[i, o])
+            setattr(
+                om,
+                "elLinkConstr_" + o.label,
+                pyo.Constraint(expr=expr),
+            )
+
+    if shLinkOutputFlows:
+        first = om.InvestmentFlow.invest[next(iter(shLinkOutputFlows))]
+        for (i, o) in shLinkOutputFlows:
+            expr = (first == om.InvestmentFlow.invest[i, o])
+            setattr(
+                om,
+                "shLinkConstr_" + o.label,
+                pyo.Constraint(expr=expr),
+            )
+
+    if dhwLinkOutputFlows:
+        first = om.InvestmentFlow.invest[next(iter(dhwLinkOutputFlows))]
+        for (i, o) in dhwLinkOutputFlows:
+            expr = (first == om.InvestmentFlow.invest[i, o])
+            setattr(
+                om,
+                "dhwLinkConstr_" + o.label,
+                pyo.Constraint(expr=expr),
+            )
+
+    return om
+
+
+def environmentalImpactlimit(om, keyword1, keyword2, limit=None):
+    """
+    Based on: oemof.solph.constraints.emission_limit
+    Function to limit the environmental impacts during the multi-objective optimization
+    :param om: model
+    :param keyword1: keyword for environmental impacts per flow, placed in a solph.Flow() object
+    :param keyword2: keyword for environmental impacts per capacity installed, placed in a solph.Investment() object
+    :param limit: limit not to be reached
+    :return:
+    """
+    flows = {}
+    transformerFlowCapacityDict = {}
+    storageCapacityDict = {}
+    for (i, o) in om.flows:
+        if hasattr(om.flows[i, o], keyword1):
+            flows[(i, o)] = om.flows[i, o]
+        if hasattr(om.flows[i, o].investment, keyword2):
+            transformerFlowCapacityDict[(i, o)] = om.flows[i, o].investment
+
+    for x in om.GenericInvestmentStorageBlock.INVESTSTORAGES:
+        if hasattr(x.investment, keyword2):
+            storageCapacityDict[x] = om.GenericInvestmentStorageBlock.invest[x]
+
+    envImpact = "totalEnvironmentalImpact"
+
+    setattr(
+        om,
+        envImpact,
+        pyo.Expression(
+            expr=sum(
+            # Environmental inpact of input flows
+                om.flow[inflow, outflow, t]
+                * om.timeincrement[t]
+                * sequence(getattr(flows[inflow, outflow], keyword1))[t]
+                for (inflow, outflow) in flows
+                for t in om.TIMESTEPS
+            )
+            # fix Environmental impact per transformer capacity
+            + sum(om.InvestmentFlow.invest[inflow, outflow] * getattr(transformerFlowCapacityDict[inflow, outflow], keyword2)
+            for (inflow, outflow) in transformerFlowCapacityDict)
+            # fix Environmental impact per storage capacity
+            + sum(om.GenericInvestmentStorageBlock.invest[x] * getattr(x.investment, keyword2) for x in storageCapacityDict)
+        ),
+    )
+    setattr(
+        om,
+        envImpact + "_constraint",
+        pyo.Constraint(expr=(getattr(om, envImpact) <= limit)),
+    )
+    return om, flows, transformerFlowCapacityDict, storageCapacityDict
+
+
+def roof_area_limit(model, keyword1, keyword2, nb):
+    r"""
+    Based on: oemof.solph.constraints.additional_investment_flow_limit
+    Constraint to limit the capacity of solar panels installed considering the roof area available
+    Parameters
+    ----------
+    model : oemof.solph.Model
+        Model to which constraints are added.
+    keyword1 : attribute to consider
+        Coefficient representing the area used by one unit of capacity of a solar panel
+    keyword2 : attribute to consider
+        Total roof area available for panels.
+    nb : int
+        Number of buildings in the neighbourhood
+
+    Note
+    ----
+    The Investment attribute of the considered (Investment-)flows requires an
+    attribute named like keyword!
+    """
+
+    for b in range(1, nb+1):
+        limit = 0
+        invest_flows = {}
+        for (i, o) in model.flows:
+            if str(b) in str(i):
+                if hasattr(model.flows[i, o].investment, keyword1):
+                    invest_flows[(i, o)] = model.flows[i, o].investment
+                    limit = getattr(model.flows[i, o].investment, keyword2)
+
+        limit_name = "invest_limit_" + keyword1 + "_building" + str(b)
+
+        setattr(
+            model,
+            limit_name,
+            pyo.Expression(
+                expr=sum(
+                    model.InvestmentFlow.invest[inflow, outflow]
+                    * getattr(invest_flows[inflow, outflow], keyword1)
+                    for (inflow, outflow) in invest_flows
+                )
+            ),
+        )
+
+        setattr(
+            model,
+            limit_name + "_constraint",
+            pyo.Constraint(expr=(getattr(model, limit_name) <= limit)),
+        )
+
+
+    return model
+
+def electricRodCapacityConstaint(om, numBuildings):
+    """constraint to set the total capacity of electric rod equal to sum of total capacity selected for HP"""
+    electricRodInputFlows = [(i, o) for (i, o) in om.flows if ("ElectricRod" in o.label)]
+    airHeatPumpInputFlows = [(i, o) for (i, o) in om.flows if ("HP" in o.label and "CHP" not in o.label and "GWHP" not in o.label)]
+    groundHeatPumpInputFlows = [(i, o) for (i, o) in om.flows if ("GWHP" in o.label and not any([c.isdigit() for c in o.label.split("__")[0]]))]
+    groundHeatPumpOutFlows = [(i, o) for (i, o) in om.flows if ("GWHP" in i.label and any([c.isdigit() for c in i.label.split("__")[0]]))]     # for splitted GSHPs
+
+    elRodCapacityTotal = 0
+    airHeatPumpCapacityTotal = 0
+    groundHeatPumpCapacityTotal = 0
+
+    for b in range(1,numBuildings+1):
+        elRodCapacity = [om.InvestmentFlow.invest[i, o] for (i, o) in electricRodInputFlows if ((f'__Building{b}') in o.label)]
+        airHeatPumpCapacity = [om.InvestmentFlow.invest[i, o] for (i, o) in airHeatPumpInputFlows if ((f'__Building{b}') in o.label)]
+        if groundHeatPumpInputFlows:
+            groundHeatPumpCapacity = [om.InvestmentFlow.invest[i, o] for (i, o) in groundHeatPumpInputFlows if ((f'__Building{b}') in o.label)]
+        else:
+            groundHeatPumpCapacity = [om.InvestmentFlow.invest[i, o] for (i, o) in groundHeatPumpOutFlows if ((f'__Building{b}') in i.label)]
+        if elRodCapacity:
+            elRodCapacity = elRodCapacity[0]
+            airHeatPumpCapacity = airHeatPumpCapacity[0] if airHeatPumpCapacity else 0
+            if groundHeatPumpInputFlows:
+                groundHeatPumpCapacity = groundHeatPumpCapacity[0] if groundHeatPumpCapacity else 0
+            else:
+                groundHeatPumpCapacity = groundHeatPumpCapacity[0] + groundHeatPumpCapacity[1] if groundHeatPumpCapacity else 0
+            elRodCapacityTotal = elRodCapacityTotal + elRodCapacity
+            airHeatPumpCapacityTotal = airHeatPumpCapacityTotal + airHeatPumpCapacity
+            groundHeatPumpCapacityTotal = groundHeatPumpCapacityTotal + groundHeatPumpCapacity
+
+    expr = (elRodCapacityTotal <= (airHeatPumpCapacityTotal + groundHeatPumpCapacityTotal))
+    setattr(
+        om,
+        "electricRodSizeConstr",
+        pyo.Constraint(expr=expr),
+    )
+    return om
+
+def totalPVCapacityConstraint(om, numBuildings):
+    pvOutFlows = [(i, o) for (i, o) in om.flows if ("pv" in i.label)]
+    pvCapacityTotal = 0
+    for b in range(1,numBuildings+1):
+        pvCapacity = [om.InvestmentFlow.invest[i, o] for (i, o) in pvOutFlows if ((f'__Building{b}') in o.label)]
+        if pvCapacity:
+            pvCapacity = pvCapacity[0]
+            pvCapacityTotal = pvCapacityTotal + pvCapacity
+    expr = (pvCapacityTotal <= 205)
+    setattr(
+        om,
+        "PVSizeConstr",
+        pyo.Constraint(expr=expr),
+    )
+    return om
+
+def PVTElectricalThermalCapacityConstraint(om, numBuildings):
+    pvtElOutFlows = [(i, o) for (i, o) in om.flows if ("elSource_pvt" in i.label)]
+    pvtShOutFlows = [(i, o) for (i, o) in om.flows if ("heatSource_SHpvt" in i.label)]
+    pvtDhwOutFlows = [(i, o) for (i, o) in om.flows if ("heatSource_DHWpvt" in i.label)]
+    for b in range(1, numBuildings + 1):
+        elCapacity = [om.InvestmentFlow.invest[i, o] for (i, o) in pvtElOutFlows if ((f'__Building{b}') in o.label)]
+        shCapacity = [om.InvestmentFlow.invest[i, o] for (i, o) in pvtShOutFlows if ((f'__Building{b}') in o.label)]
+        dhwCapacity = [om.InvestmentFlow.invest[i, o] for (i, o) in pvtDhwOutFlows if ((f'__Building{b}') in o.label)]
+        areaUnitCapEl = [getattr(om.flows[i, o].investment, 'space_el') for (i, o) in pvtElOutFlows if ((f'__Building{b}') in o.label)]
+        areaUnitCapSh = [getattr(om.flows[i, o].investment, 'space') for (i, o) in pvtShOutFlows if ((f'__Building{b}') in o.label)]
+        if elCapacity or shCapacity:
+            elCapacity = elCapacity[0]
+            shCapacity = shCapacity[0]
+            dhwCapacity = dhwCapacity[0]
+            areaUnitCapEl = areaUnitCapEl[0]
+            areaUnitCapSh = areaUnitCapSh[0]
+            expr = (elCapacity*areaUnitCapEl == shCapacity*areaUnitCapSh)
+            setattr(
+                om,
+                "PVTSizeConstrElTh_B"+str(b),
+                pyo.Constraint(expr=expr),
+            )
+            expr = (dhwCapacity == shCapacity)
+            setattr(
+                om,
+                "PVTSizeConstrDhwSh_B" + str(b),
+                pyo.Constraint(expr=expr),
+            )
+
+
     return om
```

### Comparing `optihood-0.0.0/optihood/energy_network.py` & `optihood-0.0.1/optihood/energy_network.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,1216 +1,1216 @@
-import numpy as np
-import pandas as pd
-import oemof.solph as solph
-from oemof.tools import logger
-import logging
-import os
-import pprint as pp
-from configparser import ConfigParser
-from datetime import datetime, timedelta
-try:
-    import matplotlib.pyplot as plt
-except ImportError:
-    plt = None
-from optihood.constraints import *
-from optihood.buildings import Building
-from optihood.links import Link
-
-
-class EnergyNetworkClass(solph.EnergySystem):
-    def __init__(self, timestamp, clusters=None):
-        self._timeIndexReal = timestamp             # the timeindex passed to the energy network, will be made shorter if clustering is selected
-        self._clusterDate = {}
-        if clusters:
-            self._numberOfDays = len(clusters)
-            lastDay = datetime(timestamp.year[0], 1, 1) + timedelta(self._numberOfDays - 1)
-            lastDay = lastDay.strftime('%Y-%m-%d')
-            i = 1
-            for day in clusters:
-                d_clusterIndex = datetime(timestamp.year[0], 1, 1) + timedelta(i - 1)
-                self._clusterDate[day] = d_clusterIndex.strftime('%Y-%m-%d')
-                i += 1
-            timestamp = pd.date_range("2021-01-01 00:00:00", f"{lastDay} 23:00:00", freq=timestamp.freq)
-        self._nodesList = []
-        self._storageContentSH = {}
-        self.__inputs = {}                          # dictionary of list of inputs indexed by the building label
-        self.__technologies = {}                    # dictionary of list of technologies indexed by the building label
-        self.__capacitiesTransformersBuilding = {}  # dictionary of dictionary of optimized capacities of transformers indexed by the building label
-        self.__capacitiesStoragesBuilding = {}      # dictionary of dictionary of optimized capacities of storages indexed by the building label
-        self.__costParam = {}
-        self.__envParam = {}
-        self.__capex = {}
-        self.__opex = {}
-        self.__feedIn = {}
-        self.__envImpactInputs = {}                 # dictionary of dictionary of environmental impact of different inputs indexed by the building label
-        self.__envImpactTechnologies = {}           # dictionary of dictionary of environmental impact of different technologies indexed by the building label
-        self._busDict = {}
-        self.__elHP = {}
-        self.__shHP = {}
-        self.__dhwHP = {}
-        self.__annualCopHP = {}
-        self.__elGWHP = {}
-        self.__shGWHP = {}
-        self.__dhwGWHP = {}
-        self.__annualCopGWHP = {}
-        self.__elRodEff = np.nan
-        self._dispatchMode = False                         
-        if not os.path.exists(".\\log_files"):
-            os.mkdir(".\\log_files")
-        logger.define_logging(logpath=os.getcwd(), logfile=f'.\\log_files\\optihood_{datetime.now().strftime("%d.%m.%Y_%H.%M.%S")}.log')
-
-        logging.info("Initializing the energy network")
-        super(EnergyNetworkClass, self).__init__(timeindex=timestamp)
-
-    def setFromExcel(self, filePath, numberOfBuildings, clusterSize={}, opt="costs", mergeLinkBuses=False, dispatchMode=False, includeCarbonBenefits=False):
-        # does Excel file exist?
-        if not filePath or not os.path.isfile(filePath):
-            logging.error("Excel data file {} not found.".format(filePath))                                                                               
-        self._dispatchMode = dispatchMode
-        logging.info("Defining the energy network from the excel file: {}".format(filePath))
-        data = pd.ExcelFile(filePath)
-        nodesData = self.createNodesData(data, filePath, numberOfBuildings)
-        # nodesData["buses"]["excess costs"] = nodesData["buses"]["excess costs indiv"]
-        # nodesData["electricity_cost"]["cost"] = nodesData["electricity_cost"]["cost indiv"]
-
-        if clusterSize:
-            demandProfiles = {}
-            for i in range(1, numberOfBuildings + 1):
-                demandProfiles[i] = pd.concat(
-                    [nodesData["demandProfiles"][i].loc[d] for d in clusterSize.keys()])
-            electricityImpact = pd.concat(
-                [nodesData["electricity_impact"].loc[d] * clusterSize[d] for d in clusterSize.keys()])
-            electricityCost = pd.concat(
-                [nodesData["electricity_cost"].loc[d] * clusterSize[d] for d in clusterSize.keys()])
-            if 'natGas_impact' in nodesData:
-                natGasImpact = pd.concat(
-                    [nodesData["natGas_impact"].loc[d] * clusterSize[d] for d in clusterSize.keys()])
-                natGasCost = pd.concat(
-                    [nodesData["natGas_cost"].loc[d] * clusterSize[d] for d in clusterSize.keys()])
-            weatherData = pd.concat([nodesData['weather_data'][
-                                         nodesData['weather_data']['time.mm'] == int(d.split('-')[1])][
-                                         nodesData['weather_data']['time.dd'] == int(d.split('-')[2])][
-                                         ['gls', 'str.diffus', 'tre200h0', 'ground_temp']] for d in clusterSize.keys()])
-
-            nodesData["demandProfiles"] = demandProfiles
-            nodesData["electricity_impact"] = electricityImpact
-            nodesData["electricity_cost"] = electricityCost
-            if 'natGas_impact' in nodesData:
-                nodesData["natGas_impact"] = natGasImpact
-                nodesData["natGas_cost"] = natGasCost
-            nodesData["weather_data"] = weatherData
-
-        self._convertNodes(nodesData, opt, mergeLinkBuses, includeCarbonBenefits, clusterSize)
-        logging.info("Nodes from Excel file {} successfully converted".format(filePath))
-        self.add(*self._nodesList)
-        logging.info("Nodes successfully added to the energy network")
-
-    def createNodesData(self, data, filePath, numBuildings):
-        self.__noOfBuildings = numBuildings
-        nodesData = {
-            "buses": data.parse("buses"),
-            "grid_connection": data.parse("grid_connection"),
-            "commodity_sources": data.parse("commodity_sources"),
-            "solar": data.parse("solar"),
-            "transformers": data.parse("transformers"),
-            "demand": data.parse("demand"),
-            "storages": data.parse("storages"),
-            "stratified_storage": data.parse("stratified_storage"),
-            "profiles": data.parse("profiles")
-        }
-        # update stratified_storage index
-        nodesData["stratified_storage"].set_index("label", inplace=True)
-
-        # extract input data from CSVs
-        electricityImpact = nodesData["commodity_sources"].loc[nodesData["commodity_sources"]["label"] == "electricityResource", "CO2 impact"].iloc[0]
-        electricityCost = nodesData["commodity_sources"].loc[nodesData["commodity_sources"]["label"] == "electricityResource", "variable costs"].iloc[0]
-        demandProfilesPath = nodesData["profiles"].loc[nodesData["profiles"]["name"] == "demand_profiles", "path"].iloc[0]
-        weatherDataPath = nodesData["profiles"].loc[nodesData["profiles"]["name"] == "weather_data", "path"].iloc[0]
-        if "naturalGasResource" in nodesData["commodity_sources"]["label"].values:
-            natGasCost = nodesData["commodity_sources"].loc[nodesData["commodity_sources"]["label"] == "naturalGasResource", "variable costs"].iloc[0]
-            natGasImpact = nodesData["commodity_sources"].loc[
-                nodesData["commodity_sources"]["label"] == "naturalGasResource", "CO2 impact"].iloc[0]
-
-        demandProfiles = {}  # dictionary of dataframes for each building's demand profiles
-
-        if (not os.listdir(demandProfilesPath)) or (not os.path.exists(demandProfilesPath)):
-            logging.error("Error in the demand profiles path: The folder is either empty or does not exist")
-        else:
-            i = 0
-            for filename in os.listdir(demandProfilesPath): #this path should contain csv file(s) (one for each building's profiles)
-                i += 1      # Building number
-                if i > numBuildings:
-                    logging.warning("Demand profiles folder has more files than the number of buildings specified")
-                    break
-                demandProfiles.update({i: pd.read_csv(os.path.join(demandProfilesPath, filename), delimiter=";")})
-
-            nodesData["demandProfiles"] = demandProfiles
-            # set datetime index
-            for i in range(numBuildings):
-                nodesData["demandProfiles"][i + 1].set_index("timestamp", inplace=True)
-                nodesData["demandProfiles"][i + 1].index = pd.to_datetime(nodesData["demandProfiles"][i + 1].index)
-
-        if type(electricityImpact) == np.float64:
-            # for constant impact
-            electricityImpactValue = electricityImpact
-            logging.info("Constant value for electricity impact")
-            nodesData["electricity_impact"] = pd.DataFrame()
-            nodesData["electricity_impact"]["impact"] = (nodesData["demandProfiles"][1].shape[0]) * [
-                electricityImpactValue]
-            nodesData["electricity_impact"].index = nodesData["demandProfiles"][1].index
-        elif not os.path.exists(electricityImpact):
-            logging.error("Error in electricity impact file path")
-        else:
-            nodesData["electricity_impact"] = pd.read_csv(electricityImpact, delimiter=";")
-            # set datetime index
-            nodesData["electricity_impact"].set_index("timestamp", inplace=True)
-            nodesData["electricity_impact"].index = pd.to_datetime(nodesData["electricity_impact"].index)
-
-        if type(electricityCost) == np.float64:
-            # for constant cost
-            electricityCostValue = electricityCost
-            logging.info("Constant value for electricity cost")
-            nodesData["electricity_cost"] = pd.DataFrame()
-            nodesData["electricity_cost"]["cost"] = (nodesData["demandProfiles"][1].shape[0]) * [
-                electricityCostValue]
-            nodesData["electricity_cost"].index = nodesData["demandProfiles"][1].index
-        elif not os.path.exists(electricityCost):
-            logging.error("Error in electricity cost file path")
-        else:
-            nodesData["electricity_cost"] = pd.read_csv(electricityCost, delimiter=";")
-            # set datetime index
-            nodesData["electricity_cost"].set_index("timestamp", inplace=True)
-            nodesData["electricity_cost"].index = pd.to_datetime(nodesData["electricity_cost"].index)
-
-        if "naturalGasResource" in nodesData["commodity_sources"]["label"].values:
-            if type(natGasImpact) == float or (natGasImpact.split('.')[0].replace('-','').isdigit() and natGasImpact.split('.')[1].replace('-','').isdigit()):
-                # for constant impact
-                natGasImpactValue = float(natGasImpact)
-                logging.info("Constant value for natural gas impact")
-                nodesData["natGas_impact"] = pd.DataFrame()
-                nodesData["natGas_impact"]["impact"] = (nodesData["demandProfiles"][1].shape[0]) * [
-                    natGasImpactValue]
-                nodesData["natGas_impact"].index = nodesData["demandProfiles"][1].index
-            elif not os.path.exists(natGasImpact):
-                logging.error("Error in natural gas impact file path")
-            else:
-                nodesData["natGas_impact"] = pd.read_csv(natGasImpact, delimiter=";")
-                # set datetime index
-                nodesData["natGas_impact"].set_index("timestamp", inplace=True)
-                nodesData["natGas_impact"].index = pd.to_datetime(nodesData["natGas_impact"].index)
-
-            if type(natGasCost) == np.float64:
-                # for constant cost
-                natGasCostValue = natGasCost
-                logging.info("Constant value for natural gas cost")
-                nodesData["natGas_cost"] = pd.DataFrame()
-                nodesData["natGas_cost"]["cost"] = (nodesData["demandProfiles"][1].shape[0]) * [natGasCostValue]
-                nodesData["natGas_cost"].index = nodesData["demandProfiles"][1].index
-            elif not os.path.exists(natGasCost):
-                logging.error("Error in natural gas cost file path")
-            else:
-                nodesData["natGas_cost"] = pd.read_csv(natGasCost, delimiter=";")
-                # set datetime index
-                nodesData["natGas_cost"].set_index("timestamp", inplace=True)
-                nodesData["natGas_cost"].index = pd.to_datetime(nodesData["natGas_cost"].index)
-
-        if not os.path.exists(weatherDataPath):
-            logging.error("Error in weather data file path")
-        else:
-            nodesData["weather_data"] = pd.read_csv(weatherDataPath, delimiter=";")
-            #add a timestamp column to the dataframe
-            for index, row in nodesData['weather_data'].iterrows():
-                time = f"{int(row['time.yy'])}.{int(row['time.mm']):02}.{int(row['time.dd']):02} {int(row['time.hh']):02}:00:00"
-                nodesData['weather_data'].at[index, 'timestamp'] = datetime.strptime(time, "%Y.%m.%d  %H:%M:%S")
-                #set datetime index
-            nodesData["weather_data"].set_index("timestamp", inplace=True)
-            nodesData["weather_data"].index = pd.to_datetime(nodesData["weather_data"].index)
-
-        nodesData["building_model"] = pd.DataFrame()
-        nodesData["building_model"]["tAmb"] = np.array(nodesData["weather_data"]["tre200h0"])
-        nodesData["building_model"]["IrrH"] = np.array(nodesData["weather_data"]["gls"])/1000       # conversion from W/m2 to kW/m2
-        if (nodesData['demand']['building model'].notna().any()) and (nodesData['demand']['building model'] == 'Yes').any():
-            nodesData["building_model"]["Qocc"] = np.array(pd.read_csv(r"..\excels\Internal_gains.csv", delimiter=';', header=0)["Total (kW)"])
-        else:
-            logging.info("Building model either not selected or invalid string value entered")
-        logging.info("Data from Excel file {} imported.".format(filePath))
-        return nodesData
-
-    def _convertNodes(self, data, opt, mergeLinkBuses, includeCarbonBenefits, clusterSize):
-        if not data:
-            logging.error("Nodes data is missing.")
-        self.__temperatureAmb = np.array(data["weather_data"]["tre200h0"])
-        self.__temperatureGround = np.array(data["weather_data"]["ground_temp"])
-        self.__temperatureSH = data["stratified_storage"].loc["shStorage", "temp_h"]
-        self.__temperatureDHW = data["stratified_storage"].loc["dhwStorage", "temp_h"]
-        # Transformers conversion factors input power - output power
-        if any(data["transformers"]["label"] == "CHP"):
-            self.__chpEff = float(data["transformers"][data["transformers"]["label"] == "CHP"]["efficiency"].iloc[0].split(",")[1])
-        if any(data["transformers"]["label"] == "HP"):
-            self.__hpEff = float(data["transformers"][data["transformers"]["label"] == "HP"]["efficiency"].iloc[0])
-        if any(data["transformers"]["label"] == "GWHP"):
-            self.__gwhpEff = float(data["transformers"][data["transformers"]["label"] == "GWHP"]["efficiency"].iloc[0])
-        if any(data["transformers"]["label"] == "GasBoiler"):
-            self.__gbEff = float(data["transformers"][data["transformers"]["label"] == "GasBoiler"]["efficiency"].iloc[0].split(",")[0])
-        if any(data["transformers"][data["transformers"]["label"]=="ElectricRod"]["active"] == 1):
-            self.__elRodEff = float(data["transformers"][data["transformers"]["label"] == "ElectricRod"]["efficiency"].iloc[0])
-        # Storage conversion L - kWh to display the L value
-        self.__Lsh = 4.186 * (self.__temperatureSH - data["stratified_storage"].loc["shStorage", "temp_c"]) / 3600
-        self.__Ldhw = 4.186 * (self.__temperatureDHW - data["stratified_storage"].loc["dhwStorage", "temp_c"]) / 3600
-        self._addBuildings(data, opt, mergeLinkBuses, includeCarbonBenefits, clusterSize)
-
-    def _addBuildings(self, data, opt, mergeLinkBuses, includeCarbonBenefits, clusterSize):
-        numberOfBuildings = max(data["buses"]["building"])
-        self.__buildings = [Building('Building' + str(i + 1)) for i in range(numberOfBuildings)]
-        for b in self.__buildings:
-            buildingLabel = b.getBuildingLabel()
-            i = int(buildingLabel[8:])
-            if i == 1:
-                busDictBuilding1 = b.addBus(data["buses"][data["buses"]["building"] == i], opt, mergeLinkBuses, data["electricity_impact"], clusterSize, includeCarbonBenefits)
-            else:
-                b.addBus(data["buses"][data["buses"]["building"] == i], opt, mergeLinkBuses, data["electricity_impact"], clusterSize, includeCarbonBenefits)
-            if mergeLinkBuses and i!=1:
-                b.addToBusDict(busDictBuilding1)
-            b.addGridSeparation(data["grid_connection"][data["grid_connection"]["building"] == i], mergeLinkBuses)
-            if "natGas_cost" in data:
-                natGasCost = data["natGas_cost"]
-                natGasImpact = data["natGas_impact"]
-            else:
-                natGasCost = natGasImpact = None
-            b.addSource(data["commodity_sources"][data["commodity_sources"]["building"] == i], data["electricity_impact"], data["electricity_cost"], natGasCost, natGasImpact, opt)
-            b.addSink(data["demand"][data["demand"]["building"] == i], data["demandProfiles"][i], data["building_model"], mergeLinkBuses)
-            b.addTransformer(data["transformers"][data["transformers"]["building"] == i], self.__temperatureDHW,
-                             self.__temperatureSH, self.__temperatureAmb, self.__temperatureGround, opt, mergeLinkBuses, self._dispatchMode)
-            #if any(data["transformers"]["label"] == "HP") or any(data["transformers"]["label"] == "GWHP"):   #add electricity rod if HP or GSHP is present in the available technology pool
-            #    b.addElectricRodBackup(opt)
-            b.addStorage(data["storages"][data["storages"]["building"] == i], data["stratified_storage"], opt, mergeLinkBuses, self._dispatchMode)
-            b.addSolar(data["solar"][(data["solar"]["building"] == i) & (data["solar"]["label"] == "solarCollector")], data["weather_data"], opt, mergeLinkBuses, self._dispatchMode)
-            b.addPV(data["solar"][(data["solar"]["building"] == i) & (data["solar"]["label"] == "pv")], data["weather_data"], opt, self._dispatchMode)
-            b.addPVT(data["solar"][(data["solar"]["building"] == i) & (data["solar"]["label"] == "pvt")], data["weather_data"], opt, mergeLinkBuses, self._dispatchMode)
-            self._nodesList.extend(b.getNodesList())
-            self.__inputs[buildingLabel] = b.getInputs()
-            self.__technologies[buildingLabel] = b.getTechnologies()
-            self.__costParam.update(b.getCostParam())
-            self.__envParam.update(b.getEnvParam())
-            self._busDict.update(b.getBusDict())
-            self.__capacitiesTransformersBuilding[buildingLabel] = {}
-            self.__capacitiesStoragesBuilding[buildingLabel] = {}
-            self.__envImpactInputs[buildingLabel] = {}
-            self.__opex[buildingLabel] = {}
-            self.__envImpactTechnologies[buildingLabel] = {}
-
-    def printNodes(self):
-        print("*********************************************************")
-        print("The following objects have been created from excel sheet:")
-        for n in self.nodes:
-            oobj = str(type(n)).replace("<class 'oemof.solph.", "").replace("'>", "")
-            print(oobj + ":", n.label)
-        print("*********************************************************")
-
-    def optimize(self, numberOfBuildings, solver, envImpactlimit=1000000, clusterSize={},
-                 options=None,   # solver options
-                 optConstraints=None, #optional constraints (implemented for the moment are "roof area"
-                 mergeLinkBuses=False):
-
-        if options is None:
-            options = {"gurobi": {"MIPGap": 0.01}}
-
-        optimizationModel = solph.Model(self)
-        logging.info("Optimization model built successfully")
-
-        # add constraint to limit the environmental impacts
-        optimizationModel, flows, transformerFlowCapacityDict, storageCapacityDict = environmentalImpactlimit(
-            optimizationModel, keyword1="env_per_flow", keyword2="env_per_capa", limit=envImpactlimit)
-
-        # optional constraints (available: 'roof area')
-        if optConstraints:
-            for c in optConstraints:
-                if c.lower() == "roof area":
-                    # requires 2 additional parameters in the scenario file, tab "solar", zenit angle, roof area
-                    try:
-                        optimizationModel = roof_area_limit(optimizationModel,
-                                                        keyword1="space", keyword2="roof_area", nb=numberOfBuildings)
-                        logging.info(f"Optional constraint {c} successfully added to the optimization model")
-                    except ValueError:
-                        logging.error(f"Optional constraint {c} not added to the optimization model : "
-                                      f"please check if PV efficiency, roof area and zenith angle are present in input "
-                                      f"file")
-                        pass
-                if c.lower() == 'totalpvcapacity':
-                    optimizationModel = totalPVCapacityConstraint(optimizationModel, numberOfBuildings)
-                    logging.info(f"Optional constraint {c} successfully added to the optimization model")
-        # constraint on elRod combined with HPs:
-        if not np.isnan(self.__elRodEff):
-            optimizationModel = electricRodCapacityConstaint(optimizationModel, numberOfBuildings)
-        # constraint on PVT capacity if PVT technology is selected
-        if any("pvt" in n.label for n in self.nodes):
-            optimizationModel = PVTElectricalThermalCapacityConstraint(optimizationModel, numberOfBuildings)
-        # constraint on storage content for clustering
-        """if clusterSize:
-            optimizationModel = dailySHStorageConstraint(optimizationModel)"""
-
-        logging.info("Custom constraints successfully added to the optimization model")
-
-        if solver == "gurobi":
-            logging.info("Initiating optimization using {} solver".format(solver))
-
-        optimizationModel.solve(solver=solver, cmdline_options=options[solver])
-
-        # obtain the value of the environmental impact (subject to the limit constraint)
-        # the optimization imposes an integral limit constraint on the environmental impacts
-        # total environmental impacts <= envImpactlimit
-        envImpact = optimizationModel.totalEnvironmentalImpact()
-
-        self._optimizationResults = solph.processing.results(optimizationModel)
-        self._metaResults = solph.processing.meta_results(optimizationModel)
-        logging.info("Optimization successful and results collected")
-
-        # calculate capacities invested for transformers and storages (for the entire energy network and per building)
-        capacitiesTransformersNetwork, capacitiesStoragesNetwork = self._calculateInvestedCapacities(optimizationModel, transformerFlowCapacityDict, storageCapacityDict)
-
-        if clusterSize:
-            self._postprocessingClusters(clusterSize)
-
-        # calculate results (CAPEX, OPEX, FeedIn Costs, environmental impacts etc...) for each building
-        self._calculateResultsPerBuilding(mergeLinkBuses)
-
-        return envImpact, capacitiesTransformersNetwork, capacitiesStoragesNetwork
-
-    def saveUnprocessedResults(self, resultFile):
-        with pd.ExcelWriter(resultFile) as writer:
-            busLabelList = []
-            for i in self.nodes:
-                if str(type(i)).replace("<class 'oemof.solph.", "").replace("'>", "") == "network.bus.Bus":
-                    busLabelList.append(i.label)
-            for i in busLabelList:
-                result = pd.DataFrame.from_dict(solph.views.node(self._optimizationResults, i)["sequences"])
-                result.to_excel(writer, sheet_name=i)
-            writer.save()
-
-    def _updateCapacityDictInputInvestment(self, transformerFlowCapacityDict):
-        components = ["CHP", "GWHP", "HP", "GasBoiler", "ElectricRod"]
-        for inflow, outflow in list(transformerFlowCapacityDict):
-            index = (inflow, outflow)
-            if "__" in str(inflow):
-                buildingLabel = str(inflow).split("__")[1]
-            elif "__" in str(outflow):
-                buildingLabel = str(outflow).split("__")[1]
-            if any(c in str(outflow) for c in components):
-                newoutFlow = f"shSourceBus__{buildingLabel}"
-                newIndex = (outflow,newoutFlow)
-                transformerFlowCapacityDict[newIndex] = transformerFlowCapacityDict.pop(index)
-            if 'elSource_pvt' in str(inflow):   # remove PVT electrical capacity
-                transformerFlowCapacityDict.pop(index)
-        return transformerFlowCapacityDict
-
-    def _calculateInvestedCapacities(self, optimizationModel, transformerFlowCapacityDict, storageCapacityDict):
-        capacitiesInvestedTransformers = {}
-        capacitiesInvestedStorages = {}
-        storageList = []
-
-        # Transformers capacities
-
-        for inflow, outflow in transformerFlowCapacityDict:
-            index = (str(inflow), str(outflow))
-            capacitiesInvestedTransformers[index] = optimizationModel.InvestmentFlow.invest[inflow, outflow].value
-
-        # Conversion into output capacity
-        capacitiesInvestedTransformers = self._compensateInputCapacities(capacitiesInvestedTransformers)
-
-        # update transformerFlowCapacityDict such that investment objects with input flows are accounted properly in the results calculation
-        transformerFlowCapacityDict = self._updateCapacityDictInputInvestment(transformerFlowCapacityDict)
-
-        # Update capacities
-        for inflow, outflow in transformerFlowCapacityDict:
-            index = (str(inflow), str(outflow))
-            buildingLabel = str(inflow).split("__")[1]
-            self.__capacitiesTransformersBuilding[buildingLabel].update({index: capacitiesInvestedTransformers[index]})
-
-        # Storages capacities
-        for x in storageCapacityDict:
-            index = str(x)
-            if x in storageList:  # useful when we want to implement two or more storage units of the same type
-                capacitiesInvestedStorages[index] = capacitiesInvestedStorages[index] + \
-                                                    optimizationModel.GenericInvestmentStorageBlock.invest[x].value
-            else:
-                capacitiesInvestedStorages[str(x)] = optimizationModel.GenericInvestmentStorageBlock.invest[x].value
-
-        # Convert kWh into L
-        capacitiesInvestedStorages = self._compensateStorageCapacities(capacitiesInvestedStorages)
-
-        # Update capacities
-        for x in storageCapacityDict:
-            index = str(x)
-            buildingLabel = index.split("__")[1]
-            if x in storageList:  # useful when we want to implement two or more storage units of the same type
-                self.__capacitiesStoragesBuilding[buildingLabel].update(
-                    {index: capacitiesInvestedStorages[index]})
-            else:
-                self.__capacitiesStoragesBuilding[buildingLabel].update({index: capacitiesInvestedStorages[index]})
-            storageList.append(x)
-
-        return capacitiesInvestedTransformers, capacitiesInvestedStorages
-
-    def _compensateInputCapacities(self, capacitiesTransformers):
-        # Input capacity -> output capacity
-        for first, second in list(capacitiesTransformers):
-            if "CHP" in second:
-                for index, value in enumerate(self.nodes):
-                    if second == value.label:
-                        test = self.nodes[index].conversion_factors
-                        for t in test.keys():
-                            if "shSource" in t.label:
-                                capacitiesTransformers[(second,t.label)]= capacitiesTransformers[(first,second)]*self.__chpEff
-                                del capacitiesTransformers[(first,second)]
-            elif "GWHP" in second and not any([c.isdigit() for c in second.split("__")[0]]):  # second condition added for splitted GSHPs
-                for index, value in enumerate(self.nodes):
-                    if second == value.label:
-                        test = self.nodes[index].conversion_factors
-                        for t in test.keys():
-                            if "shSource" in t.label:
-                                capacitiesTransformers[(second, t.label)] = capacitiesTransformers[(first, second)] * self.__gwhpEff
-                                del capacitiesTransformers[(first, second)]
-            elif "HP" in second and "GWHP" not in second:
-                for index, value in enumerate(self.nodes):
-                    if second == value.label:
-                        test = self.nodes[index].conversion_factors
-                        for t in test.keys():
-                            if "shSource" in t.label:
-                                capacitiesTransformers[(second, t.label)] = capacitiesTransformers[(first, second)]*self.__hpEff
-                                del capacitiesTransformers[(first, second)]
-            elif "GasBoiler" in second:
-                for index, value in enumerate(self.nodes):
-                    if second == value.label:
-                        test = self.nodes[index].conversion_factors
-                        for t in test.keys():
-                            if "shSource" in t.label:
-                                capacitiesTransformers[(second, t.label)] = capacitiesTransformers[(
-                                first, second)] * self.__gbEff
-                                del capacitiesTransformers[(first, second)]
-            elif "ElectricRod" in second:
-                for index, value in enumerate(self.nodes):
-                    if second == value.label:
-                        test = self.nodes[index].conversion_factors
-                        for t in test.keys():
-                            if "shSource" in t.label:
-                                capacitiesTransformers[(second, t.label)] = capacitiesTransformers[(
-                                first, second)] * self.__elRodEff
-                                del capacitiesTransformers[(first, second)]
-
-        return capacitiesTransformers
-
-    def _compensateStorageCapacities(self, capacitiesStorages):
-        # kWh -> L
-        for storage in capacitiesStorages.keys():
-            if "sh" in storage:
-                capacitiesStorages[storage] = capacitiesStorages[storage] / self.__Lsh
-            elif "dhw" in storage:
-                capacitiesStorages[storage] = capacitiesStorages[storage] / self.__Ldhw
-        return capacitiesStorages
-
-    def _postprocessingClusters(self, clusterSize):
-        flows = [x for x in self._optimizationResults.keys() if x[1] is not None]
-        for flow in flows:
-            extrapolated_results = None
-            for day in clusterSize:
-                temp = pd.concat([self._optimizationResults[flow]['sequences'][self._clusterDate[day]]] * clusterSize[day])
-                if extrapolated_results is not None:
-                    extrapolated_results = pd.concat([extrapolated_results, temp])
-                else:
-                    extrapolated_results = temp
-            extrapolated_results.index = self._timeIndexReal
-            extrapolated_results.columns = ['flow']
-            self._optimizationResults[flow]['sequences'] = extrapolated_results
-
-    def _calculateResultsPerBuilding(self, mergeLinkBuses):
-        for b in self.__buildings:
-            buildingLabel = b.getBuildingLabel()
-            capacityTransformers = self.__capacitiesTransformersBuilding[buildingLabel]
-            capacityStorages = self.__capacitiesStoragesBuilding[buildingLabel]
-            technologies = self.__technologies[buildingLabel]
-            inputs = self.__inputs[buildingLabel]
-
-            # CAPital investment EXpenditure
-            self.__capex[buildingLabel] = sum((self.__costParam[i][1] * (capacityTransformers[(i, o)] > 1))             # base investment cost if the technology is implemented
-                                              + (capacityTransformers[(i, o)] * self.__costParam[i][0])                 # investment cost per unit capacity
-                                              for i, o in capacityTransformers) + \
-                                          sum((self.__costParam[x][1] * (capacityStorages[x] > 1))                      # base investment cost if the technology is implemented
-                                              + (capacityStorages[x] * self.__costParam[x][0])                          # investment cost per unit capacity
-                                              for x in capacityStorages)
-
-            electricitySourceLabel = "electricityResource" + '__' + buildingLabel
-            gridBusLabel = "gridBus" + '__' + buildingLabel
-            if mergeLinkBuses:
-                electricityBusLabel = "electricityBus"
-                excessElectricityBusLabel = "excesselectricityBus"
-            else:
-                electricityBusLabel = "electricityBus" + '__' + buildingLabel
-                excessElectricityBusLabel = "excesselectricityBus" + '__' + buildingLabel
-
-            if electricitySourceLabel in self.__costParam:
-                costParamGridElectricity = self.__costParam[electricitySourceLabel].copy()
-                costParamGridElectricity.reset_index(inplace=True, drop=True)
-            else:
-                costParamGridElectricity = 0
-            if "sequences" in solph.views.node(self._optimizationResults, gridBusLabel):
-                if ((electricitySourceLabel, gridBusLabel), "flow") in solph.views.node(self._optimizationResults, gridBusLabel)["sequences"]:
-                    gridElectricityFlow = solph.views.node(self._optimizationResults, gridBusLabel)["sequences"][
-                        (electricitySourceLabel, gridBusLabel), "flow"]
-                    gridElectricityFlow.reset_index(inplace=True, drop=True)
-                else:
-                    gridElectricityFlow = 0
-            else:
-                gridElectricityFlow = 0
-
-            # OPeration EXpenditure
-            self.__opex[buildingLabel].update({i[0]: sum(
-                solph.views.node(self._optimizationResults, i[1])["sequences"][(i[0], i[1]), "flow"] * self.__costParam[
-                    i[0]]) for i in inputs})
-            c = costParamGridElectricity * gridElectricityFlow
-            if isinstance(c, (int, float)):
-                self.__opex[buildingLabel].update({electricitySourceLabel:c})
-            else:
-                self.__opex[buildingLabel].update({electricitySourceLabel: c.sum()})  # cost of grid electricity is added separately based on cost data
-
-            # Feed-in electricity cost (value will be in negative to signify monetary gain...)
-            if ((mergeLinkBuses and buildingLabel=='Building1') or not mergeLinkBuses) and \
-                    (((electricityBusLabel, excessElectricityBusLabel), "flow") in solph.views.node(self._optimizationResults, electricityBusLabel)["sequences"]):
-                self.__feedIn[buildingLabel] = sum(solph.views.node(self._optimizationResults, electricityBusLabel)
-                                                   ["sequences"][(electricityBusLabel, excessElectricityBusLabel), "flow"]) * self.__costParam[excessElectricityBusLabel]
-            else: # in case of merged links feed in for all buildings except Building1 is set to 0 (to avoid repetition)
-                self.__feedIn[buildingLabel] = 0
-            if mergeLinkBuses:
-                elInBusLabel = 'electricityInBus'
-            else:
-                elInBusLabel = 'electricityInBus__'+buildingLabel
-            # HP flows
-            if ("HP__" + buildingLabel, "shSourceBus__" + buildingLabel) in capacityTransformers:
-                self.__elHP[buildingLabel] = sum(
-                    solph.views.node(self._optimizationResults, elInBusLabel)["sequences"][
-                        (elInBusLabel, 'HP__'+buildingLabel), 'flow'])
-                self.__shHP[buildingLabel] = sum(
-                    solph.views.node(self._optimizationResults, 'HP__' + buildingLabel)["sequences"][
-                        ('HP__' + buildingLabel, 'shSourceBus__' + buildingLabel), 'flow'])
-                self.__dhwHP[buildingLabel] = sum(
-                    solph.views.node(self._optimizationResults, 'HP__' + buildingLabel)["sequences"][
-                        ('HP__' + buildingLabel, 'dhwStorageBus__' + buildingLabel), 'flow'])
-                self.__annualCopHP[buildingLabel] = (self.__shHP[buildingLabel] + self.__dhwHP[buildingLabel]) / (
-                    self.__elHP[buildingLabel] + 1e-6)
-
-            # GWHP flows
-            if ("GWHP__" + buildingLabel, "shSourceBus__" + buildingLabel) in capacityTransformers:
-                self.__elGWHP[buildingLabel] = sum(
-                    solph.views.node(self._optimizationResults, elInBusLabel)["sequences"][
-                        (elInBusLabel, 'GWHP__' + buildingLabel), 'flow'])
-                self.__shGWHP[buildingLabel] = sum(
-                    solph.views.node(self._optimizationResults, 'GWHP__' + buildingLabel)["sequences"][
-                        ('GWHP__' + buildingLabel, 'shSourceBus__' + buildingLabel), 'flow'])
-                self.__dhwGWHP[buildingLabel] = sum(
-                    solph.views.node(self._optimizationResults, 'GWHP__' + buildingLabel)["sequences"][
-                        ('GWHP__' + buildingLabel, 'dhwStorageBus__' + buildingLabel), 'flow'])
-                self.__annualCopGWHP[buildingLabel] = (self.__shGWHP[buildingLabel] + self.__dhwGWHP[buildingLabel]) / (
-                        self.__elGWHP[buildingLabel] + 1e-6)
-            else:       # splitted GSHP
-                self.__annualCopGWHP[buildingLabel] = []
-                if (f"GWHP{str(self.__temperatureSH)}__" + buildingLabel, "shSourceBus__" + buildingLabel) in capacityTransformers:
-                    self.__elGWHP[buildingLabel] = sum(
-                        solph.views.node(self._optimizationResults, elInBusLabel)["sequences"][
-                            (elInBusLabel, f"GWHP{str(self.__temperatureSH)}__" + buildingLabel), 'flow'])
-                    self.__shGWHP[buildingLabel] = sum(
-                        solph.views.node(self._optimizationResults, f"GWHP{str(self.__temperatureSH)}__" + buildingLabel)["sequences"][
-                            (f"GWHP{str(self.__temperatureSH)}__" + buildingLabel, 'shSourceBus__' + buildingLabel), 'flow'])
-                    self.__annualCopGWHP[buildingLabel].append((self.__shGWHP[buildingLabel]) / (self.__elGWHP[buildingLabel] + 1e-6))
-                if (f"GWHP{str(self.__temperatureDHW)}__" + buildingLabel, "dhwStorageBus__" + buildingLabel) in capacityTransformers:
-                    self.__elGWHP[buildingLabel] = sum(
-                        solph.views.node(self._optimizationResults, elInBusLabel)["sequences"][
-                            (elInBusLabel, f"GWHP{str(self.__temperatureDHW)}__" + buildingLabel), 'flow'])
-                    self.__dhwGWHP[buildingLabel] = sum(
-                        solph.views.node(self._optimizationResults, f"GWHP{str(self.__temperatureDHW)}__" + buildingLabel)["sequences"][
-                            (f"GWHP{str(self.__temperatureDHW)}__" + buildingLabel, 'dhwStorageBus__' + buildingLabel), 'flow'])
-                    self.__annualCopGWHP[buildingLabel].append((self.__dhwGWHP[
-                        buildingLabel]) / (self.__elGWHP[buildingLabel] + 1e-6))
-
-            if electricitySourceLabel in self.__envParam:
-                envParamGridElectricity = self.__envParam[electricitySourceLabel].copy()
-                envParamGridElectricity.reset_index(inplace=True, drop=True)
-            else:
-                envParamGridElectricity = 0
-            # gridElectricityFlow = solph.views.node(self._optimizationResults, gridBusLabel)["sequences"][
-            #     (electricitySourceLabel, gridBusLabel), "flow"]
-            # gridElectricityFlow.reset_index(inplace=True, drop=True)
-
-            # Environmental impact due to inputs (natural gas, electricity, etc...)
-            self.__envImpactInputs[buildingLabel].update({i[0]: sum(solph.views.node(self._optimizationResults, i[1])["sequences"][(i[0], i[1]), "flow"] * self.__envParam[i[0]]) for i in inputs})
-            c = envParamGridElectricity * gridElectricityFlow
-            if isinstance(c, (int, float)):
-                self.__envImpactInputs[buildingLabel].update({electricitySourceLabel: c})
-            else:
-                self.__envImpactInputs[buildingLabel].update({electricitySourceLabel: c.sum()})  # impact of grid electricity is added separately based on LCA data
-
-            # Environmental impact due to technologies (converters, storages)
-            # calculated by adding both environmental impact per capacity and per flow (electrical flow or heat flow)
-            self.__envImpactTechnologies[buildingLabel].update({i: capacityTransformers[(i, o)] * self.__envParam[i][2] +
-                                                                   sum(sum(solph.views.node(self._optimizationResults,
-                                                                                            t[0])["sequences"][((t[1], t[0]), "flow")] *
-                                                                           self.__envParam[t[1]][1] * ('electricityBus' in t[0]) + \
-                                                                           solph.views.node(self._optimizationResults,
-                                                                                            t[0])["sequences"][((t[1], t[0]), "flow")] *
-                                                                           self.__envParam[t[1]][0] * ('electricityBus' not in t[0]))
-                                                                       for t in technologies if t[1] == i)
-                                                                for i, o in capacityTransformers})
-            self.__envImpactTechnologies[buildingLabel].update({x: capacityStorages[x] * self.__envParam[x][2] +
-                                                                   sum(sum(
-                                                                       solph.views.node(self._optimizationResults,
-                                                                                        t[0])["sequences"][((t[1], t[0]), "flow")] *
-                                                                       self.__envParam[t[1]][1] * ('electricityBus' in t[0]) + \
-                                                                       solph.views.node(self._optimizationResults,
-                                                                                        t[0])["sequences"][((t[1], t[0]), "flow")] *
-                                                                       self.__envParam[t[1]][0] * ('electricityBus' not in t[0]))
-                                                                       for t in technologies if t[1] == x)
-                                                                for x in capacityStorages})
-
-    def printMetaresults(self):
-        print("Meta Results:")
-        pp.pprint(self._metaResults)
-        print("")
-        return self._metaResults
-
-    def calcStateofCharge(self, type, building):
-        if type + '__' + building in self.groups:
-            storage = self.groups[type + '__' + building]
-            # print(f"""********* State of Charge ({type},{building}) *********""")
-            # print(
-            #    self._optimizationResults[(storage, None)]["sequences"]
-            # )
-            self._storageContentSH[building] = self._optimizationResults[(storage, None)]["sequences"]
-        print("")
-
-    def printInvestedCapacities(self, capacitiesInvestedTransformers, capacitiesInvestedStorages):
-        for b in range(len(self.__buildings)):
-            buildingLabel = "Building" + str(b + 1)
-            print("************** Optimized Capacities for {} **************".format(buildingLabel))
-            if ("HP__" + buildingLabel, "shSourceBus__" + buildingLabel) in capacitiesInvestedTransformers:
-                investSH = capacitiesInvestedTransformers[("HP__" + buildingLabel, "shSourceBus__" + buildingLabel)]
-                print("Invested in {:.1f} kW HP.".format(investSH))
-                print("     Annual COP = {:.1f}".format(self.__annualCopHP[buildingLabel]))
-            if ("GWHP__" + buildingLabel, "shSourceBus__" + buildingLabel) in capacitiesInvestedTransformers:
-                investSH = capacitiesInvestedTransformers[("GWHP__" + buildingLabel, "shSourceBus__" + buildingLabel)]
-                print("Invested in {:.1f} kW GWHP.".format(investSH))
-                print("     Annual COP = {:.1f}".format(self.__annualCopGWHP[buildingLabel]))
-            if (f"GWHP{str(self.__temperatureSH)}__" + buildingLabel, "shSourceBus__" + buildingLabel) in capacitiesInvestedTransformers:
-                investSH = capacitiesInvestedTransformers[(f"GWHP{str(self.__temperatureSH)}__" + buildingLabel, "shSourceBus__" + buildingLabel)]
-                print("Invested in {:.1f} kW GWHP{}.".format(investSH, str(self.__temperatureSH)))
-                print("     Annual COP = {:.1f}".format(self.__annualCopGWHP[buildingLabel][0]))
-            if (f"GWHP{str(self.__temperatureDHW)}__" + buildingLabel, "dhwStorageBus__" + buildingLabel) in capacitiesInvestedTransformers:
-                investSH = capacitiesInvestedTransformers[(f"GWHP{str(self.__temperatureDHW)}__" + buildingLabel, "dhwStorageBus__" + buildingLabel)]
-                print("Invested in {:.1f} kW GWHP{}.".format(investSH, str(self.__temperatureDHW)))
-                print("     Annual COP = {:.1f}".format(self.__annualCopGWHP[buildingLabel][1]))
-            if ("ElectricRod__" + buildingLabel, "shSourceBus__" + buildingLabel) in capacitiesInvestedTransformers:
-                investSH = capacitiesInvestedTransformers[("ElectricRod__" + buildingLabel, "shSourceBus__" + buildingLabel)]
-                print("Invested in {:.1f} kW Electric Rod.".format(investSH))
-            if ("CHP__" + buildingLabel, "shSourceBus__" + buildingLabel) in capacitiesInvestedTransformers:
-                investSH = capacitiesInvestedTransformers["CHP__" + buildingLabel, "shSourceBus__" + buildingLabel]
-                print("Invested in {:.1f} kW CHP.".format(investSH))  # + investEL))
-            if ("GasBoiler__" + buildingLabel, "shSourceBus__" + buildingLabel) in capacitiesInvestedTransformers:
-                investSH = capacitiesInvestedTransformers["GasBoiler__" + buildingLabel, "shSourceBus__" + buildingLabel]
-                print("Invested in {:.1f} kW GasBoiler.".format(investSH))
-            if ("heat_solarCollector__" + buildingLabel, "solarConnectBus__" + buildingLabel) in capacitiesInvestedTransformers:
-                invest = capacitiesInvestedTransformers[("heat_solarCollector__" + buildingLabel, "solarConnectBus__" + buildingLabel)]
-                print("Invested in {:.1f} m² SolarCollector.".format(invest))
-            if ("pv__" + buildingLabel, "electricityProdBus__" + buildingLabel) in capacitiesInvestedTransformers:
-                invest = capacitiesInvestedTransformers[("pv__" + buildingLabel, "electricityProdBus__" + buildingLabel)]
-                print("Invested in {:.1f} kWp  PV.".format(invest))
-            if ("heatSource_SHpvt__" + buildingLabel, "pvtConnectBusSH__" + buildingLabel) in capacitiesInvestedTransformers:
-                invest = capacitiesInvestedTransformers[("heatSource_SHpvt__" + buildingLabel, "pvtConnectBusSH__" + buildingLabel)]
-                print("Invested in {:.1f} m² PVT collector.".format(invest))
-            if "electricalStorage__" + buildingLabel in capacitiesInvestedStorages:
-                invest = capacitiesInvestedStorages["electricalStorage__" + buildingLabel]
-                print("Invested in {:.1f} kWh Electrical Storage.".format(invest))
-            if "dhwStorage__" + buildingLabel in capacitiesInvestedStorages:
-                invest = capacitiesInvestedStorages["dhwStorage__" + buildingLabel]
-                print("Invested in {:.1f} L DHW Storage Tank.".format(invest))
-            if "shStorage__" + buildingLabel in capacitiesInvestedStorages:
-                invest = capacitiesInvestedStorages["shStorage__" + buildingLabel]
-                print("Invested in {:.1f} L SH Storage Tank.".format(invest))
-
-    def printCosts(self):
-        capexNetwork = sum(self.__capex["Building" + str(b + 1)] for b in range(len(self.__buildings)))
-        opexNetwork = sum(sum(self.__opex["Building" + str(b + 1)].values()) for b in range(len(self.__buildings)))
-        feedinNetwork = sum(self.__feedIn["Building" + str(b + 1)] for b in range(len(self.__buildings)))
-        print("Investment Costs for the system: {} CHF".format(capexNetwork))
-        print("Operation Costs for the system: {} CHF".format(opexNetwork))
-            # (sum(self.__opex["Building" + str(b + 1)] for b in range(len(self.__buildings)))))
-        print("Feed In Costs for the system: {} CHF".format(feedinNetwork))
-        print("Total Costs for the system: {} CHF".format(capexNetwork + opexNetwork + feedinNetwork))
-
-    def printEnvImpacts(self):
-        envImpactInputsNetwork = sum(sum(self.__envImpactInputs["Building" + str(b + 1)].values()) for b in range(len(self.__buildings)))
-        envImpactTechnologiesNetwork = sum(sum(self.__envImpactTechnologies["Building" + str(b + 1)].values()) for b in range(len(self.__buildings)))
-        print("Environmental impact from input resources for the system: {} kg CO2 eq".format(envImpactInputsNetwork))
-        print("Environmental impact from energy conversion technologies for the system: {} kg CO2 eq".format(envImpactTechnologiesNetwork))
-        print("Total: {} kg CO2 eq".format(envImpactInputsNetwork + envImpactTechnologiesNetwork))
-
-    def getTotalCosts(self):
-        capexNetwork = sum(self.__capex["Building" + str(b + 1)] for b in range(len(self.__buildings)))
-        opexNetwork = sum(
-            sum(self.__opex["Building" + str(b + 1)].values()) for b in range(len(self.__buildings)))
-        feedinNetwork = sum(self.__feedIn["Building" + str(b + 1)] for b in range(len(self.__buildings)))
-        return capexNetwork + opexNetwork + feedinNetwork
-
-    def getTotalEnvImpacts(self):
-        envImpactInputsNetwork = sum(
-            sum(self.__envImpactInputs["Building" + str(b + 1)].values()) for b in range(len(self.__buildings)))
-        envImpactTechnologiesNetwork = sum(
-            sum(self.__envImpactTechnologies["Building" + str(b + 1)].values()) for b in range(len(self.__buildings)))
-        return envImpactTechnologiesNetwork + envImpactInputsNetwork
-
-    def exportToExcel(self, file_name, mergeLinkBuses=False):
-        for i in range(1, self.__noOfBuildings+1):
-            self.calcStateofCharge("shStorage", f"Building{i}")
-        with pd.ExcelWriter(file_name) as writer:
-            busLabelList = []
-            for i in self.nodes:
-                if str(type(i)).replace("<class 'oemof.solph.", "").replace("'>", "") == "network.bus.Bus":
-                    busLabelList.append(i.label)
-            # writing results of each bus into excel
-            for i in busLabelList:
-                if "domesticHotWaterBus" in i:  # special case for DHW bus (output from transformers --> dhwStorageBus --> DHW storage --> domesticHotWaterBus --> DHW Demand)
-                    if not mergeLinkBuses:
-                        dhwStorageBusLabel = "dhwStorageBus__" + i.split("__")[1]
-                        resultDHW = pd.DataFrame.from_dict(solph.views.node(self._optimizationResults, i)["sequences"])  # result sequences of DHW bus
-                        resultDHWStorage = pd.DataFrame.from_dict(solph.views.node(self._optimizationResults, dhwStorageBusLabel)["sequences"])  # result sequences of DHW storage bus
-                        result = pd.concat([resultDHW, resultDHWStorage], axis=1, sort=True)
-                    else:
-                        result = pd.DataFrame.from_dict(solph.views.node(self._optimizationResults, i)["sequences"])  # result sequences of DHW bus
-                elif mergeLinkBuses and "dhwStorageBus" in i and "sequences" in solph.views.node(self._optimizationResults, i):
-                    result = pd.DataFrame.from_dict(solph.views.node(self._optimizationResults, i)["sequences"])  # result sequences of DHW storage bus
-                elif "dhwStorageBus" not in i:  # for all the other buses except DHW storage bus (as it is already considered with DHW bus)
-                    if 'sequences' in solph.views.node(self._optimizationResults, i):
-                        result = pd.DataFrame.from_dict(solph.views.node(self._optimizationResults, i)["sequences"])
-                        if "shSourceBus" in i and i.split("__")[1] in self._storageContentSH:
-                            result = pd.concat([result, self._storageContentSH[i.split("__")[1]]], axis=1, sort=True)
-                    else:
-                        continue
-                result[result < 0.001] = 0      # to resolve the issue of very low values in the results in certain cases, values less than 1 Watt would be replaced by 0
-                if mergeLinkBuses or "dhwStorageBus" not in i:
-                    result.to_excel(writer, sheet_name=i)
-
-            # writing the costs and environmental impacts (of different components...) for each building
-            for b in self.__buildings:
-                buildingLabel = b.getBuildingLabel()
-                costs = self.__opex[buildingLabel]
-                costs.update({"Investment": self.__capex[buildingLabel],
-                              "Feed-in": self.__feedIn[buildingLabel]})
-                    # {"Operation": self.__opex[buildingLabel],
-                    #      "Investment": self.__capex[buildingLabel],
-                    #      "Feed-in": self.__feedIn[buildingLabel],
-                    #      }
-                costsBuilding = pd.DataFrame.from_dict(costs, orient='index')
-                costsBuilding.to_excel(writer, sheet_name="costs__" + buildingLabel)
-
-                envImpact = self.__envImpactInputs[buildingLabel].copy()
-                envImpact.update(self.__envImpactTechnologies[buildingLabel])
-
-                envImpactBuilding = pd.DataFrame.from_dict(envImpact, orient='index')
-                envImpactBuilding.to_excel(writer, sheet_name="env_impacts__" + buildingLabel)
-
-                capacitiesStorages = self.__capacitiesStoragesBuilding[buildingLabel].copy()
-                capacitiesStorages.update(self.__capacitiesStoragesBuilding[buildingLabel])
-
-                capacitiesStoragesBuilding = pd.DataFrame.from_dict(capacitiesStorages, orient='index')
-                capacitiesStoragesBuilding.to_excel(writer, sheet_name="capStorages__" + buildingLabel)
-
-                capacitiesTransformers = self.__capacitiesTransformersBuilding[buildingLabel].copy()
-                capacitiesTransformers.update(self.__capacitiesTransformersBuilding[buildingLabel])
-
-                capacitiesTransformersBuilding = pd.DataFrame.from_dict(capacitiesTransformers, orient='index')
-                capacitiesTransformersBuilding.to_excel(writer, sheet_name="capTransformers__" + buildingLabel)
-
-class EnergyNetworkIndiv(EnergyNetworkClass):
-    def createScenarioFile(self, configFilePath, excelFilePath, building, numberOfBuildings=1):
-        """function to create the input excel file from a config file
-        saves the generated excel file at the path given by excelFilePath"""
-        config = ConfigParser()
-        config.read(configFilePath)
-        configData = {}
-        excelData= {}
-        columnNames = {'commodity_sources': ['label', 'building', 'to', 'variable costs', 'CO2 impact', 'active'],# column names are defined for each sheet (key of dict) in the excel file
-                       'solar': ['label', 'building', 'from', 'to', 'connect', 'electrical_consumption', 'peripheral_losses', 'latitude', 'longitude', 'tilt', 'azimuth', 'eta_0', 'a_1', 'a_2', 'temp_collector_inlet', 'delta_temp_n', 'capacity_max', 'capacity_min', 'lifetime', 'maintenance', 'installation', 'planification', 'invest_base', 'invest_cap', 'heat_impact', 'elec_impact', 'impact_cap'],
-                       'demand': ['label', 'building', 'active', 'from', 'fixed', 'nominal value', 'building model'],
-                       'transformers': ['label', 'building', 'active', 'from', 'to', 'efficiency', 'capacity_DHW', 'capacity_SH', 'capacity_el', 'capacity_min', 'lifetime', 'maintenance', 'installation', 'planification', 'invest_base', 'invest_cap', 'heat_impact', 'elec_impact', 'impact_cap'],
-                       'storages': ['label', 'building', 'active', 'from', 'to', 'efficiency inflow', 'efficiency outflow', 'initial capacity', 'capacity min', 'capacity max', 'capacity loss', 'lifetime', 'maintenance', 'installation', 'planification', 'invest_base', 'invest_cap', 'heat_impact', 'elec_impact', 'impact_cap'],
-                       'stratified_storage': ['label', 'diameter', 'temp_h', 'temp_c', 'temp_env', 'inflow_conversion_factor', 'outflow_conversion_factor', 's_iso', 'lamb_iso', 'alpha_inside', 'alpha_outside']
-                       }
-        buses = {'naturalgasresource': ['naturalGasBus', '', ''], 'electricityresource': ['gridBus', '', ''], 'solarcollector': ['dhwStorageBus', 'electricityInBus', 'solarConnectBus'],    # [to, from, connect] columns in the excel file
-                 'pv': ['electricityProdBus', '', ''], 'electricitydemand': ['', 'electricityInBus', ''], 'spaceheatingdemand': ['', 'shDemandBus', ''],
-                 'domestichotwaterdemand': ['', 'domesticHotWaterBus', ''], 'gasboiler': ['shSourceBus,dhwStorageBus', 'naturalGasBus', ''], 'electricrod': ['shSourceBus,dhwStorageBus', 'electricityInBus', ''],
-                 'chp': ['electricityProdBus,shSourceBus,dhwStorageBus', 'naturalGasBus', ''], 'ashp': ['shSourceBus,dhwStorageBus', 'electricityInBus', ''], 'gshp': ['shSourceBus,dhwStorageBus', 'electricityInBus', ''],
-                 'electricalstorage': ['electricityBus', 'electricityProdBus', ''], 'shstorage': ['spaceHeatingBus', 'shSourceBus', ''], 'dhwstorage': ['domesticHotWaterBus', 'dhwStorageBus', '']}
-        sheetToSection = {'commodity_sources':'CommoditySources', 'solar':'Solar', 'demand':'Demands', 'transformers':'Transformers', 'storages':'Storages', 'stratified_storage':'StratifiedStorage'}
-        sections = config.sections()
-        profiles = pd.DataFrame(columns=['name', 'path'])
-        updatedLabels = {'weatherpath':'weather_data', 'path':'demand_profiles', 'ashp':'HP', 'gshp':'GWHP', 'electricityresource':'electricityResource', 'naturalgasresource':'naturalGasResource', 'chp':'CHP', 'gasboiler':'GasBoiler', 'electricrod':'ElectricRod', 'pv':'pv', 'solarcollector':'solarCollector', 'electricalstorage':'electricalStorage', 'shstorage':'shStorage', 'dhwstorage':'dhwStorage', 'stratifiedstorage':'StratifiedStorage'}
-        temp_h = {}     # to store temp_h values for stratified storage parameters sheet
-        FeedinTariff = 0
-        for section in config.sections():
-            configData[section]=config.items(section)
-        configData = {k.lower(): v for k, v in configData.items()}
-        for sheet in columnNames:
-            excelData[sheet] = pd.DataFrame(columns=columnNames[sheet])
-            if sheet == 'stratified_storage':
-                newRow = pd.DataFrame(columns=columnNames[sheet])
-                newRow.at[0, 'label'] = list(temp_h)[0]
-                newRow.at[0, 'temp_h'] = list(temp_h.values())[0]
-                newRow.at[1, 'label'] = list(temp_h)[1]
-                newRow.at[1, 'temp_h'] = list(temp_h.values())[1]
-            for item in configData[sheetToSection[sheet].lower()]:
-                type = item[0]
-                if item[1] in ['True', 'False']:  # defines whether or not a component is to be added
-                    if item[1] == 'True':
-                        newRow = pd.DataFrame(columns=columnNames[sheet])
-                        newRow.at[0,'label']=updatedLabels[item[0]]
-                        newRow.at[0,'active']=int(bool(item[1]=='True'))
-                        # sheet specific options
-                        cols = newRow.columns
-                        if 'building' in cols:
-                            newRow.at[0,'building']=1
-                        if 'to' in cols:
-                            newRow.at[0,'to'] = buses[type][0]
-                        if 'from' in cols:
-                            newRow.at[0,'from'] = buses[type][1]
-                        if 'connect' in cols:
-                            newRow.at[0,'connect'] = buses[type][2]
-                        params = configData[type]
-                        if sheet == 'commodity_sources':
-                            index = [x for x, y in enumerate(params) if y[0] == 'cost'][0]
-                            newRow.at[0,'variable costs'] = params[index][1]
-                            index = [x for x, y in enumerate(params) if y[0] == 'impact'][0]
-                            newRow.at[0,'CO2 impact'] = params[index][1]
-                            if type=='electricityresource':
-                                index = [x for x, y in enumerate(params) if y[0] == 'feedintariff'][0]
-                                FeedinTariff = -float(params[index][1])
-                        else:
-                            for p in params:
-                                if sheet=='transformers' and p[0] == 'capacity_max':
-                                    newRow.at[0, 'capacity_DHW'] = p[1]
-                                    newRow.at[0, 'capacity_SH'] = p[1]
-                                    if updatedLabels[item[0]]=='CHP':
-                                        newRow.at[0, 'capacity_el'] = str(round(float(p[1])*float(newRow.at[0, 'efficiency'].split(',')[0])/float(newRow.at[0, 'efficiency'].split(',')[1]),0))
-                                elif sheet=='storages' and p[0] == 'temp_h':
-                                    temp_h[newRow.at[0,'label']] = p[1]
-                                else:
-                                    newRow.at[0,p[0]] = p[1]
-                        excelData[sheet] = pd.concat([excelData[sheet], newRow])
-                elif type=='path':       # demand path
-                    buildingFolder = [i[1] for i in configData['demands'] if i[0] == 'folders'][0].split(',')[building]
-                    buildingPath = item[1]+'\\'+ buildingFolder
-                    profiles = pd.concat([profiles, pd.DataFrame({'name': [updatedLabels[type]], 'path': [buildingPath]})])
-                elif 'path' in type:     # weather path
-                    profiles = pd.concat([profiles, pd.DataFrame({'name':[updatedLabels[type]], 'path':[item[1]]})])
-                elif sheet == 'demand' and type!='folders':
-                    newRow = pd.DataFrame(columns=columnNames[sheet])
-                    for d in ['electricityDemand', 'spaceHeatingDemand', 'domesticHotWaterDemand']:
-                        newRow.at[0, 'label'] = d
-                        newRow.at[0, 'from'] = buses[d.lower()][1]
-                        if d == 'spaceHeatingDemand' and item[1]==0:
-                            newRow.at[0, 'fixed'] = item[1]
-                            newRow.at[0, 'building model'] = 'Yes'
-                        else:
-                            newRow.at[0, 'fixed'] = 1
-                        excelData[sheet] = pd.concat([excelData[sheet], newRow])
-                    excelData[sheet]['building'] = 1
-                    excelData[sheet]['active'] = 1
-                    excelData[sheet]['nominal value'] = 1
-                elif sheet == 'stratified_storage':
-                    newRow.at[0,type] = item[1]
-                    newRow.at[1,type] = item[1]
-                else: # common parameters of all the components of that section
-                    if type!='folders':
-                        excelData[sheet][type] = item[1]
-            if sheet == 'stratified_storage':
-                excelData[sheet] = pd.concat([excelData[sheet], newRow])
-        excelData['profiles'] = profiles
-        excelData['grid_connection'] = pd.DataFrame({'label':['gridElectricity','electricitySource','producedElectricity','shSource','spaceHeating'], 'building':[1,1,1,1,1], 'from':['gridBus','electricityProdBus','electricityBus','shSourceBus','spaceHeatingBus'], 'to':['electricityInBus','electricityBus','electricityInBus','spaceHeatingBus','shDemandBus'], 'efficiency':[1,1,1,1,1]})
-
-        df = pd.DataFrame(columns=['buses'])
-        for sheet, data in excelData.items():
-            for col in ['from', 'to', 'connect']:
-                if col in data.columns:
-                    newBuses = pd.DataFrame(columns=['buses'])
-                    newBuses['buses'] = data[col].values
-                    df = pd.concat([df, newBuses])
-        df = df.assign(buses=df.buses.str.split(',')).explode('buses')['buses'].unique()
-        df = df[df != '']
-        excelData['buses'] = pd.DataFrame(columns=['label', 'building', 'excess', 'excess costs', 'active'])
-        for index in range(len(df)):
-            excelData['buses'].at[index,'label'] = df[index]
-            if df[index] == 'electricityBus' and FeedinTariff!=0:
-                excelData['buses'].at[index,'excess'] = 1
-                excelData['buses'].at[index, 'excess costs'] = FeedinTariff
-        excelData['buses']['building'] = 1
-        excelData['buses']['active'] = 1
-        excelData['buses'].loc[excelData['buses']['excess']!=1,'excess'] = 0
-        for sheet, data in excelData.items():
-            if 'building' in data.columns:
-                buildingNo = [i for i in range(1, numberOfBuildings + 1)]* len(excelData[sheet].index)
-                excelData[sheet] = pd.DataFrame(np.repeat(data.values, numberOfBuildings, axis=0), columns=data.columns)
-                excelData[sheet]['building'] = buildingNo
-        with pd.ExcelWriter(excelFilePath, engine='xlwt') as writer:
-            for sheet, data in excelData.items():
-                data.to_excel(writer, sheet_name=sheet, index=False)
-            writer.save()
-            writer.close()
-
-
-class EnergyNetworkGroup(EnergyNetworkClass):
-    def createScenarioFile(self, configFilePath, excelFilePath, numberOfBuildings):
-        """function to create the input excel file from a config file
-        saves the generated excel file at the path given by excelFilePath"""
-        config = ConfigParser()
-        config.read(configFilePath)
-        configData = {}
-        excelData = {}
-        columnNames = {'commodity_sources': ['label', 'building', 'to', 'variable costs', 'CO2 impact', 'active'],
-                       # column names are defined for each sheet (key of dict) in the excel file
-                       'solar': ['label', 'building', 'from', 'to', 'connect', 'electrical_consumption',
-                                 'peripheral_losses', 'latitude', 'longitude', 'tilt', 'azimuth', 'eta_0', 'a_1', 'a_2',
-                                 'temp_collector_inlet', 'delta_temp_n', 'capacity_max', 'capacity_min', 'lifetime',
-                                 'maintenance', 'installation', 'planification', 'invest_base', 'invest_cap',
-                                 'heat_impact', 'elec_impact', 'impact_cap'],
-                       'demand': ['label', 'building', 'active', 'from', 'fixed', 'nominal value', 'building model'],
-                       'transformers': ['label', 'building', 'active', 'from', 'to', 'efficiency', 'capacity_DHW',
-                                        'capacity_SH', 'capacity_el', 'capacity_min', 'lifetime', 'maintenance',
-                                        'installation', 'planification', 'invest_base', 'invest_cap', 'heat_impact',
-                                        'elec_impact', 'impact_cap'],
-                       'storages': ['label', 'building', 'active', 'from', 'to', 'efficiency inflow',
-                                    'efficiency outflow', 'initial capacity', 'capacity min', 'capacity max',
-                                    'capacity loss', 'lifetime', 'maintenance', 'installation', 'planification',
-                                    'invest_base', 'invest_cap', 'heat_impact', 'elec_impact', 'impact_cap'],
-                       'stratified_storage': ['label', 'diameter', 'temp_h', 'temp_c', 'temp_env',
-                                              'inflow_conversion_factor', 'outflow_conversion_factor', 's_iso',
-                                              'lamb_iso', 'alpha_inside', 'alpha_outside'],
-                       'links': ['label', 'active', 'efficiency', 'invest_base', 'invest_cap', 'investment']
-                       }
-        buses = {'naturalgasresource': ['naturalGasBus', '', ''], 'electricityresource': ['gridBus', '', ''],
-                 'solarcollector': ['dhwStorageBus', 'electricityInBus', 'solarConnectBus'],
-                 # [to, from, connect] columns in the excel file
-                 'pv': ['electricityProdBus', '', ''], 'electricitydemand': ['', 'electricityInBus', ''],
-                 'spaceheatingdemand': ['', 'shDemandBus', ''],
-                 'domestichotwaterdemand': ['', 'dhwDemandBus', ''],
-                 'gasboiler': ['shSourceBus,dhwStorageBus', 'naturalGasBus', ''],
-                 'electricrod': ['shSourceBus,dhwStorageBus', 'electricityInBus', ''],
-                 'chp': ['electricityProdBus,shSourceBus,dhwStorageBus', 'naturalGasBus', ''],
-                 'ashp': ['shSourceBus,dhwStorageBus', 'electricityInBus', ''],
-                 'gshp': ['shSourceBus,dhwStorageBus', 'electricityInBus', ''],
-                 'electricalstorage': ['electricityBus', 'electricityProdBus', ''],
-                 'shstorage': ['spaceHeatingBus', 'shSourceBus', ''],
-                 'dhwstorage': ['domesticHotWaterBus', 'dhwStorageBus', '']}
-        sheetToSection = {'commodity_sources': 'CommoditySources', 'solar': 'Solar', 'demand': 'Demands',
-                          'transformers': 'Transformers', 'storages': 'Storages',
-                          'stratified_storage': 'StratifiedStorage', 'links':'Links'}
-        sections = config.sections()
-        profiles = pd.DataFrame(columns=['name', 'path'])
-        updatedLabels = {'weatherpath': 'weather_data', 'path': 'demand_profiles', 'ashp': 'HP', 'gshp': 'GWHP',
-                         'electricityresource': 'electricityResource', 'naturalgasresource': 'naturalGasResource',
-                         'chp': 'CHP', 'gasboiler': 'GasBoiler', 'electricrod': 'ElectricRod', 'pv': 'pv',
-                         'solarcollector': 'solarCollector', 'electricalstorage': 'electricalStorage',
-                         'shstorage': 'shStorage', 'dhwstorage': 'dhwStorage', 'stratifiedstorage': 'StratifiedStorage',
-                         'ellink': 'electricityLink', 'shlink': 'shLink', 'dhwlink': 'dhwLink'}
-        efficiencyLinks = {'ellink': 0.9999, 'shlink': 0.9, 'dhwlink': 0.9}
-        temp_h = {}  # to store temp_h values for stratified storage parameters sheet
-        FeedinTariff = 0
-        for section in config.sections():
-            configData[section] = config.items(section)
-        configData = {k.lower(): v for k, v in configData.items()}
-        for sheet in columnNames:
-            excelData[sheet] = pd.DataFrame(columns=columnNames[sheet])
-            if sheet == 'stratified_storage':
-                newRow = pd.DataFrame(columns=columnNames[sheet])
-                newRow.at[0, 'label'] = list(temp_h)[0]
-                newRow.at[0, 'temp_h'] = list(temp_h.values())[0]
-                newRow.at[1, 'label'] = list(temp_h)[1]
-                newRow.at[1, 'temp_h'] = list(temp_h.values())[1]
-            for item in configData[sheetToSection[sheet].lower()]:
-                type = item[0]
-                if item[1] in ['True', 'False']:  # defines whether or not a component is to be added
-                    if item[1] == 'True':
-                        newRow = pd.DataFrame(columns=columnNames[sheet])
-                        newRow.at[0, 'label'] = updatedLabels[item[0]]
-                        newRow.at[0, 'active'] = int(bool(item[1] == 'True'))
-                        # sheet specific options
-                        cols = newRow.columns
-                        if 'building' in cols:
-                            newRow.at[0, 'building'] = 1
-                        if 'to' in cols:
-                            newRow.at[0, 'to'] = buses[type][0]
-                        if 'from' in cols:
-                            newRow.at[0, 'from'] = buses[type][1]
-                        if 'connect' in cols:
-                            newRow.at[0, 'connect'] = buses[type][2]
-                        if type in ['shlink', 'dhwlink']:
-                            params = configData['thermallink']
-                        else:
-                            params = configData[type]
-                        if sheet == 'commodity_sources':
-                            index = [x for x, y in enumerate(params) if y[0] == 'cost'][0]
-                            newRow.at[0, 'variable costs'] = params[index][1]
-                            index = [x for x, y in enumerate(params) if y[0] == 'impact'][0]
-                            newRow.at[0, 'CO2 impact'] = params[index][1]
-                            if type == 'electricityresource':
-                                index = [x for x, y in enumerate(params) if y[0] == 'feedintariff'][0]
-                                FeedinTariff = -float(params[index][1])
-                        else:
-                            if sheet == 'links':
-                                if not [x for x, y in enumerate(params) if y[0] == 'efficiency']:
-                                    newRow.at[0, 'efficiency'] = efficiencyLinks[type]
-                                newRow.at[0, 'investment'] = 1
-                            for p in params:
-                                if sheet == 'transformers' and p[0] == 'capacity_max':
-                                    newRow.at[0, 'capacity_DHW'] = p[1]
-                                    newRow.at[0, 'capacity_SH'] = p[1]
-                                    if updatedLabels[item[0]]=='CHP':
-                                        newRow.at[0, 'capacity_el'] = str(round(float(p[1])*float(newRow.at[0, 'efficiency'].split(',')[0])/float(newRow.at[0, 'efficiency'].split(',')[1]),0))
-                                elif sheet == 'storages' and p[0] == 'temp_h':
-                                    temp_h[newRow.at[0, 'label']] = p[1]
-                                else:
-                                    newRow.at[0, p[0]] = p[1]
-                        excelData[sheet] = pd.concat([excelData[sheet], newRow])
-                elif 'path' in type:  # weather path or demand path
-                    profiles = pd.concat([profiles, pd.DataFrame({'name': [updatedLabels[type]], 'path': [item[1]]})])
-                elif sheet == 'demand':
-                    newRow = pd.DataFrame(columns=columnNames[sheet])
-                    for d in ['electricityDemand', 'spaceHeatingDemand', 'domesticHotWaterDemand']:
-                        newRow.at[0, 'label'] = d
-                        newRow.at[0, 'from'] = buses[d.lower()][1]
-                        if d == 'spaceHeatingDemand' and item[1] == 0:
-                            newRow.at[0, 'fixed'] = item[1]
-                            newRow.at[0, 'building model'] = 'Yes'
-                        else:
-                            newRow.at[0, 'fixed'] = 1
-                        excelData[sheet] = pd.concat([excelData[sheet], newRow])
-                    excelData[sheet]['building'] = 1
-                    excelData[sheet]['active'] = 1
-                    excelData[sheet]['nominal value'] = 1
-                elif sheet == 'stratified_storage':
-                    newRow.at[0, type] = item[1]
-                    newRow.at[1, type] = item[1]
-                else:  # common parameters of all the components of that section
-                    excelData[sheet][type] = item[1]
-            if sheet == 'stratified_storage':
-                excelData[sheet] = pd.concat([excelData[sheet], newRow])
-        excelData['profiles'] = profiles
-        excelData['grid_connection'] = pd.DataFrame(
-            {'label': ['gridElectricity', 'electricitySource', 'producedElectricity', 'domesticHotWater', 'shSource', 'spaceHeating'],
-             'building': [1, 1, 1, 1, 1, 1],
-             'from': ['gridBus', 'electricityProdBus', 'electricityBus', 'domesticHotWaterBus', 'shSourceBus', 'spaceHeatingBus'],
-             'to': ['electricityInBus', 'electricityBus', 'electricityInBus', 'dhwDemandBus', 'spaceHeatingBus', 'shDemandBus'],
-             'efficiency': [1, 1, 1, 1, 1, 1]})
-
-        df = pd.DataFrame(columns=['buses'])
-        for sheet, data in excelData.items():
-            for col in ['from', 'to', 'connect']:
-                if col in data.columns:
-                    newBuses = pd.DataFrame(columns=['buses'])
-                    newBuses['buses'] = data[col].values
-                    df = pd.concat([df, newBuses])
-        df = df.assign(buses=df.buses.str.split(',')).explode('buses')['buses'].unique()
-        df = df[df != '']
-        excelData['buses'] = pd.DataFrame(columns=['label', 'building', 'excess', 'excess costs', 'active'])
-        for index in range(len(df)):
-            excelData['buses'].at[index, 'label'] = df[index]
-            if df[index] == 'electricityBus' and FeedinTariff != 0:
-                excelData['buses'].at[index, 'excess'] = 1
-                excelData['buses'].at[index, 'excess costs'] = FeedinTariff
-        excelData['buses']['building'] = 1
-        excelData['buses']['active'] = 1
-        excelData['buses'].loc[excelData['buses']['excess'] != 1, 'excess'] = 0
-        for sheet, data in excelData.items():
-            if 'building' in data.columns:
-                buildingNo = [i for i in range(1, numberOfBuildings + 1)] * len(excelData[sheet].index)
-                excelData[sheet] = pd.DataFrame(np.repeat(data.values, numberOfBuildings, axis=0), columns=data.columns)
-                excelData[sheet]['building'] = buildingNo
-        with pd.ExcelWriter(excelFilePath, engine='xlwt') as writer:
-            for sheet, data in excelData.items():
-                data.to_excel(writer, sheet_name=sheet, index=False)
-            writer.save()
-            writer.close()
-
-    def setFromExcel(self, filePath, numberOfBuildings, clusterSize={}, opt="costs", mergeLinkBuses=False, dispatchMode=False, includeCarbonBenefits=False):
-        # does Excel file exist?
-        if not filePath or not os.path.isfile(filePath):
-            logging.error("Excel data file {} not found.".format(filePath))
-        logging.info("Defining the energy network from the excel file: {}".format(filePath))
-        self._dispatchMode = dispatchMode
-        data = pd.ExcelFile(filePath)
-
-        nodesData = self.createNodesData(data, filePath, numberOfBuildings)
-        # nodesData["buses"]["excess costs"] = nodesData["buses"]["excess costs group"]
-        # nodesData["electricity_cost"]["cost"] = nodesData["electricity_cost"]["cost group"]
-
-        demandProfiles = {}
-        if clusterSize:
-            for i in range(1, numberOfBuildings + 1):
-                demandProfiles[i] = pd.concat(
-                    [nodesData["demandProfiles"][i].loc[d] for d in clusterSize.keys()])
-            electricityImpact = pd.concat(
-                [nodesData["electricity_impact"].loc[d]*clusterSize[d] for d in clusterSize.keys()])
-            electricityCost = pd.concat(
-                [nodesData["electricity_cost"].loc[d]*clusterSize[d] for d in clusterSize.keys()])
-            if 'natGas_impact' in nodesData:
-                natGasImpact = pd.concat(
-                    [nodesData["natGas_impact"].loc[d]*clusterSize[d] for d in clusterSize.keys()])
-                natGasCost = pd.concat(
-                    [nodesData["natGas_cost"].loc[d]*clusterSize[d] for d in clusterSize.keys()])
-            weatherData = pd.concat([nodesData['weather_data'][
-                                         nodesData['weather_data']['time.mm'] == int(d.split('-')[1])][
-                                         nodesData['weather_data']['time.dd'] == int(d.split('-')[2])][['gls', 'str.diffus', 'tre200h0', 'ground_temp']] for d in clusterSize.keys()])
-
-            nodesData["demandProfiles"] = demandProfiles
-            nodesData["electricity_impact"] = electricityImpact
-            nodesData["electricity_cost"] = electricityCost
-            if 'natGas_impact' in nodesData:
-                nodesData["natGas_impact"] = natGasImpact
-                nodesData["natGas_cost"] = natGasCost
-            nodesData["weather_data"] = weatherData
-
-        nodesData["links"]= data.parse("links")
-        self._convertNodes(nodesData, opt, mergeLinkBuses, includeCarbonBenefits, clusterSize)
-        self._addLinks(nodesData["links"], numberOfBuildings, mergeLinkBuses)
-        logging.info("Nodes from Excel file {} successfully converted".format(filePath))
-        self.add(*self._nodesList)
-        logging.info("Nodes successfully added to the energy network")
-
-
-    def _addLinks(self, data, numberOfBuildings, mergeLinkBuses):  # connects buses A and B (denotes a bidirectional link)
-        if mergeLinkBuses:
-            return
-        for i, l in data.iterrows():
-            if l["active"]:
-                if l["investment"]:
-                    investment = solph.Investment(
-                        ep_costs=l["invest_cap"],
-                        nonconvex=True,
-                        maximum=500000,
-                        offset=l["invest_base"],
-                    )
-                else:
-                    investment = None
-                busesOut = []
-                busesIn = []
-                # add two buses for each building link_out and link_in
-                for b in range(numberOfBuildings):
-                    if "sh" in l["label"]:
-                        busesOut.append(self._busDict["spaceHeatingBus" + '__Building' + str(b+1)])
-                        busesIn.append(self._busDict["shDemandBus" + '__Building' + str(b+1)])
-                    elif "dhw" in l["label"]:
-                        busesOut.append(self._busDict["domesticHotWaterBus" + '__Building' + str(b+1)])
-                        busesIn.append(self._busDict["dhwDemandBus" + '__Building' + str(b+1)])
-                    else:
-                        busesOut.append(self._busDict["electricityBus" + '__Building' + str(b + 1)])
-                        busesIn.append(self._busDict["electricityInBus" + '__Building' + str(b + 1)])
-
-                self._nodesList.append(Link(
-                    label=l["label"],
-                    inputs={busA: solph.Flow() for busA in busesOut},
-                    outputs={busB: solph.Flow(investment=investment) for busB in busesIn},
-                    conversion_factors={busB: l["efficiency"] for busB in busesIn}
+import numpy as np
+import pandas as pd
+import oemof.solph as solph
+from oemof.tools import logger
+import logging
+import os
+import pprint as pp
+from configparser import ConfigParser
+from datetime import datetime, timedelta
+try:
+    import matplotlib.pyplot as plt
+except ImportError:
+    plt = None
+from optihood.constraints import *
+from optihood.buildings import Building
+from optihood.links import Link
+
+
+class EnergyNetworkClass(solph.EnergySystem):
+    def __init__(self, timestamp, clusters=None):
+        self._timeIndexReal = timestamp             # the timeindex passed to the energy network, will be made shorter if clustering is selected
+        self._clusterDate = {}
+        if clusters:
+            self._numberOfDays = len(clusters)
+            lastDay = datetime(timestamp.year[0], 1, 1) + timedelta(self._numberOfDays - 1)
+            lastDay = lastDay.strftime('%Y-%m-%d')
+            i = 1
+            for day in clusters:
+                d_clusterIndex = datetime(timestamp.year[0], 1, 1) + timedelta(i - 1)
+                self._clusterDate[day] = d_clusterIndex.strftime('%Y-%m-%d')
+                i += 1
+            timestamp = pd.date_range("2021-01-01 00:00:00", f"{lastDay} 23:00:00", freq=timestamp.freq)
+        self._nodesList = []
+        self._storageContentSH = {}
+        self.__inputs = {}                          # dictionary of list of inputs indexed by the building label
+        self.__technologies = {}                    # dictionary of list of technologies indexed by the building label
+        self.__capacitiesTransformersBuilding = {}  # dictionary of dictionary of optimized capacities of transformers indexed by the building label
+        self.__capacitiesStoragesBuilding = {}      # dictionary of dictionary of optimized capacities of storages indexed by the building label
+        self.__costParam = {}
+        self.__envParam = {}
+        self.__capex = {}
+        self.__opex = {}
+        self.__feedIn = {}
+        self.__envImpactInputs = {}                 # dictionary of dictionary of environmental impact of different inputs indexed by the building label
+        self.__envImpactTechnologies = {}           # dictionary of dictionary of environmental impact of different technologies indexed by the building label
+        self._busDict = {}
+        self.__elHP = {}
+        self.__shHP = {}
+        self.__dhwHP = {}
+        self.__annualCopHP = {}
+        self.__elGWHP = {}
+        self.__shGWHP = {}
+        self.__dhwGWHP = {}
+        self.__annualCopGWHP = {}
+        self.__elRodEff = np.nan
+        self._dispatchMode = False                         
+        if not os.path.exists(".\\log_files"):
+            os.mkdir(".\\log_files")
+        logger.define_logging(logpath=os.getcwd(), logfile=f'.\\log_files\\optihood_{datetime.now().strftime("%d.%m.%Y_%H.%M.%S")}.log')
+
+        logging.info("Initializing the energy network")
+        super(EnergyNetworkClass, self).__init__(timeindex=timestamp)
+
+    def setFromExcel(self, filePath, numberOfBuildings, clusterSize={}, opt="costs", mergeLinkBuses=False, dispatchMode=False, includeCarbonBenefits=False):
+        # does Excel file exist?
+        if not filePath or not os.path.isfile(filePath):
+            logging.error("Excel data file {} not found.".format(filePath))                                                                               
+        self._dispatchMode = dispatchMode
+        logging.info("Defining the energy network from the excel file: {}".format(filePath))
+        data = pd.ExcelFile(filePath)
+        nodesData = self.createNodesData(data, filePath, numberOfBuildings)
+        # nodesData["buses"]["excess costs"] = nodesData["buses"]["excess costs indiv"]
+        # nodesData["electricity_cost"]["cost"] = nodesData["electricity_cost"]["cost indiv"]
+
+        if clusterSize:
+            demandProfiles = {}
+            for i in range(1, numberOfBuildings + 1):
+                demandProfiles[i] = pd.concat(
+                    [nodesData["demandProfiles"][i].loc[d] for d in clusterSize.keys()])
+            electricityImpact = pd.concat(
+                [nodesData["electricity_impact"].loc[d] * clusterSize[d] for d in clusterSize.keys()])
+            electricityCost = pd.concat(
+                [nodesData["electricity_cost"].loc[d] * clusterSize[d] for d in clusterSize.keys()])
+            if 'natGas_impact' in nodesData:
+                natGasImpact = pd.concat(
+                    [nodesData["natGas_impact"].loc[d] * clusterSize[d] for d in clusterSize.keys()])
+                natGasCost = pd.concat(
+                    [nodesData["natGas_cost"].loc[d] * clusterSize[d] for d in clusterSize.keys()])
+            weatherData = pd.concat([nodesData['weather_data'][
+                                         nodesData['weather_data']['time.mm'] == int(d.split('-')[1])][
+                                         nodesData['weather_data']['time.dd'] == int(d.split('-')[2])][
+                                         ['gls', 'str.diffus', 'tre200h0', 'ground_temp']] for d in clusterSize.keys()])
+
+            nodesData["demandProfiles"] = demandProfiles
+            nodesData["electricity_impact"] = electricityImpact
+            nodesData["electricity_cost"] = electricityCost
+            if 'natGas_impact' in nodesData:
+                nodesData["natGas_impact"] = natGasImpact
+                nodesData["natGas_cost"] = natGasCost
+            nodesData["weather_data"] = weatherData
+
+        self._convertNodes(nodesData, opt, mergeLinkBuses, includeCarbonBenefits, clusterSize)
+        logging.info("Nodes from Excel file {} successfully converted".format(filePath))
+        self.add(*self._nodesList)
+        logging.info("Nodes successfully added to the energy network")
+
+    def createNodesData(self, data, filePath, numBuildings):
+        self.__noOfBuildings = numBuildings
+        nodesData = {
+            "buses": data.parse("buses"),
+            "grid_connection": data.parse("grid_connection"),
+            "commodity_sources": data.parse("commodity_sources"),
+            "solar": data.parse("solar"),
+            "transformers": data.parse("transformers"),
+            "demand": data.parse("demand"),
+            "storages": data.parse("storages"),
+            "stratified_storage": data.parse("stratified_storage"),
+            "profiles": data.parse("profiles")
+        }
+        # update stratified_storage index
+        nodesData["stratified_storage"].set_index("label", inplace=True)
+
+        # extract input data from CSVs
+        electricityImpact = nodesData["commodity_sources"].loc[nodesData["commodity_sources"]["label"] == "electricityResource", "CO2 impact"].iloc[0]
+        electricityCost = nodesData["commodity_sources"].loc[nodesData["commodity_sources"]["label"] == "electricityResource", "variable costs"].iloc[0]
+        demandProfilesPath = nodesData["profiles"].loc[nodesData["profiles"]["name"] == "demand_profiles", "path"].iloc[0]
+        weatherDataPath = nodesData["profiles"].loc[nodesData["profiles"]["name"] == "weather_data", "path"].iloc[0]
+        if "naturalGasResource" in nodesData["commodity_sources"]["label"].values:
+            natGasCost = nodesData["commodity_sources"].loc[nodesData["commodity_sources"]["label"] == "naturalGasResource", "variable costs"].iloc[0]
+            natGasImpact = nodesData["commodity_sources"].loc[
+                nodesData["commodity_sources"]["label"] == "naturalGasResource", "CO2 impact"].iloc[0]
+
+        demandProfiles = {}  # dictionary of dataframes for each building's demand profiles
+
+        if (not os.listdir(demandProfilesPath)) or (not os.path.exists(demandProfilesPath)):
+            logging.error("Error in the demand profiles path: The folder is either empty or does not exist")
+        else:
+            i = 0
+            for filename in os.listdir(demandProfilesPath): #this path should contain csv file(s) (one for each building's profiles)
+                i += 1      # Building number
+                if i > numBuildings:
+                    logging.warning("Demand profiles folder has more files than the number of buildings specified")
+                    break
+                demandProfiles.update({i: pd.read_csv(os.path.join(demandProfilesPath, filename), delimiter=";")})
+
+            nodesData["demandProfiles"] = demandProfiles
+            # set datetime index
+            for i in range(numBuildings):
+                nodesData["demandProfiles"][i + 1].set_index("timestamp", inplace=True)
+                nodesData["demandProfiles"][i + 1].index = pd.to_datetime(nodesData["demandProfiles"][i + 1].index)
+
+        if type(electricityImpact) == np.float64:
+            # for constant impact
+            electricityImpactValue = electricityImpact
+            logging.info("Constant value for electricity impact")
+            nodesData["electricity_impact"] = pd.DataFrame()
+            nodesData["electricity_impact"]["impact"] = (nodesData["demandProfiles"][1].shape[0]) * [
+                electricityImpactValue]
+            nodesData["electricity_impact"].index = nodesData["demandProfiles"][1].index
+        elif not os.path.exists(electricityImpact):
+            logging.error("Error in electricity impact file path")
+        else:
+            nodesData["electricity_impact"] = pd.read_csv(electricityImpact, delimiter=";")
+            # set datetime index
+            nodesData["electricity_impact"].set_index("timestamp", inplace=True)
+            nodesData["electricity_impact"].index = pd.to_datetime(nodesData["electricity_impact"].index)
+
+        if type(electricityCost) == np.float64:
+            # for constant cost
+            electricityCostValue = electricityCost
+            logging.info("Constant value for electricity cost")
+            nodesData["electricity_cost"] = pd.DataFrame()
+            nodesData["electricity_cost"]["cost"] = (nodesData["demandProfiles"][1].shape[0]) * [
+                electricityCostValue]
+            nodesData["electricity_cost"].index = nodesData["demandProfiles"][1].index
+        elif not os.path.exists(electricityCost):
+            logging.error("Error in electricity cost file path")
+        else:
+            nodesData["electricity_cost"] = pd.read_csv(electricityCost, delimiter=";")
+            # set datetime index
+            nodesData["electricity_cost"].set_index("timestamp", inplace=True)
+            nodesData["electricity_cost"].index = pd.to_datetime(nodesData["electricity_cost"].index)
+
+        if "naturalGasResource" in nodesData["commodity_sources"]["label"].values:
+            if type(natGasImpact) == float or (natGasImpact.split('.')[0].replace('-','').isdigit() and natGasImpact.split('.')[1].replace('-','').isdigit()):
+                # for constant impact
+                natGasImpactValue = float(natGasImpact)
+                logging.info("Constant value for natural gas impact")
+                nodesData["natGas_impact"] = pd.DataFrame()
+                nodesData["natGas_impact"]["impact"] = (nodesData["demandProfiles"][1].shape[0]) * [
+                    natGasImpactValue]
+                nodesData["natGas_impact"].index = nodesData["demandProfiles"][1].index
+            elif not os.path.exists(natGasImpact):
+                logging.error("Error in natural gas impact file path")
+            else:
+                nodesData["natGas_impact"] = pd.read_csv(natGasImpact, delimiter=";")
+                # set datetime index
+                nodesData["natGas_impact"].set_index("timestamp", inplace=True)
+                nodesData["natGas_impact"].index = pd.to_datetime(nodesData["natGas_impact"].index)
+
+            if type(natGasCost) == np.float64:
+                # for constant cost
+                natGasCostValue = natGasCost
+                logging.info("Constant value for natural gas cost")
+                nodesData["natGas_cost"] = pd.DataFrame()
+                nodesData["natGas_cost"]["cost"] = (nodesData["demandProfiles"][1].shape[0]) * [natGasCostValue]
+                nodesData["natGas_cost"].index = nodesData["demandProfiles"][1].index
+            elif not os.path.exists(natGasCost):
+                logging.error("Error in natural gas cost file path")
+            else:
+                nodesData["natGas_cost"] = pd.read_csv(natGasCost, delimiter=";")
+                # set datetime index
+                nodesData["natGas_cost"].set_index("timestamp", inplace=True)
+                nodesData["natGas_cost"].index = pd.to_datetime(nodesData["natGas_cost"].index)
+
+        if not os.path.exists(weatherDataPath):
+            logging.error("Error in weather data file path")
+        else:
+            nodesData["weather_data"] = pd.read_csv(weatherDataPath, delimiter=";")
+            #add a timestamp column to the dataframe
+            for index, row in nodesData['weather_data'].iterrows():
+                time = f"{int(row['time.yy'])}.{int(row['time.mm']):02}.{int(row['time.dd']):02} {int(row['time.hh']):02}:00:00"
+                nodesData['weather_data'].at[index, 'timestamp'] = datetime.strptime(time, "%Y.%m.%d  %H:%M:%S")
+                #set datetime index
+            nodesData["weather_data"].set_index("timestamp", inplace=True)
+            nodesData["weather_data"].index = pd.to_datetime(nodesData["weather_data"].index)
+
+        nodesData["building_model"] = pd.DataFrame()
+        nodesData["building_model"]["tAmb"] = np.array(nodesData["weather_data"]["tre200h0"])
+        nodesData["building_model"]["IrrH"] = np.array(nodesData["weather_data"]["gls"])/1000       # conversion from W/m2 to kW/m2
+        if (nodesData['demand']['building model'].notna().any()) and (nodesData['demand']['building model'] == 'Yes').any():
+            nodesData["building_model"]["Qocc"] = np.array(pd.read_csv(r"..\excels\Internal_gains.csv", delimiter=';', header=0)["Total (kW)"])
+        else:
+            logging.info("Building model either not selected or invalid string value entered")
+        logging.info("Data from Excel file {} imported.".format(filePath))
+        return nodesData
+
+    def _convertNodes(self, data, opt, mergeLinkBuses, includeCarbonBenefits, clusterSize):
+        if not data:
+            logging.error("Nodes data is missing.")
+        self.__temperatureAmb = np.array(data["weather_data"]["tre200h0"])
+        self.__temperatureGround = np.array(data["weather_data"]["ground_temp"])
+        self.__temperatureSH = data["stratified_storage"].loc["shStorage", "temp_h"]
+        self.__temperatureDHW = data["stratified_storage"].loc["dhwStorage", "temp_h"]
+        # Transformers conversion factors input power - output power
+        if any(data["transformers"]["label"] == "CHP"):
+            self.__chpEff = float(data["transformers"][data["transformers"]["label"] == "CHP"]["efficiency"].iloc[0].split(",")[1])
+        if any(data["transformers"]["label"] == "HP"):
+            self.__hpEff = float(data["transformers"][data["transformers"]["label"] == "HP"]["efficiency"].iloc[0])
+        if any(data["transformers"]["label"] == "GWHP"):
+            self.__gwhpEff = float(data["transformers"][data["transformers"]["label"] == "GWHP"]["efficiency"].iloc[0])
+        if any(data["transformers"]["label"] == "GasBoiler"):
+            self.__gbEff = float(data["transformers"][data["transformers"]["label"] == "GasBoiler"]["efficiency"].iloc[0].split(",")[0])
+        if any(data["transformers"][data["transformers"]["label"]=="ElectricRod"]["active"] == 1):
+            self.__elRodEff = float(data["transformers"][data["transformers"]["label"] == "ElectricRod"]["efficiency"].iloc[0])
+        # Storage conversion L - kWh to display the L value
+        self.__Lsh = 4.186 * (self.__temperatureSH - data["stratified_storage"].loc["shStorage", "temp_c"]) / 3600
+        self.__Ldhw = 4.186 * (self.__temperatureDHW - data["stratified_storage"].loc["dhwStorage", "temp_c"]) / 3600
+        self._addBuildings(data, opt, mergeLinkBuses, includeCarbonBenefits, clusterSize)
+
+    def _addBuildings(self, data, opt, mergeLinkBuses, includeCarbonBenefits, clusterSize):
+        numberOfBuildings = max(data["buses"]["building"])
+        self.__buildings = [Building('Building' + str(i + 1)) for i in range(numberOfBuildings)]
+        for b in self.__buildings:
+            buildingLabel = b.getBuildingLabel()
+            i = int(buildingLabel[8:])
+            if i == 1:
+                busDictBuilding1 = b.addBus(data["buses"][data["buses"]["building"] == i], opt, mergeLinkBuses, data["electricity_impact"], clusterSize, includeCarbonBenefits)
+            else:
+                b.addBus(data["buses"][data["buses"]["building"] == i], opt, mergeLinkBuses, data["electricity_impact"], clusterSize, includeCarbonBenefits)
+            if mergeLinkBuses and i!=1:
+                b.addToBusDict(busDictBuilding1)
+            b.addGridSeparation(data["grid_connection"][data["grid_connection"]["building"] == i], mergeLinkBuses)
+            if "natGas_cost" in data:
+                natGasCost = data["natGas_cost"]
+                natGasImpact = data["natGas_impact"]
+            else:
+                natGasCost = natGasImpact = None
+            b.addSource(data["commodity_sources"][data["commodity_sources"]["building"] == i], data["electricity_impact"], data["electricity_cost"], natGasCost, natGasImpact, opt)
+            b.addSink(data["demand"][data["demand"]["building"] == i], data["demandProfiles"][i], data["building_model"], mergeLinkBuses)
+            b.addTransformer(data["transformers"][data["transformers"]["building"] == i], self.__temperatureDHW,
+                             self.__temperatureSH, self.__temperatureAmb, self.__temperatureGround, opt, mergeLinkBuses, self._dispatchMode)
+            #if any(data["transformers"]["label"] == "HP") or any(data["transformers"]["label"] == "GWHP"):   #add electricity rod if HP or GSHP is present in the available technology pool
+            #    b.addElectricRodBackup(opt)
+            b.addStorage(data["storages"][data["storages"]["building"] == i], data["stratified_storage"], opt, mergeLinkBuses, self._dispatchMode)
+            b.addSolar(data["solar"][(data["solar"]["building"] == i) & (data["solar"]["label"] == "solarCollector")], data["weather_data"], opt, mergeLinkBuses, self._dispatchMode)
+            b.addPV(data["solar"][(data["solar"]["building"] == i) & (data["solar"]["label"] == "pv")], data["weather_data"], opt, self._dispatchMode)
+            b.addPVT(data["solar"][(data["solar"]["building"] == i) & (data["solar"]["label"] == "pvt")], data["weather_data"], opt, mergeLinkBuses, self._dispatchMode)
+            self._nodesList.extend(b.getNodesList())
+            self.__inputs[buildingLabel] = b.getInputs()
+            self.__technologies[buildingLabel] = b.getTechnologies()
+            self.__costParam.update(b.getCostParam())
+            self.__envParam.update(b.getEnvParam())
+            self._busDict.update(b.getBusDict())
+            self.__capacitiesTransformersBuilding[buildingLabel] = {}
+            self.__capacitiesStoragesBuilding[buildingLabel] = {}
+            self.__envImpactInputs[buildingLabel] = {}
+            self.__opex[buildingLabel] = {}
+            self.__envImpactTechnologies[buildingLabel] = {}
+
+    def printNodes(self):
+        print("*********************************************************")
+        print("The following objects have been created from excel sheet:")
+        for n in self.nodes:
+            oobj = str(type(n)).replace("<class 'oemof.solph.", "").replace("'>", "")
+            print(oobj + ":", n.label)
+        print("*********************************************************")
+
+    def optimize(self, numberOfBuildings, solver, envImpactlimit=1000000, clusterSize={},
+                 options=None,   # solver options
+                 optConstraints=None, #optional constraints (implemented for the moment are "roof area"
+                 mergeLinkBuses=False):
+
+        if options is None:
+            options = {"gurobi": {"MIPGap": 0.01}}
+
+        optimizationModel = solph.Model(self)
+        logging.info("Optimization model built successfully")
+
+        # add constraint to limit the environmental impacts
+        optimizationModel, flows, transformerFlowCapacityDict, storageCapacityDict = environmentalImpactlimit(
+            optimizationModel, keyword1="env_per_flow", keyword2="env_per_capa", limit=envImpactlimit)
+
+        # optional constraints (available: 'roof area')
+        if optConstraints:
+            for c in optConstraints:
+                if c.lower() == "roof area":
+                    # requires 2 additional parameters in the scenario file, tab "solar", zenit angle, roof area
+                    try:
+                        optimizationModel = roof_area_limit(optimizationModel,
+                                                        keyword1="space", keyword2="roof_area", nb=numberOfBuildings)
+                        logging.info(f"Optional constraint {c} successfully added to the optimization model")
+                    except ValueError:
+                        logging.error(f"Optional constraint {c} not added to the optimization model : "
+                                      f"please check if PV efficiency, roof area and zenith angle are present in input "
+                                      f"file")
+                        pass
+                if c.lower() == 'totalpvcapacity':
+                    optimizationModel = totalPVCapacityConstraint(optimizationModel, numberOfBuildings)
+                    logging.info(f"Optional constraint {c} successfully added to the optimization model")
+        # constraint on elRod combined with HPs:
+        if not np.isnan(self.__elRodEff):
+            optimizationModel = electricRodCapacityConstaint(optimizationModel, numberOfBuildings)
+        # constraint on PVT capacity if PVT technology is selected
+        if any("pvt" in n.label for n in self.nodes):
+            optimizationModel = PVTElectricalThermalCapacityConstraint(optimizationModel, numberOfBuildings)
+        # constraint on storage content for clustering
+        """if clusterSize:
+            optimizationModel = dailySHStorageConstraint(optimizationModel)"""
+
+        logging.info("Custom constraints successfully added to the optimization model")
+
+        if solver == "gurobi":
+            logging.info("Initiating optimization using {} solver".format(solver))
+
+        optimizationModel.solve(solver=solver, cmdline_options=options[solver])
+
+        # obtain the value of the environmental impact (subject to the limit constraint)
+        # the optimization imposes an integral limit constraint on the environmental impacts
+        # total environmental impacts <= envImpactlimit
+        envImpact = optimizationModel.totalEnvironmentalImpact()
+
+        self._optimizationResults = solph.processing.results(optimizationModel)
+        self._metaResults = solph.processing.meta_results(optimizationModel)
+        logging.info("Optimization successful and results collected")
+
+        # calculate capacities invested for transformers and storages (for the entire energy network and per building)
+        capacitiesTransformersNetwork, capacitiesStoragesNetwork = self._calculateInvestedCapacities(optimizationModel, transformerFlowCapacityDict, storageCapacityDict)
+
+        if clusterSize:
+            self._postprocessingClusters(clusterSize)
+
+        # calculate results (CAPEX, OPEX, FeedIn Costs, environmental impacts etc...) for each building
+        self._calculateResultsPerBuilding(mergeLinkBuses)
+
+        return envImpact, capacitiesTransformersNetwork, capacitiesStoragesNetwork
+
+    def saveUnprocessedResults(self, resultFile):
+        with pd.ExcelWriter(resultFile) as writer:
+            busLabelList = []
+            for i in self.nodes:
+                if str(type(i)).replace("<class 'oemof.solph.", "").replace("'>", "") == "network.bus.Bus":
+                    busLabelList.append(i.label)
+            for i in busLabelList:
+                result = pd.DataFrame.from_dict(solph.views.node(self._optimizationResults, i)["sequences"])
+                result.to_excel(writer, sheet_name=i)
+            writer.save()
+
+    def _updateCapacityDictInputInvestment(self, transformerFlowCapacityDict):
+        components = ["CHP", "GWHP", "HP", "GasBoiler", "ElectricRod"]
+        for inflow, outflow in list(transformerFlowCapacityDict):
+            index = (inflow, outflow)
+            if "__" in str(inflow):
+                buildingLabel = str(inflow).split("__")[1]
+            elif "__" in str(outflow):
+                buildingLabel = str(outflow).split("__")[1]
+            if any(c in str(outflow) for c in components):
+                newoutFlow = f"shSourceBus__{buildingLabel}"
+                newIndex = (outflow,newoutFlow)
+                transformerFlowCapacityDict[newIndex] = transformerFlowCapacityDict.pop(index)
+            if 'elSource_pvt' in str(inflow):   # remove PVT electrical capacity
+                transformerFlowCapacityDict.pop(index)
+        return transformerFlowCapacityDict
+
+    def _calculateInvestedCapacities(self, optimizationModel, transformerFlowCapacityDict, storageCapacityDict):
+        capacitiesInvestedTransformers = {}
+        capacitiesInvestedStorages = {}
+        storageList = []
+
+        # Transformers capacities
+
+        for inflow, outflow in transformerFlowCapacityDict:
+            index = (str(inflow), str(outflow))
+            capacitiesInvestedTransformers[index] = optimizationModel.InvestmentFlow.invest[inflow, outflow].value
+
+        # Conversion into output capacity
+        capacitiesInvestedTransformers = self._compensateInputCapacities(capacitiesInvestedTransformers)
+
+        # update transformerFlowCapacityDict such that investment objects with input flows are accounted properly in the results calculation
+        transformerFlowCapacityDict = self._updateCapacityDictInputInvestment(transformerFlowCapacityDict)
+
+        # Update capacities
+        for inflow, outflow in transformerFlowCapacityDict:
+            index = (str(inflow), str(outflow))
+            buildingLabel = str(inflow).split("__")[1]
+            self.__capacitiesTransformersBuilding[buildingLabel].update({index: capacitiesInvestedTransformers[index]})
+
+        # Storages capacities
+        for x in storageCapacityDict:
+            index = str(x)
+            if x in storageList:  # useful when we want to implement two or more storage units of the same type
+                capacitiesInvestedStorages[index] = capacitiesInvestedStorages[index] + \
+                                                    optimizationModel.GenericInvestmentStorageBlock.invest[x].value
+            else:
+                capacitiesInvestedStorages[str(x)] = optimizationModel.GenericInvestmentStorageBlock.invest[x].value
+
+        # Convert kWh into L
+        capacitiesInvestedStorages = self._compensateStorageCapacities(capacitiesInvestedStorages)
+
+        # Update capacities
+        for x in storageCapacityDict:
+            index = str(x)
+            buildingLabel = index.split("__")[1]
+            if x in storageList:  # useful when we want to implement two or more storage units of the same type
+                self.__capacitiesStoragesBuilding[buildingLabel].update(
+                    {index: capacitiesInvestedStorages[index]})
+            else:
+                self.__capacitiesStoragesBuilding[buildingLabel].update({index: capacitiesInvestedStorages[index]})
+            storageList.append(x)
+
+        return capacitiesInvestedTransformers, capacitiesInvestedStorages
+
+    def _compensateInputCapacities(self, capacitiesTransformers):
+        # Input capacity -> output capacity
+        for first, second in list(capacitiesTransformers):
+            if "CHP" in second:
+                for index, value in enumerate(self.nodes):
+                    if second == value.label:
+                        test = self.nodes[index].conversion_factors
+                        for t in test.keys():
+                            if "shSource" in t.label:
+                                capacitiesTransformers[(second,t.label)]= capacitiesTransformers[(first,second)]*self.__chpEff
+                                del capacitiesTransformers[(first,second)]
+            elif "GWHP" in second and not any([c.isdigit() for c in second.split("__")[0]]):  # second condition added for splitted GSHPs
+                for index, value in enumerate(self.nodes):
+                    if second == value.label:
+                        test = self.nodes[index].conversion_factors
+                        for t in test.keys():
+                            if "shSource" in t.label:
+                                capacitiesTransformers[(second, t.label)] = capacitiesTransformers[(first, second)] * self.__gwhpEff
+                                del capacitiesTransformers[(first, second)]
+            elif "HP" in second and "GWHP" not in second:
+                for index, value in enumerate(self.nodes):
+                    if second == value.label:
+                        test = self.nodes[index].conversion_factors
+                        for t in test.keys():
+                            if "shSource" in t.label:
+                                capacitiesTransformers[(second, t.label)] = capacitiesTransformers[(first, second)]*self.__hpEff
+                                del capacitiesTransformers[(first, second)]
+            elif "GasBoiler" in second:
+                for index, value in enumerate(self.nodes):
+                    if second == value.label:
+                        test = self.nodes[index].conversion_factors
+                        for t in test.keys():
+                            if "shSource" in t.label:
+                                capacitiesTransformers[(second, t.label)] = capacitiesTransformers[(
+                                first, second)] * self.__gbEff
+                                del capacitiesTransformers[(first, second)]
+            elif "ElectricRod" in second:
+                for index, value in enumerate(self.nodes):
+                    if second == value.label:
+                        test = self.nodes[index].conversion_factors
+                        for t in test.keys():
+                            if "shSource" in t.label:
+                                capacitiesTransformers[(second, t.label)] = capacitiesTransformers[(
+                                first, second)] * self.__elRodEff
+                                del capacitiesTransformers[(first, second)]
+
+        return capacitiesTransformers
+
+    def _compensateStorageCapacities(self, capacitiesStorages):
+        # kWh -> L
+        for storage in capacitiesStorages.keys():
+            if "sh" in storage:
+                capacitiesStorages[storage] = capacitiesStorages[storage] / self.__Lsh
+            elif "dhw" in storage:
+                capacitiesStorages[storage] = capacitiesStorages[storage] / self.__Ldhw
+        return capacitiesStorages
+
+    def _postprocessingClusters(self, clusterSize):
+        flows = [x for x in self._optimizationResults.keys() if x[1] is not None]
+        for flow in flows:
+            extrapolated_results = None
+            for day in clusterSize:
+                temp = pd.concat([self._optimizationResults[flow]['sequences'][self._clusterDate[day]]] * clusterSize[day])
+                if extrapolated_results is not None:
+                    extrapolated_results = pd.concat([extrapolated_results, temp])
+                else:
+                    extrapolated_results = temp
+            extrapolated_results.index = self._timeIndexReal
+            extrapolated_results.columns = ['flow']
+            self._optimizationResults[flow]['sequences'] = extrapolated_results
+
+    def _calculateResultsPerBuilding(self, mergeLinkBuses):
+        for b in self.__buildings:
+            buildingLabel = b.getBuildingLabel()
+            capacityTransformers = self.__capacitiesTransformersBuilding[buildingLabel]
+            capacityStorages = self.__capacitiesStoragesBuilding[buildingLabel]
+            technologies = self.__technologies[buildingLabel]
+            inputs = self.__inputs[buildingLabel]
+
+            # CAPital investment EXpenditure
+            self.__capex[buildingLabel] = sum((self.__costParam[i][1] * (capacityTransformers[(i, o)] > 1))             # base investment cost if the technology is implemented
+                                              + (capacityTransformers[(i, o)] * self.__costParam[i][0])                 # investment cost per unit capacity
+                                              for i, o in capacityTransformers) + \
+                                          sum((self.__costParam[x][1] * (capacityStorages[x] > 1))                      # base investment cost if the technology is implemented
+                                              + (capacityStorages[x] * self.__costParam[x][0])                          # investment cost per unit capacity
+                                              for x in capacityStorages)
+
+            electricitySourceLabel = "electricityResource" + '__' + buildingLabel
+            gridBusLabel = "gridBus" + '__' + buildingLabel
+            if mergeLinkBuses:
+                electricityBusLabel = "electricityBus"
+                excessElectricityBusLabel = "excesselectricityBus"
+            else:
+                electricityBusLabel = "electricityBus" + '__' + buildingLabel
+                excessElectricityBusLabel = "excesselectricityBus" + '__' + buildingLabel
+
+            if electricitySourceLabel in self.__costParam:
+                costParamGridElectricity = self.__costParam[electricitySourceLabel].copy()
+                costParamGridElectricity.reset_index(inplace=True, drop=True)
+            else:
+                costParamGridElectricity = 0
+            if "sequences" in solph.views.node(self._optimizationResults, gridBusLabel):
+                if ((electricitySourceLabel, gridBusLabel), "flow") in solph.views.node(self._optimizationResults, gridBusLabel)["sequences"]:
+                    gridElectricityFlow = solph.views.node(self._optimizationResults, gridBusLabel)["sequences"][
+                        (electricitySourceLabel, gridBusLabel), "flow"]
+                    gridElectricityFlow.reset_index(inplace=True, drop=True)
+                else:
+                    gridElectricityFlow = 0
+            else:
+                gridElectricityFlow = 0
+
+            # OPeration EXpenditure
+            self.__opex[buildingLabel].update({i[0]: sum(
+                solph.views.node(self._optimizationResults, i[1])["sequences"][(i[0], i[1]), "flow"] * self.__costParam[
+                    i[0]]) for i in inputs})
+            c = costParamGridElectricity * gridElectricityFlow
+            if isinstance(c, (int, float)):
+                self.__opex[buildingLabel].update({electricitySourceLabel:c})
+            else:
+                self.__opex[buildingLabel].update({electricitySourceLabel: c.sum()})  # cost of grid electricity is added separately based on cost data
+
+            # Feed-in electricity cost (value will be in negative to signify monetary gain...)
+            if ((mergeLinkBuses and buildingLabel=='Building1') or not mergeLinkBuses) and \
+                    (((electricityBusLabel, excessElectricityBusLabel), "flow") in solph.views.node(self._optimizationResults, electricityBusLabel)["sequences"]):
+                self.__feedIn[buildingLabel] = sum(solph.views.node(self._optimizationResults, electricityBusLabel)
+                                                   ["sequences"][(electricityBusLabel, excessElectricityBusLabel), "flow"]) * self.__costParam[excessElectricityBusLabel]
+            else: # in case of merged links feed in for all buildings except Building1 is set to 0 (to avoid repetition)
+                self.__feedIn[buildingLabel] = 0
+            if mergeLinkBuses:
+                elInBusLabel = 'electricityInBus'
+            else:
+                elInBusLabel = 'electricityInBus__'+buildingLabel
+            # HP flows
+            if ("HP__" + buildingLabel, "shSourceBus__" + buildingLabel) in capacityTransformers:
+                self.__elHP[buildingLabel] = sum(
+                    solph.views.node(self._optimizationResults, elInBusLabel)["sequences"][
+                        (elInBusLabel, 'HP__'+buildingLabel), 'flow'])
+                self.__shHP[buildingLabel] = sum(
+                    solph.views.node(self._optimizationResults, 'HP__' + buildingLabel)["sequences"][
+                        ('HP__' + buildingLabel, 'shSourceBus__' + buildingLabel), 'flow'])
+                self.__dhwHP[buildingLabel] = sum(
+                    solph.views.node(self._optimizationResults, 'HP__' + buildingLabel)["sequences"][
+                        ('HP__' + buildingLabel, 'dhwStorageBus__' + buildingLabel), 'flow'])
+                self.__annualCopHP[buildingLabel] = (self.__shHP[buildingLabel] + self.__dhwHP[buildingLabel]) / (
+                    self.__elHP[buildingLabel] + 1e-6)
+
+            # GWHP flows
+            if ("GWHP__" + buildingLabel, "shSourceBus__" + buildingLabel) in capacityTransformers:
+                self.__elGWHP[buildingLabel] = sum(
+                    solph.views.node(self._optimizationResults, elInBusLabel)["sequences"][
+                        (elInBusLabel, 'GWHP__' + buildingLabel), 'flow'])
+                self.__shGWHP[buildingLabel] = sum(
+                    solph.views.node(self._optimizationResults, 'GWHP__' + buildingLabel)["sequences"][
+                        ('GWHP__' + buildingLabel, 'shSourceBus__' + buildingLabel), 'flow'])
+                self.__dhwGWHP[buildingLabel] = sum(
+                    solph.views.node(self._optimizationResults, 'GWHP__' + buildingLabel)["sequences"][
+                        ('GWHP__' + buildingLabel, 'dhwStorageBus__' + buildingLabel), 'flow'])
+                self.__annualCopGWHP[buildingLabel] = (self.__shGWHP[buildingLabel] + self.__dhwGWHP[buildingLabel]) / (
+                        self.__elGWHP[buildingLabel] + 1e-6)
+            else:       # splitted GSHP
+                self.__annualCopGWHP[buildingLabel] = []
+                if (f"GWHP{str(self.__temperatureSH)}__" + buildingLabel, "shSourceBus__" + buildingLabel) in capacityTransformers:
+                    self.__elGWHP[buildingLabel] = sum(
+                        solph.views.node(self._optimizationResults, elInBusLabel)["sequences"][
+                            (elInBusLabel, f"GWHP{str(self.__temperatureSH)}__" + buildingLabel), 'flow'])
+                    self.__shGWHP[buildingLabel] = sum(
+                        solph.views.node(self._optimizationResults, f"GWHP{str(self.__temperatureSH)}__" + buildingLabel)["sequences"][
+                            (f"GWHP{str(self.__temperatureSH)}__" + buildingLabel, 'shSourceBus__' + buildingLabel), 'flow'])
+                    self.__annualCopGWHP[buildingLabel].append((self.__shGWHP[buildingLabel]) / (self.__elGWHP[buildingLabel] + 1e-6))
+                if (f"GWHP{str(self.__temperatureDHW)}__" + buildingLabel, "dhwStorageBus__" + buildingLabel) in capacityTransformers:
+                    self.__elGWHP[buildingLabel] = sum(
+                        solph.views.node(self._optimizationResults, elInBusLabel)["sequences"][
+                            (elInBusLabel, f"GWHP{str(self.__temperatureDHW)}__" + buildingLabel), 'flow'])
+                    self.__dhwGWHP[buildingLabel] = sum(
+                        solph.views.node(self._optimizationResults, f"GWHP{str(self.__temperatureDHW)}__" + buildingLabel)["sequences"][
+                            (f"GWHP{str(self.__temperatureDHW)}__" + buildingLabel, 'dhwStorageBus__' + buildingLabel), 'flow'])
+                    self.__annualCopGWHP[buildingLabel].append((self.__dhwGWHP[
+                        buildingLabel]) / (self.__elGWHP[buildingLabel] + 1e-6))
+
+            if electricitySourceLabel in self.__envParam:
+                envParamGridElectricity = self.__envParam[electricitySourceLabel].copy()
+                envParamGridElectricity.reset_index(inplace=True, drop=True)
+            else:
+                envParamGridElectricity = 0
+            # gridElectricityFlow = solph.views.node(self._optimizationResults, gridBusLabel)["sequences"][
+            #     (electricitySourceLabel, gridBusLabel), "flow"]
+            # gridElectricityFlow.reset_index(inplace=True, drop=True)
+
+            # Environmental impact due to inputs (natural gas, electricity, etc...)
+            self.__envImpactInputs[buildingLabel].update({i[0]: sum(solph.views.node(self._optimizationResults, i[1])["sequences"][(i[0], i[1]), "flow"] * self.__envParam[i[0]]) for i in inputs})
+            c = envParamGridElectricity * gridElectricityFlow
+            if isinstance(c, (int, float)):
+                self.__envImpactInputs[buildingLabel].update({electricitySourceLabel: c})
+            else:
+                self.__envImpactInputs[buildingLabel].update({electricitySourceLabel: c.sum()})  # impact of grid electricity is added separately based on LCA data
+
+            # Environmental impact due to technologies (converters, storages)
+            # calculated by adding both environmental impact per capacity and per flow (electrical flow or heat flow)
+            self.__envImpactTechnologies[buildingLabel].update({i: capacityTransformers[(i, o)] * self.__envParam[i][2] +
+                                                                   sum(sum(solph.views.node(self._optimizationResults,
+                                                                                            t[0])["sequences"][((t[1], t[0]), "flow")] *
+                                                                           self.__envParam[t[1]][1] * ('electricityBus' in t[0]) + \
+                                                                           solph.views.node(self._optimizationResults,
+                                                                                            t[0])["sequences"][((t[1], t[0]), "flow")] *
+                                                                           self.__envParam[t[1]][0] * ('electricityBus' not in t[0]))
+                                                                       for t in technologies if t[1] == i)
+                                                                for i, o in capacityTransformers})
+            self.__envImpactTechnologies[buildingLabel].update({x: capacityStorages[x] * self.__envParam[x][2] +
+                                                                   sum(sum(
+                                                                       solph.views.node(self._optimizationResults,
+                                                                                        t[0])["sequences"][((t[1], t[0]), "flow")] *
+                                                                       self.__envParam[t[1]][1] * ('electricityBus' in t[0]) + \
+                                                                       solph.views.node(self._optimizationResults,
+                                                                                        t[0])["sequences"][((t[1], t[0]), "flow")] *
+                                                                       self.__envParam[t[1]][0] * ('electricityBus' not in t[0]))
+                                                                       for t in technologies if t[1] == x)
+                                                                for x in capacityStorages})
+
+    def printMetaresults(self):
+        print("Meta Results:")
+        pp.pprint(self._metaResults)
+        print("")
+        return self._metaResults
+
+    def calcStateofCharge(self, type, building):
+        if type + '__' + building in self.groups:
+            storage = self.groups[type + '__' + building]
+            # print(f"""********* State of Charge ({type},{building}) *********""")
+            # print(
+            #    self._optimizationResults[(storage, None)]["sequences"]
+            # )
+            self._storageContentSH[building] = self._optimizationResults[(storage, None)]["sequences"]
+        print("")
+
+    def printInvestedCapacities(self, capacitiesInvestedTransformers, capacitiesInvestedStorages):
+        for b in range(len(self.__buildings)):
+            buildingLabel = "Building" + str(b + 1)
+            print("************** Optimized Capacities for {} **************".format(buildingLabel))
+            if ("HP__" + buildingLabel, "shSourceBus__" + buildingLabel) in capacitiesInvestedTransformers:
+                investSH = capacitiesInvestedTransformers[("HP__" + buildingLabel, "shSourceBus__" + buildingLabel)]
+                print("Invested in {:.1f} kW HP.".format(investSH))
+                print("     Annual COP = {:.1f}".format(self.__annualCopHP[buildingLabel]))
+            if ("GWHP__" + buildingLabel, "shSourceBus__" + buildingLabel) in capacitiesInvestedTransformers:
+                investSH = capacitiesInvestedTransformers[("GWHP__" + buildingLabel, "shSourceBus__" + buildingLabel)]
+                print("Invested in {:.1f} kW GWHP.".format(investSH))
+                print("     Annual COP = {:.1f}".format(self.__annualCopGWHP[buildingLabel]))
+            if (f"GWHP{str(self.__temperatureSH)}__" + buildingLabel, "shSourceBus__" + buildingLabel) in capacitiesInvestedTransformers:
+                investSH = capacitiesInvestedTransformers[(f"GWHP{str(self.__temperatureSH)}__" + buildingLabel, "shSourceBus__" + buildingLabel)]
+                print("Invested in {:.1f} kW GWHP{}.".format(investSH, str(self.__temperatureSH)))
+                print("     Annual COP = {:.1f}".format(self.__annualCopGWHP[buildingLabel][0]))
+            if (f"GWHP{str(self.__temperatureDHW)}__" + buildingLabel, "dhwStorageBus__" + buildingLabel) in capacitiesInvestedTransformers:
+                investSH = capacitiesInvestedTransformers[(f"GWHP{str(self.__temperatureDHW)}__" + buildingLabel, "dhwStorageBus__" + buildingLabel)]
+                print("Invested in {:.1f} kW GWHP{}.".format(investSH, str(self.__temperatureDHW)))
+                print("     Annual COP = {:.1f}".format(self.__annualCopGWHP[buildingLabel][1]))
+            if ("ElectricRod__" + buildingLabel, "shSourceBus__" + buildingLabel) in capacitiesInvestedTransformers:
+                investSH = capacitiesInvestedTransformers[("ElectricRod__" + buildingLabel, "shSourceBus__" + buildingLabel)]
+                print("Invested in {:.1f} kW Electric Rod.".format(investSH))
+            if ("CHP__" + buildingLabel, "shSourceBus__" + buildingLabel) in capacitiesInvestedTransformers:
+                investSH = capacitiesInvestedTransformers["CHP__" + buildingLabel, "shSourceBus__" + buildingLabel]
+                print("Invested in {:.1f} kW CHP.".format(investSH))  # + investEL))
+            if ("GasBoiler__" + buildingLabel, "shSourceBus__" + buildingLabel) in capacitiesInvestedTransformers:
+                investSH = capacitiesInvestedTransformers["GasBoiler__" + buildingLabel, "shSourceBus__" + buildingLabel]
+                print("Invested in {:.1f} kW GasBoiler.".format(investSH))
+            if ("heat_solarCollector__" + buildingLabel, "solarConnectBus__" + buildingLabel) in capacitiesInvestedTransformers:
+                invest = capacitiesInvestedTransformers[("heat_solarCollector__" + buildingLabel, "solarConnectBus__" + buildingLabel)]
+                print("Invested in {:.1f} m² SolarCollector.".format(invest))
+            if ("pv__" + buildingLabel, "electricityProdBus__" + buildingLabel) in capacitiesInvestedTransformers:
+                invest = capacitiesInvestedTransformers[("pv__" + buildingLabel, "electricityProdBus__" + buildingLabel)]
+                print("Invested in {:.1f} kWp  PV.".format(invest))
+            if ("heatSource_SHpvt__" + buildingLabel, "pvtConnectBusSH__" + buildingLabel) in capacitiesInvestedTransformers:
+                invest = capacitiesInvestedTransformers[("heatSource_SHpvt__" + buildingLabel, "pvtConnectBusSH__" + buildingLabel)]
+                print("Invested in {:.1f} m² PVT collector.".format(invest))
+            if "electricalStorage__" + buildingLabel in capacitiesInvestedStorages:
+                invest = capacitiesInvestedStorages["electricalStorage__" + buildingLabel]
+                print("Invested in {:.1f} kWh Electrical Storage.".format(invest))
+            if "dhwStorage__" + buildingLabel in capacitiesInvestedStorages:
+                invest = capacitiesInvestedStorages["dhwStorage__" + buildingLabel]
+                print("Invested in {:.1f} L DHW Storage Tank.".format(invest))
+            if "shStorage__" + buildingLabel in capacitiesInvestedStorages:
+                invest = capacitiesInvestedStorages["shStorage__" + buildingLabel]
+                print("Invested in {:.1f} L SH Storage Tank.".format(invest))
+
+    def printCosts(self):
+        capexNetwork = sum(self.__capex["Building" + str(b + 1)] for b in range(len(self.__buildings)))
+        opexNetwork = sum(sum(self.__opex["Building" + str(b + 1)].values()) for b in range(len(self.__buildings)))
+        feedinNetwork = sum(self.__feedIn["Building" + str(b + 1)] for b in range(len(self.__buildings)))
+        print("Investment Costs for the system: {} CHF".format(capexNetwork))
+        print("Operation Costs for the system: {} CHF".format(opexNetwork))
+            # (sum(self.__opex["Building" + str(b + 1)] for b in range(len(self.__buildings)))))
+        print("Feed In Costs for the system: {} CHF".format(feedinNetwork))
+        print("Total Costs for the system: {} CHF".format(capexNetwork + opexNetwork + feedinNetwork))
+
+    def printEnvImpacts(self):
+        envImpactInputsNetwork = sum(sum(self.__envImpactInputs["Building" + str(b + 1)].values()) for b in range(len(self.__buildings)))
+        envImpactTechnologiesNetwork = sum(sum(self.__envImpactTechnologies["Building" + str(b + 1)].values()) for b in range(len(self.__buildings)))
+        print("Environmental impact from input resources for the system: {} kg CO2 eq".format(envImpactInputsNetwork))
+        print("Environmental impact from energy conversion technologies for the system: {} kg CO2 eq".format(envImpactTechnologiesNetwork))
+        print("Total: {} kg CO2 eq".format(envImpactInputsNetwork + envImpactTechnologiesNetwork))
+
+    def getTotalCosts(self):
+        capexNetwork = sum(self.__capex["Building" + str(b + 1)] for b in range(len(self.__buildings)))
+        opexNetwork = sum(
+            sum(self.__opex["Building" + str(b + 1)].values()) for b in range(len(self.__buildings)))
+        feedinNetwork = sum(self.__feedIn["Building" + str(b + 1)] for b in range(len(self.__buildings)))
+        return capexNetwork + opexNetwork + feedinNetwork
+
+    def getTotalEnvImpacts(self):
+        envImpactInputsNetwork = sum(
+            sum(self.__envImpactInputs["Building" + str(b + 1)].values()) for b in range(len(self.__buildings)))
+        envImpactTechnologiesNetwork = sum(
+            sum(self.__envImpactTechnologies["Building" + str(b + 1)].values()) for b in range(len(self.__buildings)))
+        return envImpactTechnologiesNetwork + envImpactInputsNetwork
+
+    def exportToExcel(self, file_name, mergeLinkBuses=False):
+        for i in range(1, self.__noOfBuildings+1):
+            self.calcStateofCharge("shStorage", f"Building{i}")
+        with pd.ExcelWriter(file_name) as writer:
+            busLabelList = []
+            for i in self.nodes:
+                if str(type(i)).replace("<class 'oemof.solph.", "").replace("'>", "") == "network.bus.Bus":
+                    busLabelList.append(i.label)
+            # writing results of each bus into excel
+            for i in busLabelList:
+                if "domesticHotWaterBus" in i:  # special case for DHW bus (output from transformers --> dhwStorageBus --> DHW storage --> domesticHotWaterBus --> DHW Demand)
+                    if not mergeLinkBuses:
+                        dhwStorageBusLabel = "dhwStorageBus__" + i.split("__")[1]
+                        resultDHW = pd.DataFrame.from_dict(solph.views.node(self._optimizationResults, i)["sequences"])  # result sequences of DHW bus
+                        resultDHWStorage = pd.DataFrame.from_dict(solph.views.node(self._optimizationResults, dhwStorageBusLabel)["sequences"])  # result sequences of DHW storage bus
+                        result = pd.concat([resultDHW, resultDHWStorage], axis=1, sort=True)
+                    else:
+                        result = pd.DataFrame.from_dict(solph.views.node(self._optimizationResults, i)["sequences"])  # result sequences of DHW bus
+                elif mergeLinkBuses and "dhwStorageBus" in i and "sequences" in solph.views.node(self._optimizationResults, i):
+                    result = pd.DataFrame.from_dict(solph.views.node(self._optimizationResults, i)["sequences"])  # result sequences of DHW storage bus
+                elif "dhwStorageBus" not in i:  # for all the other buses except DHW storage bus (as it is already considered with DHW bus)
+                    if 'sequences' in solph.views.node(self._optimizationResults, i):
+                        result = pd.DataFrame.from_dict(solph.views.node(self._optimizationResults, i)["sequences"])
+                        if "shSourceBus" in i and i.split("__")[1] in self._storageContentSH:
+                            result = pd.concat([result, self._storageContentSH[i.split("__")[1]]], axis=1, sort=True)
+                    else:
+                        continue
+                result[result < 0.001] = 0      # to resolve the issue of very low values in the results in certain cases, values less than 1 Watt would be replaced by 0
+                if mergeLinkBuses or "dhwStorageBus" not in i:
+                    result.to_excel(writer, sheet_name=i)
+
+            # writing the costs and environmental impacts (of different components...) for each building
+            for b in self.__buildings:
+                buildingLabel = b.getBuildingLabel()
+                costs = self.__opex[buildingLabel]
+                costs.update({"Investment": self.__capex[buildingLabel],
+                              "Feed-in": self.__feedIn[buildingLabel]})
+                    # {"Operation": self.__opex[buildingLabel],
+                    #      "Investment": self.__capex[buildingLabel],
+                    #      "Feed-in": self.__feedIn[buildingLabel],
+                    #      }
+                costsBuilding = pd.DataFrame.from_dict(costs, orient='index')
+                costsBuilding.to_excel(writer, sheet_name="costs__" + buildingLabel)
+
+                envImpact = self.__envImpactInputs[buildingLabel].copy()
+                envImpact.update(self.__envImpactTechnologies[buildingLabel])
+
+                envImpactBuilding = pd.DataFrame.from_dict(envImpact, orient='index')
+                envImpactBuilding.to_excel(writer, sheet_name="env_impacts__" + buildingLabel)
+
+                capacitiesStorages = self.__capacitiesStoragesBuilding[buildingLabel].copy()
+                capacitiesStorages.update(self.__capacitiesStoragesBuilding[buildingLabel])
+
+                capacitiesStoragesBuilding = pd.DataFrame.from_dict(capacitiesStorages, orient='index')
+                capacitiesStoragesBuilding.to_excel(writer, sheet_name="capStorages__" + buildingLabel)
+
+                capacitiesTransformers = self.__capacitiesTransformersBuilding[buildingLabel].copy()
+                capacitiesTransformers.update(self.__capacitiesTransformersBuilding[buildingLabel])
+
+                capacitiesTransformersBuilding = pd.DataFrame.from_dict(capacitiesTransformers, orient='index')
+                capacitiesTransformersBuilding.to_excel(writer, sheet_name="capTransformers__" + buildingLabel)
+
+class EnergyNetworkIndiv(EnergyNetworkClass):
+    def createScenarioFile(self, configFilePath, excelFilePath, building, numberOfBuildings=1):
+        """function to create the input excel file from a config file
+        saves the generated excel file at the path given by excelFilePath"""
+        config = ConfigParser()
+        config.read(configFilePath)
+        configData = {}
+        excelData= {}
+        columnNames = {'commodity_sources': ['label', 'building', 'to', 'variable costs', 'CO2 impact', 'active'],# column names are defined for each sheet (key of dict) in the excel file
+                       'solar': ['label', 'building', 'from', 'to', 'connect', 'electrical_consumption', 'peripheral_losses', 'latitude', 'longitude', 'tilt', 'azimuth', 'eta_0', 'a_1', 'a_2', 'temp_collector_inlet', 'delta_temp_n', 'capacity_max', 'capacity_min', 'lifetime', 'maintenance', 'installation', 'planification', 'invest_base', 'invest_cap', 'heat_impact', 'elec_impact', 'impact_cap'],
+                       'demand': ['label', 'building', 'active', 'from', 'fixed', 'nominal value', 'building model'],
+                       'transformers': ['label', 'building', 'active', 'from', 'to', 'efficiency', 'capacity_DHW', 'capacity_SH', 'capacity_el', 'capacity_min', 'lifetime', 'maintenance', 'installation', 'planification', 'invest_base', 'invest_cap', 'heat_impact', 'elec_impact', 'impact_cap'],
+                       'storages': ['label', 'building', 'active', 'from', 'to', 'efficiency inflow', 'efficiency outflow', 'initial capacity', 'capacity min', 'capacity max', 'capacity loss', 'lifetime', 'maintenance', 'installation', 'planification', 'invest_base', 'invest_cap', 'heat_impact', 'elec_impact', 'impact_cap'],
+                       'stratified_storage': ['label', 'diameter', 'temp_h', 'temp_c', 'temp_env', 'inflow_conversion_factor', 'outflow_conversion_factor', 's_iso', 'lamb_iso', 'alpha_inside', 'alpha_outside']
+                       }
+        buses = {'naturalgasresource': ['naturalGasBus', '', ''], 'electricityresource': ['gridBus', '', ''], 'solarcollector': ['dhwStorageBus', 'electricityInBus', 'solarConnectBus'],    # [to, from, connect] columns in the excel file
+                 'pv': ['electricityProdBus', '', ''], 'electricitydemand': ['', 'electricityInBus', ''], 'spaceheatingdemand': ['', 'shDemandBus', ''],
+                 'domestichotwaterdemand': ['', 'domesticHotWaterBus', ''], 'gasboiler': ['shSourceBus,dhwStorageBus', 'naturalGasBus', ''], 'electricrod': ['shSourceBus,dhwStorageBus', 'electricityInBus', ''],
+                 'chp': ['electricityProdBus,shSourceBus,dhwStorageBus', 'naturalGasBus', ''], 'ashp': ['shSourceBus,dhwStorageBus', 'electricityInBus', ''], 'gshp': ['shSourceBus,dhwStorageBus', 'electricityInBus', ''],
+                 'electricalstorage': ['electricityBus', 'electricityProdBus', ''], 'shstorage': ['spaceHeatingBus', 'shSourceBus', ''], 'dhwstorage': ['domesticHotWaterBus', 'dhwStorageBus', '']}
+        sheetToSection = {'commodity_sources':'CommoditySources', 'solar':'Solar', 'demand':'Demands', 'transformers':'Transformers', 'storages':'Storages', 'stratified_storage':'StratifiedStorage'}
+        sections = config.sections()
+        profiles = pd.DataFrame(columns=['name', 'path'])
+        updatedLabels = {'weatherpath':'weather_data', 'path':'demand_profiles', 'ashp':'HP', 'gshp':'GWHP', 'electricityresource':'electricityResource', 'naturalgasresource':'naturalGasResource', 'chp':'CHP', 'gasboiler':'GasBoiler', 'electricrod':'ElectricRod', 'pv':'pv', 'solarcollector':'solarCollector', 'electricalstorage':'electricalStorage', 'shstorage':'shStorage', 'dhwstorage':'dhwStorage', 'stratifiedstorage':'StratifiedStorage'}
+        temp_h = {}     # to store temp_h values for stratified storage parameters sheet
+        FeedinTariff = 0
+        for section in config.sections():
+            configData[section]=config.items(section)
+        configData = {k.lower(): v for k, v in configData.items()}
+        for sheet in columnNames:
+            excelData[sheet] = pd.DataFrame(columns=columnNames[sheet])
+            if sheet == 'stratified_storage':
+                newRow = pd.DataFrame(columns=columnNames[sheet])
+                newRow.at[0, 'label'] = list(temp_h)[0]
+                newRow.at[0, 'temp_h'] = list(temp_h.values())[0]
+                newRow.at[1, 'label'] = list(temp_h)[1]
+                newRow.at[1, 'temp_h'] = list(temp_h.values())[1]
+            for item in configData[sheetToSection[sheet].lower()]:
+                type = item[0]
+                if item[1] in ['True', 'False']:  # defines whether or not a component is to be added
+                    if item[1] == 'True':
+                        newRow = pd.DataFrame(columns=columnNames[sheet])
+                        newRow.at[0,'label']=updatedLabels[item[0]]
+                        newRow.at[0,'active']=int(bool(item[1]=='True'))
+                        # sheet specific options
+                        cols = newRow.columns
+                        if 'building' in cols:
+                            newRow.at[0,'building']=1
+                        if 'to' in cols:
+                            newRow.at[0,'to'] = buses[type][0]
+                        if 'from' in cols:
+                            newRow.at[0,'from'] = buses[type][1]
+                        if 'connect' in cols:
+                            newRow.at[0,'connect'] = buses[type][2]
+                        params = configData[type]
+                        if sheet == 'commodity_sources':
+                            index = [x for x, y in enumerate(params) if y[0] == 'cost'][0]
+                            newRow.at[0,'variable costs'] = params[index][1]
+                            index = [x for x, y in enumerate(params) if y[0] == 'impact'][0]
+                            newRow.at[0,'CO2 impact'] = params[index][1]
+                            if type=='electricityresource':
+                                index = [x for x, y in enumerate(params) if y[0] == 'feedintariff'][0]
+                                FeedinTariff = -float(params[index][1])
+                        else:
+                            for p in params:
+                                if sheet=='transformers' and p[0] == 'capacity_max':
+                                    newRow.at[0, 'capacity_DHW'] = p[1]
+                                    newRow.at[0, 'capacity_SH'] = p[1]
+                                    if updatedLabels[item[0]]=='CHP':
+                                        newRow.at[0, 'capacity_el'] = str(round(float(p[1])*float(newRow.at[0, 'efficiency'].split(',')[0])/float(newRow.at[0, 'efficiency'].split(',')[1]),0))
+                                elif sheet=='storages' and p[0] == 'temp_h':
+                                    temp_h[newRow.at[0,'label']] = p[1]
+                                else:
+                                    newRow.at[0,p[0]] = p[1]
+                        excelData[sheet] = pd.concat([excelData[sheet], newRow])
+                elif type=='path':       # demand path
+                    buildingFolder = [i[1] for i in configData['demands'] if i[0] == 'folders'][0].split(',')[building]
+                    buildingPath = item[1]+'\\'+ buildingFolder
+                    profiles = pd.concat([profiles, pd.DataFrame({'name': [updatedLabels[type]], 'path': [buildingPath]})])
+                elif 'path' in type:     # weather path
+                    profiles = pd.concat([profiles, pd.DataFrame({'name':[updatedLabels[type]], 'path':[item[1]]})])
+                elif sheet == 'demand' and type!='folders':
+                    newRow = pd.DataFrame(columns=columnNames[sheet])
+                    for d in ['electricityDemand', 'spaceHeatingDemand', 'domesticHotWaterDemand']:
+                        newRow.at[0, 'label'] = d
+                        newRow.at[0, 'from'] = buses[d.lower()][1]
+                        if d == 'spaceHeatingDemand' and item[1]==0:
+                            newRow.at[0, 'fixed'] = item[1]
+                            newRow.at[0, 'building model'] = 'Yes'
+                        else:
+                            newRow.at[0, 'fixed'] = 1
+                        excelData[sheet] = pd.concat([excelData[sheet], newRow])
+                    excelData[sheet]['building'] = 1
+                    excelData[sheet]['active'] = 1
+                    excelData[sheet]['nominal value'] = 1
+                elif sheet == 'stratified_storage':
+                    newRow.at[0,type] = item[1]
+                    newRow.at[1,type] = item[1]
+                else: # common parameters of all the components of that section
+                    if type!='folders':
+                        excelData[sheet][type] = item[1]
+            if sheet == 'stratified_storage':
+                excelData[sheet] = pd.concat([excelData[sheet], newRow])
+        excelData['profiles'] = profiles
+        excelData['grid_connection'] = pd.DataFrame({'label':['gridElectricity','electricitySource','producedElectricity','shSource','spaceHeating'], 'building':[1,1,1,1,1], 'from':['gridBus','electricityProdBus','electricityBus','shSourceBus','spaceHeatingBus'], 'to':['electricityInBus','electricityBus','electricityInBus','spaceHeatingBus','shDemandBus'], 'efficiency':[1,1,1,1,1]})
+
+        df = pd.DataFrame(columns=['buses'])
+        for sheet, data in excelData.items():
+            for col in ['from', 'to', 'connect']:
+                if col in data.columns:
+                    newBuses = pd.DataFrame(columns=['buses'])
+                    newBuses['buses'] = data[col].values
+                    df = pd.concat([df, newBuses])
+        df = df.assign(buses=df.buses.str.split(',')).explode('buses')['buses'].unique()
+        df = df[df != '']
+        excelData['buses'] = pd.DataFrame(columns=['label', 'building', 'excess', 'excess costs', 'active'])
+        for index in range(len(df)):
+            excelData['buses'].at[index,'label'] = df[index]
+            if df[index] == 'electricityBus' and FeedinTariff!=0:
+                excelData['buses'].at[index,'excess'] = 1
+                excelData['buses'].at[index, 'excess costs'] = FeedinTariff
+        excelData['buses']['building'] = 1
+        excelData['buses']['active'] = 1
+        excelData['buses'].loc[excelData['buses']['excess']!=1,'excess'] = 0
+        for sheet, data in excelData.items():
+            if 'building' in data.columns:
+                buildingNo = [i for i in range(1, numberOfBuildings + 1)]* len(excelData[sheet].index)
+                excelData[sheet] = pd.DataFrame(np.repeat(data.values, numberOfBuildings, axis=0), columns=data.columns)
+                excelData[sheet]['building'] = buildingNo
+        with pd.ExcelWriter(excelFilePath, engine='xlwt') as writer:
+            for sheet, data in excelData.items():
+                data.to_excel(writer, sheet_name=sheet, index=False)
+            writer.save()
+            writer.close()
+
+
+class EnergyNetworkGroup(EnergyNetworkClass):
+    def createScenarioFile(self, configFilePath, excelFilePath, numberOfBuildings):
+        """function to create the input excel file from a config file
+        saves the generated excel file at the path given by excelFilePath"""
+        config = ConfigParser()
+        config.read(configFilePath)
+        configData = {}
+        excelData = {}
+        columnNames = {'commodity_sources': ['label', 'building', 'to', 'variable costs', 'CO2 impact', 'active'],
+                       # column names are defined for each sheet (key of dict) in the excel file
+                       'solar': ['label', 'building', 'from', 'to', 'connect', 'electrical_consumption',
+                                 'peripheral_losses', 'latitude', 'longitude', 'tilt', 'azimuth', 'eta_0', 'a_1', 'a_2',
+                                 'temp_collector_inlet', 'delta_temp_n', 'capacity_max', 'capacity_min', 'lifetime',
+                                 'maintenance', 'installation', 'planification', 'invest_base', 'invest_cap',
+                                 'heat_impact', 'elec_impact', 'impact_cap'],
+                       'demand': ['label', 'building', 'active', 'from', 'fixed', 'nominal value', 'building model'],
+                       'transformers': ['label', 'building', 'active', 'from', 'to', 'efficiency', 'capacity_DHW',
+                                        'capacity_SH', 'capacity_el', 'capacity_min', 'lifetime', 'maintenance',
+                                        'installation', 'planification', 'invest_base', 'invest_cap', 'heat_impact',
+                                        'elec_impact', 'impact_cap'],
+                       'storages': ['label', 'building', 'active', 'from', 'to', 'efficiency inflow',
+                                    'efficiency outflow', 'initial capacity', 'capacity min', 'capacity max',
+                                    'capacity loss', 'lifetime', 'maintenance', 'installation', 'planification',
+                                    'invest_base', 'invest_cap', 'heat_impact', 'elec_impact', 'impact_cap'],
+                       'stratified_storage': ['label', 'diameter', 'temp_h', 'temp_c', 'temp_env',
+                                              'inflow_conversion_factor', 'outflow_conversion_factor', 's_iso',
+                                              'lamb_iso', 'alpha_inside', 'alpha_outside'],
+                       'links': ['label', 'active', 'efficiency', 'invest_base', 'invest_cap', 'investment']
+                       }
+        buses = {'naturalgasresource': ['naturalGasBus', '', ''], 'electricityresource': ['gridBus', '', ''],
+                 'solarcollector': ['dhwStorageBus', 'electricityInBus', 'solarConnectBus'],
+                 # [to, from, connect] columns in the excel file
+                 'pv': ['electricityProdBus', '', ''], 'electricitydemand': ['', 'electricityInBus', ''],
+                 'spaceheatingdemand': ['', 'shDemandBus', ''],
+                 'domestichotwaterdemand': ['', 'dhwDemandBus', ''],
+                 'gasboiler': ['shSourceBus,dhwStorageBus', 'naturalGasBus', ''],
+                 'electricrod': ['shSourceBus,dhwStorageBus', 'electricityInBus', ''],
+                 'chp': ['electricityProdBus,shSourceBus,dhwStorageBus', 'naturalGasBus', ''],
+                 'ashp': ['shSourceBus,dhwStorageBus', 'electricityInBus', ''],
+                 'gshp': ['shSourceBus,dhwStorageBus', 'electricityInBus', ''],
+                 'electricalstorage': ['electricityBus', 'electricityProdBus', ''],
+                 'shstorage': ['spaceHeatingBus', 'shSourceBus', ''],
+                 'dhwstorage': ['domesticHotWaterBus', 'dhwStorageBus', '']}
+        sheetToSection = {'commodity_sources': 'CommoditySources', 'solar': 'Solar', 'demand': 'Demands',
+                          'transformers': 'Transformers', 'storages': 'Storages',
+                          'stratified_storage': 'StratifiedStorage', 'links':'Links'}
+        sections = config.sections()
+        profiles = pd.DataFrame(columns=['name', 'path'])
+        updatedLabels = {'weatherpath': 'weather_data', 'path': 'demand_profiles', 'ashp': 'HP', 'gshp': 'GWHP',
+                         'electricityresource': 'electricityResource', 'naturalgasresource': 'naturalGasResource',
+                         'chp': 'CHP', 'gasboiler': 'GasBoiler', 'electricrod': 'ElectricRod', 'pv': 'pv',
+                         'solarcollector': 'solarCollector', 'electricalstorage': 'electricalStorage',
+                         'shstorage': 'shStorage', 'dhwstorage': 'dhwStorage', 'stratifiedstorage': 'StratifiedStorage',
+                         'ellink': 'electricityLink', 'shlink': 'shLink', 'dhwlink': 'dhwLink'}
+        efficiencyLinks = {'ellink': 0.9999, 'shlink': 0.9, 'dhwlink': 0.9}
+        temp_h = {}  # to store temp_h values for stratified storage parameters sheet
+        FeedinTariff = 0
+        for section in config.sections():
+            configData[section] = config.items(section)
+        configData = {k.lower(): v for k, v in configData.items()}
+        for sheet in columnNames:
+            excelData[sheet] = pd.DataFrame(columns=columnNames[sheet])
+            if sheet == 'stratified_storage':
+                newRow = pd.DataFrame(columns=columnNames[sheet])
+                newRow.at[0, 'label'] = list(temp_h)[0]
+                newRow.at[0, 'temp_h'] = list(temp_h.values())[0]
+                newRow.at[1, 'label'] = list(temp_h)[1]
+                newRow.at[1, 'temp_h'] = list(temp_h.values())[1]
+            for item in configData[sheetToSection[sheet].lower()]:
+                type = item[0]
+                if item[1] in ['True', 'False']:  # defines whether or not a component is to be added
+                    if item[1] == 'True':
+                        newRow = pd.DataFrame(columns=columnNames[sheet])
+                        newRow.at[0, 'label'] = updatedLabels[item[0]]
+                        newRow.at[0, 'active'] = int(bool(item[1] == 'True'))
+                        # sheet specific options
+                        cols = newRow.columns
+                        if 'building' in cols:
+                            newRow.at[0, 'building'] = 1
+                        if 'to' in cols:
+                            newRow.at[0, 'to'] = buses[type][0]
+                        if 'from' in cols:
+                            newRow.at[0, 'from'] = buses[type][1]
+                        if 'connect' in cols:
+                            newRow.at[0, 'connect'] = buses[type][2]
+                        if type in ['shlink', 'dhwlink']:
+                            params = configData['thermallink']
+                        else:
+                            params = configData[type]
+                        if sheet == 'commodity_sources':
+                            index = [x for x, y in enumerate(params) if y[0] == 'cost'][0]
+                            newRow.at[0, 'variable costs'] = params[index][1]
+                            index = [x for x, y in enumerate(params) if y[0] == 'impact'][0]
+                            newRow.at[0, 'CO2 impact'] = params[index][1]
+                            if type == 'electricityresource':
+                                index = [x for x, y in enumerate(params) if y[0] == 'feedintariff'][0]
+                                FeedinTariff = -float(params[index][1])
+                        else:
+                            if sheet == 'links':
+                                if not [x for x, y in enumerate(params) if y[0] == 'efficiency']:
+                                    newRow.at[0, 'efficiency'] = efficiencyLinks[type]
+                                newRow.at[0, 'investment'] = 1
+                            for p in params:
+                                if sheet == 'transformers' and p[0] == 'capacity_max':
+                                    newRow.at[0, 'capacity_DHW'] = p[1]
+                                    newRow.at[0, 'capacity_SH'] = p[1]
+                                    if updatedLabels[item[0]]=='CHP':
+                                        newRow.at[0, 'capacity_el'] = str(round(float(p[1])*float(newRow.at[0, 'efficiency'].split(',')[0])/float(newRow.at[0, 'efficiency'].split(',')[1]),0))
+                                elif sheet == 'storages' and p[0] == 'temp_h':
+                                    temp_h[newRow.at[0, 'label']] = p[1]
+                                else:
+                                    newRow.at[0, p[0]] = p[1]
+                        excelData[sheet] = pd.concat([excelData[sheet], newRow])
+                elif 'path' in type:  # weather path or demand path
+                    profiles = pd.concat([profiles, pd.DataFrame({'name': [updatedLabels[type]], 'path': [item[1]]})])
+                elif sheet == 'demand':
+                    newRow = pd.DataFrame(columns=columnNames[sheet])
+                    for d in ['electricityDemand', 'spaceHeatingDemand', 'domesticHotWaterDemand']:
+                        newRow.at[0, 'label'] = d
+                        newRow.at[0, 'from'] = buses[d.lower()][1]
+                        if d == 'spaceHeatingDemand' and item[1] == 0:
+                            newRow.at[0, 'fixed'] = item[1]
+                            newRow.at[0, 'building model'] = 'Yes'
+                        else:
+                            newRow.at[0, 'fixed'] = 1
+                        excelData[sheet] = pd.concat([excelData[sheet], newRow])
+                    excelData[sheet]['building'] = 1
+                    excelData[sheet]['active'] = 1
+                    excelData[sheet]['nominal value'] = 1
+                elif sheet == 'stratified_storage':
+                    newRow.at[0, type] = item[1]
+                    newRow.at[1, type] = item[1]
+                else:  # common parameters of all the components of that section
+                    excelData[sheet][type] = item[1]
+            if sheet == 'stratified_storage':
+                excelData[sheet] = pd.concat([excelData[sheet], newRow])
+        excelData['profiles'] = profiles
+        excelData['grid_connection'] = pd.DataFrame(
+            {'label': ['gridElectricity', 'electricitySource', 'producedElectricity', 'domesticHotWater', 'shSource', 'spaceHeating'],
+             'building': [1, 1, 1, 1, 1, 1],
+             'from': ['gridBus', 'electricityProdBus', 'electricityBus', 'domesticHotWaterBus', 'shSourceBus', 'spaceHeatingBus'],
+             'to': ['electricityInBus', 'electricityBus', 'electricityInBus', 'dhwDemandBus', 'spaceHeatingBus', 'shDemandBus'],
+             'efficiency': [1, 1, 1, 1, 1, 1]})
+
+        df = pd.DataFrame(columns=['buses'])
+        for sheet, data in excelData.items():
+            for col in ['from', 'to', 'connect']:
+                if col in data.columns:
+                    newBuses = pd.DataFrame(columns=['buses'])
+                    newBuses['buses'] = data[col].values
+                    df = pd.concat([df, newBuses])
+        df = df.assign(buses=df.buses.str.split(',')).explode('buses')['buses'].unique()
+        df = df[df != '']
+        excelData['buses'] = pd.DataFrame(columns=['label', 'building', 'excess', 'excess costs', 'active'])
+        for index in range(len(df)):
+            excelData['buses'].at[index, 'label'] = df[index]
+            if df[index] == 'electricityBus' and FeedinTariff != 0:
+                excelData['buses'].at[index, 'excess'] = 1
+                excelData['buses'].at[index, 'excess costs'] = FeedinTariff
+        excelData['buses']['building'] = 1
+        excelData['buses']['active'] = 1
+        excelData['buses'].loc[excelData['buses']['excess'] != 1, 'excess'] = 0
+        for sheet, data in excelData.items():
+            if 'building' in data.columns:
+                buildingNo = [i for i in range(1, numberOfBuildings + 1)] * len(excelData[sheet].index)
+                excelData[sheet] = pd.DataFrame(np.repeat(data.values, numberOfBuildings, axis=0), columns=data.columns)
+                excelData[sheet]['building'] = buildingNo
+        with pd.ExcelWriter(excelFilePath, engine='xlwt') as writer:
+            for sheet, data in excelData.items():
+                data.to_excel(writer, sheet_name=sheet, index=False)
+            writer.save()
+            writer.close()
+
+    def setFromExcel(self, filePath, numberOfBuildings, clusterSize={}, opt="costs", mergeLinkBuses=False, dispatchMode=False, includeCarbonBenefits=False):
+        # does Excel file exist?
+        if not filePath or not os.path.isfile(filePath):
+            logging.error("Excel data file {} not found.".format(filePath))
+        logging.info("Defining the energy network from the excel file: {}".format(filePath))
+        self._dispatchMode = dispatchMode
+        data = pd.ExcelFile(filePath)
+
+        nodesData = self.createNodesData(data, filePath, numberOfBuildings)
+        # nodesData["buses"]["excess costs"] = nodesData["buses"]["excess costs group"]
+        # nodesData["electricity_cost"]["cost"] = nodesData["electricity_cost"]["cost group"]
+
+        demandProfiles = {}
+        if clusterSize:
+            for i in range(1, numberOfBuildings + 1):
+                demandProfiles[i] = pd.concat(
+                    [nodesData["demandProfiles"][i].loc[d] for d in clusterSize.keys()])
+            electricityImpact = pd.concat(
+                [nodesData["electricity_impact"].loc[d]*clusterSize[d] for d in clusterSize.keys()])
+            electricityCost = pd.concat(
+                [nodesData["electricity_cost"].loc[d]*clusterSize[d] for d in clusterSize.keys()])
+            if 'natGas_impact' in nodesData:
+                natGasImpact = pd.concat(
+                    [nodesData["natGas_impact"].loc[d]*clusterSize[d] for d in clusterSize.keys()])
+                natGasCost = pd.concat(
+                    [nodesData["natGas_cost"].loc[d]*clusterSize[d] for d in clusterSize.keys()])
+            weatherData = pd.concat([nodesData['weather_data'][
+                                         nodesData['weather_data']['time.mm'] == int(d.split('-')[1])][
+                                         nodesData['weather_data']['time.dd'] == int(d.split('-')[2])][['gls', 'str.diffus', 'tre200h0', 'ground_temp']] for d in clusterSize.keys()])
+
+            nodesData["demandProfiles"] = demandProfiles
+            nodesData["electricity_impact"] = electricityImpact
+            nodesData["electricity_cost"] = electricityCost
+            if 'natGas_impact' in nodesData:
+                nodesData["natGas_impact"] = natGasImpact
+                nodesData["natGas_cost"] = natGasCost
+            nodesData["weather_data"] = weatherData
+
+        nodesData["links"]= data.parse("links")
+        self._convertNodes(nodesData, opt, mergeLinkBuses, includeCarbonBenefits, clusterSize)
+        self._addLinks(nodesData["links"], numberOfBuildings, mergeLinkBuses)
+        logging.info("Nodes from Excel file {} successfully converted".format(filePath))
+        self.add(*self._nodesList)
+        logging.info("Nodes successfully added to the energy network")
+
+
+    def _addLinks(self, data, numberOfBuildings, mergeLinkBuses):  # connects buses A and B (denotes a bidirectional link)
+        if mergeLinkBuses:
+            return
+        for i, l in data.iterrows():
+            if l["active"]:
+                if l["investment"]:
+                    investment = solph.Investment(
+                        ep_costs=l["invest_cap"],
+                        nonconvex=True,
+                        maximum=500000,
+                        offset=l["invest_base"],
+                    )
+                else:
+                    investment = None
+                busesOut = []
+                busesIn = []
+                # add two buses for each building link_out and link_in
+                for b in range(numberOfBuildings):
+                    if "sh" in l["label"]:
+                        busesOut.append(self._busDict["spaceHeatingBus" + '__Building' + str(b+1)])
+                        busesIn.append(self._busDict["shDemandBus" + '__Building' + str(b+1)])
+                    elif "dhw" in l["label"]:
+                        busesOut.append(self._busDict["domesticHotWaterBus" + '__Building' + str(b+1)])
+                        busesIn.append(self._busDict["dhwDemandBus" + '__Building' + str(b+1)])
+                    else:
+                        busesOut.append(self._busDict["electricityBus" + '__Building' + str(b + 1)])
+                        busesIn.append(self._busDict["electricityInBus" + '__Building' + str(b + 1)])
+
+                self._nodesList.append(Link(
+                    label=l["label"],
+                    inputs={busA: solph.Flow() for busA in busesOut},
+                    outputs={busB: solph.Flow(investment=investment) for busB in busesIn},
+                    conversion_factors={busB: l["efficiency"] for busB in busesIn}
                 ))
```

### Comparing `optihood-0.0.0/optihood/labelDict.py` & `optihood-0.0.1/optihood/labelDict.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,634 +1,634 @@
-def labelDictGenerator(numBuildings, labels, optimType, mergedLinks):
-    base = {"electricityLink":"elLink", "shLink":"shLink", "dhwLink":"dhwLink", "naturalGasResource":"natGas", "naturalGasBus":"natGas", "gridBus":"grid", "pv":"pv", "electricityResource":"grid", "gridElectricity":"grid", "GasBoiler":"gasBoiler",
-    "CHP":"CHP", "electricityBus":"prodEl", "electricityProdBus":"localEl", "producedElectricity":"prodEl", "electricitySource":"localEl", "electricalStorage":"Bat", "excesselectricityBus":"exEl",
-    "excessshDemandBus":"exSh", "electricityInBus":"usedEl", "HP":"HP", "GWHP":"GWHP", "GWHP35":"GWHP35", "GWHP60":"GWHP60", "solarCollector":"solar", "solarConnectBus":"solar","heat_solarCollector":"solar", "excess_solarheat":"exSolar",
-    "shSource":"prodSH","shSourceBus":"prodSH", "spaceHeatingBus":"shBus", "spaceHeating":"shBus", "shStorage":"shStor", "shDemandBus":"shBus", "dhwStorageBus":"dhwStor", "dhwStorage":"dhwStor", "domesticHotWaterBus":"dhwBus",
-    "domesticHotWater":"dhwBus", "dhwDemandBus":"dhwBus", "electricityDemand":"Q_el", "emobilityDemand":"Q_mob", "spaceHeatingDemand":"Q_sh", "domesticHotWaterDemand":"Q_dhw", "excessshSourceBus":"exSh",
-    "ElectricRod":"ElectricRod"}
-    if not mergedLinks and optimType == 'group':
-        base['electricityInBus'] = "usedEl"
-        base['spaceHeatingBus'] = "usedSH"
-        base['domesticHotWaterBus'] = "prodDHW"
-        if labels != 'default':
-            base["electricityInBus"] = labels["usedEl"]
-            base["spaceHeatingBus"] = labels["usedSH"]
-            base["spaceHeating"] = labels["shBus"]
-            base["shDemandBus"] = labels["shBus"]
-            base["domesticHotWaterBus"] = labels["prodDHW"]
-            base['domesticHotWater'] = labels["dhwBus"]
-            base['dhwDemandBus'] = labels["dhwBus"]
-    if labels != 'default':
-        if "elBus" in labels and ((mergedLinks and optimType=='group') or optimType=='indiv'): base["electricityLink"] = labels["elBus"]
-        if "elBus" in labels and not mergedLinks and optimType=='group': base["electricityLink"] = labels["elBus"] + " Link"
-        if "shBus" in labels and ((mergedLinks and optimType=='group') or optimType=='indiv'): base["shLink"] = labels["shBus"]
-        if "shBus" in labels and not mergedLinks and optimType=='group': base["shLink"] = labels["shBus"] + " Link"
-        if "dhwBus" in labels and ((mergedLinks and optimType=='group') or optimType=='indiv'): base["dhwLink"] = labels["dhwBus"]
-        if "dhwBus" in labels and not mergedLinks and optimType=='group': base["dhwLink"] = labels["dhwBus"] + " Link"
-        if "naturalGas" in labels:
-            base["naturalGasResource"] = labels["naturalGas"]
-            base["naturalGasBus"] = labels["naturalGas"]
-        if "grid" in labels:
-            base["gridBus"] = labels["grid"]
-            base["electricityResource"] = labels["grid"]
-            base["gridElectricity"] = labels["grid"]
-        if "pv" in labels: base["pv"]=labels["pv"]
-        if "gasBoiler" in labels: base["GasBoiler"]=labels["gasBoiler"]
-        if "CHP" in labels:base["CHP"]=labels["CHP"]
-        if "prodEl" in labels:
-            base["electricityBus"]=labels["prodEl"]
-            base["producedElectricity"] = labels["prodEl"]
-        if "localEl" in labels:
-            base["electricityProdBus"]=labels["localEl"]
-            base["electricitySource"]=labels["localEl"]
-        if "StorageEl" in labels:base["electricalStorage"]=labels["StorageEl"]
-        if "excessEl" in labels:base["excesselectricityBus"]=labels["excessEl"]
-        if "excessSh" in labels:
-            base["excessshDemandBus"]=labels["excessSh"]
-            base["excessshSourceBus"]=labels["excessSh"]
-        if "elBus" in labels and (mergedLinks or optimType == 'indiv'):base["electricityInBus"]=labels["elBus"]
-        if "HP" in labels:base["HP"]=labels["HP"]
-        if "GWHP" in labels:
-            base["GWHP"]=labels["GWHP"]
-            base["GWHP35"]=labels["GWHP"]+'35'# for splitted GSHP
-            base["GWHP60"] = labels["GWHP"]+'60'
-        if "solarCollector" in labels:
-            base["solarCollector"]=labels["solarCollector"]
-            base["solarConnectBus"]=labels["solarCollector"]
-            base["heat_solarCollector"]=labels["solarCollector"]
-        if "excessSolarCollector" in labels: base["excess_solarheat"]=labels["excessSolarCollector"]
-        if "prodSH" in labels:
-            base["shSource"]=labels["prodSH"]
-            base["shSourceBus"]=labels["prodSH"]
-        if "shBus" in labels and (mergedLinks or optimType == 'indiv'):
-            base["spaceHeatingBus"]=labels["shBus"]
-            base["spaceHeating"]=labels["shBus"]
-            base["shDemandBus"] = labels["shBus"]
-        if "StorageSh" in labels:base["shStorage"]=labels["StorageSh"]
-        if "StorageDhw" in labels:
-            base["dhwStorageBus"]=labels["StorageDhw"]
-            base["dhwStorage"]=labels["StorageDhw"]
-        if "dhwBus" in labels and (mergedLinks or optimType == 'indiv'):
-            base["domesticHotWaterBus"]=labels["dhwBus"]
-            base["domesticHotWater"]=labels["dhwBus"]
-            base["dhwDemandBus"]=labels["dhwBus"]
-        if "DemandEl" in labels:base["electricityDemand"]=labels["DemandEl"]
-        if "DemandMob" in labels:base["emobilityDemand"]=labels["DemandMob"]
-        if "DemandSh" in labels:base["spaceHeatingDemand"]=labels["DemandSh"]
-        if "DemandDhw" in labels:base["domesticHotWaterDemand"]=labels["DemandDhw"]
-        if "ElectricRod" in labels:base["ElectricRod"]=labels["ElectricRod"]
-
-    labelDict = {}
-
-    for b in range(1,numBuildings+1):
-        for key in base:
-            if ("grid" in base[key] or "Grid" in base[key]) and mergedLinks:    # combine grid bus for merged links
-                value = base[key]
-                key = key + "__Building" + str(b)
-            elif mergedLinks and (all(v not in key for v in ["electricityLink", "shLink", "dhwLink", "electricityInBus", "domesticHotWater", "spaceHeatingBus", "domesticHotWaterBus", "dhwDemandBus", "spaceHeating", "shDemandBus"])
-            or any(v in key for v in ["spaceHeatingDemand", 'domesticHotWaterDemand'])):            # append suffix for all values except links
-                value = base[key]+"_B"+str(b)
-                key = key+"__Building"+str(b)
-            elif ((not mergedLinks and optimType == "group") or optimType == "indiv") and all(v not in key for v in ["electricityLink", "shLink", "dhwLink"]):
-                value = base[key] + "_B" + str(b)
-                key = key + "__Building" + str(b)
-            else:
-                value = base[key]
-                if mergedLinks and any(v in key for v in ["electricityInBus", "domesticHotWater", "spaceHeatingBus", "domesticHotWaterBus", "dhwDemandBus", "spaceHeating", "shDemandBus"]):            # append suffix for all values except links
-                    key = key+"__Building"+str(b)
-            labelDict[key] = value
-
-    return labelDict
-
-def positionDictGenerator(labels, optimType, mergedLinks):
-    labelsList = ['natGas', 'grid', 'pv', 'CHP', 'gasBoiler', 'localEl', 'prodEl', 'elLink', 'shLink', 'dhwLink', 'Bat',
-                  'usedEl', 'HP', 'GWHP', 'ElectricRod', 'solar', 'exSolar', 'prodSH', 'shStor', 'dhwStor', 'exEl',
-                  'Q_el', 'Q_mob', 'Q_sh', 'Q_dhw', 'exSh', 'dhwBus', 'shBus']
-    if not mergedLinks and optimType == 'group':
-        labelsList.extend(['usedEl', 'usedSH', 'prodDHW'])
-    if labels != 'default':
-        if "elBus" in labels and ((mergedLinks and optimType=='group') or optimType=='indiv'): labelsList[7] = labels["elBus"]
-        if "elBus" in labels and not mergedLinks and optimType == 'group': labelsList[7] = labels["elBus"] + " Link"
-        if "shBus" in labels and ((mergedLinks and optimType=='group') or optimType=='indiv'): labelsList[8] = labels["shBus"]
-        if "shBus" in labels and not mergedLinks and optimType == 'group': labelsList[8] = labels["shBus"] + " Link"
-        if "dhwBus" in labels and ((mergedLinks and optimType=='group') or optimType=='indiv'): labelsList[9] = labels["dhwBus"]
-        if "dhwBus" in labels and not mergedLinks and optimType == 'group': labelsList[9] = labels["dhwBus"] + " Link"
-        if "naturalGas" in labels: labelsList[0] = labels["naturalGas"]
-        if "grid" in labels: labelsList[1] = labels["grid"]
-        if "pv" in labels: labelsList[2]=labels["pv"]
-        if "gasBoiler" in labels: labelsList[4]=labels["gasBoiler"]
-        if "CHP" in labels:labelsList[3]=labels["CHP"]
-        if "prodEl" in labels: labelsList[6] = labels["prodEl"]
-        if "localEl" in labels: labelsList[5]=labels["localEl"]
-        if "StorageEl" in labels:labelsList[10]=labels["StorageEl"]
-        if "excessEl" in labels:labelsList[20]=labels["excessEl"]
-        if "excessSh" in labels:labelsList[25]=labels["excessSh"]
-        if "elBus" in labels:labelsList[11]=labels["elBus"]
-        if "HP" in labels:labelsList[12]=labels["HP"]
-        if "GWHP" in labels:labelsList[13]=labels["GWHP"]
-        if "solarCollector" in labels:labelsList[15]=labels["solarCollector"]
-        if "excessSolarCollector" in labels: labelsList[16]=labels["excessSolarCollector"]
-        if "prodSH" in labels:labelsList[17]=labels["prodSH"]
-        if "shBus" in labels:labelsList[27] = labels["shBus"]
-        if "StorageSh" in labels:labelsList[18]=labels["StorageSh"]
-        if "StorageDhw" in labels:labelsList[19]=labels["StorageDhw"]
-        if "dhwBus" in labels:labelsList[26]=labels["dhwBus"]
-        if "DemandEl" in labels:labelsList[21]=labels["DemandEl"]
-        if "DemandMob" in labels:labelsList[22]=labels["DemandMob"]
-        if "DemandSh" in labels:labelsList[23]=labels["DemandSh"]
-        if "DemandDhw" in labels:labelsList[24]=labels["DemandDhw"]
-        if "ElectricRod" in labels:labelsList[14]=labels["ElectricRod"]
-    positionDict = {
-        labelsList[0]: [0.001, 0.65],  # X and Y positions should never be set to 0 or 1
-        labelsList[1]: [0.001, 0.15],
-        labelsList[2]: [0.001, 0.3],
-        labelsList[3]: [0.1, 0.7],
-        labelsList[4]: [0.1, 0.7],
-        labelsList[5]: [0.15, 0.3],
-        labelsList[6]: [0.3, 0.3],
-        labelsList[10]: [0.2, 0.25],
-        labelsList[11]: [0.4, 0.2],
-        labelsList[12]: [0.55, 0.5],
-        labelsList[13]: [0.55, 0.2],
-        labelsList[13]+'35': [0.55, 0.2],
-        labelsList[13]+'60': [0.55, 0.5],
-        labelsList[14]: [0.6, 0.4],
-        labelsList[15]: [0.6, 0.85],
-        labelsList[16]: [0.7, 0.95],
-        labelsList[17]: [0.65, 0.58],
-        # "usedSH":	[0.75, 0.58],
-        labelsList[18]: [0.68, 0.37],
-        labelsList[19]: [0.65, 0.85],
-        # "usedDHW": [0.8, 0.85],
-        # "prodDHW": [0.75, 0.85],
-        labelsList[20]: [0.999, 0.25],
-        labelsList[21]: [0.999, 0.15],
-        labelsList[22]: [0.999, 0.4],
-        labelsList[23]: [0.999, 0.6],
-        labelsList[24]: [0.999, 0.85],
-        labelsList[25]: [0.999, 0.7],
-        labelsList[26]: [0.8, 0.85],
-        labelsList[27]: [0.8, 0.6]
-    }
-
-    if mergedLinks and optimType=='group':
-        positionDict[labelsList[7]]= [0.4, 0.35]
-        positionDict[labelsList[8]]= [0.8, 0.35]
-        positionDict[labelsList[9]]= [0.8, 0.5]
-    elif optimType!='indiv':
-        #links
-        positionDict[labelsList[7]] = [0.45, 0.35]
-        positionDict[labelsList[8]] = [0.77, 0.35]
-        positionDict[labelsList[9]] = [0.85, 0.5]
-        # prod DHW, used SH and used El
-        if labels != 'default':
-            labelsList[28] = labels["usedEl"]
-            labelsList[29] = labels["usedSH"]
-            labelsList[30] = labels["prodDHW"]
-        positionDict[labelsList[28]] = [0.52, 0.35]
-        positionDict[labelsList[29]] = [0.75, 0.35]
-        positionDict[labelsList[30]] = [0.7, 0.5]
-
-    return positionDict
-
-labelDict = {
-    "electricityLink": "elLink",
-    "electricityLink1_2": "elLink",
-    "electricityLink1_3": "elLink",
-    "electricityLink1_4": "elLink",
-    "electricityLink1_5": "elLink",
-    "electricityLink1_6": "elLink",
-    "electricityLink2_3": "elLink",
-    "electricityLink2_4": "elLink",
-    "electricityLink2_5": "elLink",
-    "electricityLink2_6": "elLink",
-    "electricityLink3_4": "elLink",
-    "electricityLink3_5": "elLink",
-    "electricityLink3_6": "elLink",
-    "electricityLink4_5": "elLink",
-    "electricityLink4_6": "elLink",
-    "electricityLink5_6": "elLink",
-    "electricityLink2_1": "elLink",
-    "electricityLink3_2": "elLink",
-    "electricityLink3_1": "elLink",
-    "electricityLink4_3": "elLink",
-    "electricityLink4_2": "elLink",
-    "electricityLink4_1": "elLink",
-    "electricityLink5_4": "elLink",
-    "electricityLink5_3": "elLink",
-    "electricityLink5_2": "elLink",
-    "electricityLink5_1": "elLink",
-    "electricityLink6_5": "elLink",
-    "electricityLink6_4": "elLink",
-    "electricityLink6_3": "elLink",
-    "electricityLink6_2": "elLink",
-    "electricityLink6_1": "elLink",
-
-    "shLink1_2": "shLink",
-    "shLink1_3": "shLink",
-    "shLink1_4": "shLink",
-    "shLink1_5": "shLink",
-    "shLink1_6": "shLink",
-    "shLink2_3": "shLink",
-    "shLink2_4": "shLink",
-    "shLink2_5": "shLink",
-    "shLink2_6": "shLink",
-    "shLink3_4": "shLink",
-    "shLink3_5": "shLink",
-    "shLink3_6": "shLink",
-    "shLink4_5": "shLink",
-    "shLink4_6": "shLink",
-    "shLink5_6": "shLink",
-    "shLink2_1": "shLink",
-    "shLink3_2": "shLink",
-    "shLink3_1": "shLink",
-    "shLink4_3": "shLink",
-    "shLink4_2": "shLink",
-    "shLink4_1": "shLink",
-    "shLink5_1": "shLink",
-    "shLink5_2": "shLink",
-    "shLink5_3": "shLink",
-    "shLink5_4": "shLink",
-    "shLink6_5": "shLink",
-    "shLink6_4": "shLink",
-    "shLink6_3": "shLink",
-    "shLink6_2": "shLink",
-    "shLink6_1": "shLink",
-
-    "dhwLink1_2": "dhwLink",
-    "dhwLink1_3": "dhwLink",
-    "dhwLink1_4": "dhwLink",
-    "dhwLink1_5": "dhwLink",
-    "dhwLink1_6": "dhwLink",
-    "dhwLink2_3": "dhwLink",
-    "dhwLink2_4": "dhwLink",
-    "dhwLink2_5": "dhwLink",
-    "dhwLink2_6": "dhwLink",
-    "dhwLink3_4": "dhwLink",
-    "dhwLink3_5": "dhwLink",
-    "dhwLink3_6": "dhwLink",
-    "dhwLink4_5": "dhwLink",
-    "dhwLink4_6": "dhwLink",
-    "dhwLink5_6": "dhwLink",
-    "dhwLink2_1": "dhwLink",
-    "dhwLink3_2": "dhwLink",
-    "dhwLink3_1": "dhwLink",
-    "dhwLink4_3": "dhwLink",
-    "dhwLink4_2": "dhwLink",
-    "dhwLink4_1": "dhwLink",
-    "dhwLink5_1": "dhwLink",
-    "dhwLink5_2": "dhwLink",
-    "dhwLink5_3": "dhwLink",
-    "dhwLink5_4": "dhwLink",
-    "dhwLink6_5": "dhwLink",
-    "dhwLink6_4": "dhwLink",
-    "dhwLink6_3": "dhwLink",
-    "dhwLink6_2": "dhwLink",
-    "dhwLink6_1": "dhwLink",
-
-    "naturalGasResource__Building1": "natGas_B1",
-    "naturalGasBus__Building1": "natGas_B1",
-    "gridBus__Building1": "grid_B1",
-    "pv__Building1": "pv_B1",
-    "electricityResource__Building1":"grid_B1",
-    "gridElectricity__Building1": "grid_B1",
-    "GasBoiler__Building1":"gasBoiler_B1",
-    "CHP_SH__Building1": "CHP_B1",
-    "CHP_DHW__Building1": "CHP_B1",
-    "CHP__Building1": "CHP_B1",
-    "electricityBus__Building1": "prodEl_B1",
-    "electricityProdBus__Building1":"localEl_B1", #localEl is before the battery, prodEl after the battery but before the elLink
-    "producedElectricity__Building1": "prodEl_B1",
-    "electricitySource__Building1": "localEl_B1",
-    "electricalStorage__Building1": "Bat_B1",
-    "excesselectricityBus__Building1": "exEl_B1",
-    "excessshDemandBus__Building1": "exSh_B1",
-    "electricityInBus__Building1": "usedEl_B1",
-    "HP_SH__Building1": "HP_B1",
-    "HP_DHW__Building1": "HP_B1",
-    "HP__Building1": "HP_B1",
-    "GWHP_SH__Building1": "GWHP_B1",
-    "GWHP_DHW__Building1": "GWHP_B1",
-    "GWHP__Building1": "GWHP_B1",
-    "solarCollector__Building1": "solar_B1",
-    "solarConnectBus__Building1": "solar_B1",
-    'heat_solarCollector__Building1': "solar_B1",
-    'excess_solarheat__Building1':"exSolar_B1",
-    'shSource__Building1'	: "prodSH_B1",
-    'shSourceBus__Building1': "prodSH_B1",
-    "spaceHeatingBus__Building1": "shBus_B1",
-    "spaceHeating__Building1": "shBus_B1",
-    "shStorage__Building1": "shStor_B1",
-    "shDemandBus__Building1": "shBus_B1",
-    "dhwStorageBus__Building1": "dhwStor_B1",
-    "dhwStorage__Building1": "dhwStor_B1",
-    "domesticHotWaterBus__Building1": "dhwBus_B1",
-    'domesticHotWater__Building1': "dhwBus_B1",
-    "dhwDemandBus__Building1": "dhwBus_B1",
-    "electricityDemand__Building1": "Q_el_B1",
-    "emobilityDemand__Building1": "Q_mob_B1",
-    "spaceHeatingDemand__Building1": "Q_sh_B1",
-    "domesticHotWaterDemand__Building1": "Q_dhw_B1",
-    "excessshSourceBus__Building1": "exSh_B1",
-    "ElectricRod__Building1": "ElectricRod_B1",
-
-    "naturalGasResource__Building2": "natGas_B2",
-    "naturalGasBus__Building2": "natGas_B2",
-    "electricityResource__Building2": "grid_B2",
-    "gridBus__Building2": "grid_B2",
-    "pv__Building2": "pv_B2",
-    "gridElectricity__Building2": "grid_B2",
-    "GasBoiler__Building2":"gasBoiler_B2",
-    "CHP_SH__Building2": "CHP_B2",
-    "CHP_DHW__Building2": "CHP_B2",
-    "CHP__Building2": "CHP_B2",
-    "electricityBus__Building2": "prodEl_B2",
-    "electricityProdBus__Building2": "localEl_B2",
-    "producedElectricity__Building2": "prodEl_B2",
-    "electricitySource__Building2": "localEl_B2",
-    "electricalStorage__Building2": "Bat_B2",
-    "excesselectricityBus__Building2": "exEl_B2",
-    "excessshDemandBus__Building2": "exSh_B2",
-    "electricityInBus__Building2": "usedEl_B2",
-    "HP_SH__Building2": "HP_B2",
-    "HP_DHW__Building2": "HP_B2",
-    "HP__Building2": "HP_B2",
-    "GWHP_SH__Building2": "GWHP_B2",
-    "GWHP_DHW__Building2": "GWHP_B2",
-    "GWHP__Building2": "GWHP_B2",
-    "solarCollector__Building2": "solar_B2",
-    "solarConnectBus__Building2": "solar_B2",
-    'heat_solarCollector__Building2': "solar_B2",
-    'excess_solarheat__Building2': "exSolar_B2",
-    'shSource__Building2'	: "prodSH_B2",
-    'shSourceBus__Building2': "prodSH_B2",
-    "spaceHeatingBus__Building2": "shBus_B2",
-    "spaceHeating__Building2": "shBus_B2",
-    "shStorage__Building2": "shStor_B2",
-    "shDemandBus__Building2": "shBus_B2",
-    "dhwStorageBus__Building2": "dhwStor_B2",
-    "dhwStorage__Building2": "dhwStor_B2",
-    "domesticHotWaterBus__Building2": "dhwBus_B2",
-    'domesticHotWater__Building2': "dhwBus_B2",
-    "dhwDemandBus__Building2": "dhwBus_B2",
-    "electricityDemand__Building2": "Q_el_B2",
-    "emobilityDemand__Building2": "Q_mob_B2",
-    "spaceHeatingDemand__Building2":        "Q_sh_B2",
-    "domesticHotWaterDemand__Building2": "Q_dhw_B2",
-    "excessshSourceBus__Building2": "exSh_B2",
-    "ElectricRod__Building2": "ElectricRod_B2",
-
-    "naturalGasResource__Building3": "natGas_B3",
-    "naturalGasBus__Building3": "natGas_B3",
-    "electricityResource__Building3": "grid_B3",
-    "gridBus__Building3": "grid_B3",
-    "GasBoiler__Building3": "gasBoiler_B3",
-    "pv__Building3": "pv_B3",
-    "gridElectricity__Building3": "grid_B3",
-    "CHP_SH__Building3": "CHP_B3",
-    "CHP_DHW__Building3": "CHP_B3",
-    "CHP__Building3": "CHP_B3",
-    "electricityBus__Building3": "prodEl_B3",
-    "electricityProdBus__Building3": "localEl_B3",
-    "producedElectricity__Building3": "prodEl_B3",
-    "electricitySource__Building3": "localEl_B3",
-    "electricalStorage__Building3": "Bat_B3",
-    "excesselectricityBus__Building3": "exEl_B3",
-    "excessshDemandBus__Building3": "exSh_B3",
-    "electricityInBus__Building3": "usedEl_B3",
-    "HP_SH__Building3": "HP_B3",
-    "HP_DHW__Building3": "HP_B3",
-    "HP__Building3": "HP_B3",
-    "GWHP_SH__Building3": "GWHP_B3",
-    "GWHP_DHW__Building3": "GWHP_B3",
-    "GWHP__Building3": "GWHP_B3",
-    "solarCollector__Building3": "solar_B3",
-    "solarConnectBus__Building3": "solar_B3",
-    'heat_solarCollector__Building3': "solar_B3",
-    'excess_solarheat__Building3': "exSolar_B3",
-    'shSource__Building3': "prodSH_B3",
-    'shSourceBus__Building3': "prodSH_B3",
-    "spaceHeatingBus__Building3": "shBus_B3",
-    "spaceHeating__Building3": "shBus_B3",
-    "shStorage__Building3": "shStor_B3",
-    "shDemandBus__Building3": "shBus_B3",
-    "dhwStorageBus__Building3": "dhwStor_B3",
-    "dhwStorage__Building3": "dhwStor_B3",
-    "domesticHotWaterBus__Building3": "dhwBus_B3",
-    'domesticHotWater__Building3': "dhwBus_B3",
-    "dhwDemandBus__Building3": "dhwBus_B3",
-    "electricityDemand__Building3": "Q_el_B3",
-    "emobilityDemand__Building3": "Q_mob_B3",
-    "spaceHeatingDemand__Building3":        "Q_sh_B3",
-    "domesticHotWaterDemand__Building3": "Q_dhw_B3",
-    "excessshSourceBus__Building3": "exSh_B3",
-    "ElectricRod__Building3": "ElectricRod_B3",
-
-    "naturalGasResource__Building4": "natGas_B4",
-    "naturalGasBus__Building4": "natGas_B4",
-    "electricityResource__Building4": "grid_B4",
-    "gridBus__Building4": "grid_B4",
-    "pv__Building4": "pv_B4",
-    "gridElectricity__Building4": "grid_B4",
-    "GasBoiler__Building4":"gasBoiler_B4",
-    "CHP_SH__Building4": "CHP_B4",
-    "CHP_DHW__Building4": "CHP_B4",
-    "CHP__Building4": "CHP_B4",
-    "electricityBus__Building4": "prodEl_B4",
-    "electricityProdBus__Building4": "localEl_B4",
-    "producedElectricity__Building4": "prodEl_B4",
-    "electricitySource__Building4": "localEl_B4",
-    "electricalStorage__Building4": "Bat_B4",
-    "excesselectricityBus__Building4": "exEl_B4",
-    "excessshDemandBus__Building4": "exSh_B4",
-    "electricityInBus__Building4": "usedEl_B4",
-    "HP_SH__Building4": "HP_B4",
-    "HP_DHW__Building4": "HP_B4",
-    "HP__Building4": "HP_B4",
-    "GWHP_SH__Building4": "GWHP_B4",
-    "GWHP_DHW__Building4": "GWHP_B4",
-    "GWHP__Building4": "GWHP_B4",
-    "solarCollector__Building4": "solar_B4",
-    "solarConnectBus__Building4": "solar_B4",
-    'heat_solarCollector__Building4': "solar_B4",
-    'excess_solarheat__Building4': "exSolar_B4",
-    'shSource__Building4': "prodSH_B4",
-    'shSourceBus__Building4': "prodSH_B4",
-    "spaceHeatingBus__Building4": "shBus_B4",
-    "spaceHeating__Building4": "shBus_B4",
-    "shStorage__Building4": "shStor_B4",
-    "shDemandBus__Building4": "shBus_B4",
-    "dhwStorageBus__Building4": "dhwStor_B4",
-    "dhwStorage__Building4": "dhwStor_B4",
-    "domesticHotWaterBus__Building4": "dhwBus_B4",
-    'domesticHotWater__Building4': "dhwBus_B4",
-    "dhwDemandBus__Building4": "dhwBus_B4",
-    "electricityDemand__Building4": "Q_el_B4",
-    "emobilityDemand__Building4": "Q_mob_B4",
-    "spaceHeatingDemand__Building4":        "Q_sh_B4",
-    "domesticHotWaterDemand__Building4": "Q_dhw_B4",
-    "excessshSourceBus__Building4": "exSh_B4",
-    "ElectricRod__Building4": "ElectricRod_B4",
-
-    "naturalGasResource__Building5": "natGas_B5",
-    "naturalGasBus__Building5": "natGas_B5",
-    "electricityResource__Building5": "grid_B5",
-    "gridBus__Building5": "grid_B5",
-    "pv__Building5": "pv_B5",
-    "gridElectricity__Building5": "grid_B5",
-    "GasBoiler__Building5":"gasBoiler_B5",
-    "CHP_SH__Building5": "CHP_B5",
-    "CHP_DHW__Building5": "CHP_B5",
-    "CHP__Building5": "CHP_B5",
-    "electricityBus__Building5": "prodEl_B5",
-    "electricityProdBus__Building5": "localEl_B5",
-    "producedElectricity__Building5": "prodEl_B5",
-    "electricitySource__Building5": "prodEl_B5",
-    "electricalStorage__Building5": "Bat_B5",
-    "excesselectricityBus__Building5": "exEl_B5",
-    "excessshDemandBus__Building5": "exSh_B5",
-    "excessshSourceBus__Building5": "exSh_B5",
-    "electricityInBus__Building5": "usedEl_B5",
-    "HP_SH__Building5": "HP_B5",
-    "HP_DHW__Building5": "HP_B5",
-    "HP__Building5": "HP_B5",
-    "GWHP_SH__Building5": "GWHP_B5",
-    "GWHP_DHW__Building5": "GWHP_B5",
-    "GWHP__Building5": "GWHP_B5",
-    "solarCollector__Building5": "solar_B5",
-    "solarConnectBus__Building5": "solar_B5",
-    'heat_solarCollector__Building5': "solar_B5",
-    'excess_solarheat__Building5': "exSolar_B5",
-    'shSource__Building5'	: "prodSH_B5",
-    'shSourceBus__Building5': "prodSH_B5",
-    "spaceHeatingBus__Building5": "usedSH_B5",
-    "spaceHeating__Building5": "Q_sh_B5",
-    "shStorage__Building5": "shStor_B5",
-    "shDemandBus__Building5": "Q_sh_B5",
-    "dhwStorageBus__Building5": "dhwStor_B5",
-    "dhwStorage__Building5": "dhwStor_B5",
-    "domesticHotWaterBus__Building5": "prodDHW_B5",
-    'domesticHotWater__Building5': "usedDHW_B5",
-    "dhwDemandBus__Building5": "Q_dhw_B5",
-    "electricityDemand__Building5": "Q_el_B5",
-    "spaceHeatingDemand__Building5":        "Q_sh_B5",
-    "domesticHotWaterDemand__Building5": "Q_dhw_B5",
-    "ElectricRod__Building5": "ElectricRod_B5",
-
-    "naturalGasResource__Building6": "natGas_B6",
-    "naturalGasBus__Building6": "natGas_B6",
-    "electricityResource__Building6": "grid_B6",
-    "gridBus__Building6": "grid_B6",
-    "pv__Building6": "pv_B6",
-    "gridElectricity__Building6": "grid_B6",
-    "GasBoiler__Building6":"gasBoiler_B6",
-    "CHP_SH__Building6": "CHP_B6",
-    "CHP_DHW__Building6": "CHP_B6",
-    "CHP__Building6": "CHP_B6",
-    "electricityBus__Building6": "prodEl_B6",
-    "electricityProdBus__Building6": "localEl_B6",
-    "producedElectricity__Building6": "prodEl_B6",
-    "electricitySource__Building6": "prodEl_B6",
-    "electricalStorage__Building6": "Bat_B6",
-    "excesselectricityBus__Building6": "exEl_B6",
-    "excessshDemandBus__Building6": "exSh_B6",
-    "excessshSourceBus__Building6": "exSh_B6",
-    "electricityInBus__Building6": "usedEl_B6",
-    "HP_SH__Building6": "HP_B6",
-    "HP_DHW__Building6": "HP_B6",
-    "HP__Building6": "HP_B6",
-    "GWHP_SH__Building6": "GWHP_B6",
-    "GWHP_DHW__Building6": "GWHP_B6",
-    "GWHP__Building6": "GWHP_B6",
-    "solarCollector__Building6": "solar_B6",
-    "solarConnectBus__Building6": "solar_B6",
-    'heat_solarCollector__Building6': "solar_B6",
-    'excess_solarheat__Building6': "exSolar_B6",
-    'shSource__Building6'	: "prodSH_B6",
-    'shSourceBus__Building6': "prodSH_B6",
-    "spaceHeatingBus__Building6": "usedSH_B6",
-    "spaceHeating__Building6": "Q_sh_B6",
-    "shStorage__Building6": "shStor_B6",
-    "shDemandBus__Building6": "Q_sh_B6",
-    "dhwStorageBus__Building6": "dhwStor_B6",
-    "dhwStorage__Building6": "dhwStor_B6",
-    "domesticHotWaterBus__Building6": "prodDHW_B6",
-    'domesticHotWater__Building6': "usedDHW_B6",
-    "dhwDemandBus__Building6": "Q_dhw_B6",
-    "electricityDemand__Building6": "Q_el_B6",
-    "spaceHeatingDemand__Building6":        "Q_sh_B6",
-    "domesticHotWaterDemand__Building6": "Q_dhw_B6",
-    "ElectricRod__Building6": "ElectricRod_B6",
-}
-
-labelPositionDict={
-    "natGas":	[0.001, 0.65], #X and Y positions should never be set to 0 or 1
-    "grid":	[0.001, 0.15],
-    "pv":   [0.001, 0.3],
-    "CHP":	[0.1, 0.7],
-    "gasBoiler": [0.1, 0.7],
-    "localEl":	[0.15, 0.3],
-    "prodEl":[0.3,0.3],
-    "elLink":	[0.4, 0.35],
-    "shLink": [0.8, 0.35],
-    "dhwLink": [0.8, 0.5],
-	"Bat":	[0.2, 0.25],
-    "usedEl":	[0.4, 0.2],
-    "HP":	[0.55, 0.5],
-    "GWHP":	[0.55, 0.2],
-    "ElectricRod": [0.6, 0.4],
-    "solar":	[0.6, 0.85],
-    "exSolar": [0.7, 0.95],
-    "prodSH": [0.65, 0.58],
-    #"usedSH":	[0.75, 0.58],
-    "shStor":	[0.68, 0.37],
-    "dhwStor":	[0.65, 0.85],
-    #"usedDHW": [0.8, 0.85],
-    #"prodDHW": [0.75, 0.85],
-    "exEl": [0.999, 0.25],
-    "Q_el":	[0.999, 0.15],
-    "Q_mob":[0.999, 0.4],
-    "Q_sh":	[0.999, 0.6],
-    "Q_dhw":[0.999, 0.85],
-    "exSh": [0.999, 0.7],
-    "dhwBus":[0.8, 0.85],
-    "shBus": [0.8, 0.6]
-	}
-
-fullPositionDict={
-        "naturalGas":	[0.001, 0.75],
-        "gridBus":	[0.001, 0.2],
-        "pv":   [0.001, 0.3],
-        "gridElect":	[0.1, 0.05],
-        "electricityProdBus": [0.1, 0.2],
-        "CHP":	[0.1, 0.6],
-        "GasBoiler": [0.1, 0.7],
-        "electricitySource": [0.15, 0.2],
-        "electricityBus":	[0.2, 0.2],
-        "producedElectricity":	[0.3, 0.25],
-        "electricityLink":	[0.3, 0.35],
-        "electricalStorage":	[0.3, 0.25],
-        "excesselect":	[0.5, 0.05],
-        "electricityInBus":	[0.5, 0.2],
-        "HP":	[0.6, 0.5],
-        "GWHP":	[0.6, 0.2],
-        "ElectricRod": [0.6, 0.4],
-        "heat_solarCollector": [0.4, 0.85],
-        "solarConnect": [0.5, 0.85],
-        "solarCollector_":	[0.6, 0.85],
-        "excess_solarheat":[0.6,0.85],
-        'shSource_': [0.63, 0.58],
-        'shLink': [0.64, 0.58],
-        'shSourceBus': [0.66, 0.58],
-        "spaceHeatingBus":	[0.7, 0.58],
-        "spaceHeating_":	[0.8, 0.6],
-        "shStorage":	[0.8, 0.37],
-        "shDemandBus":	[0.9, 0.6],
-        "dhwStorageBus":	[0.7, 0.9],
-        "dhwStorage_":	[0.8, 0.9],
-        "domesticHotWater_":	[0.92, 0.9],
-        "domesticHotWaterBus":	[0.9, 0.9],
-        "dhwDemandBus":	[0.95, 0.9],
-        "electricityDemand":	[0.999, 0.1],
-        "spaceHeatingDemand_":	[0.999, 0.6],
-        "domesticHotWaterDemand":	[0.999, 0.9]
+def labelDictGenerator(numBuildings, labels, optimType, mergedLinks):
+    base = {"electricityLink":"elLink", "shLink":"shLink", "dhwLink":"dhwLink", "naturalGasResource":"natGas", "naturalGasBus":"natGas", "gridBus":"grid", "pv":"pv", "electricityResource":"grid", "gridElectricity":"grid", "GasBoiler":"gasBoiler",
+    "CHP":"CHP", "electricityBus":"prodEl", "electricityProdBus":"localEl", "producedElectricity":"prodEl", "electricitySource":"localEl", "electricalStorage":"Bat", "excesselectricityBus":"exEl",
+    "excessshDemandBus":"exSh", "electricityInBus":"usedEl", "HP":"HP", "GWHP":"GWHP", "GWHP35":"GWHP35", "GWHP60":"GWHP60", "solarCollector":"solar", "solarConnectBus":"solar","heat_solarCollector":"solar", "excess_solarheat":"exSolar",
+    "shSource":"prodSH","shSourceBus":"prodSH", "spaceHeatingBus":"shBus", "spaceHeating":"shBus", "shStorage":"shStor", "shDemandBus":"shBus", "dhwStorageBus":"dhwStor", "dhwStorage":"dhwStor", "domesticHotWaterBus":"dhwBus",
+    "domesticHotWater":"dhwBus", "dhwDemandBus":"dhwBus", "electricityDemand":"Q_el", "emobilityDemand":"Q_mob", "spaceHeatingDemand":"Q_sh", "domesticHotWaterDemand":"Q_dhw", "excessshSourceBus":"exSh",
+    "ElectricRod":"ElectricRod"}
+    if not mergedLinks and optimType == 'group':
+        base['electricityInBus'] = "usedEl"
+        base['spaceHeatingBus'] = "usedSH"
+        base['domesticHotWaterBus'] = "prodDHW"
+        if labels != 'default':
+            base["electricityInBus"] = labels["usedEl"]
+            base["spaceHeatingBus"] = labels["usedSH"]
+            base["spaceHeating"] = labels["shBus"]
+            base["shDemandBus"] = labels["shBus"]
+            base["domesticHotWaterBus"] = labels["prodDHW"]
+            base['domesticHotWater'] = labels["dhwBus"]
+            base['dhwDemandBus'] = labels["dhwBus"]
+    if labels != 'default':
+        if "elBus" in labels and ((mergedLinks and optimType=='group') or optimType=='indiv'): base["electricityLink"] = labels["elBus"]
+        if "elBus" in labels and not mergedLinks and optimType=='group': base["electricityLink"] = labels["elBus"] + " Link"
+        if "shBus" in labels and ((mergedLinks and optimType=='group') or optimType=='indiv'): base["shLink"] = labels["shBus"]
+        if "shBus" in labels and not mergedLinks and optimType=='group': base["shLink"] = labels["shBus"] + " Link"
+        if "dhwBus" in labels and ((mergedLinks and optimType=='group') or optimType=='indiv'): base["dhwLink"] = labels["dhwBus"]
+        if "dhwBus" in labels and not mergedLinks and optimType=='group': base["dhwLink"] = labels["dhwBus"] + " Link"
+        if "naturalGas" in labels:
+            base["naturalGasResource"] = labels["naturalGas"]
+            base["naturalGasBus"] = labels["naturalGas"]
+        if "grid" in labels:
+            base["gridBus"] = labels["grid"]
+            base["electricityResource"] = labels["grid"]
+            base["gridElectricity"] = labels["grid"]
+        if "pv" in labels: base["pv"]=labels["pv"]
+        if "gasBoiler" in labels: base["GasBoiler"]=labels["gasBoiler"]
+        if "CHP" in labels:base["CHP"]=labels["CHP"]
+        if "prodEl" in labels:
+            base["electricityBus"]=labels["prodEl"]
+            base["producedElectricity"] = labels["prodEl"]
+        if "localEl" in labels:
+            base["electricityProdBus"]=labels["localEl"]
+            base["electricitySource"]=labels["localEl"]
+        if "StorageEl" in labels:base["electricalStorage"]=labels["StorageEl"]
+        if "excessEl" in labels:base["excesselectricityBus"]=labels["excessEl"]
+        if "excessSh" in labels:
+            base["excessshDemandBus"]=labels["excessSh"]
+            base["excessshSourceBus"]=labels["excessSh"]
+        if "elBus" in labels and (mergedLinks or optimType == 'indiv'):base["electricityInBus"]=labels["elBus"]
+        if "HP" in labels:base["HP"]=labels["HP"]
+        if "GWHP" in labels:
+            base["GWHP"]=labels["GWHP"]
+            base["GWHP35"]=labels["GWHP"]+'35'# for splitted GSHP
+            base["GWHP60"] = labels["GWHP"]+'60'
+        if "solarCollector" in labels:
+            base["solarCollector"]=labels["solarCollector"]
+            base["solarConnectBus"]=labels["solarCollector"]
+            base["heat_solarCollector"]=labels["solarCollector"]
+        if "excessSolarCollector" in labels: base["excess_solarheat"]=labels["excessSolarCollector"]
+        if "prodSH" in labels:
+            base["shSource"]=labels["prodSH"]
+            base["shSourceBus"]=labels["prodSH"]
+        if "shBus" in labels and (mergedLinks or optimType == 'indiv'):
+            base["spaceHeatingBus"]=labels["shBus"]
+            base["spaceHeating"]=labels["shBus"]
+            base["shDemandBus"] = labels["shBus"]
+        if "StorageSh" in labels:base["shStorage"]=labels["StorageSh"]
+        if "StorageDhw" in labels:
+            base["dhwStorageBus"]=labels["StorageDhw"]
+            base["dhwStorage"]=labels["StorageDhw"]
+        if "dhwBus" in labels and (mergedLinks or optimType == 'indiv'):
+            base["domesticHotWaterBus"]=labels["dhwBus"]
+            base["domesticHotWater"]=labels["dhwBus"]
+            base["dhwDemandBus"]=labels["dhwBus"]
+        if "DemandEl" in labels:base["electricityDemand"]=labels["DemandEl"]
+        if "DemandMob" in labels:base["emobilityDemand"]=labels["DemandMob"]
+        if "DemandSh" in labels:base["spaceHeatingDemand"]=labels["DemandSh"]
+        if "DemandDhw" in labels:base["domesticHotWaterDemand"]=labels["DemandDhw"]
+        if "ElectricRod" in labels:base["ElectricRod"]=labels["ElectricRod"]
+
+    labelDict = {}
+
+    for b in range(1,numBuildings+1):
+        for key in base:
+            if ("grid" in base[key] or "Grid" in base[key]) and mergedLinks:    # combine grid bus for merged links
+                value = base[key]
+                key = key + "__Building" + str(b)
+            elif mergedLinks and (all(v not in key for v in ["electricityLink", "shLink", "dhwLink", "electricityInBus", "domesticHotWater", "spaceHeatingBus", "domesticHotWaterBus", "dhwDemandBus", "spaceHeating", "shDemandBus"])
+            or any(v in key for v in ["spaceHeatingDemand", 'domesticHotWaterDemand'])):            # append suffix for all values except links
+                value = base[key]+"_B"+str(b)
+                key = key+"__Building"+str(b)
+            elif ((not mergedLinks and optimType == "group") or optimType == "indiv") and all(v not in key for v in ["electricityLink", "shLink", "dhwLink"]):
+                value = base[key] + "_B" + str(b)
+                key = key + "__Building" + str(b)
+            else:
+                value = base[key]
+                if mergedLinks and any(v in key for v in ["electricityInBus", "domesticHotWater", "spaceHeatingBus", "domesticHotWaterBus", "dhwDemandBus", "spaceHeating", "shDemandBus"]):            # append suffix for all values except links
+                    key = key+"__Building"+str(b)
+            labelDict[key] = value
+
+    return labelDict
+
+def positionDictGenerator(labels, optimType, mergedLinks):
+    labelsList = ['natGas', 'grid', 'pv', 'CHP', 'gasBoiler', 'localEl', 'prodEl', 'elLink', 'shLink', 'dhwLink', 'Bat',
+                  'usedEl', 'HP', 'GWHP', 'ElectricRod', 'solar', 'exSolar', 'prodSH', 'shStor', 'dhwStor', 'exEl',
+                  'Q_el', 'Q_mob', 'Q_sh', 'Q_dhw', 'exSh', 'dhwBus', 'shBus']
+    if not mergedLinks and optimType == 'group':
+        labelsList.extend(['usedEl', 'usedSH', 'prodDHW'])
+    if labels != 'default':
+        if "elBus" in labels and ((mergedLinks and optimType=='group') or optimType=='indiv'): labelsList[7] = labels["elBus"]
+        if "elBus" in labels and not mergedLinks and optimType == 'group': labelsList[7] = labels["elBus"] + " Link"
+        if "shBus" in labels and ((mergedLinks and optimType=='group') or optimType=='indiv'): labelsList[8] = labels["shBus"]
+        if "shBus" in labels and not mergedLinks and optimType == 'group': labelsList[8] = labels["shBus"] + " Link"
+        if "dhwBus" in labels and ((mergedLinks and optimType=='group') or optimType=='indiv'): labelsList[9] = labels["dhwBus"]
+        if "dhwBus" in labels and not mergedLinks and optimType == 'group': labelsList[9] = labels["dhwBus"] + " Link"
+        if "naturalGas" in labels: labelsList[0] = labels["naturalGas"]
+        if "grid" in labels: labelsList[1] = labels["grid"]
+        if "pv" in labels: labelsList[2]=labels["pv"]
+        if "gasBoiler" in labels: labelsList[4]=labels["gasBoiler"]
+        if "CHP" in labels:labelsList[3]=labels["CHP"]
+        if "prodEl" in labels: labelsList[6] = labels["prodEl"]
+        if "localEl" in labels: labelsList[5]=labels["localEl"]
+        if "StorageEl" in labels:labelsList[10]=labels["StorageEl"]
+        if "excessEl" in labels:labelsList[20]=labels["excessEl"]
+        if "excessSh" in labels:labelsList[25]=labels["excessSh"]
+        if "elBus" in labels:labelsList[11]=labels["elBus"]
+        if "HP" in labels:labelsList[12]=labels["HP"]
+        if "GWHP" in labels:labelsList[13]=labels["GWHP"]
+        if "solarCollector" in labels:labelsList[15]=labels["solarCollector"]
+        if "excessSolarCollector" in labels: labelsList[16]=labels["excessSolarCollector"]
+        if "prodSH" in labels:labelsList[17]=labels["prodSH"]
+        if "shBus" in labels:labelsList[27] = labels["shBus"]
+        if "StorageSh" in labels:labelsList[18]=labels["StorageSh"]
+        if "StorageDhw" in labels:labelsList[19]=labels["StorageDhw"]
+        if "dhwBus" in labels:labelsList[26]=labels["dhwBus"]
+        if "DemandEl" in labels:labelsList[21]=labels["DemandEl"]
+        if "DemandMob" in labels:labelsList[22]=labels["DemandMob"]
+        if "DemandSh" in labels:labelsList[23]=labels["DemandSh"]
+        if "DemandDhw" in labels:labelsList[24]=labels["DemandDhw"]
+        if "ElectricRod" in labels:labelsList[14]=labels["ElectricRod"]
+    positionDict = {
+        labelsList[0]: [0.001, 0.65],  # X and Y positions should never be set to 0 or 1
+        labelsList[1]: [0.001, 0.15],
+        labelsList[2]: [0.001, 0.3],
+        labelsList[3]: [0.1, 0.7],
+        labelsList[4]: [0.1, 0.7],
+        labelsList[5]: [0.15, 0.3],
+        labelsList[6]: [0.3, 0.3],
+        labelsList[10]: [0.2, 0.25],
+        labelsList[11]: [0.4, 0.2],
+        labelsList[12]: [0.55, 0.5],
+        labelsList[13]: [0.55, 0.2],
+        labelsList[13]+'35': [0.55, 0.2],
+        labelsList[13]+'60': [0.55, 0.5],
+        labelsList[14]: [0.6, 0.4],
+        labelsList[15]: [0.6, 0.85],
+        labelsList[16]: [0.7, 0.95],
+        labelsList[17]: [0.65, 0.58],
+        # "usedSH":	[0.75, 0.58],
+        labelsList[18]: [0.68, 0.37],
+        labelsList[19]: [0.65, 0.85],
+        # "usedDHW": [0.8, 0.85],
+        # "prodDHW": [0.75, 0.85],
+        labelsList[20]: [0.999, 0.25],
+        labelsList[21]: [0.999, 0.15],
+        labelsList[22]: [0.999, 0.4],
+        labelsList[23]: [0.999, 0.6],
+        labelsList[24]: [0.999, 0.85],
+        labelsList[25]: [0.999, 0.7],
+        labelsList[26]: [0.8, 0.85],
+        labelsList[27]: [0.8, 0.6]
+    }
+
+    if mergedLinks and optimType=='group':
+        positionDict[labelsList[7]]= [0.4, 0.35]
+        positionDict[labelsList[8]]= [0.8, 0.35]
+        positionDict[labelsList[9]]= [0.8, 0.5]
+    elif optimType!='indiv':
+        #links
+        positionDict[labelsList[7]] = [0.45, 0.35]
+        positionDict[labelsList[8]] = [0.77, 0.35]
+        positionDict[labelsList[9]] = [0.85, 0.5]
+        # prod DHW, used SH and used El
+        if labels != 'default':
+            labelsList[28] = labels["usedEl"]
+            labelsList[29] = labels["usedSH"]
+            labelsList[30] = labels["prodDHW"]
+        positionDict[labelsList[28]] = [0.52, 0.35]
+        positionDict[labelsList[29]] = [0.75, 0.35]
+        positionDict[labelsList[30]] = [0.7, 0.5]
+
+    return positionDict
+
+labelDict = {
+    "electricityLink": "elLink",
+    "electricityLink1_2": "elLink",
+    "electricityLink1_3": "elLink",
+    "electricityLink1_4": "elLink",
+    "electricityLink1_5": "elLink",
+    "electricityLink1_6": "elLink",
+    "electricityLink2_3": "elLink",
+    "electricityLink2_4": "elLink",
+    "electricityLink2_5": "elLink",
+    "electricityLink2_6": "elLink",
+    "electricityLink3_4": "elLink",
+    "electricityLink3_5": "elLink",
+    "electricityLink3_6": "elLink",
+    "electricityLink4_5": "elLink",
+    "electricityLink4_6": "elLink",
+    "electricityLink5_6": "elLink",
+    "electricityLink2_1": "elLink",
+    "electricityLink3_2": "elLink",
+    "electricityLink3_1": "elLink",
+    "electricityLink4_3": "elLink",
+    "electricityLink4_2": "elLink",
+    "electricityLink4_1": "elLink",
+    "electricityLink5_4": "elLink",
+    "electricityLink5_3": "elLink",
+    "electricityLink5_2": "elLink",
+    "electricityLink5_1": "elLink",
+    "electricityLink6_5": "elLink",
+    "electricityLink6_4": "elLink",
+    "electricityLink6_3": "elLink",
+    "electricityLink6_2": "elLink",
+    "electricityLink6_1": "elLink",
+
+    "shLink1_2": "shLink",
+    "shLink1_3": "shLink",
+    "shLink1_4": "shLink",
+    "shLink1_5": "shLink",
+    "shLink1_6": "shLink",
+    "shLink2_3": "shLink",
+    "shLink2_4": "shLink",
+    "shLink2_5": "shLink",
+    "shLink2_6": "shLink",
+    "shLink3_4": "shLink",
+    "shLink3_5": "shLink",
+    "shLink3_6": "shLink",
+    "shLink4_5": "shLink",
+    "shLink4_6": "shLink",
+    "shLink5_6": "shLink",
+    "shLink2_1": "shLink",
+    "shLink3_2": "shLink",
+    "shLink3_1": "shLink",
+    "shLink4_3": "shLink",
+    "shLink4_2": "shLink",
+    "shLink4_1": "shLink",
+    "shLink5_1": "shLink",
+    "shLink5_2": "shLink",
+    "shLink5_3": "shLink",
+    "shLink5_4": "shLink",
+    "shLink6_5": "shLink",
+    "shLink6_4": "shLink",
+    "shLink6_3": "shLink",
+    "shLink6_2": "shLink",
+    "shLink6_1": "shLink",
+
+    "dhwLink1_2": "dhwLink",
+    "dhwLink1_3": "dhwLink",
+    "dhwLink1_4": "dhwLink",
+    "dhwLink1_5": "dhwLink",
+    "dhwLink1_6": "dhwLink",
+    "dhwLink2_3": "dhwLink",
+    "dhwLink2_4": "dhwLink",
+    "dhwLink2_5": "dhwLink",
+    "dhwLink2_6": "dhwLink",
+    "dhwLink3_4": "dhwLink",
+    "dhwLink3_5": "dhwLink",
+    "dhwLink3_6": "dhwLink",
+    "dhwLink4_5": "dhwLink",
+    "dhwLink4_6": "dhwLink",
+    "dhwLink5_6": "dhwLink",
+    "dhwLink2_1": "dhwLink",
+    "dhwLink3_2": "dhwLink",
+    "dhwLink3_1": "dhwLink",
+    "dhwLink4_3": "dhwLink",
+    "dhwLink4_2": "dhwLink",
+    "dhwLink4_1": "dhwLink",
+    "dhwLink5_1": "dhwLink",
+    "dhwLink5_2": "dhwLink",
+    "dhwLink5_3": "dhwLink",
+    "dhwLink5_4": "dhwLink",
+    "dhwLink6_5": "dhwLink",
+    "dhwLink6_4": "dhwLink",
+    "dhwLink6_3": "dhwLink",
+    "dhwLink6_2": "dhwLink",
+    "dhwLink6_1": "dhwLink",
+
+    "naturalGasResource__Building1": "natGas_B1",
+    "naturalGasBus__Building1": "natGas_B1",
+    "gridBus__Building1": "grid_B1",
+    "pv__Building1": "pv_B1",
+    "electricityResource__Building1":"grid_B1",
+    "gridElectricity__Building1": "grid_B1",
+    "GasBoiler__Building1":"gasBoiler_B1",
+    "CHP_SH__Building1": "CHP_B1",
+    "CHP_DHW__Building1": "CHP_B1",
+    "CHP__Building1": "CHP_B1",
+    "electricityBus__Building1": "prodEl_B1",
+    "electricityProdBus__Building1":"localEl_B1", #localEl is before the battery, prodEl after the battery but before the elLink
+    "producedElectricity__Building1": "prodEl_B1",
+    "electricitySource__Building1": "localEl_B1",
+    "electricalStorage__Building1": "Bat_B1",
+    "excesselectricityBus__Building1": "exEl_B1",
+    "excessshDemandBus__Building1": "exSh_B1",
+    "electricityInBus__Building1": "usedEl_B1",
+    "HP_SH__Building1": "HP_B1",
+    "HP_DHW__Building1": "HP_B1",
+    "HP__Building1": "HP_B1",
+    "GWHP_SH__Building1": "GWHP_B1",
+    "GWHP_DHW__Building1": "GWHP_B1",
+    "GWHP__Building1": "GWHP_B1",
+    "solarCollector__Building1": "solar_B1",
+    "solarConnectBus__Building1": "solar_B1",
+    'heat_solarCollector__Building1': "solar_B1",
+    'excess_solarheat__Building1':"exSolar_B1",
+    'shSource__Building1'	: "prodSH_B1",
+    'shSourceBus__Building1': "prodSH_B1",
+    "spaceHeatingBus__Building1": "shBus_B1",
+    "spaceHeating__Building1": "shBus_B1",
+    "shStorage__Building1": "shStor_B1",
+    "shDemandBus__Building1": "shBus_B1",
+    "dhwStorageBus__Building1": "dhwStor_B1",
+    "dhwStorage__Building1": "dhwStor_B1",
+    "domesticHotWaterBus__Building1": "dhwBus_B1",
+    'domesticHotWater__Building1': "dhwBus_B1",
+    "dhwDemandBus__Building1": "dhwBus_B1",
+    "electricityDemand__Building1": "Q_el_B1",
+    "emobilityDemand__Building1": "Q_mob_B1",
+    "spaceHeatingDemand__Building1": "Q_sh_B1",
+    "domesticHotWaterDemand__Building1": "Q_dhw_B1",
+    "excessshSourceBus__Building1": "exSh_B1",
+    "ElectricRod__Building1": "ElectricRod_B1",
+
+    "naturalGasResource__Building2": "natGas_B2",
+    "naturalGasBus__Building2": "natGas_B2",
+    "electricityResource__Building2": "grid_B2",
+    "gridBus__Building2": "grid_B2",
+    "pv__Building2": "pv_B2",
+    "gridElectricity__Building2": "grid_B2",
+    "GasBoiler__Building2":"gasBoiler_B2",
+    "CHP_SH__Building2": "CHP_B2",
+    "CHP_DHW__Building2": "CHP_B2",
+    "CHP__Building2": "CHP_B2",
+    "electricityBus__Building2": "prodEl_B2",
+    "electricityProdBus__Building2": "localEl_B2",
+    "producedElectricity__Building2": "prodEl_B2",
+    "electricitySource__Building2": "localEl_B2",
+    "electricalStorage__Building2": "Bat_B2",
+    "excesselectricityBus__Building2": "exEl_B2",
+    "excessshDemandBus__Building2": "exSh_B2",
+    "electricityInBus__Building2": "usedEl_B2",
+    "HP_SH__Building2": "HP_B2",
+    "HP_DHW__Building2": "HP_B2",
+    "HP__Building2": "HP_B2",
+    "GWHP_SH__Building2": "GWHP_B2",
+    "GWHP_DHW__Building2": "GWHP_B2",
+    "GWHP__Building2": "GWHP_B2",
+    "solarCollector__Building2": "solar_B2",
+    "solarConnectBus__Building2": "solar_B2",
+    'heat_solarCollector__Building2': "solar_B2",
+    'excess_solarheat__Building2': "exSolar_B2",
+    'shSource__Building2'	: "prodSH_B2",
+    'shSourceBus__Building2': "prodSH_B2",
+    "spaceHeatingBus__Building2": "shBus_B2",
+    "spaceHeating__Building2": "shBus_B2",
+    "shStorage__Building2": "shStor_B2",
+    "shDemandBus__Building2": "shBus_B2",
+    "dhwStorageBus__Building2": "dhwStor_B2",
+    "dhwStorage__Building2": "dhwStor_B2",
+    "domesticHotWaterBus__Building2": "dhwBus_B2",
+    'domesticHotWater__Building2': "dhwBus_B2",
+    "dhwDemandBus__Building2": "dhwBus_B2",
+    "electricityDemand__Building2": "Q_el_B2",
+    "emobilityDemand__Building2": "Q_mob_B2",
+    "spaceHeatingDemand__Building2":        "Q_sh_B2",
+    "domesticHotWaterDemand__Building2": "Q_dhw_B2",
+    "excessshSourceBus__Building2": "exSh_B2",
+    "ElectricRod__Building2": "ElectricRod_B2",
+
+    "naturalGasResource__Building3": "natGas_B3",
+    "naturalGasBus__Building3": "natGas_B3",
+    "electricityResource__Building3": "grid_B3",
+    "gridBus__Building3": "grid_B3",
+    "GasBoiler__Building3": "gasBoiler_B3",
+    "pv__Building3": "pv_B3",
+    "gridElectricity__Building3": "grid_B3",
+    "CHP_SH__Building3": "CHP_B3",
+    "CHP_DHW__Building3": "CHP_B3",
+    "CHP__Building3": "CHP_B3",
+    "electricityBus__Building3": "prodEl_B3",
+    "electricityProdBus__Building3": "localEl_B3",
+    "producedElectricity__Building3": "prodEl_B3",
+    "electricitySource__Building3": "localEl_B3",
+    "electricalStorage__Building3": "Bat_B3",
+    "excesselectricityBus__Building3": "exEl_B3",
+    "excessshDemandBus__Building3": "exSh_B3",
+    "electricityInBus__Building3": "usedEl_B3",
+    "HP_SH__Building3": "HP_B3",
+    "HP_DHW__Building3": "HP_B3",
+    "HP__Building3": "HP_B3",
+    "GWHP_SH__Building3": "GWHP_B3",
+    "GWHP_DHW__Building3": "GWHP_B3",
+    "GWHP__Building3": "GWHP_B3",
+    "solarCollector__Building3": "solar_B3",
+    "solarConnectBus__Building3": "solar_B3",
+    'heat_solarCollector__Building3': "solar_B3",
+    'excess_solarheat__Building3': "exSolar_B3",
+    'shSource__Building3': "prodSH_B3",
+    'shSourceBus__Building3': "prodSH_B3",
+    "spaceHeatingBus__Building3": "shBus_B3",
+    "spaceHeating__Building3": "shBus_B3",
+    "shStorage__Building3": "shStor_B3",
+    "shDemandBus__Building3": "shBus_B3",
+    "dhwStorageBus__Building3": "dhwStor_B3",
+    "dhwStorage__Building3": "dhwStor_B3",
+    "domesticHotWaterBus__Building3": "dhwBus_B3",
+    'domesticHotWater__Building3': "dhwBus_B3",
+    "dhwDemandBus__Building3": "dhwBus_B3",
+    "electricityDemand__Building3": "Q_el_B3",
+    "emobilityDemand__Building3": "Q_mob_B3",
+    "spaceHeatingDemand__Building3":        "Q_sh_B3",
+    "domesticHotWaterDemand__Building3": "Q_dhw_B3",
+    "excessshSourceBus__Building3": "exSh_B3",
+    "ElectricRod__Building3": "ElectricRod_B3",
+
+    "naturalGasResource__Building4": "natGas_B4",
+    "naturalGasBus__Building4": "natGas_B4",
+    "electricityResource__Building4": "grid_B4",
+    "gridBus__Building4": "grid_B4",
+    "pv__Building4": "pv_B4",
+    "gridElectricity__Building4": "grid_B4",
+    "GasBoiler__Building4":"gasBoiler_B4",
+    "CHP_SH__Building4": "CHP_B4",
+    "CHP_DHW__Building4": "CHP_B4",
+    "CHP__Building4": "CHP_B4",
+    "electricityBus__Building4": "prodEl_B4",
+    "electricityProdBus__Building4": "localEl_B4",
+    "producedElectricity__Building4": "prodEl_B4",
+    "electricitySource__Building4": "localEl_B4",
+    "electricalStorage__Building4": "Bat_B4",
+    "excesselectricityBus__Building4": "exEl_B4",
+    "excessshDemandBus__Building4": "exSh_B4",
+    "electricityInBus__Building4": "usedEl_B4",
+    "HP_SH__Building4": "HP_B4",
+    "HP_DHW__Building4": "HP_B4",
+    "HP__Building4": "HP_B4",
+    "GWHP_SH__Building4": "GWHP_B4",
+    "GWHP_DHW__Building4": "GWHP_B4",
+    "GWHP__Building4": "GWHP_B4",
+    "solarCollector__Building4": "solar_B4",
+    "solarConnectBus__Building4": "solar_B4",
+    'heat_solarCollector__Building4': "solar_B4",
+    'excess_solarheat__Building4': "exSolar_B4",
+    'shSource__Building4': "prodSH_B4",
+    'shSourceBus__Building4': "prodSH_B4",
+    "spaceHeatingBus__Building4": "shBus_B4",
+    "spaceHeating__Building4": "shBus_B4",
+    "shStorage__Building4": "shStor_B4",
+    "shDemandBus__Building4": "shBus_B4",
+    "dhwStorageBus__Building4": "dhwStor_B4",
+    "dhwStorage__Building4": "dhwStor_B4",
+    "domesticHotWaterBus__Building4": "dhwBus_B4",
+    'domesticHotWater__Building4': "dhwBus_B4",
+    "dhwDemandBus__Building4": "dhwBus_B4",
+    "electricityDemand__Building4": "Q_el_B4",
+    "emobilityDemand__Building4": "Q_mob_B4",
+    "spaceHeatingDemand__Building4":        "Q_sh_B4",
+    "domesticHotWaterDemand__Building4": "Q_dhw_B4",
+    "excessshSourceBus__Building4": "exSh_B4",
+    "ElectricRod__Building4": "ElectricRod_B4",
+
+    "naturalGasResource__Building5": "natGas_B5",
+    "naturalGasBus__Building5": "natGas_B5",
+    "electricityResource__Building5": "grid_B5",
+    "gridBus__Building5": "grid_B5",
+    "pv__Building5": "pv_B5",
+    "gridElectricity__Building5": "grid_B5",
+    "GasBoiler__Building5":"gasBoiler_B5",
+    "CHP_SH__Building5": "CHP_B5",
+    "CHP_DHW__Building5": "CHP_B5",
+    "CHP__Building5": "CHP_B5",
+    "electricityBus__Building5": "prodEl_B5",
+    "electricityProdBus__Building5": "localEl_B5",
+    "producedElectricity__Building5": "prodEl_B5",
+    "electricitySource__Building5": "prodEl_B5",
+    "electricalStorage__Building5": "Bat_B5",
+    "excesselectricityBus__Building5": "exEl_B5",
+    "excessshDemandBus__Building5": "exSh_B5",
+    "excessshSourceBus__Building5": "exSh_B5",
+    "electricityInBus__Building5": "usedEl_B5",
+    "HP_SH__Building5": "HP_B5",
+    "HP_DHW__Building5": "HP_B5",
+    "HP__Building5": "HP_B5",
+    "GWHP_SH__Building5": "GWHP_B5",
+    "GWHP_DHW__Building5": "GWHP_B5",
+    "GWHP__Building5": "GWHP_B5",
+    "solarCollector__Building5": "solar_B5",
+    "solarConnectBus__Building5": "solar_B5",
+    'heat_solarCollector__Building5': "solar_B5",
+    'excess_solarheat__Building5': "exSolar_B5",
+    'shSource__Building5'	: "prodSH_B5",
+    'shSourceBus__Building5': "prodSH_B5",
+    "spaceHeatingBus__Building5": "usedSH_B5",
+    "spaceHeating__Building5": "Q_sh_B5",
+    "shStorage__Building5": "shStor_B5",
+    "shDemandBus__Building5": "Q_sh_B5",
+    "dhwStorageBus__Building5": "dhwStor_B5",
+    "dhwStorage__Building5": "dhwStor_B5",
+    "domesticHotWaterBus__Building5": "prodDHW_B5",
+    'domesticHotWater__Building5': "usedDHW_B5",
+    "dhwDemandBus__Building5": "Q_dhw_B5",
+    "electricityDemand__Building5": "Q_el_B5",
+    "spaceHeatingDemand__Building5":        "Q_sh_B5",
+    "domesticHotWaterDemand__Building5": "Q_dhw_B5",
+    "ElectricRod__Building5": "ElectricRod_B5",
+
+    "naturalGasResource__Building6": "natGas_B6",
+    "naturalGasBus__Building6": "natGas_B6",
+    "electricityResource__Building6": "grid_B6",
+    "gridBus__Building6": "grid_B6",
+    "pv__Building6": "pv_B6",
+    "gridElectricity__Building6": "grid_B6",
+    "GasBoiler__Building6":"gasBoiler_B6",
+    "CHP_SH__Building6": "CHP_B6",
+    "CHP_DHW__Building6": "CHP_B6",
+    "CHP__Building6": "CHP_B6",
+    "electricityBus__Building6": "prodEl_B6",
+    "electricityProdBus__Building6": "localEl_B6",
+    "producedElectricity__Building6": "prodEl_B6",
+    "electricitySource__Building6": "prodEl_B6",
+    "electricalStorage__Building6": "Bat_B6",
+    "excesselectricityBus__Building6": "exEl_B6",
+    "excessshDemandBus__Building6": "exSh_B6",
+    "excessshSourceBus__Building6": "exSh_B6",
+    "electricityInBus__Building6": "usedEl_B6",
+    "HP_SH__Building6": "HP_B6",
+    "HP_DHW__Building6": "HP_B6",
+    "HP__Building6": "HP_B6",
+    "GWHP_SH__Building6": "GWHP_B6",
+    "GWHP_DHW__Building6": "GWHP_B6",
+    "GWHP__Building6": "GWHP_B6",
+    "solarCollector__Building6": "solar_B6",
+    "solarConnectBus__Building6": "solar_B6",
+    'heat_solarCollector__Building6': "solar_B6",
+    'excess_solarheat__Building6': "exSolar_B6",
+    'shSource__Building6'	: "prodSH_B6",
+    'shSourceBus__Building6': "prodSH_B6",
+    "spaceHeatingBus__Building6": "usedSH_B6",
+    "spaceHeating__Building6": "Q_sh_B6",
+    "shStorage__Building6": "shStor_B6",
+    "shDemandBus__Building6": "Q_sh_B6",
+    "dhwStorageBus__Building6": "dhwStor_B6",
+    "dhwStorage__Building6": "dhwStor_B6",
+    "domesticHotWaterBus__Building6": "prodDHW_B6",
+    'domesticHotWater__Building6': "usedDHW_B6",
+    "dhwDemandBus__Building6": "Q_dhw_B6",
+    "electricityDemand__Building6": "Q_el_B6",
+    "spaceHeatingDemand__Building6":        "Q_sh_B6",
+    "domesticHotWaterDemand__Building6": "Q_dhw_B6",
+    "ElectricRod__Building6": "ElectricRod_B6",
+}
+
+labelPositionDict={
+    "natGas":	[0.001, 0.65], #X and Y positions should never be set to 0 or 1
+    "grid":	[0.001, 0.15],
+    "pv":   [0.001, 0.3],
+    "CHP":	[0.1, 0.7],
+    "gasBoiler": [0.1, 0.7],
+    "localEl":	[0.15, 0.3],
+    "prodEl":[0.3,0.3],
+    "elLink":	[0.4, 0.35],
+    "shLink": [0.8, 0.35],
+    "dhwLink": [0.8, 0.5],
+	"Bat":	[0.2, 0.25],
+    "usedEl":	[0.4, 0.2],
+    "HP":	[0.55, 0.5],
+    "GWHP":	[0.55, 0.2],
+    "ElectricRod": [0.6, 0.4],
+    "solar":	[0.6, 0.85],
+    "exSolar": [0.7, 0.95],
+    "prodSH": [0.65, 0.58],
+    #"usedSH":	[0.75, 0.58],
+    "shStor":	[0.68, 0.37],
+    "dhwStor":	[0.65, 0.85],
+    #"usedDHW": [0.8, 0.85],
+    #"prodDHW": [0.75, 0.85],
+    "exEl": [0.999, 0.25],
+    "Q_el":	[0.999, 0.15],
+    "Q_mob":[0.999, 0.4],
+    "Q_sh":	[0.999, 0.6],
+    "Q_dhw":[0.999, 0.85],
+    "exSh": [0.999, 0.7],
+    "dhwBus":[0.8, 0.85],
+    "shBus": [0.8, 0.6]
+	}
+
+fullPositionDict={
+        "naturalGas":	[0.001, 0.75],
+        "gridBus":	[0.001, 0.2],
+        "pv":   [0.001, 0.3],
+        "gridElect":	[0.1, 0.05],
+        "electricityProdBus": [0.1, 0.2],
+        "CHP":	[0.1, 0.6],
+        "GasBoiler": [0.1, 0.7],
+        "electricitySource": [0.15, 0.2],
+        "electricityBus":	[0.2, 0.2],
+        "producedElectricity":	[0.3, 0.25],
+        "electricityLink":	[0.3, 0.35],
+        "electricalStorage":	[0.3, 0.25],
+        "excesselect":	[0.5, 0.05],
+        "electricityInBus":	[0.5, 0.2],
+        "HP":	[0.6, 0.5],
+        "GWHP":	[0.6, 0.2],
+        "ElectricRod": [0.6, 0.4],
+        "heat_solarCollector": [0.4, 0.85],
+        "solarConnect": [0.5, 0.85],
+        "solarCollector_":	[0.6, 0.85],
+        "excess_solarheat":[0.6,0.85],
+        'shSource_': [0.63, 0.58],
+        'shLink': [0.64, 0.58],
+        'shSourceBus': [0.66, 0.58],
+        "spaceHeatingBus":	[0.7, 0.58],
+        "spaceHeating_":	[0.8, 0.6],
+        "shStorage":	[0.8, 0.37],
+        "shDemandBus":	[0.9, 0.6],
+        "dhwStorageBus":	[0.7, 0.9],
+        "dhwStorage_":	[0.8, 0.9],
+        "domesticHotWater_":	[0.92, 0.9],
+        "domesticHotWaterBus":	[0.9, 0.9],
+        "dhwDemandBus":	[0.95, 0.9],
+        "electricityDemand":	[0.999, 0.1],
+        "spaceHeatingDemand_":	[0.999, 0.6],
+        "domesticHotWaterDemand":	[0.999, 0.9]
         }
```

### Comparing `optihood-0.0.0/optihood/links.py` & `optihood-0.0.1/optihood/links.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from pyomo.core.base.block import SimpleBlock
-from pyomo.environ import BuildAction
-from pyomo.environ import Constraint
-
-from oemof.solph import network as solph_network
-from oemof.solph.plumbing import sequence as solph_sequence
-
-class Link(solph_network.Transformer):
-    r"""
-    A transformer to model links between different buildings
-    The constraint defined in a new constraint block equates the sum of all the input flows
-    to the sum of all the output flows
-    """
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-    def constraint_group(self):
-        return LinkBlock
-
-class LinkBlock(SimpleBlock):
-    r"""Block for the linear relation of nodes of type Link"""
-    CONSTRAINT_GROUP = True
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-    def _create(self, group=None):
-        """Creates the two linear constraints for nodes of type Link
-        """
-        if group is None:
-            return None
-
-        m = self.parent_block()
-        in_flows = {n: [i for i in n.inputs.keys()] for n in group}
-        out_flows = {n: [o for o in n.outputs.keys()] for n in group}
-        efficiency = [n.conversion_factors[next(iter(n.outputs.keys()))] for n in group][0][0]   # conversion factors of all the output flows of all the groups will be equal, therefore first value is chosen
-
-        def _input_output_relation(block):
-            """Constraint defining the relation between input and outputs."""
-            self.input_output_relation = Constraint(group, m.TIMESTEPS, noruleinit=True)
-
-            for t in m.TIMESTEPS:
-                for g in group:
-                    lhs = sum(m.flow[i, g, t] for i in in_flows[g]) * efficiency
-                    rhs = sum(m.flow[g, o, t] for o in out_flows[g])
-                    block.input_output_relation.add((g, t), (lhs == rhs))
-
+from pyomo.core.base.block import SimpleBlock
+from pyomo.environ import BuildAction
+from pyomo.environ import Constraint
+
+from oemof.solph import network as solph_network
+from oemof.solph.plumbing import sequence as solph_sequence
+
+class Link(solph_network.Transformer):
+    r"""
+    A transformer to model links between different buildings
+    The constraint defined in a new constraint block equates the sum of all the input flows
+    to the sum of all the output flows
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def constraint_group(self):
+        return LinkBlock
+
+class LinkBlock(SimpleBlock):
+    r"""Block for the linear relation of nodes of type Link"""
+    CONSTRAINT_GROUP = True
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def _create(self, group=None):
+        """Creates the two linear constraints for nodes of type Link
+        """
+        if group is None:
+            return None
+
+        m = self.parent_block()
+        in_flows = {n: [i for i in n.inputs.keys()] for n in group}
+        out_flows = {n: [o for o in n.outputs.keys()] for n in group}
+        efficiency = [n.conversion_factors[next(iter(n.outputs.keys()))] for n in group][0][0]   # conversion factors of all the output flows of all the groups will be equal, therefore first value is chosen
+
+        def _input_output_relation(block):
+            """Constraint defining the relation between input and outputs."""
+            self.input_output_relation = Constraint(group, m.TIMESTEPS, noruleinit=True)
+
+            for t in m.TIMESTEPS:
+                for g in group:
+                    lhs = sum(m.flow[i, g, t] for i in in_flows[g]) * efficiency
+                    rhs = sum(m.flow[g, o, t] for o in out_flows[g])
+                    block.input_output_relation.add((g, t), (lhs == rhs))
+
         self.input_output_relation_build = BuildAction(rule=_input_output_relation)
```

### Comparing `optihood-0.0.0/optihood/plot_functions.py` & `optihood-0.0.1/optihood/plot_functions.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,1192 +1,1192 @@
-import matplotlib.pyplot as plt
-import matplotlib.gridspec as gridspec
-import matplotlib.ticker as tkr
-
-from bokeh.plotting import figure, show
-from bokeh.layouts import layout, gridplot
-from bokeh.models import DatetimeTickFormatter, HoverTool, Legend
-from bokeh.palettes import *
-from bokeh.io import output_file
-
-from openpyxl import load_workbook
-from datetime import datetime
-from dateutil.parser import isoparse
-import itertools
-import pandas as pd
-import os
-
-# This file defines different functions for the plotting of the results of the optimization.
-# The plots are made at the end of this file, introducing a .xls file previously created during the optimization.
-# An important parameter "optMode" needs to be set when running the code (look in the __main__ fragment)
-
-
-def monthlyBalance(data, bus, new_legends):
-    """
-    Function for the definition of the monthly summary of a bus
-    :param data: dict type, results from the optimization applied to one bus
-    :param bus: str type, bus from which the summary is required
-    :param new_legends: dict type, new legends to plot on the graph
-    :return:
-    """
-    building = "__" + bus.split("__")[1]
-    data_month = data.resample('1m').sum()
-    monthShortNames = ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul', 'Aug', 'Sep', 'Oct', 'Nov', 'Dec']
-
-    while len(data_month) != len(monthShortNames):
-        data.drop(data.index[-1], inplace=True)
-        data_month = data.resample('1m').sum()
-    neg_flow = []
-    pos_flow = []
-    for i in data.columns:
-        a = [i.strip("()").split(", ")]
-        if "Bus" in a[0][0]:
-            neg_flow.append(i)
-        else:
-            pos_flow.append(i)
-    plt.figure()
-    mark = []
-    for i in neg_flow:
-        plt.bar(monthShortNames, -data_month[i], label=new_legends[i.replace(building, "")], bottom=sum(mark))
-        mark.append(-data_month[i])
-    mark = []
-    for i in pos_flow:
-        plt.bar(monthShortNames, data_month[i], label=new_legends[i.replace(building, "")], bottom=sum(mark))
-        mark.append(data_month[i])
-
-    ax = plt.gca()
-    # Shrink current axis by 20%
-    box = ax.get_position()
-    ax.set_position([box.x0, box.y0, box.width * 0.8, box.height])
-
-    # Put a legend to the right of the current axis
-    ax.legend(loc='center left', bbox_to_anchor=(1, 0.5))
-    plt.grid(axis='y')
-    if "electricity" in bus or "grid" in bus:
-        plt.title("Monthly electricity balance for " + building.replace("__", ""))
-    elif "spaceHeating" in bus:
-        plt.title("Monthly space heating balance for " + building.replace("__", ""))
-    else:
-        plt.title("Monthly domestic hot water balance for " + building.replace("__", ""))
-    plt.show()
-
-
-def hourlyDailyPlot(data, bus, palette, new_legends):
-    """
-    Function for the bokeh plot of hourly and daily balance of a bus
-    :param data: list of dict type, results from the optimization
-    :param bus: list of str type, buses from which the summary is required
-    :param palette: palette type form bokeh.palettes (For example, Category10_8), different types can be found on
-    https://docs.bokeh.org/en/latest/docs/reference/palettes.html or
-    https://docs.bokeh.org/en/latest/_modules/bokeh/palettes.html
-    :param new_legends: dict type, new legends to plot on the graph
-    For example, Category10_8
-    :return:
-    """
-    p_figs = []
-    p_figs_h = []
-    p_figs_d = []
-    p_plots = []
-    a = []
-    b = 1
-    bus = [x for x in bus if 'electricityProdBus' not in x and 'electricityInBus' not in x]
-    for i in range(0, len(data)):
-        building = '__' + bus[i].split("__")[1]
-
-        if "electricity" in bus[i]:
-            dt = data[i]
-            dt.pop(f"(('electricityProdBus{building}', 'electricitySource{building}'), 'flow')")
-            data_day = dt.resample('1d').sum()
-            p1 = figure(title="Hourly electricity flows for " + building.replace("__", ""), x_axis_label="Date", y_axis_label="Energy (kWh)", sizing_mode="scale_both")
-            p1.add_layout(Legend(), 'right')
-            p1.add_tools(HoverTool(tooltips=[('Time', '@x{%d/%m/%Y %H:%M:%S}'), ('Energy', '@y{0.00}')],
-                                   formatters={'@x': 'datetime'},
-                                   mode='mouse'))
-            p2 = figure(title="Daily electricity flows for " + building.replace("__", ""), x_axis_label="Date", y_axis_label="Energy (kWh)", sizing_mode="scale_both")
-            p2.add_layout(Legend(), 'right')
-            p2.add_tools(HoverTool(tooltips=[('Date', '@x{%d/%m/%Y}'), ('Energy', '@y{0.00}')],
-                                   formatters={'@x': 'datetime'},
-                                   mode='mouse'))
-            if len(p_figs_h) > 0:
-                p1.x_range = p_figs_h[0].x_range
-                p2.x_range = p_figs_d[0].x_range
-            colors = itertools.cycle(palette)
-            for j, color in zip(dt.columns, colors):
-                p1.line(dt.index, dt[j], legend_label=new_legends[j.replace(building, "")], color=color, line_width=1.5)
-                p2.line(data_day.index, data_day[j], legend_label=new_legends[j.replace(building, "")], color=color, line_width=1.5)
-            p_figs.append([p1, p2])
-            p_figs_h.append(p1)
-            p_figs_d.append(p2)
-            p_plots.append(p1)
-            p_plots.append(p2)
-
-        elif "shSource" in bus[i] or "spaceHeatingBus" in bus[i]:
-            dt = data[i]
-            data_day = dt.resample('1d').sum()
-            p3 = figure(title="Hourly space heating flows for " + building.replace("__", ""), x_axis_label="Date", y_axis_label="Energy (kWh)", sizing_mode="scale_both")
-            p3.add_layout(Legend(), 'right')
-            p3.add_tools(HoverTool(tooltips=[('Time', '@x{%d/%m/%Y %H:%M:%S}'), ('Energy', '@y{0.00}')],
-                                   formatters={'@x': 'datetime'},
-                                   mode='mouse'))
-            p4 = figure(title="Daily space heating flows for " + building.replace("__", ""), x_axis_label="Date", y_axis_label="Energy (kWh)", sizing_mode="scale_both")
-            p4.add_layout(Legend(), 'right')
-            p4.add_tools(HoverTool(tooltips=[('Date', '@x{%d/%m/%Y}'), ('Energy', '@y{0.00}')],
-                                   formatters={'@x': 'datetime'},
-                                   mode='mouse'))
-            if len(p_figs_h) > 0:
-                p3.x_range = p_figs_h[0].x_range
-                p4.x_range = p_figs_d[0].x_range
-            colors = itertools.cycle(palette)
-            for j, color in zip(dt.columns, colors):
-                p3.line(dt.index, dt[j], legend_label=new_legends[j.replace(building, "")], color=color, line_width=1.5)
-                p4.line(data_day.index, data_day[j], legend_label=new_legends[j.replace(building, "")], color=color, line_width=1.5)
-            p_figs.append([p3, p4])
-            p_figs_h.append(p3)
-            p_figs_d.append(p4)
-            p_plots.append(p3)
-            p_plots.append(p4)
-
-        else:
-            dt = data[i]
-            data_day = dt.resample('1d').sum()
-
-            p5 = figure(title="Hourly domestic hot water flows for " + building.replace("__", ""), x_axis_label="Date", y_axis_label="Energy (kWh)", sizing_mode="scale_both")
-            p5.add_layout(Legend(), 'right')
-            p5.add_tools(HoverTool(tooltips=[('Time', '@x{%d/%m/%Y %H:%M:%S}'), ('Energy', '@y{0.00}')],
-                                   formatters={'@x': 'datetime'},
-                                   mode='mouse'))
-            p6 = figure(title="Daily domestic hot water flows for "  + building.replace("__", ""), x_axis_label="Date", y_axis_label="Energy (kWh)", sizing_mode="scale_both")
-            p6.add_layout(Legend(), 'right')
-            p6.add_tools(HoverTool(tooltips=[('Date', '@x{%d/%m/%Y}'), ('Energy', '@y{0.00}')],
-                                   formatters={'@x': 'datetime'},
-                                   mode='mouse'))
-            if len(p_figs_h) > 0:
-                p5.x_range = p_figs_h[0].x_range
-                p6.x_range = p_figs_d[0].x_range
-            colors = itertools.cycle(palette)
-            for j, color in zip(dt.columns, colors):
-                p5.line(dt.index, dt[j], legend_label=new_legends[j.replace(building, "")], color=color, line_width=1.5)
-                p6.line(data_day.index, data_day[j], legend_label=new_legends[j.replace(building, "")], color=color, line_width=1.5)
-            p_figs.append([p5, p6])
-            p_figs_h.append(p5)
-            p_figs_d.append(p6)
-            p_plots.append(p5)
-            p_plots.append(p6)
-
-    for p in p_plots:
-        p.xaxis[0].formatter = DatetimeTickFormatter(months="%d %b")
-        p.legend.click_policy = "hide"
-        p.legend.location = "top_left"
-        p.legend.label_text_font_size = "8pt"
-
-    return (p_figs_h, p_figs_d)
-
-
-def toColor(COLORS, obj=None):
-    """
-    Function from the URBS platform https://github.com/ojdo/urbs/blob/1house/comp.py
-    Assign a deterministic pseudo-random color to argument.
-    If COLORS[obj] is set, return that. For strings, this value depends only
-    on the string content, so that same strings always yield the same color.
-    :param COLORS: dict of components and their assigned color
-    :param obj: any hashable object
-    :return: a (r, g, b) color tuple if COLORS[obj] is set, otherwise a hexstring
-    """
-    try:
-        color = tuple(rgb / 255.0 for rgb in COLORS[obj])
-    except KeyError:
-        # random deterministic color
-        import hashlib
-        color = '#' + hashlib.sha1(obj.encode()).hexdigest()[-6:]
-    return color
-
-
-def groupHbarPlots(ax, group_size, inner_sep=None):
-    """
-    Function from the URBS platform https://github.com/ojdo/urbs/blob/1house/comp.py
-    Group bars of a horizontal barplot closer together.
-    Given an existing horizontal bar plot handle ax, move bars of a given group size (>=2) closer together,
-    reducing the distance within the bars of a group, but increasing the distance between different groups.
-    By default, bars are placed within a coordinate system 1 unit apart. The space between two bars has
-    size 1 - bar_height, which can be specified in matplotlib (and pandas) using the `width` argument.
-    :param ax: matplotlib axis
-    :param group_size: int type, how many bars to group together
-    :param inner_sep: float type, vertical spacing within group (optional). Default: reduce the distance to a half
-    :return:
-    """
-    handles, labels = ax.get_legend_handles_labels()
-    bar_height = handles[0][0].get_height()  # assumption: identical for all
-
-    if inner_sep is None:
-        inner_sep = 0.5 * (1 - bar_height)
-
-    for column, handle in enumerate(handles):
-        for row, patch in enumerate(handle.patches):
-            group_number, row_within_group = divmod(row, group_size)
-
-            group_offset = (group_number * group_size
-                            + 0.5 * (group_size - 1) * (1 - inner_sep)
-                            - 0.5 * (group_size * bar_height))
-
-            patch.set_y(row_within_group * (bar_height + inner_sep)
-                        + group_offset)
-
-
-def deduplicateLegend(handles, labels):
-    """
-    Function from the URBS platform https://github.com/ojdo/urbs/blob/1house/comp.py
-    Remove double entries from figure legend.
-    :param handles: list of legend entry handles
-    :param labels: list of legend entry labels
-    :return: (handles, labels) tuple of lists with duplicate labels removed
-    """
-    new_handles = []
-    new_labels = []
-    for hdl, lbl in zip(handles, labels):
-        if not lbl in new_labels:
-            new_handles.append(hdl)
-            new_labels.append(lbl)
-    # also, sort both lists accordingly
-    new_labels, new_handles = (list(t) for t in zip(*sorted(zip(new_labels, new_handles))))
-    return (new_handles, new_labels)
-
-
-def resultingDataDiagram(elBus, shBus, dhwBus, costs, env, COLORS, building, newLegends):
-    """
-    Function inspired from the URBS platform https://github.com/ojdo/urbs/blob/1house/comp.py
-    Function plotting the different results of the optimization. First, costs will be plotted, then the energy produced,
-    comparing energy for electricity bus, sh and dhw bus, and finally the retrieved energy from the storages.
-    :param elBus: dict type, results from the optimization applied to one bus.
-    :param shBus: dict type, results from the optimization applied to one bus.
-    :param dhwBus: dict type, results from the optimization applied to one bus.
-    :param costs: dict type, resulting costs from the optimization
-    :param env: dict type, resulting environmental impacts from the optimization
-    :param COLORS: list type, different colors for the different components of the system
-    :param building: str type, name of the building
-    :return: Four bar plots and the costs, environmental impacts, production and storage dict created
-    """
-    production = {}
-    storage = {}
-    alpha = 0
-    if optMode == "group":
-        list = []
-
-    for flow in elBus.keys():
-        if "Storage" in flow and "out" in newLegends[flow.replace("__Building"+str(building), "")]:
-            storage[newLegends[flow.replace("__Building"+str(building), "")]] = [0, 0, sum(elBus[flow])]
-        elif optMode == "group" and ("electricityLink" in flow):
-            if "_in" in newLegends[flow.replace("__Building" + str(building), "")]:
-                if newLegends[flow.replace("__Building" + str(building), "")].replace("_in", "") in list:
-                    production[newLegends[flow.replace("__Building" + str(building), "")].replace("_in", "")][2] -= sum(elBus[flow])
-                else:
-                    production[newLegends[flow.replace("__Building" + str(building), "")].replace("_in", "")] = [0, 0, -sum(elBus[flow])]
-                    list.append(newLegends[flow.replace("__Building" + str(building), "")].replace("_in", ""))
-            elif "_out" in newLegends[flow.replace("__Building" + str(building), "")]:
-                if newLegends[flow.replace("__Building" + str(building), "")].replace("_out", "") in list:
-                    production[newLegends[flow.replace("__Building" + str(building), "")].replace("_out", "")][2] += sum(elBus[flow])
-                else:
-                    production[newLegends[flow.replace("__Building" + str(building), "")].replace("_out", "")] = [0, 0, sum(elBus[flow])]
-                    list.append(newLegends[flow.replace("__Building" + str(building), "")].replace("_out", ""))
-        elif "Storage" not in flow and "Demand" not in flow:
-            production[newLegends[flow.replace("__Building"+str(building), "")]] = [0, 0, sum(elBus[flow])]
-
-            # specific for negative flows
-            if "HP_SH" in flow or "HP_DHW" in flow:
-                alpha += sum(elBus[flow])
-
-    production["HP"] = [0, 0, -alpha]
-
-    for flow in shBus.keys():
-        if "Storage" in flow and "out" in newLegends[flow.replace("__Building"+str(building), "")]:
-            storage[newLegends[flow.replace("__Building"+str(building), "")]] = [0, sum(shBus[flow]), 0]
-        elif "Storage" not in flow and "Demand" not in flow:
-            production[newLegends[flow.replace("__Building"+str(building), "")]] = [0, sum(shBus[flow]), 0]
-
-    for flow in dhwBus.keys():
-        if "Storage__" in flow and "out" in newLegends[flow.replace("__Building"+str(building), "")]:
-            storage[newLegends[flow.replace("__Building"+str(building), "")]] = [sum(dhwBus[flow]), 0, 0]
-        elif "Storage__" not in flow and "Demand" not in flow:
-            production[newLegends[flow.replace("__Building"+str(building), "")]] = [sum(dhwBus[flow]), 0, 0]
-
-    costs = costs.transpose()
-    costs = costs.rename(index={0: building})
-
-    env = env.transpose()
-    for i in env.columns:
-        for j in newLegends.keys():
-            if i.replace("__Building"+str(building), "") in j:
-                env = env.rename(columns={i: newLegends[j]})
-
-    production = pd.DataFrame.from_dict(production, orient='index')
-    production = production.transpose()
-
-    storage = pd.DataFrame.from_dict(storage, orient='index', columns=["dhw", "sh", "elec"])
-    storage = storage.transpose()
-
-    fig = plt.figure(figsize=(18, 8))
-    gs = gridspec.GridSpec(1, 4, width_ratios=[3, 4, 8, 3], wspace=0.03)
-
-    ax0 = plt.subplot(gs[0])
-    costs_colors = [toColor(COLORS, x) for x in costs.columns]
-    bp0 = costs.plot(ax=ax0, kind='barh', color=costs_colors, stacked=True, linewidth=0)
-
-    ax1 = plt.subplot(gs[1])
-    env_colors = [toColor(COLORS, x) for x in env.columns]
-    bp1 = env.plot(ax=ax1, kind='barh', color=env_colors, stacked=True, linewidth=0)
-
-    ax2 = plt.subplot(gs[2])
-    production_colors = [toColor(COLORS, x) for x in production.columns]
-    bp2 = production.plot(ax=ax2, kind='barh', color=production_colors, stacked=True, linewidth=0, width=.5)
-
-    ax3 = plt.subplot(gs[3])
-    storage_colors = [toColor(COLORS, x) for x in storage.columns]
-    bp3 = storage.plot(ax=ax3, kind='barh', color=storage_colors, stacked=True, linewidth=0)
-
-    # remove scenario names from other bar plots
-    for ax in [ax1, ax2]:
-        ax.set_yticklabels('')
-    for ax in [ax2, ax3]:
-        groupHbarPlots(ax, group_size=3, inner_sep=0.01)
-    ax3.yaxis.tick_right()
-
-    # set limits and ticks for both axes
-    for ax in [ax0, ax1, ax2, ax3]:
-        ax.yaxis.grid(False)
-        ax.xaxis.grid(True, 'major', linestyle='-')
-        ax.xaxis.set_ticks_position('none')
-        ax.yaxis.set_ticks_position('none')
-
-        # group 1,000,000 with commas
-        xmin, xmax = ax.get_xlim()
-        if xmax > 90 or xmin < -90:
-            group_thousands_and_skip_first = tkr.FuncFormatter(
-                lambda x, pos: '' if pos == 0 else '{:0,d}'.format(int(x)))
-            ax.xaxis.set_major_formatter(group_thousands_and_skip_first)
-        else:
-            skip_lowest = tkr.FuncFormatter(
-                lambda x, pos: '' if pos == 0 else x)
-            ax.xaxis.set_major_formatter(skip_lowest)
-
-        # legend
-        # set style arguments
-        legend_style = {'frameon': False,
-                        'loc': 'lower center',
-                        'ncol': 2,
-                        'bbox_to_anchor': (0.5, .99)}
-        # get handels and labels, remove duplicate labels
-        handles, labels = deduplicateLegend(*ax.get_legend_handles_labels())
-        # set legend to use those
-        lg = ax.legend(handles, labels, **legend_style)
-        # finally, remove lines from patches
-        plt.setp(lg.get_patches(), linewidth=0)
-
-    ax0.set_xlabel('Total costs (CHF)')
-    ax1.set_xlabel('Total environmental impacts (kgCo2eq)')
-    ax2.set_xlabel('Total energy produced (kWh)')
-    ax3.set_xlabel('Retrieved energy (kWh)')
-    return fig, costs, env, production, storage
-
-
-def resultingDataDiagramLoop(elec, sh, dhw, costs, env, colors, buildings, newLegends):
-    """
-    Function inspired from the URBS platform https://github.com/ojdo/urbs/blob/1house/comp.py
-    Function plotting the graph comparing the different buildings/scenarios on costs, energy produced and energy
-    retrieved from storages
-    :param elec: list of dict type, optimization results
-    :param sh: list of dict type, optimization results
-    :param dhw: list of dict type, optimization results
-    :param costs: list of dict type, optimization results
-    :param env: list of dict type, optimization results
-    :param colors: list type, different colors for the different components of the system
-    :param buildings: list of str type, name of the different buildings
-    :return: figure created
-    """
-    n_costs, n_env, n_production, n_storage = resultingDataDiagram(elec[0], sh[0], dhw[0], costs[0], env[0], colors, buildings[0], newLegends)[1:]
-    for i in range(1, len(elec)):
-        a, b, c, d = resultingDataDiagram(elec[i], sh[i], dhw[i], costs[i], env[i], colors, buildings[i],newLegends)[1:]
-        n_costs = pd.concat([n_costs, a])
-        n_env = pd.concat([n_env, b])
-        n_production = pd.concat([n_production, c])
-        n_storage = pd.concat([n_storage, d])
-
-    fig = plt.figure(figsize=(18, 8))
-    gs = gridspec.GridSpec(1, 4, width_ratios=[4, 3, 8, 3], wspace=0.03)
-
-    ax0 = plt.subplot(gs[0])
-    costs_colors = [toColor(colors, x) for x in n_costs.columns]
-    bp0 = n_costs.plot(ax=ax0, kind='barh', color=costs_colors, stacked=True, linewidth=0)
-
-    ax1 = plt.subplot(gs[1])
-    env_colors = [toColor(colors, x) for x in n_env.columns]
-    bp1 = n_env.plot(ax=ax1, kind='barh', color=env_colors, stacked=True, linewidth=0)
-
-    ax2 = plt.subplot(gs[2])
-    production_colors = [toColor(colors, x) for x in n_production.columns]
-    bp2 = n_production.plot(ax=ax2, kind='barh', color=production_colors, stacked=True, linewidth=0, width=.5)
-
-    ax3 = plt.subplot(gs[3])
-    storage_colors = [toColor(colors, x) for x in n_storage.columns]
-    bp3 = n_storage.plot(ax=ax3, kind='barh', color=storage_colors, stacked=True, linewidth=0)
-
-    # remove scenario names from other bar plots
-    for ax in [ax1, ax2, ax3]:
-        ax.set_yticklabels('')
-    for ax in [ax2, ax3]:
-        groupHbarPlots(ax, group_size=3, inner_sep=0.01)
-
-    # set limits and ticks for both axes
-    for ax in [ax0, ax1, ax2, ax3]:
-        ax.yaxis.grid(False)
-        ax.xaxis.grid(True, 'major', linestyle='-')
-        ax.xaxis.set_ticks_position('none')
-        ax.yaxis.set_ticks_position('none')
-
-        # group 1,000,000 with commas
-        xmin, xmax = ax.get_xlim()
-        if xmax > 90 or xmin < -90:
-            group_thousands_and_skip_first = tkr.FuncFormatter(
-                lambda x, pos: '' if pos == 0 else '{:0,d}'.format(int(x)))
-            ax.xaxis.set_major_formatter(group_thousands_and_skip_first)
-        else:
-            skip_lowest = tkr.FuncFormatter(
-                lambda x, pos: '' if pos == 0 else x)
-            ax.xaxis.set_major_formatter(skip_lowest)
-
-        # legend
-        # set style arguments
-        legend_style = {'frameon': False,
-                        'loc': 'lower center',
-                        'ncol': 2,
-                        'bbox_to_anchor': (0.5, .99)}
-        # get handels and labels, remove duplicate labels
-        handles, labels = deduplicateLegend(*ax.get_legend_handles_labels())
-        # set legend to use those
-        lg = ax.legend(handles, labels, **legend_style)
-        # finally, remove lines from patches
-        plt.setp(lg.get_patches(), linewidth=0)
-
-    ax0.set_xlabel('Total costs (CHF)')
-    ax1.set_xlabel('Total environmental impacts (kgCo2eq)')
-    ax2.set_xlabel('Total energy produced (kWh)\n First line: electricity, Second line: space heating,\n Third line: domestic hot water')
-    ax3.set_xlabel('Retrieved energy (kWh)\n First line: electricity, Second line: space heating,\n Third line: domestic hot water')
-
-    return fig
-
-def resultingDataDemandDiagram(elBus, shBus, dhwBus, COLORS, building, newLegends):
-    """
-    Function inspired from the URBS platform https://github.com/ojdo/urbs/blob/1house/comp.py
-    Function plotting the different results of the optimization. First, costs will be plotted, then the energy produced,
-    comparing energy for electricity bus, sh and dhw bus, and finally the retrieved energy from the storages.
-    :param elBus: dict type, results from the optimization applied to one bus. Called like "solph.views.node(results, bus)"
-    :param shBus: dict type, results from the optimization applied to one bus. Called like "solph.views.node(results, bus)"
-    :param dhwBus: dict type, results from the optimization applied to one bus. Called like "solph.views.node(results, bus)"
-    :param COLORS: list type, different colors for the different components of the system
-    :param building: str type, name of the building
-    :return: Three bar plots and the elec, sh and dhw dict created
-    """
-    elec = {}
-    sh = {}
-    dhw = {}
-    if optMode == "group":
-        list = []
-    for flow in elBus.keys():
-        if "Demand" in flow:
-            elec[newLegends[flow.replace("__Building"+str(building), "")]] = [0, 0, sum(elBus[flow])]
-        elif "producedElectricity" in flow or "gridElectricity" in flow:
-            elec[newLegends[flow.replace("__Building" + str(building), "")]] = [0, sum(elBus[flow]), 0]
-        elif optMode == "group" and "electricityLink" in flow and "_in" not in newLegends[flow.replace("__Building" + str(building), "")]:
-            if newLegends[flow.replace("__Building" + str(building), "")] in list:
-                elec[newLegends[flow.replace("__Building" + str(building), "")]][0] += sum(elBus[flow])
-            else:
-                elec[newLegends[flow.replace("__Building" + str(building), "")]] = [sum(elBus[flow]), 0, 0]
-                list.append(newLegends[flow.replace("__Building" + str(building), "")])
-        else:
-            elec[newLegends[flow.replace("__Building"+str(building), "")]] = [sum(elBus[flow]), 0, 0]
-
-        if "Storage" in flow and "in" in newLegends[flow.replace("__Building"+str(building), "")]:
-            del elec[newLegends[flow.replace("__Building"+str(building), "")]]
-        elif "electricity" not in flow[5:] and "Demand" not in flow:
-            del elec[newLegends[flow.replace("__Building" + str(building), "")]]
-        elif "Resource" in flow or "excess" in flow:
-            del elec[newLegends[flow.replace("__Building" + str(building), "")]]
-
-    for flow in shBus.keys():
-        if "Demand" in flow:
-            sh[newLegends[flow.replace("__Building" + str(building), "")]] = [0, 0, sum(shBus[flow])]
-        else:
-            sh[newLegends[flow.replace("__Building" + str(building), "")]] = [0, sum(shBus[flow]), 0]
-        if "Storage" in flow and "in" in newLegends[flow.replace("__Building"+str(building), "")]:
-            del sh[newLegends[flow.replace("__Building"+str(building), "")]]
-
-    for flow in dhwBus.keys():
-        if "Demand" in flow:
-            dhw[newLegends[flow.replace("__Building" + str(building), "")]] = [0, 0, sum(dhwBus[flow])]
-        else:
-            dhw[newLegends[flow.replace("__Building" + str(building), "")]] = [0, sum(dhwBus[flow]), 0]
-
-        if "Storage_" in flow:
-            del dhw[newLegends[flow.replace("__Building"+str(building), "")]]
-
-    elec = pd.DataFrame.from_dict(elec, orient='index')
-    elec = elec.transpose()
-
-    sh = pd.DataFrame.from_dict(sh, orient='index')
-    sh = sh.transpose()
-
-    dhw = pd.DataFrame.from_dict(dhw, orient='index')
-    dhw = dhw.transpose()
-
-    fig = plt.figure(figsize=(18, 8))
-    gs = gridspec.GridSpec(1, 3, wspace=0.1)
-
-    ax0 = plt.subplot(gs[0])
-    elec_colors = [toColor(COLORS, x) for x in elec.columns]
-    bp0 = elec.plot(ax=ax0, kind='barh', color=elec_colors, stacked=True, linewidth=0, width=.5)
-
-    ax1 = plt.subplot(gs[1])
-    sh_colors = [toColor(COLORS, x) for x in sh.columns]
-    bp1 = sh.plot(ax=ax1, kind='barh', color=sh_colors, stacked=True, linewidth=0)
-
-    ax2 = plt.subplot(gs[2])
-    dhw_colors = [toColor(COLORS, x) for x in dhw.columns]
-    bp2 = dhw.plot(ax=ax2, kind='barh', color=dhw_colors, stacked=True, linewidth=0)
-
-    # remove scenario names from other bar plots
-    ax0.set_yticklabels(('', '', 'Building '+str(building)))
-    for ax in [ax1, ax2]:
-        ax.set_yticklabels('')
-    for ax in [ax0, ax1, ax2]:
-        groupHbarPlots(ax, group_size=3, inner_sep=0.0)
-
-    # set limits and ticks for both axes
-    for ax in [ax0, ax1, ax2]:
-        ax.yaxis.grid(False)
-        ax.xaxis.grid(True, 'major', linestyle='-')
-        ax.xaxis.set_ticks_position('none')
-        ax.yaxis.set_ticks_position('none')
-
-        # group 1,000,000 with commas
-        xmin, xmax = ax.get_xlim()
-        if xmax > 90 or xmin < -90:
-            group_thousands_and_skip_first = tkr.FuncFormatter(
-                lambda x, pos: '' if pos == 0 else '{:0,d}'.format(int(x)))
-            ax.xaxis.set_major_formatter(group_thousands_and_skip_first)
-        else:
-            skip_lowest = tkr.FuncFormatter(
-                lambda x, pos: '' if pos == 0 else x)
-            ax.xaxis.set_major_formatter(skip_lowest)
-
-        # legend
-        # set style arguments
-        legend_style = {'frameon': False,
-                        'loc': 'lower center',
-                        'ncol': 3,
-                        'bbox_to_anchor': (0.5, .99)}
-        # get handels and labels, remove duplicate labels
-        handles, labels = deduplicateLegend(*ax.get_legend_handles_labels())
-        # set legend to use those
-        lg = ax.legend(handles, labels, **legend_style)
-        # finally, remove lines from patches
-        plt.setp(lg.get_patches(), linewidth=0)
-
-    ax0.set_xlabel('Demand and energy produced\n for electricity (kWh)')
-    ax1.set_xlabel('Demand and energy produced\n for space heating (kWh)')
-    ax2.set_xlabel('Demand and energy produced\n for domestic hot water (kWh)')
-
-    return fig, elec, sh, dhw
-
-def resultingDataDemandDiagramLoop(elec, sh, dhw, colors, buildings, newLegends):
-    """
-    Function inspired from the URBS platform https://github.com/ojdo/urbs/blob/1house/comp.py
-    Function plotting the graph comparing the different buildings/scenarios on costs, energy produced and energy
-    retrieved from storages
-    :param elec: list of dict type, optimization results
-    :param sh: list of dict type, optimization results
-    :param dhw: list of dict type, optimization results
-    :param colors: list type, different colors for the different components of the system
-    :param buildings: list of str type, name of the different buildings
-    :return: figure created
-    """
-    n_elec, n_sh, n_dhw = resultingDataDemandDiagram(elec[0], sh[0], dhw[0], colors, int(buildings[0]))[1:]
-    for i in range(1, len(elec)):
-        a, b, c = resultingDataDemandDiagram(elec[i], sh[i], dhw[i], colors, buildings[i])[1:]
-        n_elec = pd.concat([n_elec, a])
-        n_sh = pd.concat([n_sh, b])
-        n_dhw = pd.concat([n_dhw, c])
-
-    fig = plt.figure(figsize=(18, 8))
-    gs = gridspec.GridSpec(1, 3, wspace=0.1)
-
-    ax0 = plt.subplot(gs[0])
-    elec_colors = [toColor(colors, x) for x in n_elec.columns]
-    bp0 = n_elec.plot(ax=ax0, kind='barh', color=elec_colors, stacked=True, linewidth=0, width=.5)
-
-    ax1 = plt.subplot(gs[1])
-    sh_colors = [toColor(colors, x) for x in n_sh.columns]
-    bp1 = n_sh.plot(ax=ax1, kind='barh', color=sh_colors, stacked=True, linewidth=0)
-
-    ax2 = plt.subplot(gs[2])
-    dhw_colors = [toColor(colors, x) for x in n_dhw.columns]
-    bp2 = n_dhw.plot(ax=ax2, kind='barh', color=dhw_colors, stacked=True, linewidth=0)
-
-    # remove scenario names from other bar plots
-    liste = []
-    for i in buildings:
-        liste.append('')
-        liste.append('')
-        liste.append('Building '+str(i))
-    ax0.set_yticklabels(liste)
-    for ax in [ax1, ax2]:
-        ax.set_yticklabels('')
-    for ax in [ax0, ax1, ax2]:
-        groupHbarPlots(ax, group_size=3, inner_sep=0.0)
-
-    # set limits and ticks for both axes
-    for ax in [ax0, ax1, ax2]:
-        ax.yaxis.grid(False)
-        ax.xaxis.grid(True, 'major', linestyle='-')
-        ax.xaxis.set_ticks_position('none')
-        ax.yaxis.set_ticks_position('none')
-
-        # group 1,000,000 with commas
-        xmin, xmax = ax.get_xlim()
-        if xmax > 90 or xmin < -90:
-            group_thousands_and_skip_first = tkr.FuncFormatter(
-                lambda x, pos: '' if pos == 0 else '{:0,d}'.format(int(x)))
-            ax.xaxis.set_major_formatter(group_thousands_and_skip_first)
-        else:
-            skip_lowest = tkr.FuncFormatter(
-                lambda x, pos: '' if pos == 0 else x)
-            ax.xaxis.set_major_formatter(skip_lowest)
-
-        # legend
-        # set style arguments
-        legend_style = {'frameon': False,
-                        'loc': 'lower center',
-                        'ncol': 3,
-                        'bbox_to_anchor': (0.5, .99)}
-        # get handels and labels, remove duplicate labels
-        handles, labels = deduplicateLegend(*ax.get_legend_handles_labels())
-        # set legend to use those
-        lg = ax.legend(handles, labels, **legend_style)
-        # finally, remove lines from patches
-        plt.setp(lg.get_patches(), linewidth=0)
-
-    ax0.set_xlabel('Demand and energy produced\n for electricity (kWh)')
-    ax1.set_xlabel('Demand and energy produced\n for space heating (kWh)')
-    ax2.set_xlabel('Demand and energy produced\n for domestic hot water (kWh)')
-
-    return fig
-
-
-def getData(filepath):
-    """
-    Function for the results recovery from an Excel file
-    :param filepath: path to the Excel containing the results of the optimization
-    :return: the different dicts created during the optimization
-    """
-    wb = load_workbook(filepath, read_only=True, keep_links=False)
-    dict_sheet = {}
-    for sheet in wb.sheetnames:
-        dict_sheet[sheet] = pd.read_excel(filepath, sheet_name=sheet, index_col=0, engine='openpyxl')
-
-    return dict_sheet
-
-def loadPlottingData(resultFilePath, numberOfBuildings):
-    """
-    Function for loading the data from excel file into variables
-    :param resultFilePath: path to the Excel containing the results of the optimization
-    :return: the different variables created after reading the excel file
-    """
-    buses = getData(resultFilePath)
-    elec_names = []
-    elec_dict = []
-    sh_names = []
-    sh_dict = []
-    dhw_names = []
-    dhw_dict = []
-    costs_names = []
-    costs_dict = []
-    env_names = []
-    env_dict = []
-
-    buildings_dict = []
-    buildings_names = []
-    buildings_number = []
-    beta = list(buses.keys())
-    for i in beta:
-        alpha = []
-        alpha_a = []
-        # Merged buses, if present, are assigned to Building 1 for plotting
-        if i in ["electricityBus", "electricityInBus", "domesticHotWaterBus", "dhwDemandBus", "spaceHeatingBus", "shDemandBus"]:
-            i = i + f'__Building{building}'
-        building = i.split("Building")[1]  # building number
-        beta_bis = beta.copy()
-        firstElBus = True
-        firstShBus = True
-        firstDhwBus = True
-        for j in beta:
-            if any('Building' in v for v in beta) and any(f'Building{building}' in v for v in beta):
-                j_buses = j
-                # Merged buses, if present, are assigned to Building 1 for plotting
-                if j in ["electricityBus", "electricityInBus", "domesticHotWaterBus", "dhwDemandBus", "spaceHeatingBus",
-                         "shDemandBus"]:
-                    j = j + f'__Building{building}'
-                if j.endswith(building) and (
-                        "electricityBus" in j or "electricityInBus" in j or "electricityProdBus" in j or "spaceHeatingBus" in j or "shDemandBus" in j or "shSourceBus" in j or "domesticHotWaterBus" in j or "dhwDemandBus" in j):
-                    """if "shDemandBus" not in j and "shSourceBus" not in j and "dhwDemandBus" not in j:
-                        alpha.append(j)"""
-                    if firstElBus and "electricity" in j:
-                        alpha.append(f"electricityBus__Building{building}")
-                        firstElBus = False
-                    elif firstShBus and ("spaceHeatingBus" in j or "shDemandBus" in j or "shSourceBus" in j):
-                        alpha.append(f"spaceHeatingBus__Building{building}")
-                        firstShBus = False
-                    elif firstDhwBus and ("domesticHotWaterBus" in j or "dhwDemandBus" in j):
-                        alpha.append(f"domesticHotWaterBus__Building{building}")
-                        firstDhwBus = False
-                    if j_buses != j:
-                        building_df = buses[j_buses].loc[:, buses[j_buses].columns.str.contains(
-                            f'Building{building}')]  # extract columns related to a given building
-                        if building == '1':
-                            building_df = pd.concat(
-                                [building_df, buses[j_buses].loc[:, ~buses[j_buses].columns.str.contains(f'Building')]],
-                                axis=1)
-                    else:
-                        building_df = buses[j_buses]
-                    if ("electricityBus" in j) or ("electricityInBus" in j) or ("electricityProdBus" in j):
-                        # find the index of electricity bus to merge the results of electricityBus, electricityInBus and electricityProdBus
-                        index = -1
-                        for ind in range(len(alpha_a)):
-                            if "electricityBus" in alpha_a[ind].keys()[0] or "electricityInBus" in alpha_a[ind].keys()[0] or "electricityProdBus" in alpha_a[ind].keys()[0]:
-                                index = ind
-                        if index != -1:
-                                alpha_a[index] = pd.concat((alpha_a[index], building_df), axis=1)
-                        else:
-                            alpha_a.append(building_df)
-                    elif ("spaceHeatingBus" in j) or ("shDemandBus" in j) or ("shSourceBus" in j):
-                        # find the index of spaceHeatingBus to merge the results of spaceHeatingBus, shDemandBus and shSourceBus
-                        index = -1
-                        for ind in range(len(alpha_a)):
-                            if "spaceHeatingBus" in alpha_a[ind].keys()[0] or "shDemandBus" in alpha_a[ind].keys()[0] or "shSourceBus" in alpha_a[ind].keys()[0]:
-                                index = ind
-                        if index != -1:
-                            alpha_a[index] = pd.concat((alpha_a[index], building_df), axis=1)
-                        else:
-                            index = len(alpha_a)
-                            alpha_a.append(building_df)
-                        flows_to_delete = [
-                            f"(('spaceHeating__Building{building}', 'shDemandBus__Building{building}'), 'flow')",
-                            f"(('shSourceBus__Building{building}', 'shSource__Building{building}'), 'flow')",
-                            f"(('spaceHeating', 'shDemandBus'), 'flow')"]
-                        for flow in flows_to_delete:
-                            if flow in alpha_a[index].columns:
-                                alpha_a[index].pop(flow)
-                    else:
-                        # find the index of domesticHotWaterBus to merge the results of domesticHotWaterBus and dhwDemandBus
-                        index = -1
-                        for ind in range(len(alpha_a)):
-                            if "domesticHotWaterBus" in alpha_a[ind].keys()[0] or "dhwDemandBus" in alpha_a[ind].keys()[0]:
-                                index = ind
-                        if index != -1:
-                            alpha_a[index] = pd.concat((alpha_a[index], building_df), axis=1)
-                        else:
-                            index = len(alpha_a)
-                            alpha_a.append(building_df)
-                        flows_to_delete = [
-                            f"(('domesticHotWater__Building{building}', 'dhwDemandBus__Building{building}'), 'flow')",
-                            f"(('domesticHotWater', 'dhwDemandBus'), 'flow')"]
-                        for flow in flows_to_delete:
-                            if flow in alpha_a[index].columns:
-                                alpha_a[index].pop(flow)
-                    beta_bis.remove(j_buses)
-        if alpha != []:
-            buildings_dict.append(alpha_a)
-            buildings_names.append(alpha)
-            buildings_number.append(building)
-        """for a in alpha:
-            beta.remove(a)"""
-        beta = [x for x in beta if f"Building{building}" not in x]
-
-    firstShBus = True
-    firstDhwBus = True
-    mergedElBuses = []
-    mergedShBuses = []
-    mergedDhwBuses = []
-    mergedLinks = False
-    b = 1  # initial building number
-    for i in buses.keys():
-        i_buses = i
-        if 'Building' in i:
-            b = int(i.split("Building")[1])  # building number
-        # Merged buses, if present, are assigned to Building 1 for plotting
-        if i in ["electricityBus", "electricityInBus", "domesticHotWaterBus", "dhwDemandBus", "spaceHeatingBus",
-                 "shDemandBus"]:
-            i = i + f'__Building{b}'
-        tt = {}
-
-        if i_buses != i:
-            if 'electricity' in i:
-                mergedElBuses.append(i_buses)
-            elif 'spaceHeating' in i or 'shDemand' in i:
-                mergedShBuses.append(i_buses)
-            else:
-                mergedDhwBuses.append(i_buses)
-            mergedLinks = True
-            building_df = buses[i_buses].loc[:, buses[i_buses].columns.str.contains(
-                f'Building{b}')]  # extract columns related to a given building
-            if b == 1:
-                building_df = pd.concat(
-                    [building_df, buses[i_buses].loc[:, ~buses[i_buses].columns.str.contains(f'Building')]], axis=1)
-        else:
-            building_df = buses[i_buses]
-
-        if ("electricityBus" in i) or ("electricityInBus" in i) or ("electricityProdBus" in i):
-            if b != 1 and mergedLinks:
-                for elBusName in mergedElBuses:
-                    elec_names.append(elBusName + f"__Building{b}")
-                    mergedbus_df = buses[elBusName].loc[:, buses[elBusName].columns.str.contains(f'Building{b}')]
-                    if b <= len(
-                            elec_dict):  # to merge the data of the two electricity buses of the same  (elec_dict[0] should have all the electricity related data of building 1, and so on...)
-                        elec_dict[b - 1] = pd.concat((elec_dict[b - 1], mergedbus_df), axis=1)
-                    else:
-                        elec_dict.append(mergedbus_df)
-            elec_names.append(i)
-            if b <= len(
-                    elec_dict):  # to merge the data of the two electricity buses of the same  (elec_dict[0] should have all the electricity related data of building 1, and so on...)
-                elec_dict[b - 1] = pd.concat((elec_dict[b - 1], building_df), axis=1)
-            else:
-                elec_dict.append(building_df)
-
-        if ("spaceHeating" in i) or ("shDemand" in i) or ("shSource" in i):
-            if any(str(b) not in v for v in sh_names):
-                firstShBus=True
-            if b != 1 and mergedLinks:
-                for shBusName in mergedShBuses:
-                    mergedbus_df = buses[shBusName].loc[:, buses[shBusName].columns.str.contains(f'Building{b}')]
-                    if firstShBus:
-                        sh_names.append(i)
-                        sh_dict.append(mergedbus_df)
-                        firstShBus = False
-                    else:
-                        ind = len(sh_names) - 1
-                        sh_dict[ind] = pd.concat((sh_dict[ind], mergedbus_df), axis=1)
-                        flows_to_delete = [f"(('spaceHeating__Building{b}', 'shDemandBus__Building{b}'), 'flow')",
-                                           f"(('shSourceBus__Building{b}', 'shSource__Building{b}'), 'flow')",
-                                           f"(('spaceHeating', 'shDemandBus'), 'flow')"]
-                        for flow in flows_to_delete:
-                            if flow in sh_dict[ind].columns:
-                                sh_dict[ind].pop(flow)
-            if firstShBus:
-                sh_names.append(i)
-                sh_dict.append(building_df)
-                firstShBus = False
-            else:
-                ind = len(sh_names) - 1
-                sh_dict[ind] = pd.concat((sh_dict[ind], building_df), axis=1)
-                flows_to_delete = [f"(('spaceHeating__Building{b}', 'shDemandBus__Building{b}'), 'flow')",
-                    f"(('shSourceBus__Building{b}', 'shSource__Building{b}'), 'flow')",
-                    f"(('spaceHeating', 'shDemandBus'), 'flow')"]
-                for flow in flows_to_delete:
-                    if flow in sh_dict[ind].columns:
-                        sh_dict[ind].pop(flow)
-        if ("domesticHotWater" in i) or ("dhwDemand" in i):
-            if any(str(b) not in v for v in dhw_names):
-                firstDhwBus=True
-            if firstDhwBus:
-                dhw_names.append(i)
-                dhw_dict.append(building_df)
-                firstDhwBus = False
-            else:
-                ind = len(dhw_names) - 1
-                dhw_dict[ind] = pd.concat((dhw_dict[ind], building_df), axis=1)
-                flows_to_delete = [f"(('domesticHotWater__Building{b}', 'dhwDemandBus__Building{b}'), 'flow')",
-                                   f"(('domesticHotWater', 'dhwDemandBus'), 'flow')"]
-                for flow in flows_to_delete:
-                    if flow in dhw_dict[ind].columns:
-                        dhw_dict[ind].pop(flow)
-        if b != 1 and mergedLinks and "dhwStorageBus" in i:
-            if any(str(b) not in v for v in dhw_names):
-                firstDhwBus=True
-            for dhwBusName in mergedDhwBuses:
-                mergedbus_df = buses[dhwBusName].loc[:, buses[dhwBusName].columns.str.contains(f'Building{b}')]
-                if firstDhwBus:
-                    dhw_names.append(f'domesticHotWaterBus__Building{b}')
-                    dhw_dict.append(mergedbus_df)
-                    firstDhwBus = False
-                else:
-                    ind = len(dhw_names) - 1
-                    dhw_dict[ind] = pd.concat((dhw_dict[ind], mergedbus_df), axis=1)
-                    flows_to_delete = [f"(('domesticHotWater__Building{b}', 'dhwDemandBus__Building{b}'), 'flow')",
-                                       f"(('domesticHotWater', 'dhwDemandBus'), 'flow')"]
-                    for flow in flows_to_delete:
-                        if flow in dhw_dict[ind].columns:
-                            dhw_dict[ind].pop(flow)
-        if "costs" in i:
-            costs_names.append(i)
-            costs_dict.append(buses[i_buses])
-        if "env_impacts" in i:
-            env_names.append(i)
-            env_dict.append(buses[i_buses])
-
-    return buses, elec_names, elec_dict, sh_names, sh_dict, dhw_names, dhw_dict, costs_names, costs_dict, env_names, env_dict,\
-           buildings_dict, buildings_names, buildings_number
-
-def createPlot(resultFilePath, basePath, numberOfBuildings, plotLevel, plotType, flowType, plotAnnualHorizontalBar, newLegends):
-    # load the plotting data from excel file into variables
-    buses, elec_names, elec_dict, sh_names, sh_dict, dhw_names, dhw_dict, costs_names, costs_dict, env_names, env_dict, \
-    buildings_dict, buildings_names, buildings_number = loadPlottingData(resultFilePath, numberOfBuildings)
-
-    if flowType == "all":
-        if plotType == "energy balance":
-            names = elec_names + sh_names + dhw_names
-        elif plotType == "bokeh":
-            names = buildings_names
-            dict = buildings_dict
-    elif flowType == "electricity":
-        names = elec_names
-        if plotType == "bokeh":
-            dict = elec_dict
-    elif flowType == "space heat":
-        names = sh_names
-        if plotType == "bokeh":
-            dict = sh_dict
-    elif flowType == "domestic hot water":
-        names = dhw_names
-        if plotType == "bokeh":
-            dict = dhw_dict
-    else:
-        raise ValueError("Illegal value for the parameter flow type")
-
-    months = ["Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"]
-
-    if plotType == "energy balance":
-        if plotLevel == "allMonths":
-            for i in names:
-                if "electricityBus" not in i:
-                    monthlyBalance(buses[i], i, newLegends)
-    elif plotType == "bokeh":
-        ncols = 2
-        if plotLevel in months:
-            if flowType == "all":
-                for i in range(len(buildings_names)):
-                    tempDict = dict[i]
-                    for j in range(len(tempDict)):
-                        tempDict[j] = tempDict[j][tempDict[j].index.strftime('%b') == plotLevel]
-                    dict[i] = tempDict
-            else:
-                for i in range(len(dict)):
-                    dict[i] = dict[i][dict[i].index.strftime('%b') == plotLevel]
-
-        elif any(chr.isdigit() for chr in plotLevel):
-            if isoparse(plotLevel):
-                if flowType == "all":
-                    for i in range(len(buildings_names)):
-                        tempDict = dict[i]
-                        for j in range(len(tempDict)):
-                            tempDict[j] = tempDict[j][tempDict[j].index.date == datetime.strptime(plotLevel, "%Y-%m-%d").date()]
-                        dict[i] = tempDict
-                else:
-                    for i in range(len(dict)):
-                        dict[i] = dict[i][dict[i].index.date == datetime.strptime(plotLevel, "%Y-%m-%d").date()]
-
-        if flowType == "all":
-            plotsHourly = []
-            plotsDaily = []
-            for i in range(len(buildings_names)):
-                plotsH, plotsD = hourlyDailyPlot(dict[i], names[i], Category20_12, newLegends)
-                plotsHourly.extend(plotsH)
-                plotsDaily.extend(plotsD)
-        else:
-            plotsHourly, plotsDaily = hourlyDailyPlot(dict, names, Set1_9, newLegends)
-
-        if not os.path.exists(basePath):
-            os.makedirs(basePath)
-
-        output_file(os.path.join(basePath,"HourlyBokehPlots.html"))
-        grid = gridplot(plotsHourly, ncols=ncols, plot_width=850, plot_height=500, sizing_mode="fixed")
-        show(grid)
-        if not any(chr.isdigit() for chr in plotLevel):
-            output_file(os.path.join(basePath,"DailyBokehPlots.html"))
-            grid = gridplot(plotsDaily, ncols=ncols, plot_width=850, plot_height=500, sizing_mode="fixed")
-            show(grid)
-    else:
-        raise ValueError("Illegal value for the parameter plot type")
-
-    if plotAnnualHorizontalBar == True:
-        my_colors = {
-            'Battery_out': (100, 160, 200),
-            'Battery_in': (100, 160, 200),
-            'Storage_sh_out': (196, 7, 27),
-            'Storage_dhw_out': (196, 7, 27),
-            'HP_dhw': (62, 173, 0),
-            'HP_sh': (62, 173, 0),
-            'HP': (62, 173, 0),
-            'CHP_elec': (0, 101, 189),
-            'CHP_sh': (0, 101, 189),
-            'CHP_dhw': (128, 0, 128),
-            'CHP': (0, 101, 189),
-            'Gas_sh': (0, 110, 120),
-            'GasBoiler': (0, 110, 120),
-            'PV_elec': (0, 128, 90),
-            'SolarCollector': (188, 128, 90),
-            'Inputs': (252, 93, 93),
-            'Operation': (252, 93, 93),
-            'Investment': (0, 119, 138),
-            'Feed-in': (0, 215, 203),
-            'Demand_elec': (131, 166, 151),
-            'Demand_sh': (131, 166, 151),
-            'Demand_dhw': (131, 166, 151),
-            'Grid_purchase': (237, 127, 16)
-        }
-        if optMode == "group":
-            my_colors['electricityLink_in'] = (255, 215, 0)
-            my_colors['electricityLink_out'] = (255, 215, 0)
-            my_colors['electricityLink'] = (255, 215, 0)
-            
-        COLORS = {}
-        for name, color in my_colors.items():
-            COLORS[name] = color
-        """
-        for i in range(len(buildings_names)):
-            fig1 = resultingDataDiagram(elec_dict[i], sh_dict[i], dhw_dict[i], costs_dict[i], env_dict[i], COLORS, buildings_number[i])[0]
-            fig2 = resultingDataDemandDiagram(elec_dict[i], sh_dict[i], dhw_dict[i], COLORS, buildings_number[i])[0]
-        """
-        fig3 = resultingDataDiagramLoop(elec_dict, sh_dict, dhw_dict, costs_dict, env_dict, COLORS, buildings_number, newLegends)
-        fig4 = resultingDataDemandDiagramLoop(elec_dict, sh_dict, dhw_dict, COLORS, buildings_number,newLegends)
-        plt.show()
-
-
-def plot(excelFileName, figureFilePath, numberOfBuildings, plotLevel, plotType, flowType, plotlabels='default', plotAnnualHorizontalBar=False):
-    #####################################
-    ########## Classic plots  ###########
-    #####################################
-    # New legends need to be defined by hand for each new flow added to the energy network
-    if plotlabels == 'default':
-        newLegends = {
-            "(('naturalGasResource', 'naturalGasBus'), 'flow')": "NaturalGas",
-            "(('electricityBus', 'excesselectricityBus'), 'flow')": "Feed-in",
-            "(('electricityProdBus', 'electricalStorage'), 'flow')": "Battery_in",
-            "(('electricityInBus', 'electricityDemand'), 'flow')": "Demand_elec",
-            "(('electricityInBus', 'emobilityDemand'), 'flow')": "Demand_mobility",
-            "(('electricityInBus', 'HP'), 'flow')": "HP",
-            "(('electricityInBus', 'GWHP'), 'flow')": "GWHP",
-            "(('CHP', 'electricityProdBus'), 'flow')": "CHP_elec",
-            "(('electricalStorage', 'electricityBus'), 'flow')": "Battery_out",
-            "(('electricitySource', 'electricityBus'), 'flow')": "Elect_produced (not stored)",
-            "(('electricityResource', 'gridBus'), 'flow')": "Grid_purchase",
-            "(('dhwStorage', 'domesticHotWaterBus'), 'flow')": "Storage_dhw_out",
-            "(('dhwStorageBus', 'dhwStorage'), 'flow')": "Storage_dhw_in",
-            "(('domesticHotWaterBus', 'domesticHotWater'), 'flow')": "dhw_direct_to_load",
-            "(('dhwDemandBus', 'domesticHotWaterDemand'), 'flow')": "Demand_dhw",
-            "(('HP', 'dhwStorageBus'), 'flow')": "HP_dhw",
-            "(('GWHP', 'dhwStorageBus'), 'flow')": "GWHP_dhw",
-            "(('CHP', 'dhwStorageBus'), 'flow')": "CHP_dhw",
-            "(('shSource', 'spaceHeatingBus'), 'flow')": "SH_produced (not stored)",
-            "(('shStorage', 'spaceHeatingBus'), 'flow')": "Storage_sh_out",
-            "storage_content": "Storage_content",
-            "(('shSourceBus', 'shStorage'), 'flow')": "Storage_sh_in",
-            "(('spaceHeatingBus', 'spaceHeating'), 'flow')": "SH_direct_to_load",
-            "(('shDemandBus', 'spaceHeatingDemand'), 'flow')": "Demand_sh",
-            "(('shDemandBus', 'excessshDemandBus'), 'flow')": "Excess SH production",
-            "(('shSourceBus', 'excessshSourceBus'), 'flow')": "Excess SH production",
-            "(('CHP', 'shSourceBus'), 'flow')": "CHP_sh",
-            "(('GasBoiler', 'shSourceBus'), 'flow')": "Gas_sh",
-            "(('GasBoiler', 'dhwStorageBus'), 'flow')": "Gas_dhw",
-            "(('HP', 'shSourceBus'), 'flow')": "HP_sh",
-            "(('GWHP', 'shSourceBus'), 'flow')": "GWHP_sh",
-            "(('electricityBus', 'producedElectricity'), 'flow')": "Self_consumption",
-            "(('gridBus', 'gridElectricity'), 'flow')": "Electricity_grid",
-            "(('pv', 'electricityProdBus'), 'flow')": "PV_elec",
-            "(('solarCollector', 'dhwStorageBus'), 'flow')": "SolarCollector",
-            "(('electricityInBus', 'solarCollector'), 'flow')": "SolarCollector",
-            "(('gridElectricity', 'electricityInBus'), 'flow')": "Electricity_grid",
-            "(('producedElectricity', 'electricityInBus'), 'flow')": "Self_consumption",
-            "(('electricityProdBus', 'electricitySource'), 'flow')": "Battery_bypass",
-            "(('domesticHotWaterBus', 'domesticHotWaterDemand'), 'flow')": "Demand_dhw",
-            "(('electricityInBus', 'ElectricRod'), 'flow')": "Electric_rod",
-            "(('ElectricRod', 'shSourceBus'), 'flow')": "Electric_rod_sh",
-            "(('ElectricRod', 'dhwStorageBus'), 'flow')": "Electric_rod_dhw",
-            "(('electricityInBus', 'GWHP35'), 'flow')": "GWHP35",
-            "(('electricityInBus', 'GWHP60'), 'flow')": "GWHP60",
-            "(('GWHP60', 'dhwStorageBus'), 'flow')": "GWHP60_dhw",
-            "(('GWHP35', 'shSourceBus'), 'flow')": "GWHP35_sh",
-        }
-        newLegends["(('electricityBus', 'electricityLink'), 'flow')"] = "electricityLink_out"
-        newLegends["(('electricityLink', 'electricityInBus'), 'flow')"] = "electricityLink_in"
-        newLegends["(('spaceHeatingBus', 'shLink'), 'flow')"] = "shLink_out"
-        newLegends["(('shLink', 'shDemandBus'), 'flow')"] = "shLink_in"
-        newLegends["(('domesticHotWaterBus', 'dhwLink'), 'flow')"] = "dhwLink_out"
-        newLegends["(('dhwLink', 'dhwDemandBus'), 'flow')"] = "dhwLink_in"
-    else:
-        newLegends = {
-            "(('naturalGasResource', 'naturalGasBus'), 'flow')": plotlabels["naturalGas"],
-            "(('electricityBus', 'excesselectricityBus'), 'flow')": plotlabels["excessEl"],
-            "(('electricityProdBus', 'electricalStorage'), 'flow')": plotlabels["StorageEl"]+"_in",
-            "(('electricityInBus', 'electricityDemand'), 'flow')": plotlabels["DemandEl"],
-            "(('electricityInBus', 'emobilityDemand'), 'flow')": plotlabels["DemandMob"],
-            "(('electricityInBus', 'HP'), 'flow')": plotlabels["HP"],
-            "(('electricityInBus', 'GWHP'), 'flow')": plotlabels["GWHP"],
-            "(('CHP', 'electricityProdBus'), 'flow')": plotlabels["CHP"]+"_el",
-            "(('electricalStorage', 'electricityBus'), 'flow')": plotlabels["StorageEl"]+"_out",
-            "(('electricitySource', 'electricityBus'), 'flow')": plotlabels["localEl"],
-            "(('electricityResource', 'gridBus'), 'flow')": plotlabels["grid"],
-            "(('dhwStorage', 'domesticHotWaterBus'), 'flow')": plotlabels["StorageDhw"]+"_out",
-            "(('dhwStorageBus', 'dhwStorage'), 'flow')": plotlabels["StorageDhw"]+"_in",
-            "(('domesticHotWaterBus', 'domesticHotWater'), 'flow')": "DHW_direct_to_load",
-            "(('dhwDemandBus', 'domesticHotWaterDemand'), 'flow')": plotlabels["DemandDhw"],
-            "(('HP', 'dhwStorageBus'), 'flow')": plotlabels["HP"]+"_dhw",
-            "(('GWHP', 'dhwStorageBus'), 'flow')": plotlabels["GWHP"]+"_dhw",
-            "(('CHP', 'dhwStorageBus'), 'flow')": plotlabels["CHP"]+"_dhw",
-            "(('shSource', 'spaceHeatingBus'), 'flow')": plotlabels["prodSH"]+" (not stored)",
-            "(('shStorage', 'spaceHeatingBus'), 'flow')": plotlabels["StorageSh"]+"_out",
-            "storage_content": "Storage_content",
-            "(('shSourceBus', 'shStorage'), 'flow')": plotlabels["StorageSh"]+"_in",
-            "(('spaceHeatingBus', 'spaceHeating'), 'flow')": "SH_direct_to_load",
-            "(('shDemandBus', 'spaceHeatingDemand'), 'flow')": plotlabels["DemandSh"],
-            "(('shDemandBus', 'excessshDemandBus'), 'flow')": plotlabels["excessSh"],
-            "(('shSourceBus', 'excessshSourceBus'), 'flow')": plotlabels["excessSh"],
-            "(('CHP', 'shSourceBus'), 'flow')": plotlabels["CHP"]+"_sh",
-            "(('GasBoiler', 'shSourceBus'), 'flow')": plotlabels["gasBoiler"]+"_sh",
-            "(('GasBoiler', 'dhwStorageBus'), 'flow')": plotlabels["gasBoiler"]+"_dhw",
-            "(('HP', 'shSourceBus'), 'flow')": plotlabels["HP"]+"_sh",
-            "(('GWHP', 'shSourceBus'), 'flow')": plotlabels["GWHP"]+"_sh",
-            "(('electricityBus', 'producedElectricity'), 'flow')": "Self_consumption",
-            "(('gridBus', 'gridElectricity'), 'flow')": plotlabels["grid"],
-            "(('pv', 'electricityProdBus'), 'flow')": plotlabels["pv"]+"_el",
-            "(('solarCollector', 'dhwStorageBus'), 'flow')": plotlabels["solarCollector"],
-            "(('electricityInBus', 'solarCollector'), 'flow')": plotlabels["solarCollector"],
-            "(('gridElectricity', 'electricityInBus'), 'flow')": plotlabels["grid"],
-            "(('producedElectricity', 'electricityInBus'), 'flow')": "Self_consumption",
-            "(('electricityProdBus', 'electricitySource'), 'flow')": plotlabels["StorageEl"]+"_bypass",
-            "(('domesticHotWaterBus', 'domesticHotWaterDemand'), 'flow')": plotlabels["DemandDhw"],
-            "(('electricityInBus', 'ElectricRod'), 'flow')": plotlabels["ElectricRod"],
-            "(('ElectricRod', 'shSourceBus'), 'flow')": plotlabels["ElectricRod"]+"_sh",
-            "(('ElectricRod', 'dhwStorageBus'), 'flow')": plotlabels["ElectricRod"]+"_dhw",
-            "(('electricityInBus', 'GWHP35'), 'flow')": plotlabels["GWHP"]+"35",
-            "(('electricityInBus', 'GWHP60'), 'flow')": plotlabels["GWHP"]+"60",
-            "(('GWHP60', 'dhwStorageBus'), 'flow')": plotlabels["GWHP"]+"60_dhw",
-            "(('GWHP35', 'shSourceBus'), 'flow')": plotlabels["GWHP"]+"35_sh",
-        }
-        newLegends["(('electricityBus', 'electricityLink'), 'flow')"] = plotlabels["elBus"]+" Link (out)"
-        newLegends["(('electricityLink', 'electricityInBus'), 'flow')"] =plotlabels["elBus"]+" Link (in)"
-        newLegends["(('spaceHeatingBus', 'shLink'), 'flow')"] = plotlabels["shBus"]+" Link (out)"
-        newLegends["(('shLink', 'shDemandBus'), 'flow')"] = plotlabels["shBus"]+" Link (in)"
-        newLegends["(('domesticHotWaterBus', 'dhwLink'), 'flow')"] = plotlabels["dhwBus"]+" Link (out)"
-        newLegends["(('dhwLink', 'dhwDemandBus'), 'flow')"] = plotlabels["dhwBus"]+" Link (in)"
-
-    createPlot(excelFileName, figureFilePath, numberOfBuildings, plotLevel, plotType, flowType, plotAnnualHorizontalBar, newLegends)
-
-
-if __name__ == '__main__':
-
-    optMode = "group"  # parameter defining whether the results file corresponds to "indiv" or "group" optimization
-    numberOfBuildings = 4
-    plotOptim = 1  # defines the number of the optimization to plot
-    plotLevel = "allMonths"  # permissible values (for energy balance plot): "allMonths" {for all months}
-    # or specific month {"Jan", "Feb", "Mar", etc. three letter abbreviation of the month name}
-    # or specific date {format: YYYY-MM-DD}
-    plotType = "energy balance"  # permissible values: "energy balance", "bokeh"
-    flowType = "electricity"  # permissible values: "all", "electricity", "space heat", "domestic hot water"
-    plotAnnualHorizontalBar = False  # determines whether the annual horizontal bar is plot or not
-
-    plot(os.path.join(r"..\data\Results", f"results{numberOfBuildings}_{plotOptim}_{optMode}.xlsx"), r"..\data\Figures", plotLevel, plotType, flowType, plotAnnualHorizontalBar)
+import matplotlib.pyplot as plt
+import matplotlib.gridspec as gridspec
+import matplotlib.ticker as tkr
+
+from bokeh.plotting import figure, show
+from bokeh.layouts import layout, gridplot
+from bokeh.models import DatetimeTickFormatter, HoverTool, Legend
+from bokeh.palettes import *
+from bokeh.io import output_file
+
+from openpyxl import load_workbook
+from datetime import datetime
+from dateutil.parser import isoparse
+import itertools
+import pandas as pd
+import os
+
+# This file defines different functions for the plotting of the results of the optimization.
+# The plots are made at the end of this file, introducing a .xls file previously created during the optimization.
+# An important parameter "optMode" needs to be set when running the code (look in the __main__ fragment)
+
+
+def monthlyBalance(data, bus, new_legends):
+    """
+    Function for the definition of the monthly summary of a bus
+    :param data: dict type, results from the optimization applied to one bus
+    :param bus: str type, bus from which the summary is required
+    :param new_legends: dict type, new legends to plot on the graph
+    :return:
+    """
+    building = "__" + bus.split("__")[1]
+    data_month = data.resample('1m').sum()
+    monthShortNames = ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul', 'Aug', 'Sep', 'Oct', 'Nov', 'Dec']
+
+    while len(data_month) != len(monthShortNames):
+        data.drop(data.index[-1], inplace=True)
+        data_month = data.resample('1m').sum()
+    neg_flow = []
+    pos_flow = []
+    for i in data.columns:
+        a = [i.strip("()").split(", ")]
+        if "Bus" in a[0][0]:
+            neg_flow.append(i)
+        else:
+            pos_flow.append(i)
+    plt.figure()
+    mark = []
+    for i in neg_flow:
+        plt.bar(monthShortNames, -data_month[i], label=new_legends[i.replace(building, "")], bottom=sum(mark))
+        mark.append(-data_month[i])
+    mark = []
+    for i in pos_flow:
+        plt.bar(monthShortNames, data_month[i], label=new_legends[i.replace(building, "")], bottom=sum(mark))
+        mark.append(data_month[i])
+
+    ax = plt.gca()
+    # Shrink current axis by 20%
+    box = ax.get_position()
+    ax.set_position([box.x0, box.y0, box.width * 0.8, box.height])
+
+    # Put a legend to the right of the current axis
+    ax.legend(loc='center left', bbox_to_anchor=(1, 0.5))
+    plt.grid(axis='y')
+    if "electricity" in bus or "grid" in bus:
+        plt.title("Monthly electricity balance for " + building.replace("__", ""))
+    elif "spaceHeating" in bus:
+        plt.title("Monthly space heating balance for " + building.replace("__", ""))
+    else:
+        plt.title("Monthly domestic hot water balance for " + building.replace("__", ""))
+    plt.show()
+
+
+def hourlyDailyPlot(data, bus, palette, new_legends):
+    """
+    Function for the bokeh plot of hourly and daily balance of a bus
+    :param data: list of dict type, results from the optimization
+    :param bus: list of str type, buses from which the summary is required
+    :param palette: palette type form bokeh.palettes (For example, Category10_8), different types can be found on
+    https://docs.bokeh.org/en/latest/docs/reference/palettes.html or
+    https://docs.bokeh.org/en/latest/_modules/bokeh/palettes.html
+    :param new_legends: dict type, new legends to plot on the graph
+    For example, Category10_8
+    :return:
+    """
+    p_figs = []
+    p_figs_h = []
+    p_figs_d = []
+    p_plots = []
+    a = []
+    b = 1
+    bus = [x for x in bus if 'electricityProdBus' not in x and 'electricityInBus' not in x]
+    for i in range(0, len(data)):
+        building = '__' + bus[i].split("__")[1]
+
+        if "electricity" in bus[i]:
+            dt = data[i]
+            dt.pop(f"(('electricityProdBus{building}', 'electricitySource{building}'), 'flow')")
+            data_day = dt.resample('1d').sum()
+            p1 = figure(title="Hourly electricity flows for " + building.replace("__", ""), x_axis_label="Date", y_axis_label="Energy (kWh)", sizing_mode="scale_both")
+            p1.add_layout(Legend(), 'right')
+            p1.add_tools(HoverTool(tooltips=[('Time', '@x{%d/%m/%Y %H:%M:%S}'), ('Energy', '@y{0.00}')],
+                                   formatters={'@x': 'datetime'},
+                                   mode='mouse'))
+            p2 = figure(title="Daily electricity flows for " + building.replace("__", ""), x_axis_label="Date", y_axis_label="Energy (kWh)", sizing_mode="scale_both")
+            p2.add_layout(Legend(), 'right')
+            p2.add_tools(HoverTool(tooltips=[('Date', '@x{%d/%m/%Y}'), ('Energy', '@y{0.00}')],
+                                   formatters={'@x': 'datetime'},
+                                   mode='mouse'))
+            if len(p_figs_h) > 0:
+                p1.x_range = p_figs_h[0].x_range
+                p2.x_range = p_figs_d[0].x_range
+            colors = itertools.cycle(palette)
+            for j, color in zip(dt.columns, colors):
+                p1.line(dt.index, dt[j], legend_label=new_legends[j.replace(building, "")], color=color, line_width=1.5)
+                p2.line(data_day.index, data_day[j], legend_label=new_legends[j.replace(building, "")], color=color, line_width=1.5)
+            p_figs.append([p1, p2])
+            p_figs_h.append(p1)
+            p_figs_d.append(p2)
+            p_plots.append(p1)
+            p_plots.append(p2)
+
+        elif "shSource" in bus[i] or "spaceHeatingBus" in bus[i]:
+            dt = data[i]
+            data_day = dt.resample('1d').sum()
+            p3 = figure(title="Hourly space heating flows for " + building.replace("__", ""), x_axis_label="Date", y_axis_label="Energy (kWh)", sizing_mode="scale_both")
+            p3.add_layout(Legend(), 'right')
+            p3.add_tools(HoverTool(tooltips=[('Time', '@x{%d/%m/%Y %H:%M:%S}'), ('Energy', '@y{0.00}')],
+                                   formatters={'@x': 'datetime'},
+                                   mode='mouse'))
+            p4 = figure(title="Daily space heating flows for " + building.replace("__", ""), x_axis_label="Date", y_axis_label="Energy (kWh)", sizing_mode="scale_both")
+            p4.add_layout(Legend(), 'right')
+            p4.add_tools(HoverTool(tooltips=[('Date', '@x{%d/%m/%Y}'), ('Energy', '@y{0.00}')],
+                                   formatters={'@x': 'datetime'},
+                                   mode='mouse'))
+            if len(p_figs_h) > 0:
+                p3.x_range = p_figs_h[0].x_range
+                p4.x_range = p_figs_d[0].x_range
+            colors = itertools.cycle(palette)
+            for j, color in zip(dt.columns, colors):
+                p3.line(dt.index, dt[j], legend_label=new_legends[j.replace(building, "")], color=color, line_width=1.5)
+                p4.line(data_day.index, data_day[j], legend_label=new_legends[j.replace(building, "")], color=color, line_width=1.5)
+            p_figs.append([p3, p4])
+            p_figs_h.append(p3)
+            p_figs_d.append(p4)
+            p_plots.append(p3)
+            p_plots.append(p4)
+
+        else:
+            dt = data[i]
+            data_day = dt.resample('1d').sum()
+
+            p5 = figure(title="Hourly domestic hot water flows for " + building.replace("__", ""), x_axis_label="Date", y_axis_label="Energy (kWh)", sizing_mode="scale_both")
+            p5.add_layout(Legend(), 'right')
+            p5.add_tools(HoverTool(tooltips=[('Time', '@x{%d/%m/%Y %H:%M:%S}'), ('Energy', '@y{0.00}')],
+                                   formatters={'@x': 'datetime'},
+                                   mode='mouse'))
+            p6 = figure(title="Daily domestic hot water flows for "  + building.replace("__", ""), x_axis_label="Date", y_axis_label="Energy (kWh)", sizing_mode="scale_both")
+            p6.add_layout(Legend(), 'right')
+            p6.add_tools(HoverTool(tooltips=[('Date', '@x{%d/%m/%Y}'), ('Energy', '@y{0.00}')],
+                                   formatters={'@x': 'datetime'},
+                                   mode='mouse'))
+            if len(p_figs_h) > 0:
+                p5.x_range = p_figs_h[0].x_range
+                p6.x_range = p_figs_d[0].x_range
+            colors = itertools.cycle(palette)
+            for j, color in zip(dt.columns, colors):
+                p5.line(dt.index, dt[j], legend_label=new_legends[j.replace(building, "")], color=color, line_width=1.5)
+                p6.line(data_day.index, data_day[j], legend_label=new_legends[j.replace(building, "")], color=color, line_width=1.5)
+            p_figs.append([p5, p6])
+            p_figs_h.append(p5)
+            p_figs_d.append(p6)
+            p_plots.append(p5)
+            p_plots.append(p6)
+
+    for p in p_plots:
+        p.xaxis[0].formatter = DatetimeTickFormatter(months="%d %b")
+        p.legend.click_policy = "hide"
+        p.legend.location = "top_left"
+        p.legend.label_text_font_size = "8pt"
+
+    return (p_figs_h, p_figs_d)
+
+
+def toColor(COLORS, obj=None):
+    """
+    Function from the URBS platform https://github.com/ojdo/urbs/blob/1house/comp.py
+    Assign a deterministic pseudo-random color to argument.
+    If COLORS[obj] is set, return that. For strings, this value depends only
+    on the string content, so that same strings always yield the same color.
+    :param COLORS: dict of components and their assigned color
+    :param obj: any hashable object
+    :return: a (r, g, b) color tuple if COLORS[obj] is set, otherwise a hexstring
+    """
+    try:
+        color = tuple(rgb / 255.0 for rgb in COLORS[obj])
+    except KeyError:
+        # random deterministic color
+        import hashlib
+        color = '#' + hashlib.sha1(obj.encode()).hexdigest()[-6:]
+    return color
+
+
+def groupHbarPlots(ax, group_size, inner_sep=None):
+    """
+    Function from the URBS platform https://github.com/ojdo/urbs/blob/1house/comp.py
+    Group bars of a horizontal barplot closer together.
+    Given an existing horizontal bar plot handle ax, move bars of a given group size (>=2) closer together,
+    reducing the distance within the bars of a group, but increasing the distance between different groups.
+    By default, bars are placed within a coordinate system 1 unit apart. The space between two bars has
+    size 1 - bar_height, which can be specified in matplotlib (and pandas) using the `width` argument.
+    :param ax: matplotlib axis
+    :param group_size: int type, how many bars to group together
+    :param inner_sep: float type, vertical spacing within group (optional). Default: reduce the distance to a half
+    :return:
+    """
+    handles, labels = ax.get_legend_handles_labels()
+    bar_height = handles[0][0].get_height()  # assumption: identical for all
+
+    if inner_sep is None:
+        inner_sep = 0.5 * (1 - bar_height)
+
+    for column, handle in enumerate(handles):
+        for row, patch in enumerate(handle.patches):
+            group_number, row_within_group = divmod(row, group_size)
+
+            group_offset = (group_number * group_size
+                            + 0.5 * (group_size - 1) * (1 - inner_sep)
+                            - 0.5 * (group_size * bar_height))
+
+            patch.set_y(row_within_group * (bar_height + inner_sep)
+                        + group_offset)
+
+
+def deduplicateLegend(handles, labels):
+    """
+    Function from the URBS platform https://github.com/ojdo/urbs/blob/1house/comp.py
+    Remove double entries from figure legend.
+    :param handles: list of legend entry handles
+    :param labels: list of legend entry labels
+    :return: (handles, labels) tuple of lists with duplicate labels removed
+    """
+    new_handles = []
+    new_labels = []
+    for hdl, lbl in zip(handles, labels):
+        if not lbl in new_labels:
+            new_handles.append(hdl)
+            new_labels.append(lbl)
+    # also, sort both lists accordingly
+    new_labels, new_handles = (list(t) for t in zip(*sorted(zip(new_labels, new_handles))))
+    return (new_handles, new_labels)
+
+
+def resultingDataDiagram(elBus, shBus, dhwBus, costs, env, COLORS, building, newLegends):
+    """
+    Function inspired from the URBS platform https://github.com/ojdo/urbs/blob/1house/comp.py
+    Function plotting the different results of the optimization. First, costs will be plotted, then the energy produced,
+    comparing energy for electricity bus, sh and dhw bus, and finally the retrieved energy from the storages.
+    :param elBus: dict type, results from the optimization applied to one bus.
+    :param shBus: dict type, results from the optimization applied to one bus.
+    :param dhwBus: dict type, results from the optimization applied to one bus.
+    :param costs: dict type, resulting costs from the optimization
+    :param env: dict type, resulting environmental impacts from the optimization
+    :param COLORS: list type, different colors for the different components of the system
+    :param building: str type, name of the building
+    :return: Four bar plots and the costs, environmental impacts, production and storage dict created
+    """
+    production = {}
+    storage = {}
+    alpha = 0
+    if optMode == "group":
+        list = []
+
+    for flow in elBus.keys():
+        if "Storage" in flow and "out" in newLegends[flow.replace("__Building"+str(building), "")]:
+            storage[newLegends[flow.replace("__Building"+str(building), "")]] = [0, 0, sum(elBus[flow])]
+        elif optMode == "group" and ("electricityLink" in flow):
+            if "_in" in newLegends[flow.replace("__Building" + str(building), "")]:
+                if newLegends[flow.replace("__Building" + str(building), "")].replace("_in", "") in list:
+                    production[newLegends[flow.replace("__Building" + str(building), "")].replace("_in", "")][2] -= sum(elBus[flow])
+                else:
+                    production[newLegends[flow.replace("__Building" + str(building), "")].replace("_in", "")] = [0, 0, -sum(elBus[flow])]
+                    list.append(newLegends[flow.replace("__Building" + str(building), "")].replace("_in", ""))
+            elif "_out" in newLegends[flow.replace("__Building" + str(building), "")]:
+                if newLegends[flow.replace("__Building" + str(building), "")].replace("_out", "") in list:
+                    production[newLegends[flow.replace("__Building" + str(building), "")].replace("_out", "")][2] += sum(elBus[flow])
+                else:
+                    production[newLegends[flow.replace("__Building" + str(building), "")].replace("_out", "")] = [0, 0, sum(elBus[flow])]
+                    list.append(newLegends[flow.replace("__Building" + str(building), "")].replace("_out", ""))
+        elif "Storage" not in flow and "Demand" not in flow:
+            production[newLegends[flow.replace("__Building"+str(building), "")]] = [0, 0, sum(elBus[flow])]
+
+            # specific for negative flows
+            if "HP_SH" in flow or "HP_DHW" in flow:
+                alpha += sum(elBus[flow])
+
+    production["HP"] = [0, 0, -alpha]
+
+    for flow in shBus.keys():
+        if "Storage" in flow and "out" in newLegends[flow.replace("__Building"+str(building), "")]:
+            storage[newLegends[flow.replace("__Building"+str(building), "")]] = [0, sum(shBus[flow]), 0]
+        elif "Storage" not in flow and "Demand" not in flow:
+            production[newLegends[flow.replace("__Building"+str(building), "")]] = [0, sum(shBus[flow]), 0]
+
+    for flow in dhwBus.keys():
+        if "Storage__" in flow and "out" in newLegends[flow.replace("__Building"+str(building), "")]:
+            storage[newLegends[flow.replace("__Building"+str(building), "")]] = [sum(dhwBus[flow]), 0, 0]
+        elif "Storage__" not in flow and "Demand" not in flow:
+            production[newLegends[flow.replace("__Building"+str(building), "")]] = [sum(dhwBus[flow]), 0, 0]
+
+    costs = costs.transpose()
+    costs = costs.rename(index={0: building})
+
+    env = env.transpose()
+    for i in env.columns:
+        for j in newLegends.keys():
+            if i.replace("__Building"+str(building), "") in j:
+                env = env.rename(columns={i: newLegends[j]})
+
+    production = pd.DataFrame.from_dict(production, orient='index')
+    production = production.transpose()
+
+    storage = pd.DataFrame.from_dict(storage, orient='index', columns=["dhw", "sh", "elec"])
+    storage = storage.transpose()
+
+    fig = plt.figure(figsize=(18, 8))
+    gs = gridspec.GridSpec(1, 4, width_ratios=[3, 4, 8, 3], wspace=0.03)
+
+    ax0 = plt.subplot(gs[0])
+    costs_colors = [toColor(COLORS, x) for x in costs.columns]
+    bp0 = costs.plot(ax=ax0, kind='barh', color=costs_colors, stacked=True, linewidth=0)
+
+    ax1 = plt.subplot(gs[1])
+    env_colors = [toColor(COLORS, x) for x in env.columns]
+    bp1 = env.plot(ax=ax1, kind='barh', color=env_colors, stacked=True, linewidth=0)
+
+    ax2 = plt.subplot(gs[2])
+    production_colors = [toColor(COLORS, x) for x in production.columns]
+    bp2 = production.plot(ax=ax2, kind='barh', color=production_colors, stacked=True, linewidth=0, width=.5)
+
+    ax3 = plt.subplot(gs[3])
+    storage_colors = [toColor(COLORS, x) for x in storage.columns]
+    bp3 = storage.plot(ax=ax3, kind='barh', color=storage_colors, stacked=True, linewidth=0)
+
+    # remove scenario names from other bar plots
+    for ax in [ax1, ax2]:
+        ax.set_yticklabels('')
+    for ax in [ax2, ax3]:
+        groupHbarPlots(ax, group_size=3, inner_sep=0.01)
+    ax3.yaxis.tick_right()
+
+    # set limits and ticks for both axes
+    for ax in [ax0, ax1, ax2, ax3]:
+        ax.yaxis.grid(False)
+        ax.xaxis.grid(True, 'major', linestyle='-')
+        ax.xaxis.set_ticks_position('none')
+        ax.yaxis.set_ticks_position('none')
+
+        # group 1,000,000 with commas
+        xmin, xmax = ax.get_xlim()
+        if xmax > 90 or xmin < -90:
+            group_thousands_and_skip_first = tkr.FuncFormatter(
+                lambda x, pos: '' if pos == 0 else '{:0,d}'.format(int(x)))
+            ax.xaxis.set_major_formatter(group_thousands_and_skip_first)
+        else:
+            skip_lowest = tkr.FuncFormatter(
+                lambda x, pos: '' if pos == 0 else x)
+            ax.xaxis.set_major_formatter(skip_lowest)
+
+        # legend
+        # set style arguments
+        legend_style = {'frameon': False,
+                        'loc': 'lower center',
+                        'ncol': 2,
+                        'bbox_to_anchor': (0.5, .99)}
+        # get handels and labels, remove duplicate labels
+        handles, labels = deduplicateLegend(*ax.get_legend_handles_labels())
+        # set legend to use those
+        lg = ax.legend(handles, labels, **legend_style)
+        # finally, remove lines from patches
+        plt.setp(lg.get_patches(), linewidth=0)
+
+    ax0.set_xlabel('Total costs (CHF)')
+    ax1.set_xlabel('Total environmental impacts (kgCo2eq)')
+    ax2.set_xlabel('Total energy produced (kWh)')
+    ax3.set_xlabel('Retrieved energy (kWh)')
+    return fig, costs, env, production, storage
+
+
+def resultingDataDiagramLoop(elec, sh, dhw, costs, env, colors, buildings, newLegends):
+    """
+    Function inspired from the URBS platform https://github.com/ojdo/urbs/blob/1house/comp.py
+    Function plotting the graph comparing the different buildings/scenarios on costs, energy produced and energy
+    retrieved from storages
+    :param elec: list of dict type, optimization results
+    :param sh: list of dict type, optimization results
+    :param dhw: list of dict type, optimization results
+    :param costs: list of dict type, optimization results
+    :param env: list of dict type, optimization results
+    :param colors: list type, different colors for the different components of the system
+    :param buildings: list of str type, name of the different buildings
+    :return: figure created
+    """
+    n_costs, n_env, n_production, n_storage = resultingDataDiagram(elec[0], sh[0], dhw[0], costs[0], env[0], colors, buildings[0], newLegends)[1:]
+    for i in range(1, len(elec)):
+        a, b, c, d = resultingDataDiagram(elec[i], sh[i], dhw[i], costs[i], env[i], colors, buildings[i],newLegends)[1:]
+        n_costs = pd.concat([n_costs, a])
+        n_env = pd.concat([n_env, b])
+        n_production = pd.concat([n_production, c])
+        n_storage = pd.concat([n_storage, d])
+
+    fig = plt.figure(figsize=(18, 8))
+    gs = gridspec.GridSpec(1, 4, width_ratios=[4, 3, 8, 3], wspace=0.03)
+
+    ax0 = plt.subplot(gs[0])
+    costs_colors = [toColor(colors, x) for x in n_costs.columns]
+    bp0 = n_costs.plot(ax=ax0, kind='barh', color=costs_colors, stacked=True, linewidth=0)
+
+    ax1 = plt.subplot(gs[1])
+    env_colors = [toColor(colors, x) for x in n_env.columns]
+    bp1 = n_env.plot(ax=ax1, kind='barh', color=env_colors, stacked=True, linewidth=0)
+
+    ax2 = plt.subplot(gs[2])
+    production_colors = [toColor(colors, x) for x in n_production.columns]
+    bp2 = n_production.plot(ax=ax2, kind='barh', color=production_colors, stacked=True, linewidth=0, width=.5)
+
+    ax3 = plt.subplot(gs[3])
+    storage_colors = [toColor(colors, x) for x in n_storage.columns]
+    bp3 = n_storage.plot(ax=ax3, kind='barh', color=storage_colors, stacked=True, linewidth=0)
+
+    # remove scenario names from other bar plots
+    for ax in [ax1, ax2, ax3]:
+        ax.set_yticklabels('')
+    for ax in [ax2, ax3]:
+        groupHbarPlots(ax, group_size=3, inner_sep=0.01)
+
+    # set limits and ticks for both axes
+    for ax in [ax0, ax1, ax2, ax3]:
+        ax.yaxis.grid(False)
+        ax.xaxis.grid(True, 'major', linestyle='-')
+        ax.xaxis.set_ticks_position('none')
+        ax.yaxis.set_ticks_position('none')
+
+        # group 1,000,000 with commas
+        xmin, xmax = ax.get_xlim()
+        if xmax > 90 or xmin < -90:
+            group_thousands_and_skip_first = tkr.FuncFormatter(
+                lambda x, pos: '' if pos == 0 else '{:0,d}'.format(int(x)))
+            ax.xaxis.set_major_formatter(group_thousands_and_skip_first)
+        else:
+            skip_lowest = tkr.FuncFormatter(
+                lambda x, pos: '' if pos == 0 else x)
+            ax.xaxis.set_major_formatter(skip_lowest)
+
+        # legend
+        # set style arguments
+        legend_style = {'frameon': False,
+                        'loc': 'lower center',
+                        'ncol': 2,
+                        'bbox_to_anchor': (0.5, .99)}
+        # get handels and labels, remove duplicate labels
+        handles, labels = deduplicateLegend(*ax.get_legend_handles_labels())
+        # set legend to use those
+        lg = ax.legend(handles, labels, **legend_style)
+        # finally, remove lines from patches
+        plt.setp(lg.get_patches(), linewidth=0)
+
+    ax0.set_xlabel('Total costs (CHF)')
+    ax1.set_xlabel('Total environmental impacts (kgCo2eq)')
+    ax2.set_xlabel('Total energy produced (kWh)\n First line: electricity, Second line: space heating,\n Third line: domestic hot water')
+    ax3.set_xlabel('Retrieved energy (kWh)\n First line: electricity, Second line: space heating,\n Third line: domestic hot water')
+
+    return fig
+
+def resultingDataDemandDiagram(elBus, shBus, dhwBus, COLORS, building, newLegends):
+    """
+    Function inspired from the URBS platform https://github.com/ojdo/urbs/blob/1house/comp.py
+    Function plotting the different results of the optimization. First, costs will be plotted, then the energy produced,
+    comparing energy for electricity bus, sh and dhw bus, and finally the retrieved energy from the storages.
+    :param elBus: dict type, results from the optimization applied to one bus. Called like "solph.views.node(results, bus)"
+    :param shBus: dict type, results from the optimization applied to one bus. Called like "solph.views.node(results, bus)"
+    :param dhwBus: dict type, results from the optimization applied to one bus. Called like "solph.views.node(results, bus)"
+    :param COLORS: list type, different colors for the different components of the system
+    :param building: str type, name of the building
+    :return: Three bar plots and the elec, sh and dhw dict created
+    """
+    elec = {}
+    sh = {}
+    dhw = {}
+    if optMode == "group":
+        list = []
+    for flow in elBus.keys():
+        if "Demand" in flow:
+            elec[newLegends[flow.replace("__Building"+str(building), "")]] = [0, 0, sum(elBus[flow])]
+        elif "producedElectricity" in flow or "gridElectricity" in flow:
+            elec[newLegends[flow.replace("__Building" + str(building), "")]] = [0, sum(elBus[flow]), 0]
+        elif optMode == "group" and "electricityLink" in flow and "_in" not in newLegends[flow.replace("__Building" + str(building), "")]:
+            if newLegends[flow.replace("__Building" + str(building), "")] in list:
+                elec[newLegends[flow.replace("__Building" + str(building), "")]][0] += sum(elBus[flow])
+            else:
+                elec[newLegends[flow.replace("__Building" + str(building), "")]] = [sum(elBus[flow]), 0, 0]
+                list.append(newLegends[flow.replace("__Building" + str(building), "")])
+        else:
+            elec[newLegends[flow.replace("__Building"+str(building), "")]] = [sum(elBus[flow]), 0, 0]
+
+        if "Storage" in flow and "in" in newLegends[flow.replace("__Building"+str(building), "")]:
+            del elec[newLegends[flow.replace("__Building"+str(building), "")]]
+        elif "electricity" not in flow[5:] and "Demand" not in flow:
+            del elec[newLegends[flow.replace("__Building" + str(building), "")]]
+        elif "Resource" in flow or "excess" in flow:
+            del elec[newLegends[flow.replace("__Building" + str(building), "")]]
+
+    for flow in shBus.keys():
+        if "Demand" in flow:
+            sh[newLegends[flow.replace("__Building" + str(building), "")]] = [0, 0, sum(shBus[flow])]
+        else:
+            sh[newLegends[flow.replace("__Building" + str(building), "")]] = [0, sum(shBus[flow]), 0]
+        if "Storage" in flow and "in" in newLegends[flow.replace("__Building"+str(building), "")]:
+            del sh[newLegends[flow.replace("__Building"+str(building), "")]]
+
+    for flow in dhwBus.keys():
+        if "Demand" in flow:
+            dhw[newLegends[flow.replace("__Building" + str(building), "")]] = [0, 0, sum(dhwBus[flow])]
+        else:
+            dhw[newLegends[flow.replace("__Building" + str(building), "")]] = [0, sum(dhwBus[flow]), 0]
+
+        if "Storage_" in flow:
+            del dhw[newLegends[flow.replace("__Building"+str(building), "")]]
+
+    elec = pd.DataFrame.from_dict(elec, orient='index')
+    elec = elec.transpose()
+
+    sh = pd.DataFrame.from_dict(sh, orient='index')
+    sh = sh.transpose()
+
+    dhw = pd.DataFrame.from_dict(dhw, orient='index')
+    dhw = dhw.transpose()
+
+    fig = plt.figure(figsize=(18, 8))
+    gs = gridspec.GridSpec(1, 3, wspace=0.1)
+
+    ax0 = plt.subplot(gs[0])
+    elec_colors = [toColor(COLORS, x) for x in elec.columns]
+    bp0 = elec.plot(ax=ax0, kind='barh', color=elec_colors, stacked=True, linewidth=0, width=.5)
+
+    ax1 = plt.subplot(gs[1])
+    sh_colors = [toColor(COLORS, x) for x in sh.columns]
+    bp1 = sh.plot(ax=ax1, kind='barh', color=sh_colors, stacked=True, linewidth=0)
+
+    ax2 = plt.subplot(gs[2])
+    dhw_colors = [toColor(COLORS, x) for x in dhw.columns]
+    bp2 = dhw.plot(ax=ax2, kind='barh', color=dhw_colors, stacked=True, linewidth=0)
+
+    # remove scenario names from other bar plots
+    ax0.set_yticklabels(('', '', 'Building '+str(building)))
+    for ax in [ax1, ax2]:
+        ax.set_yticklabels('')
+    for ax in [ax0, ax1, ax2]:
+        groupHbarPlots(ax, group_size=3, inner_sep=0.0)
+
+    # set limits and ticks for both axes
+    for ax in [ax0, ax1, ax2]:
+        ax.yaxis.grid(False)
+        ax.xaxis.grid(True, 'major', linestyle='-')
+        ax.xaxis.set_ticks_position('none')
+        ax.yaxis.set_ticks_position('none')
+
+        # group 1,000,000 with commas
+        xmin, xmax = ax.get_xlim()
+        if xmax > 90 or xmin < -90:
+            group_thousands_and_skip_first = tkr.FuncFormatter(
+                lambda x, pos: '' if pos == 0 else '{:0,d}'.format(int(x)))
+            ax.xaxis.set_major_formatter(group_thousands_and_skip_first)
+        else:
+            skip_lowest = tkr.FuncFormatter(
+                lambda x, pos: '' if pos == 0 else x)
+            ax.xaxis.set_major_formatter(skip_lowest)
+
+        # legend
+        # set style arguments
+        legend_style = {'frameon': False,
+                        'loc': 'lower center',
+                        'ncol': 3,
+                        'bbox_to_anchor': (0.5, .99)}
+        # get handels and labels, remove duplicate labels
+        handles, labels = deduplicateLegend(*ax.get_legend_handles_labels())
+        # set legend to use those
+        lg = ax.legend(handles, labels, **legend_style)
+        # finally, remove lines from patches
+        plt.setp(lg.get_patches(), linewidth=0)
+
+    ax0.set_xlabel('Demand and energy produced\n for electricity (kWh)')
+    ax1.set_xlabel('Demand and energy produced\n for space heating (kWh)')
+    ax2.set_xlabel('Demand and energy produced\n for domestic hot water (kWh)')
+
+    return fig, elec, sh, dhw
+
+def resultingDataDemandDiagramLoop(elec, sh, dhw, colors, buildings, newLegends):
+    """
+    Function inspired from the URBS platform https://github.com/ojdo/urbs/blob/1house/comp.py
+    Function plotting the graph comparing the different buildings/scenarios on costs, energy produced and energy
+    retrieved from storages
+    :param elec: list of dict type, optimization results
+    :param sh: list of dict type, optimization results
+    :param dhw: list of dict type, optimization results
+    :param colors: list type, different colors for the different components of the system
+    :param buildings: list of str type, name of the different buildings
+    :return: figure created
+    """
+    n_elec, n_sh, n_dhw = resultingDataDemandDiagram(elec[0], sh[0], dhw[0], colors, int(buildings[0]))[1:]
+    for i in range(1, len(elec)):
+        a, b, c = resultingDataDemandDiagram(elec[i], sh[i], dhw[i], colors, buildings[i])[1:]
+        n_elec = pd.concat([n_elec, a])
+        n_sh = pd.concat([n_sh, b])
+        n_dhw = pd.concat([n_dhw, c])
+
+    fig = plt.figure(figsize=(18, 8))
+    gs = gridspec.GridSpec(1, 3, wspace=0.1)
+
+    ax0 = plt.subplot(gs[0])
+    elec_colors = [toColor(colors, x) for x in n_elec.columns]
+    bp0 = n_elec.plot(ax=ax0, kind='barh', color=elec_colors, stacked=True, linewidth=0, width=.5)
+
+    ax1 = plt.subplot(gs[1])
+    sh_colors = [toColor(colors, x) for x in n_sh.columns]
+    bp1 = n_sh.plot(ax=ax1, kind='barh', color=sh_colors, stacked=True, linewidth=0)
+
+    ax2 = plt.subplot(gs[2])
+    dhw_colors = [toColor(colors, x) for x in n_dhw.columns]
+    bp2 = n_dhw.plot(ax=ax2, kind='barh', color=dhw_colors, stacked=True, linewidth=0)
+
+    # remove scenario names from other bar plots
+    liste = []
+    for i in buildings:
+        liste.append('')
+        liste.append('')
+        liste.append('Building '+str(i))
+    ax0.set_yticklabels(liste)
+    for ax in [ax1, ax2]:
+        ax.set_yticklabels('')
+    for ax in [ax0, ax1, ax2]:
+        groupHbarPlots(ax, group_size=3, inner_sep=0.0)
+
+    # set limits and ticks for both axes
+    for ax in [ax0, ax1, ax2]:
+        ax.yaxis.grid(False)
+        ax.xaxis.grid(True, 'major', linestyle='-')
+        ax.xaxis.set_ticks_position('none')
+        ax.yaxis.set_ticks_position('none')
+
+        # group 1,000,000 with commas
+        xmin, xmax = ax.get_xlim()
+        if xmax > 90 or xmin < -90:
+            group_thousands_and_skip_first = tkr.FuncFormatter(
+                lambda x, pos: '' if pos == 0 else '{:0,d}'.format(int(x)))
+            ax.xaxis.set_major_formatter(group_thousands_and_skip_first)
+        else:
+            skip_lowest = tkr.FuncFormatter(
+                lambda x, pos: '' if pos == 0 else x)
+            ax.xaxis.set_major_formatter(skip_lowest)
+
+        # legend
+        # set style arguments
+        legend_style = {'frameon': False,
+                        'loc': 'lower center',
+                        'ncol': 3,
+                        'bbox_to_anchor': (0.5, .99)}
+        # get handels and labels, remove duplicate labels
+        handles, labels = deduplicateLegend(*ax.get_legend_handles_labels())
+        # set legend to use those
+        lg = ax.legend(handles, labels, **legend_style)
+        # finally, remove lines from patches
+        plt.setp(lg.get_patches(), linewidth=0)
+
+    ax0.set_xlabel('Demand and energy produced\n for electricity (kWh)')
+    ax1.set_xlabel('Demand and energy produced\n for space heating (kWh)')
+    ax2.set_xlabel('Demand and energy produced\n for domestic hot water (kWh)')
+
+    return fig
+
+
+def getData(filepath):
+    """
+    Function for the results recovery from an Excel file
+    :param filepath: path to the Excel containing the results of the optimization
+    :return: the different dicts created during the optimization
+    """
+    wb = load_workbook(filepath, read_only=True, keep_links=False)
+    dict_sheet = {}
+    for sheet in wb.sheetnames:
+        dict_sheet[sheet] = pd.read_excel(filepath, sheet_name=sheet, index_col=0, engine='openpyxl')
+
+    return dict_sheet
+
+def loadPlottingData(resultFilePath, numberOfBuildings):
+    """
+    Function for loading the data from excel file into variables
+    :param resultFilePath: path to the Excel containing the results of the optimization
+    :return: the different variables created after reading the excel file
+    """
+    buses = getData(resultFilePath)
+    elec_names = []
+    elec_dict = []
+    sh_names = []
+    sh_dict = []
+    dhw_names = []
+    dhw_dict = []
+    costs_names = []
+    costs_dict = []
+    env_names = []
+    env_dict = []
+
+    buildings_dict = []
+    buildings_names = []
+    buildings_number = []
+    beta = list(buses.keys())
+    for i in beta:
+        alpha = []
+        alpha_a = []
+        # Merged buses, if present, are assigned to Building 1 for plotting
+        if i in ["electricityBus", "electricityInBus", "domesticHotWaterBus", "dhwDemandBus", "spaceHeatingBus", "shDemandBus"]:
+            i = i + f'__Building{building}'
+        building = i.split("Building")[1]  # building number
+        beta_bis = beta.copy()
+        firstElBus = True
+        firstShBus = True
+        firstDhwBus = True
+        for j in beta:
+            if any('Building' in v for v in beta) and any(f'Building{building}' in v for v in beta):
+                j_buses = j
+                # Merged buses, if present, are assigned to Building 1 for plotting
+                if j in ["electricityBus", "electricityInBus", "domesticHotWaterBus", "dhwDemandBus", "spaceHeatingBus",
+                         "shDemandBus"]:
+                    j = j + f'__Building{building}'
+                if j.endswith(building) and (
+                        "electricityBus" in j or "electricityInBus" in j or "electricityProdBus" in j or "spaceHeatingBus" in j or "shDemandBus" in j or "shSourceBus" in j or "domesticHotWaterBus" in j or "dhwDemandBus" in j):
+                    """if "shDemandBus" not in j and "shSourceBus" not in j and "dhwDemandBus" not in j:
+                        alpha.append(j)"""
+                    if firstElBus and "electricity" in j:
+                        alpha.append(f"electricityBus__Building{building}")
+                        firstElBus = False
+                    elif firstShBus and ("spaceHeatingBus" in j or "shDemandBus" in j or "shSourceBus" in j):
+                        alpha.append(f"spaceHeatingBus__Building{building}")
+                        firstShBus = False
+                    elif firstDhwBus and ("domesticHotWaterBus" in j or "dhwDemandBus" in j):
+                        alpha.append(f"domesticHotWaterBus__Building{building}")
+                        firstDhwBus = False
+                    if j_buses != j:
+                        building_df = buses[j_buses].loc[:, buses[j_buses].columns.str.contains(
+                            f'Building{building}')]  # extract columns related to a given building
+                        if building == '1':
+                            building_df = pd.concat(
+                                [building_df, buses[j_buses].loc[:, ~buses[j_buses].columns.str.contains(f'Building')]],
+                                axis=1)
+                    else:
+                        building_df = buses[j_buses]
+                    if ("electricityBus" in j) or ("electricityInBus" in j) or ("electricityProdBus" in j):
+                        # find the index of electricity bus to merge the results of electricityBus, electricityInBus and electricityProdBus
+                        index = -1
+                        for ind in range(len(alpha_a)):
+                            if "electricityBus" in alpha_a[ind].keys()[0] or "electricityInBus" in alpha_a[ind].keys()[0] or "electricityProdBus" in alpha_a[ind].keys()[0]:
+                                index = ind
+                        if index != -1:
+                                alpha_a[index] = pd.concat((alpha_a[index], building_df), axis=1)
+                        else:
+                            alpha_a.append(building_df)
+                    elif ("spaceHeatingBus" in j) or ("shDemandBus" in j) or ("shSourceBus" in j):
+                        # find the index of spaceHeatingBus to merge the results of spaceHeatingBus, shDemandBus and shSourceBus
+                        index = -1
+                        for ind in range(len(alpha_a)):
+                            if "spaceHeatingBus" in alpha_a[ind].keys()[0] or "shDemandBus" in alpha_a[ind].keys()[0] or "shSourceBus" in alpha_a[ind].keys()[0]:
+                                index = ind
+                        if index != -1:
+                            alpha_a[index] = pd.concat((alpha_a[index], building_df), axis=1)
+                        else:
+                            index = len(alpha_a)
+                            alpha_a.append(building_df)
+                        flows_to_delete = [
+                            f"(('spaceHeating__Building{building}', 'shDemandBus__Building{building}'), 'flow')",
+                            f"(('shSourceBus__Building{building}', 'shSource__Building{building}'), 'flow')",
+                            f"(('spaceHeating', 'shDemandBus'), 'flow')"]
+                        for flow in flows_to_delete:
+                            if flow in alpha_a[index].columns:
+                                alpha_a[index].pop(flow)
+                    else:
+                        # find the index of domesticHotWaterBus to merge the results of domesticHotWaterBus and dhwDemandBus
+                        index = -1
+                        for ind in range(len(alpha_a)):
+                            if "domesticHotWaterBus" in alpha_a[ind].keys()[0] or "dhwDemandBus" in alpha_a[ind].keys()[0]:
+                                index = ind
+                        if index != -1:
+                            alpha_a[index] = pd.concat((alpha_a[index], building_df), axis=1)
+                        else:
+                            index = len(alpha_a)
+                            alpha_a.append(building_df)
+                        flows_to_delete = [
+                            f"(('domesticHotWater__Building{building}', 'dhwDemandBus__Building{building}'), 'flow')",
+                            f"(('domesticHotWater', 'dhwDemandBus'), 'flow')"]
+                        for flow in flows_to_delete:
+                            if flow in alpha_a[index].columns:
+                                alpha_a[index].pop(flow)
+                    beta_bis.remove(j_buses)
+        if alpha != []:
+            buildings_dict.append(alpha_a)
+            buildings_names.append(alpha)
+            buildings_number.append(building)
+        """for a in alpha:
+            beta.remove(a)"""
+        beta = [x for x in beta if f"Building{building}" not in x]
+
+    firstShBus = True
+    firstDhwBus = True
+    mergedElBuses = []
+    mergedShBuses = []
+    mergedDhwBuses = []
+    mergedLinks = False
+    b = 1  # initial building number
+    for i in buses.keys():
+        i_buses = i
+        if 'Building' in i:
+            b = int(i.split("Building")[1])  # building number
+        # Merged buses, if present, are assigned to Building 1 for plotting
+        if i in ["electricityBus", "electricityInBus", "domesticHotWaterBus", "dhwDemandBus", "spaceHeatingBus",
+                 "shDemandBus"]:
+            i = i + f'__Building{b}'
+        tt = {}
+
+        if i_buses != i:
+            if 'electricity' in i:
+                mergedElBuses.append(i_buses)
+            elif 'spaceHeating' in i or 'shDemand' in i:
+                mergedShBuses.append(i_buses)
+            else:
+                mergedDhwBuses.append(i_buses)
+            mergedLinks = True
+            building_df = buses[i_buses].loc[:, buses[i_buses].columns.str.contains(
+                f'Building{b}')]  # extract columns related to a given building
+            if b == 1:
+                building_df = pd.concat(
+                    [building_df, buses[i_buses].loc[:, ~buses[i_buses].columns.str.contains(f'Building')]], axis=1)
+        else:
+            building_df = buses[i_buses]
+
+        if ("electricityBus" in i) or ("electricityInBus" in i) or ("electricityProdBus" in i):
+            if b != 1 and mergedLinks:
+                for elBusName in mergedElBuses:
+                    elec_names.append(elBusName + f"__Building{b}")
+                    mergedbus_df = buses[elBusName].loc[:, buses[elBusName].columns.str.contains(f'Building{b}')]
+                    if b <= len(
+                            elec_dict):  # to merge the data of the two electricity buses of the same  (elec_dict[0] should have all the electricity related data of building 1, and so on...)
+                        elec_dict[b - 1] = pd.concat((elec_dict[b - 1], mergedbus_df), axis=1)
+                    else:
+                        elec_dict.append(mergedbus_df)
+            elec_names.append(i)
+            if b <= len(
+                    elec_dict):  # to merge the data of the two electricity buses of the same  (elec_dict[0] should have all the electricity related data of building 1, and so on...)
+                elec_dict[b - 1] = pd.concat((elec_dict[b - 1], building_df), axis=1)
+            else:
+                elec_dict.append(building_df)
+
+        if ("spaceHeating" in i) or ("shDemand" in i) or ("shSource" in i):
+            if any(str(b) not in v for v in sh_names):
+                firstShBus=True
+            if b != 1 and mergedLinks:
+                for shBusName in mergedShBuses:
+                    mergedbus_df = buses[shBusName].loc[:, buses[shBusName].columns.str.contains(f'Building{b}')]
+                    if firstShBus:
+                        sh_names.append(i)
+                        sh_dict.append(mergedbus_df)
+                        firstShBus = False
+                    else:
+                        ind = len(sh_names) - 1
+                        sh_dict[ind] = pd.concat((sh_dict[ind], mergedbus_df), axis=1)
+                        flows_to_delete = [f"(('spaceHeating__Building{b}', 'shDemandBus__Building{b}'), 'flow')",
+                                           f"(('shSourceBus__Building{b}', 'shSource__Building{b}'), 'flow')",
+                                           f"(('spaceHeating', 'shDemandBus'), 'flow')"]
+                        for flow in flows_to_delete:
+                            if flow in sh_dict[ind].columns:
+                                sh_dict[ind].pop(flow)
+            if firstShBus:
+                sh_names.append(i)
+                sh_dict.append(building_df)
+                firstShBus = False
+            else:
+                ind = len(sh_names) - 1
+                sh_dict[ind] = pd.concat((sh_dict[ind], building_df), axis=1)
+                flows_to_delete = [f"(('spaceHeating__Building{b}', 'shDemandBus__Building{b}'), 'flow')",
+                    f"(('shSourceBus__Building{b}', 'shSource__Building{b}'), 'flow')",
+                    f"(('spaceHeating', 'shDemandBus'), 'flow')"]
+                for flow in flows_to_delete:
+                    if flow in sh_dict[ind].columns:
+                        sh_dict[ind].pop(flow)
+        if ("domesticHotWater" in i) or ("dhwDemand" in i):
+            if any(str(b) not in v for v in dhw_names):
+                firstDhwBus=True
+            if firstDhwBus:
+                dhw_names.append(i)
+                dhw_dict.append(building_df)
+                firstDhwBus = False
+            else:
+                ind = len(dhw_names) - 1
+                dhw_dict[ind] = pd.concat((dhw_dict[ind], building_df), axis=1)
+                flows_to_delete = [f"(('domesticHotWater__Building{b}', 'dhwDemandBus__Building{b}'), 'flow')",
+                                   f"(('domesticHotWater', 'dhwDemandBus'), 'flow')"]
+                for flow in flows_to_delete:
+                    if flow in dhw_dict[ind].columns:
+                        dhw_dict[ind].pop(flow)
+        if b != 1 and mergedLinks and "dhwStorageBus" in i:
+            if any(str(b) not in v for v in dhw_names):
+                firstDhwBus=True
+            for dhwBusName in mergedDhwBuses:
+                mergedbus_df = buses[dhwBusName].loc[:, buses[dhwBusName].columns.str.contains(f'Building{b}')]
+                if firstDhwBus:
+                    dhw_names.append(f'domesticHotWaterBus__Building{b}')
+                    dhw_dict.append(mergedbus_df)
+                    firstDhwBus = False
+                else:
+                    ind = len(dhw_names) - 1
+                    dhw_dict[ind] = pd.concat((dhw_dict[ind], mergedbus_df), axis=1)
+                    flows_to_delete = [f"(('domesticHotWater__Building{b}', 'dhwDemandBus__Building{b}'), 'flow')",
+                                       f"(('domesticHotWater', 'dhwDemandBus'), 'flow')"]
+                    for flow in flows_to_delete:
+                        if flow in dhw_dict[ind].columns:
+                            dhw_dict[ind].pop(flow)
+        if "costs" in i:
+            costs_names.append(i)
+            costs_dict.append(buses[i_buses])
+        if "env_impacts" in i:
+            env_names.append(i)
+            env_dict.append(buses[i_buses])
+
+    return buses, elec_names, elec_dict, sh_names, sh_dict, dhw_names, dhw_dict, costs_names, costs_dict, env_names, env_dict,\
+           buildings_dict, buildings_names, buildings_number
+
+def createPlot(resultFilePath, basePath, numberOfBuildings, plotLevel, plotType, flowType, plotAnnualHorizontalBar, newLegends):
+    # load the plotting data from excel file into variables
+    buses, elec_names, elec_dict, sh_names, sh_dict, dhw_names, dhw_dict, costs_names, costs_dict, env_names, env_dict, \
+    buildings_dict, buildings_names, buildings_number = loadPlottingData(resultFilePath, numberOfBuildings)
+
+    if flowType == "all":
+        if plotType == "energy balance":
+            names = elec_names + sh_names + dhw_names
+        elif plotType == "bokeh":
+            names = buildings_names
+            dict = buildings_dict
+    elif flowType == "electricity":
+        names = elec_names
+        if plotType == "bokeh":
+            dict = elec_dict
+    elif flowType == "space heat":
+        names = sh_names
+        if plotType == "bokeh":
+            dict = sh_dict
+    elif flowType == "domestic hot water":
+        names = dhw_names
+        if plotType == "bokeh":
+            dict = dhw_dict
+    else:
+        raise ValueError("Illegal value for the parameter flow type")
+
+    months = ["Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"]
+
+    if plotType == "energy balance":
+        if plotLevel == "allMonths":
+            for i in names:
+                if "electricityBus" not in i:
+                    monthlyBalance(buses[i], i, newLegends)
+    elif plotType == "bokeh":
+        ncols = 2
+        if plotLevel in months:
+            if flowType == "all":
+                for i in range(len(buildings_names)):
+                    tempDict = dict[i]
+                    for j in range(len(tempDict)):
+                        tempDict[j] = tempDict[j][tempDict[j].index.strftime('%b') == plotLevel]
+                    dict[i] = tempDict
+            else:
+                for i in range(len(dict)):
+                    dict[i] = dict[i][dict[i].index.strftime('%b') == plotLevel]
+
+        elif any(chr.isdigit() for chr in plotLevel):
+            if isoparse(plotLevel):
+                if flowType == "all":
+                    for i in range(len(buildings_names)):
+                        tempDict = dict[i]
+                        for j in range(len(tempDict)):
+                            tempDict[j] = tempDict[j][tempDict[j].index.date == datetime.strptime(plotLevel, "%Y-%m-%d").date()]
+                        dict[i] = tempDict
+                else:
+                    for i in range(len(dict)):
+                        dict[i] = dict[i][dict[i].index.date == datetime.strptime(plotLevel, "%Y-%m-%d").date()]
+
+        if flowType == "all":
+            plotsHourly = []
+            plotsDaily = []
+            for i in range(len(buildings_names)):
+                plotsH, plotsD = hourlyDailyPlot(dict[i], names[i], Category20_12, newLegends)
+                plotsHourly.extend(plotsH)
+                plotsDaily.extend(plotsD)
+        else:
+            plotsHourly, plotsDaily = hourlyDailyPlot(dict, names, Set1_9, newLegends)
+
+        if not os.path.exists(basePath):
+            os.makedirs(basePath)
+
+        output_file(os.path.join(basePath,"HourlyBokehPlots.html"))
+        grid = gridplot(plotsHourly, ncols=ncols, plot_width=850, plot_height=500, sizing_mode="fixed")
+        show(grid)
+        if not any(chr.isdigit() for chr in plotLevel):
+            output_file(os.path.join(basePath,"DailyBokehPlots.html"))
+            grid = gridplot(plotsDaily, ncols=ncols, plot_width=850, plot_height=500, sizing_mode="fixed")
+            show(grid)
+    else:
+        raise ValueError("Illegal value for the parameter plot type")
+
+    if plotAnnualHorizontalBar == True:
+        my_colors = {
+            'Battery_out': (100, 160, 200),
+            'Battery_in': (100, 160, 200),
+            'Storage_sh_out': (196, 7, 27),
+            'Storage_dhw_out': (196, 7, 27),
+            'HP_dhw': (62, 173, 0),
+            'HP_sh': (62, 173, 0),
+            'HP': (62, 173, 0),
+            'CHP_elec': (0, 101, 189),
+            'CHP_sh': (0, 101, 189),
+            'CHP_dhw': (128, 0, 128),
+            'CHP': (0, 101, 189),
+            'Gas_sh': (0, 110, 120),
+            'GasBoiler': (0, 110, 120),
+            'PV_elec': (0, 128, 90),
+            'SolarCollector': (188, 128, 90),
+            'Inputs': (252, 93, 93),
+            'Operation': (252, 93, 93),
+            'Investment': (0, 119, 138),
+            'Feed-in': (0, 215, 203),
+            'Demand_elec': (131, 166, 151),
+            'Demand_sh': (131, 166, 151),
+            'Demand_dhw': (131, 166, 151),
+            'Grid_purchase': (237, 127, 16)
+        }
+        if optMode == "group":
+            my_colors['electricityLink_in'] = (255, 215, 0)
+            my_colors['electricityLink_out'] = (255, 215, 0)
+            my_colors['electricityLink'] = (255, 215, 0)
+            
+        COLORS = {}
+        for name, color in my_colors.items():
+            COLORS[name] = color
+        """
+        for i in range(len(buildings_names)):
+            fig1 = resultingDataDiagram(elec_dict[i], sh_dict[i], dhw_dict[i], costs_dict[i], env_dict[i], COLORS, buildings_number[i])[0]
+            fig2 = resultingDataDemandDiagram(elec_dict[i], sh_dict[i], dhw_dict[i], COLORS, buildings_number[i])[0]
+        """
+        fig3 = resultingDataDiagramLoop(elec_dict, sh_dict, dhw_dict, costs_dict, env_dict, COLORS, buildings_number, newLegends)
+        fig4 = resultingDataDemandDiagramLoop(elec_dict, sh_dict, dhw_dict, COLORS, buildings_number,newLegends)
+        plt.show()
+
+
+def plot(excelFileName, figureFilePath, numberOfBuildings, plotLevel, plotType, flowType, plotlabels='default', plotAnnualHorizontalBar=False):
+    #####################################
+    ########## Classic plots  ###########
+    #####################################
+    # New legends need to be defined by hand for each new flow added to the energy network
+    if plotlabels == 'default':
+        newLegends = {
+            "(('naturalGasResource', 'naturalGasBus'), 'flow')": "NaturalGas",
+            "(('electricityBus', 'excesselectricityBus'), 'flow')": "Feed-in",
+            "(('electricityProdBus', 'electricalStorage'), 'flow')": "Battery_in",
+            "(('electricityInBus', 'electricityDemand'), 'flow')": "Demand_elec",
+            "(('electricityInBus', 'emobilityDemand'), 'flow')": "Demand_mobility",
+            "(('electricityInBus', 'HP'), 'flow')": "HP",
+            "(('electricityInBus', 'GWHP'), 'flow')": "GWHP",
+            "(('CHP', 'electricityProdBus'), 'flow')": "CHP_elec",
+            "(('electricalStorage', 'electricityBus'), 'flow')": "Battery_out",
+            "(('electricitySource', 'electricityBus'), 'flow')": "Elect_produced (not stored)",
+            "(('electricityResource', 'gridBus'), 'flow')": "Grid_purchase",
+            "(('dhwStorage', 'domesticHotWaterBus'), 'flow')": "Storage_dhw_out",
+            "(('dhwStorageBus', 'dhwStorage'), 'flow')": "Storage_dhw_in",
+            "(('domesticHotWaterBus', 'domesticHotWater'), 'flow')": "dhw_direct_to_load",
+            "(('dhwDemandBus', 'domesticHotWaterDemand'), 'flow')": "Demand_dhw",
+            "(('HP', 'dhwStorageBus'), 'flow')": "HP_dhw",
+            "(('GWHP', 'dhwStorageBus'), 'flow')": "GWHP_dhw",
+            "(('CHP', 'dhwStorageBus'), 'flow')": "CHP_dhw",
+            "(('shSource', 'spaceHeatingBus'), 'flow')": "SH_produced (not stored)",
+            "(('shStorage', 'spaceHeatingBus'), 'flow')": "Storage_sh_out",
+            "storage_content": "Storage_content",
+            "(('shSourceBus', 'shStorage'), 'flow')": "Storage_sh_in",
+            "(('spaceHeatingBus', 'spaceHeating'), 'flow')": "SH_direct_to_load",
+            "(('shDemandBus', 'spaceHeatingDemand'), 'flow')": "Demand_sh",
+            "(('shDemandBus', 'excessshDemandBus'), 'flow')": "Excess SH production",
+            "(('shSourceBus', 'excessshSourceBus'), 'flow')": "Excess SH production",
+            "(('CHP', 'shSourceBus'), 'flow')": "CHP_sh",
+            "(('GasBoiler', 'shSourceBus'), 'flow')": "Gas_sh",
+            "(('GasBoiler', 'dhwStorageBus'), 'flow')": "Gas_dhw",
+            "(('HP', 'shSourceBus'), 'flow')": "HP_sh",
+            "(('GWHP', 'shSourceBus'), 'flow')": "GWHP_sh",
+            "(('electricityBus', 'producedElectricity'), 'flow')": "Self_consumption",
+            "(('gridBus', 'gridElectricity'), 'flow')": "Electricity_grid",
+            "(('pv', 'electricityProdBus'), 'flow')": "PV_elec",
+            "(('solarCollector', 'dhwStorageBus'), 'flow')": "SolarCollector",
+            "(('electricityInBus', 'solarCollector'), 'flow')": "SolarCollector",
+            "(('gridElectricity', 'electricityInBus'), 'flow')": "Electricity_grid",
+            "(('producedElectricity', 'electricityInBus'), 'flow')": "Self_consumption",
+            "(('electricityProdBus', 'electricitySource'), 'flow')": "Battery_bypass",
+            "(('domesticHotWaterBus', 'domesticHotWaterDemand'), 'flow')": "Demand_dhw",
+            "(('electricityInBus', 'ElectricRod'), 'flow')": "Electric_rod",
+            "(('ElectricRod', 'shSourceBus'), 'flow')": "Electric_rod_sh",
+            "(('ElectricRod', 'dhwStorageBus'), 'flow')": "Electric_rod_dhw",
+            "(('electricityInBus', 'GWHP35'), 'flow')": "GWHP35",
+            "(('electricityInBus', 'GWHP60'), 'flow')": "GWHP60",
+            "(('GWHP60', 'dhwStorageBus'), 'flow')": "GWHP60_dhw",
+            "(('GWHP35', 'shSourceBus'), 'flow')": "GWHP35_sh",
+        }
+        newLegends["(('electricityBus', 'electricityLink'), 'flow')"] = "electricityLink_out"
+        newLegends["(('electricityLink', 'electricityInBus'), 'flow')"] = "electricityLink_in"
+        newLegends["(('spaceHeatingBus', 'shLink'), 'flow')"] = "shLink_out"
+        newLegends["(('shLink', 'shDemandBus'), 'flow')"] = "shLink_in"
+        newLegends["(('domesticHotWaterBus', 'dhwLink'), 'flow')"] = "dhwLink_out"
+        newLegends["(('dhwLink', 'dhwDemandBus'), 'flow')"] = "dhwLink_in"
+    else:
+        newLegends = {
+            "(('naturalGasResource', 'naturalGasBus'), 'flow')": plotlabels["naturalGas"],
+            "(('electricityBus', 'excesselectricityBus'), 'flow')": plotlabels["excessEl"],
+            "(('electricityProdBus', 'electricalStorage'), 'flow')": plotlabels["StorageEl"]+"_in",
+            "(('electricityInBus', 'electricityDemand'), 'flow')": plotlabels["DemandEl"],
+            "(('electricityInBus', 'emobilityDemand'), 'flow')": plotlabels["DemandMob"],
+            "(('electricityInBus', 'HP'), 'flow')": plotlabels["HP"],
+            "(('electricityInBus', 'GWHP'), 'flow')": plotlabels["GWHP"],
+            "(('CHP', 'electricityProdBus'), 'flow')": plotlabels["CHP"]+"_el",
+            "(('electricalStorage', 'electricityBus'), 'flow')": plotlabels["StorageEl"]+"_out",
+            "(('electricitySource', 'electricityBus'), 'flow')": plotlabels["localEl"],
+            "(('electricityResource', 'gridBus'), 'flow')": plotlabels["grid"],
+            "(('dhwStorage', 'domesticHotWaterBus'), 'flow')": plotlabels["StorageDhw"]+"_out",
+            "(('dhwStorageBus', 'dhwStorage'), 'flow')": plotlabels["StorageDhw"]+"_in",
+            "(('domesticHotWaterBus', 'domesticHotWater'), 'flow')": "DHW_direct_to_load",
+            "(('dhwDemandBus', 'domesticHotWaterDemand'), 'flow')": plotlabels["DemandDhw"],
+            "(('HP', 'dhwStorageBus'), 'flow')": plotlabels["HP"]+"_dhw",
+            "(('GWHP', 'dhwStorageBus'), 'flow')": plotlabels["GWHP"]+"_dhw",
+            "(('CHP', 'dhwStorageBus'), 'flow')": plotlabels["CHP"]+"_dhw",
+            "(('shSource', 'spaceHeatingBus'), 'flow')": plotlabels["prodSH"]+" (not stored)",
+            "(('shStorage', 'spaceHeatingBus'), 'flow')": plotlabels["StorageSh"]+"_out",
+            "storage_content": "Storage_content",
+            "(('shSourceBus', 'shStorage'), 'flow')": plotlabels["StorageSh"]+"_in",
+            "(('spaceHeatingBus', 'spaceHeating'), 'flow')": "SH_direct_to_load",
+            "(('shDemandBus', 'spaceHeatingDemand'), 'flow')": plotlabels["DemandSh"],
+            "(('shDemandBus', 'excessshDemandBus'), 'flow')": plotlabels["excessSh"],
+            "(('shSourceBus', 'excessshSourceBus'), 'flow')": plotlabels["excessSh"],
+            "(('CHP', 'shSourceBus'), 'flow')": plotlabels["CHP"]+"_sh",
+            "(('GasBoiler', 'shSourceBus'), 'flow')": plotlabels["gasBoiler"]+"_sh",
+            "(('GasBoiler', 'dhwStorageBus'), 'flow')": plotlabels["gasBoiler"]+"_dhw",
+            "(('HP', 'shSourceBus'), 'flow')": plotlabels["HP"]+"_sh",
+            "(('GWHP', 'shSourceBus'), 'flow')": plotlabels["GWHP"]+"_sh",
+            "(('electricityBus', 'producedElectricity'), 'flow')": "Self_consumption",
+            "(('gridBus', 'gridElectricity'), 'flow')": plotlabels["grid"],
+            "(('pv', 'electricityProdBus'), 'flow')": plotlabels["pv"]+"_el",
+            "(('solarCollector', 'dhwStorageBus'), 'flow')": plotlabels["solarCollector"],
+            "(('electricityInBus', 'solarCollector'), 'flow')": plotlabels["solarCollector"],
+            "(('gridElectricity', 'electricityInBus'), 'flow')": plotlabels["grid"],
+            "(('producedElectricity', 'electricityInBus'), 'flow')": "Self_consumption",
+            "(('electricityProdBus', 'electricitySource'), 'flow')": plotlabels["StorageEl"]+"_bypass",
+            "(('domesticHotWaterBus', 'domesticHotWaterDemand'), 'flow')": plotlabels["DemandDhw"],
+            "(('electricityInBus', 'ElectricRod'), 'flow')": plotlabels["ElectricRod"],
+            "(('ElectricRod', 'shSourceBus'), 'flow')": plotlabels["ElectricRod"]+"_sh",
+            "(('ElectricRod', 'dhwStorageBus'), 'flow')": plotlabels["ElectricRod"]+"_dhw",
+            "(('electricityInBus', 'GWHP35'), 'flow')": plotlabels["GWHP"]+"35",
+            "(('electricityInBus', 'GWHP60'), 'flow')": plotlabels["GWHP"]+"60",
+            "(('GWHP60', 'dhwStorageBus'), 'flow')": plotlabels["GWHP"]+"60_dhw",
+            "(('GWHP35', 'shSourceBus'), 'flow')": plotlabels["GWHP"]+"35_sh",
+        }
+        newLegends["(('electricityBus', 'electricityLink'), 'flow')"] = plotlabels["elBus"]+" Link (out)"
+        newLegends["(('electricityLink', 'electricityInBus'), 'flow')"] =plotlabels["elBus"]+" Link (in)"
+        newLegends["(('spaceHeatingBus', 'shLink'), 'flow')"] = plotlabels["shBus"]+" Link (out)"
+        newLegends["(('shLink', 'shDemandBus'), 'flow')"] = plotlabels["shBus"]+" Link (in)"
+        newLegends["(('domesticHotWaterBus', 'dhwLink'), 'flow')"] = plotlabels["dhwBus"]+" Link (out)"
+        newLegends["(('dhwLink', 'dhwDemandBus'), 'flow')"] = plotlabels["dhwBus"]+" Link (in)"
+
+    createPlot(excelFileName, figureFilePath, numberOfBuildings, plotLevel, plotType, flowType, plotAnnualHorizontalBar, newLegends)
+
+
+if __name__ == '__main__':
+
+    optMode = "group"  # parameter defining whether the results file corresponds to "indiv" or "group" optimization
+    numberOfBuildings = 4
+    plotOptim = 1  # defines the number of the optimization to plot
+    plotLevel = "allMonths"  # permissible values (for energy balance plot): "allMonths" {for all months}
+    # or specific month {"Jan", "Feb", "Mar", etc. three letter abbreviation of the month name}
+    # or specific date {format: YYYY-MM-DD}
+    plotType = "energy balance"  # permissible values: "energy balance", "bokeh"
+    flowType = "electricity"  # permissible values: "all", "electricity", "space heat", "domestic hot water"
+    plotAnnualHorizontalBar = False  # determines whether the annual horizontal bar is plot or not
+
+    plot(os.path.join(r"..\data\Results", f"results{numberOfBuildings}_{plotOptim}_{optMode}.xlsx"), r"..\data\Figures", plotLevel, plotType, flowType, plotAnnualHorizontalBar)
```

### Comparing `optihood-0.0.0/optihood/plot_sankey.py` & `optihood-0.0.1/optihood/plot_sankey.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,245 +1,245 @@
-import sys
-from random import random
-import os
-import plotly.graph_objects as go
-import pandas as pd
-from optihood.plot_functions import getData
-import numpy as np
-from optihood.labelDict import labelDictGenerator, positionDictGenerator
-from matplotlib import colors
-
-def addCapacities(nodes, dataDict, buildings, UseLabelDict, labelDict, mergedLinks):
-    capacities = ["sufficient"] * len(nodes)
-    for i in buildings:
-        capTransformers=dataDict["capTransformers__Building"+str(i)]
-        capStorages=dataDict["capStorages__Building"+str(i)]
-        for j, k in capStorages.iterrows():
-            if k[0] < 0.1: # if the installed capacity is 0 then skip (sometimes as an error very low capacites are selected. To handle this k<0.01kW is set as the condition for comparison)
-                continue
-            index=nodes.index(labelDict[j])
-            #nodes[index]=nodes[index]+" "+str(round(k[0],2))+" kWh"
-            if "Bat" in labelDict[j]:
-                capacities[index] = str(round(k[0], 1)) + " kWh"
-            else:
-                capacities[index] = str(round(k[0], 1)) + " L"
-        for j, k in capTransformers.iterrows():
-            if k[0] < 0.001:     # if the installed capacity is 0 then skip (sometimes as an error very low capacites are selected. To handle this k<0.001kW is set as the condition for comparison
-                continue
-            jComponents=j.split("'")
-            if 'Bus' in jComponents[1]:
-                j =jComponents[3]
-            else:
-                j=jComponents[1]
-
-            index=nodes.index(labelDict[j])
-
-            #nodes[index]=nodes[index]+" "+str(k[0])+" kW"
-            if round(k[0],1) == 0:
-                capacities[index] = str(round(k[0], 2)) + " kW"
-            else:
-                capacities[index] = str(round(k[0], 1)) + " kW"
-    return capacities
-
-
-def readResults(fileName, buildings, ColorDict, UseLabelDict, labelDict, positionDict, labels, mergedLinks):
-    dataDict = getData(fileName)
-    keys=dataDict.keys()
-    nodes, sources, targets, values,x,y = createSankeyData(dataDict, keys, UseLabelDict, labelDict, positionDict, buildings, mergedLinks)
-    capacities = addCapacities(nodes, dataDict, buildings, UseLabelDict, labelDict, mergedLinks)
-    nodesColors = pd.Series(createColorList(nodes, ColorDict, labels))
-    linksColors = nodesColors[sources]
-    linksColors = np.where(nodesColors[targets] == ColorDict["dhw"], ColorDict["dhw"], linksColors)
-    linksColors = np.where(nodesColors[targets] == ColorDict["sh"], ColorDict["sh"], linksColors)
-    linksColors = np.where(nodesColors[targets] == ColorDict["elec"], ColorDict["elec"], linksColors)
-
-    data = [go.Sankey(
-        arrangement="snap",
-        valuesuffix="kWh",
-        node={
-            "pad":25,
-            "thickness":15,
-            "line":dict(color="black", width=0.5),
-            "label":nodes,#+str(values),
-            "color":nodesColors.tolist(),
-            #"groups":[linkGroup],
-            "customdata": capacities,
-            "hovertemplate":  '%{label} has %{customdata} capacity installed',
-            "x":x,
-            "y":y,
-            },
-        link={
-            "source":sources,
-            "target":targets,
-            "value":values,
-            "color":linksColors.tolist(),
-            },
-        )]
-    return data
-
-
-def createSankeyData(dataDict, keys, UseLabelDict, labelDict, PositionDict, buildings=[], mergedLinks=False):
-    sources = [] #contains index of node
-    targets = [] #contains index of node
-    values = []
-    nodes = []
-    # (x,y) is the position of the node
-    x=[] #equivalent in dimension to nodes
-    y=[] #equivalent in dimension to nodes
-    linkGroup=[]
-    mergedComponents = ["electricityBus", "electricityInBus", "domesticHotWaterBus", "dhwDemandBus", "spaceHeatingBus", "shDemandBus", "excesselectricityBus", "producedElectricity", "spaceHeating", "domesticHotWater"]
-
-    for key in keys:
-        df = dataDict[key]
-        dfKeys = df.keys()
-        if "dhwStorageBus" in key and not mergedComponents:
-            continue
-        if all([str(i) not in key for i in buildings]) and key not in mergedComponents:
-            continue
-        for dfKey in dfKeys:
-            if isinstance(dfKey, int) or "storage_content" in dfKey:
-                continue
-
-            dfKeySplit = dfKey.split("'")
-            sourceNodeName=dfKeySplit[1]
-            targetNodeName =dfKeySplit[3]
-
-            if mergedLinks:
-                # for the sake for representation the merged buses (if present) are added to Building 1
-                if sourceNodeName in mergedComponents:
-                    sourceNodeName = sourceNodeName + '__Building1'
-                if targetNodeName in mergedComponents:
-                    targetNodeName = targetNodeName + '__Building1'
-
-
-            if sourceNodeName in labelDict:
-                sourceNodeName = labelDict[sourceNodeName]
-            if targetNodeName in labelDict:
-                targetNodeName = labelDict[targetNodeName]
-            if sourceNodeName == targetNodeName:
-                continue
-            if "exSolar" in targetNodeName:
-                continue
-
-            if "Resource" not in sourceNodeName:
-                dfKeyValues = df[dfKey].values
-                value = sum(dfKeyValues)
-                if value < 0.001:
-                    continue
-                values.append(value)
-                if sourceNodeName not in nodes:
-                    nodes.append(sourceNodeName)
-                    for posKey in PositionDict.keys():
-                        if posKey in sourceNodeName and posKey[0:2] == sourceNodeName[0:2]: #second part of the term added for CHP and HP
-                            x.append(PositionDict[posKey][0])
-                            if labelDict["electricityLink"] in sourceNodeName:
-                                y.append((0.5-(PositionDict[posKey][1]))/len(buildings))
-                            elif labelDict["shLink"] in sourceNodeName:
-                                y.append((0.5 - (PositionDict[posKey][1])) / len(buildings))
-                            elif labelDict["dhwLink"] in sourceNodeName:
-                                y.append((0.5 - (PositionDict[posKey][1])) / len(buildings))
-                            elif ("grid" in sourceNodeName or "Grid" in sourceNodeName) and mergedLinks:
-                                buildingNumber = 1
-                                temp = (PositionDict[posKey][1]) / len(buildings) + buildingNumber / len(buildings)
-                                y.append(temp)
-                            else:
-                                buildingNumber=buildings.index(int(sourceNodeName.split('_')[-1][1:]))
-                                temp = (PositionDict[posKey][1]) / len(buildings) + buildingNumber / len(buildings)
-                                y.append(temp)
-                sources.append(nodes.index(sourceNodeName))
-
-                if targetNodeName not in nodes:
-                    nodes.append(targetNodeName)
-                    for posKey in PositionDict.keys():
-                        if posKey in targetNodeName and posKey[0:2] == targetNodeName[0:2]:
-                            x.append(PositionDict[posKey][0])
-                            if labelDict["electricityLink"] in targetNodeName:
-                                y.append((0.5-(PositionDict[posKey][1]))/len(buildings))
-                            elif labelDict["shLink"] in targetNodeName:
-                                y.append((0.5 - (PositionDict[posKey][1])) / len(buildings))
-                            elif labelDict["dhwLink"] in targetNodeName:
-                                y.append((0.5 - (PositionDict[posKey][1])) / len(buildings))
-                            elif ("grid" in sourceNodeName or "Grid" in sourceNodeName) and mergedLinks:
-                                buildingNumber = 1
-                                temp = (PositionDict[posKey][1]) / len(buildings) + buildingNumber / len(buildings)
-                                y.append(temp)
-                            else:
-                                buildingNumber=buildings.index(int(targetNodeName.split('_')[-1][1:]))
-                                temp = (PositionDict[posKey][1]) / len(buildings) + (buildingNumber) / len(buildings)
-                                y.append(temp)
-                targets.append(nodes.index(targetNodeName))
-    return nodes, sources, targets, values, x, y
-
-
-def createColorList(inputList, ColorDict, labels):
-    colorsList=[]
-    for n in inputList:
-        if (labels!='default' and labels["naturalGas"] in n) or (labels=='default' and "natGas" in n):           # Check for whether labels of a specific type are defined or not should be added here
-            color = ColorDict["gas"]
-        elif (labels!='default' and (labels["excessSh"] in n or labels["prodSH"] in n or labels["shBus"] in n or labels["StorageSh"] in n or labels["DemandSh"] in n)) or (labels=='default' and any(v in n for v in ["shLink", "prodSH", "shBus", "shStor", "Q_sh", "exSh", "usedSH"])):
-            color = ColorDict["sh"]
-        elif (labels!='default' and (labels["solarCollector"] in n or labels["excessSolarCollector"] in n or labels["StorageDhw"] in n or labels["dhwBus"] in n or labels["DemandDhw"] in n)) or (labels=='default' and any(v in n for v in ["dhwLink", "solar", "exSolar", "dhwStor", "dhwBus", "Q_dhw", "prodDHW"])):
-            color = ColorDict["dhw"]
-        elif (labels!='default' and (labels["elBus"] in n or labels["grid"] in n or labels["pv"] in n or labels["prodEl"] in n or labels["localEl"] in n or labels["StorageEl"] in n or labels["excessEl"] in n or labels["DemandEl"] in n or labels["DemandMob"] in n))  or (labels=='default' and any(v in n for v in ["elLink", "grid", "pv", "prodEl", "localEl", "Bat", "exEl", "usedEl", "Q_el", "Q_mob"])):
-            color = ColorDict["elec"]
-        else:
-            color = ColorDict["other"]
-        colorsList.append(color)
-    return colorsList
-
-
-def displaySankey(fileName, UseLabelDict, labelDict, positionDict, labels, buildings, mergedLinks, hideBuildingNumber):
-    OPACITY = 0.6
-    ColorDict = {"elec": 'rgba' + str(colors.to_rgba("skyblue", OPACITY)),
-                 "gas": 'rgba' + str(colors.to_rgba("darkgray", OPACITY)),
-                 "dhw": 'rgba' + str(colors.to_rgba("red", OPACITY)),
-                 "sh": 'rgba' + str(colors.to_rgba("magenta", OPACITY)),
-                 "other": 'rgba' + str(colors.to_rgba("deeppink", OPACITY))
-                 }
-    data = readResults(fileName, buildings, ColorDict, UseLabelDict, labelDict, positionDict, labels, mergedLinks)
-
-    node = data[0]['node']
-    link = data[0]['link']
-    if hideBuildingNumber == True:
-        node['label'] = tuple(s if not "_B" in s else s.split("_")[0] for s in node['label'])
-    fig = go.Figure(go.Sankey(arrangement = "perpendicular",
-                              link=link,
-                              node=node
-                              )) #snap, perpendicular,freeform, fixed
-    fig.update_layout(
-        title=fileName +" for buildings " + str(buildings),
-        font=dict(size=10, color='black'),
-        paper_bgcolor='rgba(0,0,0,0)',
-        plot_bgcolor='rgba(0,0,0,0)',
-    )
-    fig.add_hline(y=0, line_color='rgba(0,0,0,0)')
-    if len(buildings)%2==0:
-        fig.add_hline(y=0.5, line_dash="dash")
-    if len(buildings)%3==0:
-        fig.add_hline(y=0.33, line_dash="dash")
-        fig.add_hline(y=0.66, line_dash="dash")
-    if len(buildings)%4==0:
-        fig.add_hline(y=0.25, line_dash="dash")
-        fig.add_hline(y=0.75, line_dash="dash")
-    fig.add_hline(y=1.0, line_color='rgba(0,0,0,0)')
-    fig.update_xaxes(visible=False)
-    fig.update_yaxes(visible=False)
-    return fig
-
-
-def plot(excelFileName, outputFileName, numberOfBuildings, UseLabelDict, labels, optimType, mergedLinks=False, hideBuildingNumber=False):
-    BUILDINGSLIST = list(range(1, numberOfBuildings + 1))
-    labelDict = labelDictGenerator(numberOfBuildings, labels, optimType, mergedLinks)
-    positionDict = positionDictGenerator(labels, optimType, mergedLinks)
-    fig = displaySankey(excelFileName, UseLabelDict, labelDict, positionDict, labels, BUILDINGSLIST, mergedLinks, hideBuildingNumber)
-    fig.show()
-    fig.write_html(outputFileName)
-
-
-if __name__ == "__main__":
-    optMode = "group"  # parameter defining whether the results file corresponds to "indiv" or "group" optimization
-    numberOfBuildings = 4
-    plotOptim = 3  # defines the number of the optimization to plot
-    UseLabelDict = True
-    excelFileName = os.path.join(r"..\data\Results", f"results{numberOfBuildings}_{plotOptim}_{optMode}.xlsx")
-    outputFileName = os.path.join(r"..\data\figures", f"Sankey_{plotOptim}.html")
-    plot(excelFileName, outputFileName, numberOfBuildings, UseLabelDict, labels='default', optimType=optMode)
+import sys
+from random import random
+import os
+import plotly.graph_objects as go
+import pandas as pd
+from optihood.plot_functions import getData
+import numpy as np
+from optihood.labelDict import labelDictGenerator, positionDictGenerator
+from matplotlib import colors
+
+def addCapacities(nodes, dataDict, buildings, UseLabelDict, labelDict, mergedLinks):
+    capacities = ["sufficient"] * len(nodes)
+    for i in buildings:
+        capTransformers=dataDict["capTransformers__Building"+str(i)]
+        capStorages=dataDict["capStorages__Building"+str(i)]
+        for j, k in capStorages.iterrows():
+            if k[0] < 0.1: # if the installed capacity is 0 then skip (sometimes as an error very low capacites are selected. To handle this k<0.01kW is set as the condition for comparison)
+                continue
+            index=nodes.index(labelDict[j])
+            #nodes[index]=nodes[index]+" "+str(round(k[0],2))+" kWh"
+            if "Bat" in labelDict[j]:
+                capacities[index] = str(round(k[0], 1)) + " kWh"
+            else:
+                capacities[index] = str(round(k[0], 1)) + " L"
+        for j, k in capTransformers.iterrows():
+            if k[0] < 0.001:     # if the installed capacity is 0 then skip (sometimes as an error very low capacites are selected. To handle this k<0.001kW is set as the condition for comparison
+                continue
+            jComponents=j.split("'")
+            if 'Bus' in jComponents[1]:
+                j =jComponents[3]
+            else:
+                j=jComponents[1]
+
+            index=nodes.index(labelDict[j])
+
+            #nodes[index]=nodes[index]+" "+str(k[0])+" kW"
+            if round(k[0],1) == 0:
+                capacities[index] = str(round(k[0], 2)) + " kW"
+            else:
+                capacities[index] = str(round(k[0], 1)) + " kW"
+    return capacities
+
+
+def readResults(fileName, buildings, ColorDict, UseLabelDict, labelDict, positionDict, labels, mergedLinks):
+    dataDict = getData(fileName)
+    keys=dataDict.keys()
+    nodes, sources, targets, values,x,y = createSankeyData(dataDict, keys, UseLabelDict, labelDict, positionDict, buildings, mergedLinks)
+    capacities = addCapacities(nodes, dataDict, buildings, UseLabelDict, labelDict, mergedLinks)
+    nodesColors = pd.Series(createColorList(nodes, ColorDict, labels))
+    linksColors = nodesColors[sources]
+    linksColors = np.where(nodesColors[targets] == ColorDict["dhw"], ColorDict["dhw"], linksColors)
+    linksColors = np.where(nodesColors[targets] == ColorDict["sh"], ColorDict["sh"], linksColors)
+    linksColors = np.where(nodesColors[targets] == ColorDict["elec"], ColorDict["elec"], linksColors)
+
+    data = [go.Sankey(
+        arrangement="snap",
+        valuesuffix="kWh",
+        node={
+            "pad":25,
+            "thickness":15,
+            "line":dict(color="black", width=0.5),
+            "label":nodes,#+str(values),
+            "color":nodesColors.tolist(),
+            #"groups":[linkGroup],
+            "customdata": capacities,
+            "hovertemplate":  '%{label} has %{customdata} capacity installed',
+            "x":x,
+            "y":y,
+            },
+        link={
+            "source":sources,
+            "target":targets,
+            "value":values,
+            "color":linksColors.tolist(),
+            },
+        )]
+    return data
+
+
+def createSankeyData(dataDict, keys, UseLabelDict, labelDict, PositionDict, buildings=[], mergedLinks=False):
+    sources = [] #contains index of node
+    targets = [] #contains index of node
+    values = []
+    nodes = []
+    # (x,y) is the position of the node
+    x=[] #equivalent in dimension to nodes
+    y=[] #equivalent in dimension to nodes
+    linkGroup=[]
+    mergedComponents = ["electricityBus", "electricityInBus", "domesticHotWaterBus", "dhwDemandBus", "spaceHeatingBus", "shDemandBus", "excesselectricityBus", "producedElectricity", "spaceHeating", "domesticHotWater"]
+
+    for key in keys:
+        df = dataDict[key]
+        dfKeys = df.keys()
+        if "dhwStorageBus" in key and not mergedComponents:
+            continue
+        if all([str(i) not in key for i in buildings]) and key not in mergedComponents:
+            continue
+        for dfKey in dfKeys:
+            if isinstance(dfKey, int) or "storage_content" in dfKey:
+                continue
+
+            dfKeySplit = dfKey.split("'")
+            sourceNodeName=dfKeySplit[1]
+            targetNodeName =dfKeySplit[3]
+
+            if mergedLinks:
+                # for the sake for representation the merged buses (if present) are added to Building 1
+                if sourceNodeName in mergedComponents:
+                    sourceNodeName = sourceNodeName + '__Building1'
+                if targetNodeName in mergedComponents:
+                    targetNodeName = targetNodeName + '__Building1'
+
+
+            if sourceNodeName in labelDict:
+                sourceNodeName = labelDict[sourceNodeName]
+            if targetNodeName in labelDict:
+                targetNodeName = labelDict[targetNodeName]
+            if sourceNodeName == targetNodeName:
+                continue
+            if "exSolar" in targetNodeName:
+                continue
+
+            if "Resource" not in sourceNodeName:
+                dfKeyValues = df[dfKey].values
+                value = sum(dfKeyValues)
+                if value < 0.001:
+                    continue
+                values.append(value)
+                if sourceNodeName not in nodes:
+                    nodes.append(sourceNodeName)
+                    for posKey in PositionDict.keys():
+                        if posKey in sourceNodeName and posKey[0:2] == sourceNodeName[0:2]: #second part of the term added for CHP and HP
+                            x.append(PositionDict[posKey][0])
+                            if labelDict["electricityLink"] in sourceNodeName:
+                                y.append((0.5-(PositionDict[posKey][1]))/len(buildings))
+                            elif labelDict["shLink"] in sourceNodeName:
+                                y.append((0.5 - (PositionDict[posKey][1])) / len(buildings))
+                            elif labelDict["dhwLink"] in sourceNodeName:
+                                y.append((0.5 - (PositionDict[posKey][1])) / len(buildings))
+                            elif ("grid" in sourceNodeName or "Grid" in sourceNodeName) and mergedLinks:
+                                buildingNumber = 1
+                                temp = (PositionDict[posKey][1]) / len(buildings) + buildingNumber / len(buildings)
+                                y.append(temp)
+                            else:
+                                buildingNumber=buildings.index(int(sourceNodeName.split('_')[-1][1:]))
+                                temp = (PositionDict[posKey][1]) / len(buildings) + buildingNumber / len(buildings)
+                                y.append(temp)
+                sources.append(nodes.index(sourceNodeName))
+
+                if targetNodeName not in nodes:
+                    nodes.append(targetNodeName)
+                    for posKey in PositionDict.keys():
+                        if posKey in targetNodeName and posKey[0:2] == targetNodeName[0:2]:
+                            x.append(PositionDict[posKey][0])
+                            if labelDict["electricityLink"] in targetNodeName:
+                                y.append((0.5-(PositionDict[posKey][1]))/len(buildings))
+                            elif labelDict["shLink"] in targetNodeName:
+                                y.append((0.5 - (PositionDict[posKey][1])) / len(buildings))
+                            elif labelDict["dhwLink"] in targetNodeName:
+                                y.append((0.5 - (PositionDict[posKey][1])) / len(buildings))
+                            elif ("grid" in sourceNodeName or "Grid" in sourceNodeName) and mergedLinks:
+                                buildingNumber = 1
+                                temp = (PositionDict[posKey][1]) / len(buildings) + buildingNumber / len(buildings)
+                                y.append(temp)
+                            else:
+                                buildingNumber=buildings.index(int(targetNodeName.split('_')[-1][1:]))
+                                temp = (PositionDict[posKey][1]) / len(buildings) + (buildingNumber) / len(buildings)
+                                y.append(temp)
+                targets.append(nodes.index(targetNodeName))
+    return nodes, sources, targets, values, x, y
+
+
+def createColorList(inputList, ColorDict, labels):
+    colorsList=[]
+    for n in inputList:
+        if (labels!='default' and labels["naturalGas"] in n) or (labels=='default' and "natGas" in n):           # Check for whether labels of a specific type are defined or not should be added here
+            color = ColorDict["gas"]
+        elif (labels!='default' and (labels["excessSh"] in n or labels["prodSH"] in n or labels["shBus"] in n or labels["StorageSh"] in n or labels["DemandSh"] in n)) or (labels=='default' and any(v in n for v in ["shLink", "prodSH", "shBus", "shStor", "Q_sh", "exSh", "usedSH"])):
+            color = ColorDict["sh"]
+        elif (labels!='default' and (labels["solarCollector"] in n or labels["excessSolarCollector"] in n or labels["StorageDhw"] in n or labels["dhwBus"] in n or labels["DemandDhw"] in n)) or (labels=='default' and any(v in n for v in ["dhwLink", "solar", "exSolar", "dhwStor", "dhwBus", "Q_dhw", "prodDHW"])):
+            color = ColorDict["dhw"]
+        elif (labels!='default' and (labels["elBus"] in n or labels["grid"] in n or labels["pv"] in n or labels["prodEl"] in n or labels["localEl"] in n or labels["StorageEl"] in n or labels["excessEl"] in n or labels["DemandEl"] in n or labels["DemandMob"] in n))  or (labels=='default' and any(v in n for v in ["elLink", "grid", "pv", "prodEl", "localEl", "Bat", "exEl", "usedEl", "Q_el", "Q_mob"])):
+            color = ColorDict["elec"]
+        else:
+            color = ColorDict["other"]
+        colorsList.append(color)
+    return colorsList
+
+
+def displaySankey(fileName, UseLabelDict, labelDict, positionDict, labels, buildings, mergedLinks, hideBuildingNumber):
+    OPACITY = 0.6
+    ColorDict = {"elec": 'rgba' + str(colors.to_rgba("skyblue", OPACITY)),
+                 "gas": 'rgba' + str(colors.to_rgba("darkgray", OPACITY)),
+                 "dhw": 'rgba' + str(colors.to_rgba("red", OPACITY)),
+                 "sh": 'rgba' + str(colors.to_rgba("magenta", OPACITY)),
+                 "other": 'rgba' + str(colors.to_rgba("deeppink", OPACITY))
+                 }
+    data = readResults(fileName, buildings, ColorDict, UseLabelDict, labelDict, positionDict, labels, mergedLinks)
+
+    node = data[0]['node']
+    link = data[0]['link']
+    if hideBuildingNumber == True:
+        node['label'] = tuple(s if not "_B" in s else s.split("_")[0] for s in node['label'])
+    fig = go.Figure(go.Sankey(arrangement = "perpendicular",
+                              link=link,
+                              node=node
+                              )) #snap, perpendicular,freeform, fixed
+    fig.update_layout(
+        title=fileName +" for buildings " + str(buildings),
+        font=dict(size=10, color='black'),
+        paper_bgcolor='rgba(0,0,0,0)',
+        plot_bgcolor='rgba(0,0,0,0)',
+    )
+    fig.add_hline(y=0, line_color='rgba(0,0,0,0)')
+    if len(buildings)%2==0:
+        fig.add_hline(y=0.5, line_dash="dash")
+    if len(buildings)%3==0:
+        fig.add_hline(y=0.33, line_dash="dash")
+        fig.add_hline(y=0.66, line_dash="dash")
+    if len(buildings)%4==0:
+        fig.add_hline(y=0.25, line_dash="dash")
+        fig.add_hline(y=0.75, line_dash="dash")
+    fig.add_hline(y=1.0, line_color='rgba(0,0,0,0)')
+    fig.update_xaxes(visible=False)
+    fig.update_yaxes(visible=False)
+    return fig
+
+
+def plot(excelFileName, outputFileName, numberOfBuildings, UseLabelDict, labels, optimType, mergedLinks=False, hideBuildingNumber=False):
+    BUILDINGSLIST = list(range(1, numberOfBuildings + 1))
+    labelDict = labelDictGenerator(numberOfBuildings, labels, optimType, mergedLinks)
+    positionDict = positionDictGenerator(labels, optimType, mergedLinks)
+    fig = displaySankey(excelFileName, UseLabelDict, labelDict, positionDict, labels, BUILDINGSLIST, mergedLinks, hideBuildingNumber)
+    fig.show()
+    fig.write_html(outputFileName)
+
+
+if __name__ == "__main__":
+    optMode = "group"  # parameter defining whether the results file corresponds to "indiv" or "group" optimization
+    numberOfBuildings = 4
+    plotOptim = 3  # defines the number of the optimization to plot
+    UseLabelDict = True
+    excelFileName = os.path.join(r"..\data\Results", f"results{numberOfBuildings}_{plotOptim}_{optMode}.xlsx")
+    outputFileName = os.path.join(r"..\data\figures", f"Sankey_{plotOptim}.html")
+    plot(excelFileName, outputFileName, numberOfBuildings, UseLabelDict, labels='default', optimType=optMode)
```

### Comparing `optihood-0.0.0/optihood/sinks.py` & `optihood-0.0.1/optihood/sinks.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,288 +1,288 @@
-"""
-under-development component for a linear RC model for heating a Building
-"""
-
-import oemof.solph as solph
-from oemof.solph.plumbing import sequence
-from pyomo.core.base.block import SimpleBlock
-from pyomo.environ import BuildAction
-from pyomo.environ import Constraint
-from pyomo.environ import Expression
-from pyomo.environ import NonNegativeReals, Reals, Boolean
-from pyomo.environ import Set
-from pyomo.environ import Var
-
-class SinkRCModel(solph.Sink):
-    """
-    Building RC Model implemented as a custom Sink component
-
-    Parameters
-    ----------
-    rDistribution : Thermal resistance between indoor and distribution system states [K/kW]
-    cDistribution : Thermal capacity of distribution system state [kWh/K]
-    rIndoor : Thermal resistance between indoor and wall states [K/kW]
-    cIndoor : Thermal capacity of indoor air state [kWh/K]
-    rWall : Thermal resistance between wall state and outside [K/kW]
-    cWall  : Thermal capacity of wall state [kWh/K]
-    areaWindows : aperture area of windows [m^2]
-    qDistributionMin : Minimum operating power from the SC tank to the distribution system [kW]
-    qDistributionMax : Maximum operating power from the SC tank to the distribution system [kW]
-    tIndoorMin : Indoor minimum comfort temperature [ºC]
-    tIndoorMax : Indoor maximum comfort temperature [ºC]
-    tIndoorInit : Indoor initial temperature [ºC]
-    tWallInit : Wall initial temperature [ºC]
-    tDistributionInit : Distribution system initial temperature [ºC]
-    tAmbient : Ambient outside air temperature at each timestep [ºC]
-    totalIrradiationHorizontal : Total horizontal irradiation at each timestep [kW/m^2]
-    heatGainOccupants : Internal heat gains from occupants at each timestep [kW]
-    """
-
-    def __init__(
-            self,
-            tAmbient,
-            totalIrradiationHorizontal,
-            heatGainOccupants,
-            rDistribution=0.75,
-            cDistribution=0.26,
-            rIndoor=0.09,
-            cIndoor=0.97,
-            rWall=1.70,
-            cWall=226.30,
-            areaWindows=1.5,
-            qDistributionMin=0,
-            qDistributionMax=1000,
-            tIndoorMin=19,
-            tIndoorMax=23,
-            tIndoorInit=21,
-            tWallInit=21,
-            tDistributionInit=21,
-            **kwargs,
-    ):
-        super().__init__(**kwargs)
-        self.rDistribution = rDistribution
-        self.cDistribution = cDistribution
-        self.rIndoor = rIndoor
-        self.cIndoor = cIndoor
-        self.rWall = rWall
-        self.cWall = cWall
-        self.areaWindows = areaWindows
-        self.qDistributionMin = qDistributionMin
-        self.qDistributionMax = qDistributionMax
-        self.tIndoorMin = tIndoorMin
-        self.tIndoorMax = tIndoorMax
-        self.tIndoorInit = tIndoorInit
-        self.tWallInit = tWallInit
-        self.tDistributionInit = tDistributionInit
-        self.tAmbient = sequence(tAmbient)
-        self.totalIrradiationHorizontal = sequence(totalIrradiationHorizontal)
-        self.heatGainOccupants = sequence(heatGainOccupants)
-
-    def constraint_group(self):
-        return SinkRCModelBlock
-
-class SinkRCModelBlock(SimpleBlock):
-    """
-    Constraints for SinkRCModel Class
-    """
-    CONSTRAINT_GROUP = True
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-    def _create(self, group=None):
-        if group is None:
-            return None
-
-        m = self.parent_block()
-
-        # for all Sink RC model components get inflow from a bus
-        for n in group:
-            n.inflow = list(n.inputs)[0]
-
-        #  ************* SET OF CUSTOM SINK COMPONENTS *****************************
-
-        # Set of Sink RC model Components
-        self.sinkrc = Set(initialize=[n for n in group])
-
-        #  ************* DECISION VARIABLES *****************************
-
-        # Variable indoor temperature
-        self.tIndoor = Var(self.sinkrc, m.TIMESTEPS, within=Reals)
-
-        # Variable wall temperature
-        self.tWall = Var(self.sinkrc, m.TIMESTEPS, within=Reals)
-
-        # Variable distribution temperature
-        self.tDistribution = Var(self.sinkrc, m.TIMESTEPS, within=Reals)
-
-        # Variable indoor comfort temperature range violation
-        self.epsilonIndoor = Var(self.sinkrc, m.TIMESTEPS, within=NonNegativeReals)
-
-        # Variable indoor final temperature requirement violation
-        self.deltaIndoor = Var(self.sinkrc, within=NonNegativeReals)
-
-        # Variable binary indicator (0 whenever Q = 0)
-        # self.Xsc_dis = Var(self.sinkrc, m.TIMESTEPS, within=Boolean)
-
-        #  ************* CONSTRAINTS *****************************
-
-        def _initial_indoor_temperature_rule(block):
-            """set initial values of indoor temperature
-            """
-            for g in group:
-                lhs = self.tIndoor[g, 0]
-                rhs = g.tIndoorInit
-                block.initial_indoor_temperature.add((g, 0), (lhs == rhs))
-
-        self.initial_indoor_temperature = Constraint(group, m.TIMESTEPS, noruleinit=True)
-        self.initial_indoor_temperature_build = BuildAction(rule=_initial_indoor_temperature_rule)
-
-        def _initial_wall_temperature_rule(block):
-            """set initial values of wall temperature
-            """
-            for g in group:
-                lhs = self.tWall[g, 0]
-                rhs = g.tWallInit
-                block.initial_wall_temperature.add((g, 0), (lhs == rhs))
-
-        self.initial_wall_temperature = Constraint(group, m.TIMESTEPS, noruleinit=True)
-        self.initial_wall_temperature_build = BuildAction(rule=_initial_wall_temperature_rule)
-
-        def _initial_distribution_temperature_rule(block):
-            """set initial values of distribution temperature
-            """
-            for g in group:
-                lhs = self.tDistribution[g, 0]
-                rhs = g.tDistributionInit
-                block.initial_distribution_temperature.add((g, 0), (lhs == rhs))
-
-        self.initial_distribution_temperature = Constraint(group, m.TIMESTEPS, noruleinit=True)
-        self.initial_distribution_temperature_build = BuildAction(rule=_initial_distribution_temperature_rule)
-
-        #def _boolean_indicator_set_rule(block):
-        #    """sets the value of boolean indicator self.Xsc_dis
-        #    value is set to False whenever qDistribution = 0, otherwise True
-        #    """
-        #    for t in m.TIMESTEPS:
-        #        for g in group:
-        #            lhs = self.Xsc_dis[g, t]
-        #            rhs = not(m.flow[g.inflow, g, t] == 0)
-
-         #           block.boolean_indicator_set.add((g, t), (lhs == rhs))
-
-        #self.boolean_indicator_set = Constraint(group, m.TIMESTEPS, noruleinit=True)
-        #self.boolean_indicator_set_build = BuildAction(rule=_boolean_indicator_set_rule)
-
-        def _indoor_comfort_upper_limit_rule(block):
-            """Indoor comfort temperature < = maximum limit
-            """
-            for t in m.TIMESTEPS:
-                for g in group:
-                    lhs = self.tIndoor[g, t]
-                    #rhs = g.tIndoorMax
-                    rhs = g.tIndoorMax + self.epsilonIndoor[g, t]
-                    block.indoor_comfort_upper_limit.add((g, t), (lhs <= rhs))
-
-        self.indoor_comfort_upper_limit = Constraint(group, m.TIMESTEPS, noruleinit=True)
-        self.indoor_comfort_upper_limit_build = BuildAction(rule=_indoor_comfort_upper_limit_rule)
-
-        def _indoor_comfort_lower_limit_rule(block):
-            """Indoor comfort temperature > = minimum limit
-            """
-            for t in m.TIMESTEPS:
-                for g in group:
-                    lhs = self.tIndoor[g, t]
-                    # rhs = g.tIndoorMin
-                    rhs = g.tIndoorMin - self.epsilonIndoor[g, t]
-                    block.indoor_comfort_lower_limit.add((g, t), (lhs >= rhs))
-
-        self.indoor_comfort_lower_limit = Constraint(group, m.TIMESTEPS, noruleinit=True)
-        self.indoor_comfort_lower_limit_build = BuildAction(rule=_indoor_comfort_lower_limit_rule)
-
-        def _indoor_final_temperature_rule(block):
-            """Indoor temperature at the final timestamp should be higher than initial indoor temperature
-            """
-            t = m.TIMESTEPS[-1] #final timestep
-            for g in group:
-                lhs = self.tIndoor[g, t]
-                #rhs = g.tIndoorInit
-                rhs = g.tIndoorInit - self.deltaIndoor[g]
-                block.indoor_final_temperature.add((g, t), (lhs >= rhs))
-
-        self.indoor_final_temperature = Constraint(group, m.TIMESTEPS, noruleinit=True)
-        self.indoor_final_temperature_build = BuildAction(rule=_indoor_final_temperature_rule)
-
-        def _q_distribution_upper_limit_rule(block):
-            """q distribution < = maximum limit
-            """
-            for t in m.TIMESTEPS:
-                for g in group:
-                    lhs = m.flow[g.inflow, g, t]
-                    rhs = g.qDistributionMax
-                    # rhs = g.qDistributionMax * self.Xsc_dis[g, t]
-                    block.q_distribution_upper_limit.add((g, t), (lhs <= rhs))
-
-        self.q_distribution_upper_limit = Constraint(group, m.TIMESTEPS, noruleinit=True)
-        self.q_distribution_upper_limit_build = BuildAction(rule=_q_distribution_upper_limit_rule)
-
-        def _q_distribution_lower_limit_rule(block):
-            """q distribution > = minimum limit
-            """
-            for t in m.TIMESTEPS:
-                for g in group:
-                    lhs = m.flow[g.inflow, g, t]
-                    rhs = g.qDistributionMin
-                    # rhs = g.qDistributionMin * self.Xsc_dis[g, t]
-                    block.q_distribution_lower_limit.add((g, t), (lhs >= rhs))
-
-        self.q_distribution_lower_limit = Constraint(group, m.TIMESTEPS, noruleinit=True)
-        self.q_distribution_lower_limit_build = BuildAction(rule=_q_distribution_lower_limit_rule)
-
-        def _indoor_temperature_equation_rule(block):
-            """discrete state space equation for tIndoor
-            """
-            for g in group:
-                c2 = 1/(g.rIndoor*g.cIndoor)
-                c3 = 1/(g.rDistribution*g.cIndoor)
-                c1 = 1 - c2 - c3
-                c4 = g.areaWindows/g.cIndoor
-                for t in m.TIMESTEPS:
-                    if t!= m.TIMESTEPS[-1]:
-                        lhs = self.tIndoor[g, t+1]
-                        rhs = c1*self.tIndoor[g, t] + c2*self.tWall[g, t] + c3*self.tDistribution[g, t] + c4*(g.totalIrradiationHorizontal[t] + g.heatGainOccupants[t])
-                        block.indoor_temperature_equation.add((g, t), (lhs == rhs))
-
-        self.indoor_temperature_equation = Constraint(group, m.TIMESTEPS, noruleinit=True)
-        self.indoor_temperature_equation_build = BuildAction(rule=_indoor_temperature_equation_rule)
-
-        def _wall_temperature_equation_rule(block):
-            """discrete state space equation for tWall
-            """
-            for g in group:
-                c1 = 1 / (g.rIndoor * g.cWall)
-                c3 = 1 / (g.rWall * g.cWall)
-                c2 = 1 - c1 - c3
-                for t in m.TIMESTEPS:
-                    if t != m.TIMESTEPS[-1]:
-                        lhs = self.tWall[g, t + 1]
-                        rhs = c1 * self.tIndoor[g, t] + c2 * self.tWall[g, t] + c3 * g.tAmbient[t]
-                        block.wall_temperature_equation.add((g, t), (lhs == rhs))
-
-        self.wall_temperature_equation = Constraint(group, m.TIMESTEPS, noruleinit=True)
-        self.wall_temperature_equation_build = BuildAction(rule=_wall_temperature_equation_rule)
-
-        def _distribution_temperature_equation_rule(block):
-            """discrete state space equation for tDistribution
-            """
-            for g in group:
-                c1 = 1 / (g.rDistribution * g.cDistribution)
-                c2 = 1 - c1
-                c3 = 1 /g.cDistribution
-                for t in m.TIMESTEPS:
-                    if t != m.TIMESTEPS[-1]:
-                        lhs = self.tDistribution[g, t + 1]
-                        rhs = c1 * self.tIndoor[g, t] + c2 * self.tDistribution[g, t] + c3 * m.flow[g.inflow, g, t]
-                        block.distribution_temperature_equation.add((g, t), (lhs == rhs))
-
-        self.distribution_temperature_equation = Constraint(group, m.TIMESTEPS, noruleinit=True)
+"""
+under-development component for a linear RC model for heating a Building
+"""
+
+import oemof.solph as solph
+from oemof.solph.plumbing import sequence
+from pyomo.core.base.block import SimpleBlock
+from pyomo.environ import BuildAction
+from pyomo.environ import Constraint
+from pyomo.environ import Expression
+from pyomo.environ import NonNegativeReals, Reals, Boolean
+from pyomo.environ import Set
+from pyomo.environ import Var
+
+class SinkRCModel(solph.Sink):
+    """
+    Building RC Model implemented as a custom Sink component
+
+    Parameters
+    ----------
+    rDistribution : Thermal resistance between indoor and distribution system states [K/kW]
+    cDistribution : Thermal capacity of distribution system state [kWh/K]
+    rIndoor : Thermal resistance between indoor and wall states [K/kW]
+    cIndoor : Thermal capacity of indoor air state [kWh/K]
+    rWall : Thermal resistance between wall state and outside [K/kW]
+    cWall  : Thermal capacity of wall state [kWh/K]
+    areaWindows : aperture area of windows [m^2]
+    qDistributionMin : Minimum operating power from the SC tank to the distribution system [kW]
+    qDistributionMax : Maximum operating power from the SC tank to the distribution system [kW]
+    tIndoorMin : Indoor minimum comfort temperature [ºC]
+    tIndoorMax : Indoor maximum comfort temperature [ºC]
+    tIndoorInit : Indoor initial temperature [ºC]
+    tWallInit : Wall initial temperature [ºC]
+    tDistributionInit : Distribution system initial temperature [ºC]
+    tAmbient : Ambient outside air temperature at each timestep [ºC]
+    totalIrradiationHorizontal : Total horizontal irradiation at each timestep [kW/m^2]
+    heatGainOccupants : Internal heat gains from occupants at each timestep [kW]
+    """
+
+    def __init__(
+            self,
+            tAmbient,
+            totalIrradiationHorizontal,
+            heatGainOccupants,
+            rDistribution=0.75,
+            cDistribution=0.26,
+            rIndoor=0.09,
+            cIndoor=0.97,
+            rWall=1.70,
+            cWall=226.30,
+            areaWindows=1.5,
+            qDistributionMin=0,
+            qDistributionMax=1000,
+            tIndoorMin=19,
+            tIndoorMax=23,
+            tIndoorInit=21,
+            tWallInit=21,
+            tDistributionInit=21,
+            **kwargs,
+    ):
+        super().__init__(**kwargs)
+        self.rDistribution = rDistribution
+        self.cDistribution = cDistribution
+        self.rIndoor = rIndoor
+        self.cIndoor = cIndoor
+        self.rWall = rWall
+        self.cWall = cWall
+        self.areaWindows = areaWindows
+        self.qDistributionMin = qDistributionMin
+        self.qDistributionMax = qDistributionMax
+        self.tIndoorMin = tIndoorMin
+        self.tIndoorMax = tIndoorMax
+        self.tIndoorInit = tIndoorInit
+        self.tWallInit = tWallInit
+        self.tDistributionInit = tDistributionInit
+        self.tAmbient = sequence(tAmbient)
+        self.totalIrradiationHorizontal = sequence(totalIrradiationHorizontal)
+        self.heatGainOccupants = sequence(heatGainOccupants)
+
+    def constraint_group(self):
+        return SinkRCModelBlock
+
+class SinkRCModelBlock(SimpleBlock):
+    """
+    Constraints for SinkRCModel Class
+    """
+    CONSTRAINT_GROUP = True
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def _create(self, group=None):
+        if group is None:
+            return None
+
+        m = self.parent_block()
+
+        # for all Sink RC model components get inflow from a bus
+        for n in group:
+            n.inflow = list(n.inputs)[0]
+
+        #  ************* SET OF CUSTOM SINK COMPONENTS *****************************
+
+        # Set of Sink RC model Components
+        self.sinkrc = Set(initialize=[n for n in group])
+
+        #  ************* DECISION VARIABLES *****************************
+
+        # Variable indoor temperature
+        self.tIndoor = Var(self.sinkrc, m.TIMESTEPS, within=Reals)
+
+        # Variable wall temperature
+        self.tWall = Var(self.sinkrc, m.TIMESTEPS, within=Reals)
+
+        # Variable distribution temperature
+        self.tDistribution = Var(self.sinkrc, m.TIMESTEPS, within=Reals)
+
+        # Variable indoor comfort temperature range violation
+        self.epsilonIndoor = Var(self.sinkrc, m.TIMESTEPS, within=NonNegativeReals)
+
+        # Variable indoor final temperature requirement violation
+        self.deltaIndoor = Var(self.sinkrc, within=NonNegativeReals)
+
+        # Variable binary indicator (0 whenever Q = 0)
+        # self.Xsc_dis = Var(self.sinkrc, m.TIMESTEPS, within=Boolean)
+
+        #  ************* CONSTRAINTS *****************************
+
+        def _initial_indoor_temperature_rule(block):
+            """set initial values of indoor temperature
+            """
+            for g in group:
+                lhs = self.tIndoor[g, 0]
+                rhs = g.tIndoorInit
+                block.initial_indoor_temperature.add((g, 0), (lhs == rhs))
+
+        self.initial_indoor_temperature = Constraint(group, m.TIMESTEPS, noruleinit=True)
+        self.initial_indoor_temperature_build = BuildAction(rule=_initial_indoor_temperature_rule)
+
+        def _initial_wall_temperature_rule(block):
+            """set initial values of wall temperature
+            """
+            for g in group:
+                lhs = self.tWall[g, 0]
+                rhs = g.tWallInit
+                block.initial_wall_temperature.add((g, 0), (lhs == rhs))
+
+        self.initial_wall_temperature = Constraint(group, m.TIMESTEPS, noruleinit=True)
+        self.initial_wall_temperature_build = BuildAction(rule=_initial_wall_temperature_rule)
+
+        def _initial_distribution_temperature_rule(block):
+            """set initial values of distribution temperature
+            """
+            for g in group:
+                lhs = self.tDistribution[g, 0]
+                rhs = g.tDistributionInit
+                block.initial_distribution_temperature.add((g, 0), (lhs == rhs))
+
+        self.initial_distribution_temperature = Constraint(group, m.TIMESTEPS, noruleinit=True)
+        self.initial_distribution_temperature_build = BuildAction(rule=_initial_distribution_temperature_rule)
+
+        #def _boolean_indicator_set_rule(block):
+        #    """sets the value of boolean indicator self.Xsc_dis
+        #    value is set to False whenever qDistribution = 0, otherwise True
+        #    """
+        #    for t in m.TIMESTEPS:
+        #        for g in group:
+        #            lhs = self.Xsc_dis[g, t]
+        #            rhs = not(m.flow[g.inflow, g, t] == 0)
+
+         #           block.boolean_indicator_set.add((g, t), (lhs == rhs))
+
+        #self.boolean_indicator_set = Constraint(group, m.TIMESTEPS, noruleinit=True)
+        #self.boolean_indicator_set_build = BuildAction(rule=_boolean_indicator_set_rule)
+
+        def _indoor_comfort_upper_limit_rule(block):
+            """Indoor comfort temperature < = maximum limit
+            """
+            for t in m.TIMESTEPS:
+                for g in group:
+                    lhs = self.tIndoor[g, t]
+                    #rhs = g.tIndoorMax
+                    rhs = g.tIndoorMax + self.epsilonIndoor[g, t]
+                    block.indoor_comfort_upper_limit.add((g, t), (lhs <= rhs))
+
+        self.indoor_comfort_upper_limit = Constraint(group, m.TIMESTEPS, noruleinit=True)
+        self.indoor_comfort_upper_limit_build = BuildAction(rule=_indoor_comfort_upper_limit_rule)
+
+        def _indoor_comfort_lower_limit_rule(block):
+            """Indoor comfort temperature > = minimum limit
+            """
+            for t in m.TIMESTEPS:
+                for g in group:
+                    lhs = self.tIndoor[g, t]
+                    # rhs = g.tIndoorMin
+                    rhs = g.tIndoorMin - self.epsilonIndoor[g, t]
+                    block.indoor_comfort_lower_limit.add((g, t), (lhs >= rhs))
+
+        self.indoor_comfort_lower_limit = Constraint(group, m.TIMESTEPS, noruleinit=True)
+        self.indoor_comfort_lower_limit_build = BuildAction(rule=_indoor_comfort_lower_limit_rule)
+
+        def _indoor_final_temperature_rule(block):
+            """Indoor temperature at the final timestamp should be higher than initial indoor temperature
+            """
+            t = m.TIMESTEPS[-1] #final timestep
+            for g in group:
+                lhs = self.tIndoor[g, t]
+                #rhs = g.tIndoorInit
+                rhs = g.tIndoorInit - self.deltaIndoor[g]
+                block.indoor_final_temperature.add((g, t), (lhs >= rhs))
+
+        self.indoor_final_temperature = Constraint(group, m.TIMESTEPS, noruleinit=True)
+        self.indoor_final_temperature_build = BuildAction(rule=_indoor_final_temperature_rule)
+
+        def _q_distribution_upper_limit_rule(block):
+            """q distribution < = maximum limit
+            """
+            for t in m.TIMESTEPS:
+                for g in group:
+                    lhs = m.flow[g.inflow, g, t]
+                    rhs = g.qDistributionMax
+                    # rhs = g.qDistributionMax * self.Xsc_dis[g, t]
+                    block.q_distribution_upper_limit.add((g, t), (lhs <= rhs))
+
+        self.q_distribution_upper_limit = Constraint(group, m.TIMESTEPS, noruleinit=True)
+        self.q_distribution_upper_limit_build = BuildAction(rule=_q_distribution_upper_limit_rule)
+
+        def _q_distribution_lower_limit_rule(block):
+            """q distribution > = minimum limit
+            """
+            for t in m.TIMESTEPS:
+                for g in group:
+                    lhs = m.flow[g.inflow, g, t]
+                    rhs = g.qDistributionMin
+                    # rhs = g.qDistributionMin * self.Xsc_dis[g, t]
+                    block.q_distribution_lower_limit.add((g, t), (lhs >= rhs))
+
+        self.q_distribution_lower_limit = Constraint(group, m.TIMESTEPS, noruleinit=True)
+        self.q_distribution_lower_limit_build = BuildAction(rule=_q_distribution_lower_limit_rule)
+
+        def _indoor_temperature_equation_rule(block):
+            """discrete state space equation for tIndoor
+            """
+            for g in group:
+                c2 = 1/(g.rIndoor*g.cIndoor)
+                c3 = 1/(g.rDistribution*g.cIndoor)
+                c1 = 1 - c2 - c3
+                c4 = g.areaWindows/g.cIndoor
+                for t in m.TIMESTEPS:
+                    if t!= m.TIMESTEPS[-1]:
+                        lhs = self.tIndoor[g, t+1]
+                        rhs = c1*self.tIndoor[g, t] + c2*self.tWall[g, t] + c3*self.tDistribution[g, t] + c4*(g.totalIrradiationHorizontal[t] + g.heatGainOccupants[t])
+                        block.indoor_temperature_equation.add((g, t), (lhs == rhs))
+
+        self.indoor_temperature_equation = Constraint(group, m.TIMESTEPS, noruleinit=True)
+        self.indoor_temperature_equation_build = BuildAction(rule=_indoor_temperature_equation_rule)
+
+        def _wall_temperature_equation_rule(block):
+            """discrete state space equation for tWall
+            """
+            for g in group:
+                c1 = 1 / (g.rIndoor * g.cWall)
+                c3 = 1 / (g.rWall * g.cWall)
+                c2 = 1 - c1 - c3
+                for t in m.TIMESTEPS:
+                    if t != m.TIMESTEPS[-1]:
+                        lhs = self.tWall[g, t + 1]
+                        rhs = c1 * self.tIndoor[g, t] + c2 * self.tWall[g, t] + c3 * g.tAmbient[t]
+                        block.wall_temperature_equation.add((g, t), (lhs == rhs))
+
+        self.wall_temperature_equation = Constraint(group, m.TIMESTEPS, noruleinit=True)
+        self.wall_temperature_equation_build = BuildAction(rule=_wall_temperature_equation_rule)
+
+        def _distribution_temperature_equation_rule(block):
+            """discrete state space equation for tDistribution
+            """
+            for g in group:
+                c1 = 1 / (g.rDistribution * g.cDistribution)
+                c2 = 1 - c1
+                c3 = 1 /g.cDistribution
+                for t in m.TIMESTEPS:
+                    if t != m.TIMESTEPS[-1]:
+                        lhs = self.tDistribution[g, t + 1]
+                        rhs = c1 * self.tIndoor[g, t] + c2 * self.tDistribution[g, t] + c3 * m.flow[g.inflow, g, t]
+                        block.distribution_temperature_equation.add((g, t), (lhs == rhs))
+
+        self.distribution_temperature_equation = Constraint(group, m.TIMESTEPS, noruleinit=True)
         self.distribution_temperature_equation_build = BuildAction(rule=_distribution_temperature_equation_rule)
```

### Comparing `optihood-0.0.0/optihood/sources.py` & `optihood-0.0.1/optihood/sources.py`

 * *Files identical despite different names*

### Comparing `optihood-0.0.0/optihood/storages.py` & `optihood-0.0.1/optihood/storages.py`

 * *Files identical despite different names*

### Comparing `optihood-0.0.0/optihood.egg-info/PKG-INFO` & `optihood-0.0.1/optihood.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,363 +1,366 @@
-Metadata-Version: 2.1
-Name: optihood
-Version: 0.0.0
-Summary: optihood optimization framework
-Home-page: https://optihood.readthedocs.io
-Author: Institute for Solar Technology (SPF), OST Rapperswil
-Author-email: neha.dimri@ost.ch
-License: UNKNOWN
-Description: # optihood: energy modelling and optimization framework
-        
-        optihood provides a complete python-based framework to **OPTI**mize the investment in alternative energy
-        technologies (heat pump, solar thermal, PV, etc.) as well as the operation of available energy resources (natural gas,
-        sun, grid electricity, etc.) for decentralized energy networks on a neighbour**HOOD**-scale. It is designed to facilitate 
-        the researchers and energy planners in optimizing an energy neighbourhood in terms of cost and/or environmental criteria. 
-        It enables the users to perform both single-objective and multi-objective optimization and analysis. The energy model and 
-        it's associated parameters can be defined easily using an excel file. Additionally, a variety of plotting methods are 
-        defined for easy and fast result visualization.
-        
-        ## Documentation
-        The documentation can be found on https://optihood.readthedocs.io/.
-        
-        ## Prerequisites
-        In order to use optihood, the following prerequisites are needed on your machine:
-        
-        - [Python 3.9](https://www.python.org/downloads/) is installed.
-        - Git is installed
-        - An active [Github](https://github.com/) account to clone the repo.
-        - A solver is installed. [Gurobi solver](https://www.gurobi.com/resource/parallelism-linear-mixed-integer-programming/)
-        is recommended, although other solvers like CBC, GLPK, Cplex could also be used.
-        
-        ## Installation
-        
-        As of now, optihood is available as an open source code and needs to be installed from source. Please follow the
-        instructions mentioned below to complete the installation. The commands given below are suited for the Windows platform
-        and should be run from within the optihood directory in a Command Prompt. For other platforms, similar alternative
-        commands could be used.
-        
-        1. Clone the optihood repo to a folder called 'optihood' on your local machine:
-            ```commandline
-            git clone https://github.com/SPF-OST/OptiHood.git
-            ```
-        2. All the next commands should be run from within the optihood folder. Create a virtual environment and activate it:
-            ```commandline
-            py -3.9 -m venv venv
-            venv\Scripts\activate
-            ```    
-        3. Install the requirements into the created virtual environment:
-            ```commandline
-            pip install wheel
-            pip install -r requirements.txt
-            ```
-        
-        
-            It might be required to install C++ build tools. To do that, click on the link that appears with the error message and follow the instructions (it is the lapack package that is missing). In order to be able to 
-            install the missing package, it is required to have a complete Visual Studio instance and installing it with the "Desktop development with C++" workload.
-           
-        4.  Verify the installation of the oemof package and the solver by running the installation test in your virtual environment:
-            ```commandline
-            oemof_installation_test
-            ```
-        
-            
-            If the installation is successful a message similar to the following would display (the installed solver would be marked as working):
-            ```commandline
-            *****************************
-            Solver installed with oemof
-            cbc: not working
-            glpk: not working
-            gurobi: working
-            cplex: not working
-            
-            *****************************
-            oemof successfully installed.
-            *****************************
-            ```
-        5.  To test whether the installation worked well, you could run a [basic example](https://github.com/SPF-OST/OptiHood/tree/main/data/examples/).
-        
-        ## Defining an energy network
-        
-        Optihood offers a several functionalities to define an energy network, optimize it and visualize the results, which
-        provides the user with a complete framework for optimization without the need to code by hand. 
-        
-        An energy network can be defined as an object of the EnergyNetworkIndiv class or the EnergyNetworkGroup class. This
-        object then acts as the primary container for the model. The EnergyNetworkClass is the main parent class, from which 
-        two child classes EnergyNetworkIndiv and EnergyNetworkGroup are inherited. Either EnergyNetworkIndiv class or 
-        EnergyNetworkGroup class could be used to define an energy network. The choice mainly depends on whether the buildings 
-        are linked together (electrically and/or thermally) or not.
-        
-        If the buildings within an energy network do not share electricity and/or heat, EnergyNetworkIndiv class is used:
-        
-            import EnergyNetworkIndiv
-            network = EnergyNetworkIndiv(dateTimeIndex, tSH=35, tDHW=55)
-            
-        Otherwise, if the buildings are expected to share energy (electrical and/or heat), EnergyNetworkGroup class is used:
-        
-            import EnergyNetworkGroup
-            network = EnergyNetworkGroup(dateTimeIndex, tSH=35, tDHW=55)
-            
-        The first parameter to be passed in both the cases is a Datetime index. This parameter gives the time range for an
-        optimization model. The Datetime index could be defined using date_range() in pandas:
-        
-            import pandas as pd
-            dateTimeIndex = pd.date_range('2021-01-01 00:00:00', '2021-12-31 23:00:00', freq="60min")
-            
-        The second and the third parameters tSH and tDHW define the temperatures for space heating and domestic hot water
-        production, respectively.
-        
-        Once the 'network' object has been created, the next step then is to build the model from an input excel file which
-        defines different components which constitute the model, how they are connected and their associated parameters:
-        
-            network.setFromExcel(inputExcelFilePath, numberOfBuildings, clusterSize, opt)
-            
-        'inputExcelFilePath' gives the path of the excel input file. 'numberofBuildings' is an integer parameter specifying the
-        number of buildings defined in the excel file. The last two parameters clusterSize and opt are optional. The 'opt'
-        parameter could be either 'costs' (default value) or 'env' depending on which criteria should be optimized. The
-        'clusterSize' parameter is used to provide a selected number of days which could be assumed representative of the entire
-        time range. For example: two typical days could be selected to model the entire year, which could represent two clusters
-        summer and winter. This would improve the optimization speed. If not given during the function call, the default value
-        of the clusterSize parameter assumes no day clusters.
-        
-        ## Input Excel File
-        
-        The input excel file is used to define an optimization model and set the model parameters. Each sheet of this excel file
-        is structured to defin different components, such as buses, storages and transformers, their respective parameters,
-        connections between these components and the building to which they belong.
-        
-        The input excel file typically has 9-10 sheets, each defining a different component type of the model.
-        
-        ### buses
-        This excel sheet defines the buses used in the energy network. Buses define the connections between different
-        components. Each row of this excel sheet represents a bus node in the model.
-        
-        - **label** (string):
-            label name of the bus. Should be unique for each building i.e. different buildings could have the same label for two
-            buses but for one building the buses should not have duplicate labels.
-        
-        - **active** (0 or 1):
-            If set to 1 then the corresponding bus is active, otherwise (if 0) then the bus is inactive in the model. Could be
-            used to optimize different scenarios with different buses without the need to re-construct the base excel file.
-        
-        - **excess** (0 or 1):
-            If set to 1 then the corresponding bus has the possibility of having an excess flow unbalanced to the demand. An
-            additional sink node is automatically added in this case to accept this excess flow. If set to 0 then the bus cannot
-            have an excess flow.
-        
-        - **excess costs** (float):
-            The associated cost of excess flow from a bus. Relevant only if **excess** is set to 1. Could be negative to denote
-            monetary gains such as in case of PV feed-in.
-        
-        - **building** (integer):
-            Building number to which the bus belongs. Should be unique for each building.
-        
-        ### commodity_sources
-        This sheet defines the different commodity sources which serve as an energy input to the model. The parameters **label**,
-        **active** and **building** are analogous to the parameters described earlier for buses.
-        
-        - **to** (string):
-            Label of bus to which the energy from the commodity source flows. The corresponding bus label should exist in
-            the buses sheet.
-        
-        - **variable costs** (float):
-            Cost per kW of the commodity source.
-        
-        - **CO2 impact** (float):
-            CO2 impact per kW of the commodity source.
-        
-        ### demand
-        The nodes related to the energy demand i.e. sink are defined in this sheet. The parameters **label**, **active** and
-        **building** are analogous to the parameters described earlier for buses.
-        
-        - **from** (string):
-            Label of the bus from which the energy flows to the demand node. The corresponding bus label should exist in
-            the buses sheet.
-        
-        - **fixed** (0 or 1):
-            If set to 1, the energy demand profiles are fixed and a path to the demand profiles should then be given in the
-            csv_data sheet of the input excel file. If set to 0, the optimizer will select the demand profiles for optimum
-            operation (a total annual demand profile could be given in this case). At the present development stage only fixed
-            demands are accepted.
-        
-        - **nominal value** (float):
-            The demand profiles series should be normalized values. this parameter then defines the maximum demand with which
-            the normalized series is multiplied to obtain the actual demand profile series. If set to 1, then the given demand
-            profile series is taken as it is (not normalized).
-        
-        ### transformers
-        The nodes related to the energy conversion units (or transformers) such as CHP, heat pump, etc. are given in this excel
-        sheet. The parameters **label**, **active** and **building** are analogous to the parameters described earlier for buses.
-        
-        - **from** (string):
-            Label of bus from which the energy flows to the transformer node. The corresponding bus label should exist in
-            the buses sheet.
-        
-        - **to** (strings separated by comma):
-            Label of the bus(es) to which the energy flows from the transformer node. Different bus labels should be separated
-            by a comma (,), for example: Bus1, Bus2, Bus3. The bus label(s) should exist in the buses sheet.
-        
-        - **efficiency** (float values separated by comma):
-            Conversion efficiency from input to the output(s) of the transformer node. Efficiencies should be separated by
-            a comma (,) in the case with more than one outputs (i.e. when more than one buses are listed under **to**).
-        
-        - **capacity_DHW** (float):
-            Maximum capacity limit for domestic hot water (DHW) production from the transformer unit in kW. Could be left blank
-            if the parameter is not relevant to a transformer (for example if a transformer does not produce DHW)
-        
-        - **capacity_SH** (float):
-            Maximum capacity limit for space heat (SH) production from the transformer unit in kW. Could be left blank if the
-            parameter is not relevant to a transformer (for example if a transformer does not produce SH)
-        
-        - **capacity_el** (float):
-            Maximum capacity limit for electricity production from the transformer unit in kW. Could be left blank if the
-            parameter is not relevant to a transformer (for example if a transformer does not produce electricity). Note for CHP
-            this parameter acts as the main capacity against which optimization is performed.
-        
-        - **capacity_min** (float):
-            Minimum capacity to be installed in kW for an investment in the transformer unit.
-        
-        - **lifetime** (non-negative integer):
-            Lifetime of the node in years.
-        
-        - **invest_base** (float):
-            Base investment cost of the node.
-        
-        - **invest_cap** (float):
-            Investment cost per unit installed capacity (i.e. per kW) of the node.
-        
-        - **maintenance** (float):
-            Maintenance cost of the node. Given as a percentage of the base investment cost **invest_base**. For example:
-            if the investment cost is to be taken as 5% of **invest_base**, then the value of **maintenance** field should be 0.05.
-            Set as 0 if this cost is to be ignored.
-        
-        - **installation** (float):
-            Installation cost of the node. Given as a percentage of the base investment cost **invest_base**. For example:
-            if the Installation cost is to be taken as 15% of **invest_base**, then **installation** field should be 0.15. Set
-            as 0 if this cost is to be ignored.
-        
-        - **planification** (float):
-            Cost associated with planning. Given as a percentage of the base investment cost **invest_base**. For example:
-            if the planning cost is 5% of **invest_base**, then **planification** should be 0.05. Set as 0 if this cost is to be
-            ignored.
-        
-        - **heat_impact** (float):
-            Environmental impact for heat production. Set as 0 if there is no impact due to heat production.
-        
-        - **elec_impact** (float):
-            Environmental impact for electricity production. Set as 0 if there is no impact due to electricity production.
-        
-        - **impact_cap** (float):
-            Environmental impact per unit installed capacity i.e. per kW of the node. Set as 0 if there is no impact per
-            installed capacity of the node.
-        
-        ### solar
-        This excel sheet defines the parameters related to the solar components such as solar thermal collector and PV panels.
-        The parameters **label**, **active** and **building** are analogous to the parameters described earlier for buses.
-        **from** and **to** parameters have been previously defined for commodity sources and demand sheets, respectively, while
-        the cost and environmental impact paramaters are described under transformers sheet.
-        
-        - **connect** (string):
-            Label of the bus which connects a solar collector to the model. This bus allows excess heat production from the solar
-            collector. A node for heat sink is created automatically. The given bus label should exist in the buses sheet. This
-            parameter is irrelevant for PV.
-        
-        - **electrical_consumption** (float):
-            Electrical consumption of the solar component. Given as a percentage fraction of the energy produced. 0.02 means
-            the electrical consumption is 2% of the energy is produced.
-        
-        - **peripheral_losses** (float):
-            Peripheral losses of the solar component. Given as a percentage fraction of the energy produced. 0.05 means 5% of
-            the energy produced is lost to the surrounding environment.
-        
-        - **latitude** (float):
-            Latitude of the geographical location where the solar collector/panel is placed. Given in degrees.
-        
-        - **longitude** (float):
-            Longitude of the geographical location where the solar collector/panel is placed. Given in degrees.
-        
-        - **tilt** (float):
-            Tilt angle of the solar collector/panel. Given in degrees.
-        
-        - **azimuth** (float):
-            Azimuth angle of the solar collector/panel. Given in degrees.
-        
-        - **eta_0**, **a_1** and **a_2** (float):
-            Efficiency parameters of the solar thermal collector. Solar thermal collector is linearized using the pre-calculations
-            given in [oemof-thermal](https://oemof-thermal.readthedocs.io/en/latest/solar_thermal_collector.html).
-        
-        - **temp_collector_inlet** (float):
-            Inlet fluid temperature of the solar thermal collector. Given in degree C.
-        
-        - **delta_temp_n** (float):
-            Temperature difference between the inlet fluid and the mean fluid temperature in case of solar collector. For PV,
-            this parameter denotes the temperature difference between the solar cells and the ambient.
-        
-        - **capacity_max** (float):
-            Maximum capacity limit in kW.
-        
-        - **capacity_min** (float):
-            Minimum possible capacity in kW for the installation of solar collector/panel.
-        
-        ### storages
-        This excel sheet defines the parameters related to the energy storage units such as battery and hot water tank. **label**,
-        **active** and **building** have been defined previously for buses excel sheet. A description of **from** and **to** has
-        been given in commodity sources and demand sheets, respectively. The cost and environmental impact parameters are
-        described in the transformers sheet section. **capacity_min** and **capacity_max** are described in the solar excel sheet
-        section.
-        
-        - **efficiency inflow** (float):
-            Charging efficiency of battery. This parameter is not relevant for thermal storages.
-        
-        - **efficiency outflow** (float):
-            Discharging efficiency of battery. This parameter is not relevant for thermal storages.
-        
-        - **initial capacity** (float):
-            initial capacity of the storage. This parameter is expressed as a fraction of the total storage capacity. 0 means storage is initially 
-            assumed to be empty, 1 denotes that the storage is 100% full initially, while 0.5 means the storage is at 50% capacity initially.
-        
-        - **capacity loss** (float):
-            Losses from battery storage. This parameter is not relevant for thermal storages.
-        
-        ### stratified_storage
-        This excel sheet defines the parameters relevant to stratified thermal storage. The pre-calculations given in [oemof-thermal](https://oemof-thermal.readthedocs.io/en/latest/stratified_thermal_storage.html)
-        have been used to linearize the thermal hot water storage. The parameter names used here are similar to the parameters
-        defined in oemof-thermal.
-        
-        ### links
-        This excel sheet defines the parameters for electricity and space heating links. The buildings could share electricity
-        production and/or space heat production. Links allow this sharing to be possible. **label** and **active** have been
-        defined already for buses excel sheet. **invest_base** and **invest_cap** parameters (defined in the transformers sheet
-        section) are only relevant for space heating links in the present stage of development.
-        
-        - **buildingA** (integer):
-            Building number of the first building of the link. This should match with the values typically given in the
-            **building** parameter in the other excel sheets.
-        
-        - **buildingB** (integer):
-            Building number of the second building of the link. This should match with the values typically given in the
-            **building** parameter in the other excel sheets.
-        
-        - **efficiency from A to B** (integer):
-            Efficiency of energy transfer over the link from **buildingA** to **buildingB**.
-        
-        - **efficiency from B to A** (integer):
-            Efficiency of energy transfer over the link from **buildingB** to **buildingA**.
-        
-        ### csv_data
-        The paths to CSV files containing demand profiles, weather data and electricity impact data are to be given in this
-        excel sheet. **INFO** gives further information about each row.
-        
-        ### grid_connection
-        This excel sheet should not be modified by the users. It defines the separation of the flows from electricity grid and
-        the produced electricity flows to make sure that the grid electricity is not stored in batteries.
-        
-        
-        ## Collaborators
-        
-        SPF/OST & HEIG-VD
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: ==3.9
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: optihood
+Version: 0.0.1
+Summary: optihood optimization framework
+Home-page: https://optihood.readthedocs.io
+Author: Institute for Solar Technology (SPF), OST Rapperswil
+Author-email: neha.dimri@ost.ch
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# optihood: energy modelling and optimization framework
+
+optihood provides a complete python-based framework to **OPTI**mize the investment in alternative energy
+technologies (heat pump, solar thermal, PV, etc.) as well as the operation of available energy resources (natural gas,
+sun, grid electricity, etc.) for decentralized energy networks on a neighbour**HOOD**-scale. It is designed to facilitate 
+the researchers and energy planners in optimizing an energy neighbourhood in terms of cost and/or environmental criteria. 
+It enables the users to perform both single-objective and multi-objective optimization and analysis. The energy model and 
+it's associated parameters can be defined easily using an excel file. Additionally, a variety of plotting methods are 
+defined for easy and fast result visualization.
+
+## Documentation
+The documentation can be found on https://optihood.readthedocs.io/.
+
+## Prerequisites
+In order to use optihood, the following prerequisites are needed on your machine:
+
+- [Python 3.9](https://www.python.org/downloads/) is installed.
+- Git is installed
+- An active [Github](https://github.com/) account to clone the repo.
+- A solver is installed. [Gurobi solver](https://www.gurobi.com/resource/parallelism-linear-mixed-integer-programming/)
+is recommended, although other solvers like CBC, GLPK, Cplex could also be used.
+
+## Installation
+
+As of now, optihood is available as an open source code and needs to be installed from source. Please follow the
+instructions mentioned below to complete the installation. The commands given below are suited for the Windows platform
+and should be run from within the optihood directory in a Command Prompt. For other platforms, similar alternative
+commands could be used.
+
+1. Clone the optihood repo to a folder called 'optihood' on your local machine:
+    ```commandline
+    git clone https://github.com/SPF-OST/OptiHood.git
+    ```
+2. All the next commands should be run from within the optihood folder. Create a virtual environment and activate it:
+    ```commandline
+    py -3.9 -m venv venv
+    venv\Scripts\activate
+    ```    
+3. Install the requirements into the created virtual environment:
+    ```commandline
+    pip install wheel
+    pip install -r requirements.txt
+    ```
+
+
+    It might be required to install C++ build tools. To do that, click on the link that appears with the error message and follow the instructions (it is the lapack package that is missing). In order to be able to 
+    install the missing package, it is required to have a complete Visual Studio instance and installing it with the "Desktop development with C++" workload.
+   
+4.  Verify the installation of the oemof package and the solver by running the installation test in your virtual environment:
+    ```commandline
+    oemof_installation_test
+    ```
+
+    
+    If the installation is successful a message similar to the following would display (the installed solver would be marked as working):
+    ```commandline
+    *****************************
+    Solver installed with oemof
+    cbc: not working
+    glpk: not working
+    gurobi: working
+    cplex: not working
+    
+    *****************************
+    oemof successfully installed.
+    *****************************
+    ```
+5.  To test whether the installation worked well, you could run a [basic example](https://github.com/SPF-OST/OptiHood/tree/main/data/examples/).
+
+## Defining an energy network
+
+Optihood offers a several functionalities to define an energy network, optimize it and visualize the results, which
+provides the user with a complete framework for optimization without the need to code by hand. 
+
+An energy network can be defined as an object of the EnergyNetworkIndiv class or the EnergyNetworkGroup class. This
+object then acts as the primary container for the model. The EnergyNetworkClass is the main parent class, from which 
+two child classes EnergyNetworkIndiv and EnergyNetworkGroup are inherited. Either EnergyNetworkIndiv class or 
+EnergyNetworkGroup class could be used to define an energy network. The choice mainly depends on whether the buildings 
+are linked together (electrically and/or thermally) or not.
+
+If the buildings within an energy network do not share electricity and/or heat, EnergyNetworkIndiv class is used:
+
+    import EnergyNetworkIndiv
+    network = EnergyNetworkIndiv(dateTimeIndex, tSH=35, tDHW=55)
+    
+Otherwise, if the buildings are expected to share energy (electrical and/or heat), EnergyNetworkGroup class is used:
+
+    import EnergyNetworkGroup
+    network = EnergyNetworkGroup(dateTimeIndex, tSH=35, tDHW=55)
+    
+The first parameter to be passed in both the cases is a Datetime index. This parameter gives the time range for an
+optimization model. The Datetime index could be defined using date_range() in pandas:
+
+    import pandas as pd
+    dateTimeIndex = pd.date_range('2021-01-01 00:00:00', '2021-12-31 23:00:00', freq="60min")
+    
+The second and the third parameters tSH and tDHW define the temperatures for space heating and domestic hot water
+production, respectively.
+
+Once the 'network' object has been created, the next step then is to build the model from an input excel file which
+defines different components which constitute the model, how they are connected and their associated parameters:
+
+    network.setFromExcel(inputExcelFilePath, numberOfBuildings, clusterSize, opt)
+    
+'inputExcelFilePath' gives the path of the excel input file. 'numberofBuildings' is an integer parameter specifying the
+number of buildings defined in the excel file. The last two parameters clusterSize and opt are optional. The 'opt'
+parameter could be either 'costs' (default value) or 'env' depending on which criteria should be optimized. The
+'clusterSize' parameter is used to provide a selected number of days which could be assumed representative of the entire
+time range. For example: two typical days could be selected to model the entire year, which could represent two clusters
+summer and winter. This would improve the optimization speed. If not given during the function call, the default value
+of the clusterSize parameter assumes no day clusters.
+
+## Input Excel File
+
+The input excel file is used to define an optimization model and set the model parameters. Each sheet of this excel file
+is structured to defin different components, such as buses, storages and transformers, their respective parameters,
+connections between these components and the building to which they belong.
+
+The input excel file typically has 9-10 sheets, each defining a different component type of the model.
+
+### buses
+This excel sheet defines the buses used in the energy network. Buses define the connections between different
+components. Each row of this excel sheet represents a bus node in the model.
+
+- **label** (string):
+    label name of the bus. Should be unique for each building i.e. different buildings could have the same label for two
+    buses but for one building the buses should not have duplicate labels.
+
+- **active** (0 or 1):
+    If set to 1 then the corresponding bus is active, otherwise (if 0) then the bus is inactive in the model. Could be
+    used to optimize different scenarios with different buses without the need to re-construct the base excel file.
+
+- **excess** (0 or 1):
+    If set to 1 then the corresponding bus has the possibility of having an excess flow unbalanced to the demand. An
+    additional sink node is automatically added in this case to accept this excess flow. If set to 0 then the bus cannot
+    have an excess flow.
+
+- **excess costs** (float):
+    The associated cost of excess flow from a bus. Relevant only if **excess** is set to 1. Could be negative to denote
+    monetary gains such as in case of PV feed-in.
+
+- **building** (integer):
+    Building number to which the bus belongs. Should be unique for each building.
+
+### commodity_sources
+This sheet defines the different commodity sources which serve as an energy input to the model. The parameters **label**,
+**active** and **building** are analogous to the parameters described earlier for buses.
+
+- **to** (string):
+    Label of bus to which the energy from the commodity source flows. The corresponding bus label should exist in
+    the buses sheet.
+
+- **variable costs** (float):
+    Cost per kW of the commodity source.
+
+- **CO2 impact** (float):
+    CO2 impact per kW of the commodity source.
+
+### demand
+The nodes related to the energy demand i.e. sink are defined in this sheet. The parameters **label**, **active** and
+**building** are analogous to the parameters described earlier for buses.
+
+- **from** (string):
+    Label of the bus from which the energy flows to the demand node. The corresponding bus label should exist in
+    the buses sheet.
+
+- **fixed** (0 or 1):
+    If set to 1, the energy demand profiles are fixed and a path to the demand profiles should then be given in the
+    csv_data sheet of the input excel file. If set to 0, the optimizer will select the demand profiles for optimum
+    operation (a total annual demand profile could be given in this case). At the present development stage only fixed
+    demands are accepted.
+
+- **nominal value** (float):
+    The demand profiles series should be normalized values. this parameter then defines the maximum demand with which
+    the normalized series is multiplied to obtain the actual demand profile series. If set to 1, then the given demand
+    profile series is taken as it is (not normalized).
+
+### transformers
+The nodes related to the energy conversion units (or transformers) such as CHP, heat pump, etc. are given in this excel
+sheet. The parameters **label**, **active** and **building** are analogous to the parameters described earlier for buses.
+
+- **from** (string):
+    Label of bus from which the energy flows to the transformer node. The corresponding bus label should exist in
+    the buses sheet.
+
+- **to** (strings separated by comma):
+    Label of the bus(es) to which the energy flows from the transformer node. Different bus labels should be separated
+    by a comma (,), for example: Bus1, Bus2, Bus3. The bus label(s) should exist in the buses sheet.
+
+- **efficiency** (float values separated by comma):
+    Conversion efficiency from input to the output(s) of the transformer node. Efficiencies should be separated by
+    a comma (,) in the case with more than one outputs (i.e. when more than one buses are listed under **to**).
+
+- **capacity_DHW** (float):
+    Maximum capacity limit for domestic hot water (DHW) production from the transformer unit in kW. Could be left blank
+    if the parameter is not relevant to a transformer (for example if a transformer does not produce DHW)
+
+- **capacity_SH** (float):
+    Maximum capacity limit for space heat (SH) production from the transformer unit in kW. Could be left blank if the
+    parameter is not relevant to a transformer (for example if a transformer does not produce SH)
+
+- **capacity_el** (float):
+    Maximum capacity limit for electricity production from the transformer unit in kW. Could be left blank if the
+    parameter is not relevant to a transformer (for example if a transformer does not produce electricity). Note for CHP
+    this parameter acts as the main capacity against which optimization is performed.
+
+- **capacity_min** (float):
+    Minimum capacity to be installed in kW for an investment in the transformer unit.
+
+- **lifetime** (non-negative integer):
+    Lifetime of the node in years.
+
+- **invest_base** (float):
+    Base investment cost of the node.
+
+- **invest_cap** (float):
+    Investment cost per unit installed capacity (i.e. per kW) of the node.
+
+- **maintenance** (float):
+    Maintenance cost of the node. Given as a percentage of the base investment cost **invest_base**. For example:
+    if the investment cost is to be taken as 5% of **invest_base**, then the value of **maintenance** field should be 0.05.
+    Set as 0 if this cost is to be ignored.
+
+- **installation** (float):
+    Installation cost of the node. Given as a percentage of the base investment cost **invest_base**. For example:
+    if the Installation cost is to be taken as 15% of **invest_base**, then **installation** field should be 0.15. Set
+    as 0 if this cost is to be ignored.
+
+- **planification** (float):
+    Cost associated with planning. Given as a percentage of the base investment cost **invest_base**. For example:
+    if the planning cost is 5% of **invest_base**, then **planification** should be 0.05. Set as 0 if this cost is to be
+    ignored.
+
+- **heat_impact** (float):
+    Environmental impact for heat production. Set as 0 if there is no impact due to heat production.
+
+- **elec_impact** (float):
+    Environmental impact for electricity production. Set as 0 if there is no impact due to electricity production.
+
+- **impact_cap** (float):
+    Environmental impact per unit installed capacity i.e. per kW of the node. Set as 0 if there is no impact per
+    installed capacity of the node.
+
+### solar
+This excel sheet defines the parameters related to the solar components such as solar thermal collector and PV panels.
+The parameters **label**, **active** and **building** are analogous to the parameters described earlier for buses.
+**from** and **to** parameters have been previously defined for commodity sources and demand sheets, respectively, while
+the cost and environmental impact paramaters are described under transformers sheet.
+
+- **connect** (string):
+    Label of the bus which connects a solar collector to the model. This bus allows excess heat production from the solar
+    collector. A node for heat sink is created automatically. The given bus label should exist in the buses sheet. This
+    parameter is irrelevant for PV.
+
+- **electrical_consumption** (float):
+    Electrical consumption of the solar component. Given as a percentage fraction of the energy produced. 0.02 means
+    the electrical consumption is 2% of the energy is produced.
+
+- **peripheral_losses** (float):
+    Peripheral losses of the solar component. Given as a percentage fraction of the energy produced. 0.05 means 5% of
+    the energy produced is lost to the surrounding environment.
+
+- **latitude** (float):
+    Latitude of the geographical location where the solar collector/panel is placed. Given in degrees.
+
+- **longitude** (float):
+    Longitude of the geographical location where the solar collector/panel is placed. Given in degrees.
+
+- **tilt** (float):
+    Tilt angle of the solar collector/panel. Given in degrees.
+
+- **azimuth** (float):
+    Azimuth angle of the solar collector/panel. Given in degrees.
+
+- **eta_0**, **a_1** and **a_2** (float):
+    Efficiency parameters of the solar thermal collector. Solar thermal collector is linearized using the pre-calculations
+    given in [oemof-thermal](https://oemof-thermal.readthedocs.io/en/latest/solar_thermal_collector.html).
+
+- **temp_collector_inlet** (float):
+    Inlet fluid temperature of the solar thermal collector. Given in degree C.
+
+- **delta_temp_n** (float):
+    Temperature difference between the inlet fluid and the mean fluid temperature in case of solar collector. For PV,
+    this parameter denotes the temperature difference between the solar cells and the ambient.
+
+- **capacity_max** (float):
+    Maximum capacity limit in kW.
+
+- **capacity_min** (float):
+    Minimum possible capacity in kW for the installation of solar collector/panel.
+
+### storages
+This excel sheet defines the parameters related to the energy storage units such as battery and hot water tank. **label**,
+**active** and **building** have been defined previously for buses excel sheet. A description of **from** and **to** has
+been given in commodity sources and demand sheets, respectively. The cost and environmental impact parameters are
+described in the transformers sheet section. **capacity_min** and **capacity_max** are described in the solar excel sheet
+section.
+
+- **efficiency inflow** (float):
+    Charging efficiency of battery. This parameter is not relevant for thermal storages.
+
+- **efficiency outflow** (float):
+    Discharging efficiency of battery. This parameter is not relevant for thermal storages.
+
+- **initial capacity** (float):
+    initial capacity of the storage. This parameter is expressed as a fraction of the total storage capacity. 0 means storage is initially 
+    assumed to be empty, 1 denotes that the storage is 100% full initially, while 0.5 means the storage is at 50% capacity initially.
+
+- **capacity loss** (float):
+    Losses from battery storage. This parameter is not relevant for thermal storages.
+
+### stratified_storage
+This excel sheet defines the parameters relevant to stratified thermal storage. The pre-calculations given in [oemof-thermal](https://oemof-thermal.readthedocs.io/en/latest/stratified_thermal_storage.html)
+have been used to linearize the thermal hot water storage. The parameter names used here are similar to the parameters
+defined in oemof-thermal.
+
+### links
+This excel sheet defines the parameters for electricity and space heating links. The buildings could share electricity
+production and/or space heat production. Links allow this sharing to be possible. **label** and **active** have been
+defined already for buses excel sheet. **invest_base** and **invest_cap** parameters (defined in the transformers sheet
+section) are only relevant for space heating links in the present stage of development.
+
+- **buildingA** (integer):
+    Building number of the first building of the link. This should match with the values typically given in the
+    **building** parameter in the other excel sheets.
+
+- **buildingB** (integer):
+    Building number of the second building of the link. This should match with the values typically given in the
+    **building** parameter in the other excel sheets.
+
+- **efficiency from A to B** (integer):
+    Efficiency of energy transfer over the link from **buildingA** to **buildingB**.
+
+- **efficiency from B to A** (integer):
+    Efficiency of energy transfer over the link from **buildingB** to **buildingA**.
+
+### csv_data
+The paths to CSV files containing demand profiles, weather data and electricity impact data are to be given in this
+excel sheet. **INFO** gives further information about each row.
+
+### grid_connection
+This excel sheet should not be modified by the users. It defines the separation of the flows from electricity grid and
+the produced electricity flows to make sure that the grid electricity is not stored in batteries.
+
+
+## Collaborators
+
+SPF/OST & HEIG-VD
+
+
```

