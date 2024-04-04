# Comparing `tmp/InfraFair-1.0.0.tar.gz` & `tmp/InfraFair-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InfraFair-1.0.0.tar", last modified: Sat Jan 20 10:02:54 2024, max compression
+gzip compressed data, was "InfraFair-1.1.0.tar", last modified: Thu Apr  4 08:30:32 2024, max compression
```

## Comparing `InfraFair-1.0.0.tar` & `InfraFair-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-01-20 10:02:54.981871 InfraFair-1.0.0/
-drwxrwxrwx   0        0        0        0 2024-01-20 10:02:54.970693 InfraFair-1.0.0/InfraFair/
--rw-rw-rw-   0        0        0   143484 2024-01-09 05:00:49.000000 InfraFair-1.0.0/InfraFair/InfraFair.py
--rw-rw-rw-   0        0        0      184 2024-01-09 05:00:49.000000 InfraFair-1.0.0/InfraFair/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-20 10:02:54.981871 InfraFair-1.0.0/InfraFair.egg-info/
--rw-rw-rw-   0        0        0     1024 2024-01-20 10:02:54.000000 InfraFair-1.0.0/InfraFair.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-01-20 10:02:54.000000 InfraFair-1.0.0/InfraFair.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       72 2024-01-20 10:02:54.000000 InfraFair-1.0.0/InfraFair.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-01-20 10:02:54.000000 InfraFair-1.0.0/InfraFair.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-01-20 10:02:54.000000 InfraFair-1.0.0/InfraFair.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35184 2024-01-09 05:00:49.000000 InfraFair-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1024 2024-01-20 10:02:54.981871 InfraFair-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     7339 2024-01-09 05:00:49.000000 InfraFair-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-01-20 10:02:54.996875 InfraFair-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2124 2024-01-09 05:00:49.000000 InfraFair-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 08:30:32.451384 InfraFair-1.1.0/
+drwxrwxrwx   0        0        0        0 2024-04-04 08:30:32.416560 InfraFair-1.1.0/InfraFair/
+-rw-rw-rw-   0        0        0   191072 2024-04-04 07:36:36.000000 InfraFair-1.1.0/InfraFair/InfraFair.py
+-rw-rw-rw-   0        0        0      184 2024-04-04 08:23:30.000000 InfraFair-1.1.0/InfraFair/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 08:30:32.447311 InfraFair-1.1.0/InfraFair.egg-info/
+-rw-rw-rw-   0        0        0      916 2024-04-04 08:30:32.000000 InfraFair-1.1.0/InfraFair.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2024-04-04 08:30:32.000000 InfraFair-1.1.0/InfraFair.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       72 2024-04-04 08:30:32.000000 InfraFair-1.1.0/InfraFair.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-04 08:30:32.000000 InfraFair-1.1.0/InfraFair.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-04 08:30:32.000000 InfraFair-1.1.0/InfraFair.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    34523 2023-11-27 17:41:21.000000 InfraFair-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      916 2024-04-04 08:30:32.451384 InfraFair-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6056 2023-12-05 00:25:44.000000 InfraFair-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-04 08:30:32.451384 InfraFair-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2131 2024-04-04 08:27:18.000000 InfraFair-1.1.0/setup.py
```

### Comparing `InfraFair-1.0.0/InfraFair/InfraFair.py` & `InfraFair-1.1.0/InfraFair/InfraFair.py`

 * *Files 24% similar despite different names*

```diff
@@ -46,43 +46,42 @@
   $$ |  $$  __$$\ $$$$\     $$  __$$\  \____$$\ $$$$$\     \____$$\ $$ |$$  __$$\ 
   $$ |  $$ |  $$ |$$  _|    $$ |  \__| $$$$$$$ |$$  __|    $$$$$$$ |$$ |$$ |  \__|
   $$ |  $$ |  $$ |$$ |      $$ |      $$  __$$ |$$ |      $$  __$$ |$$ |$$ |      
 $$$$$$\ $$ |  $$ |$$ |      $$ |      \$$$$$$$ |$$ |      \$$$$$$$ |$$ |$$ |      
 \______|\__|  \__|\__|      \__|       \_______|\__|       \_______|\__|\__|      
 """
 
+
 #%% utility/auxiliary functions
 
 def get_line_index(lines: pd.DataFrame, node1: int, node2: int) -> int:
     "This function return the index of the line, from the lines matrix, connecting two nodes"
     # Note: The assumption here is that there is no two lines with the same nodes, i.e., no double circuits
 
     line_name   = str(node1) + "-" + str(node2)
     temp        = lines[lines["Line"]  == line_name].index.values
-    if not temp: # if it is empty
+    if len(temp) == 0: # if it is empty
         line_name   = str(node2) + "-" + str(node1)
-    
-    return lines[lines["Line"]  == line_name].index.values[0]
+      
+    return lines[lines["Line"]  == line_name].index.values
 
 
 def get_node_index(node: int, nodes_matrix: pd.DataFrame) -> int:
     "This function return the index of a node"
 
     return nodes_matrix[nodes_matrix["Node"] == node].index.values[0]
 
 
 def get_total_nodal_flows(flows: np.ndarray, gen: np.ndarray, dem: np.ndarray) -> np.ndarray:
     "This function return a flow matrix with the generation and demand as inflows and outflows, respectively"
 
-    nodal                   = dem - gen
-    flows_node              = np.zeros(flows.shape)
-    flows_node[:, :]        = flows[:, :]
-    for i in range(len(flows_node)):
-        flows_node[i, i]    = nodal[i, 0]
-    
+    nodal       = dem - gen
+    flows_node  = np.diag(nodal[:,0])
+    flows_node  += flows
+
     return flows_node
 
 
 def get_node_owner(node: int, nodes_matrix: pd.DataFrame, column: str) -> int:
     "This function return the country of a node"
 
     return nodes_matrix[column][nodes_matrix[nodes_matrix["Node"] == node].index.values[0]]
@@ -239,38 +238,38 @@
 
 
 #%% primary functions
 
 def get_input_matrices(lines_matrix: pd.DataFrame, nodes_matrix: pd.DataFrame, attribute_matrix: pd.DataFrame, attribute_dic:dict, SO_owner: bool = False, process_line_ownership: bool = False, reactance: bool = False) -> Tuple[np.ndarray, np.ndarray, list, np.ndarray, np.ndarray, np.ndarray, pd.DataFrame, pd.DataFrame, pd.DataFrame]:
     "This function prepares the basic input matrices from the excel file and also returns interconnections between countries and owners of the lines"
 
-    gen                 = nodes_matrix["Generation"].to_numpy()[None].transpose()         # The generation matrix
+    gen                 = nodes_matrix["Generation"].to_numpy()[None].transpose()           # The generation matrix
     dem                 = nodes_matrix["Demand"].to_numpy()[None].transpose()               # The demand matrix
     phi                 = lines_matrix["Flow"].to_numpy()[None].transpose()                 # The flow matrix
     phi_positive        = np.absolute(phi)                                                  # Positive flow matrix
     interconnections_C  = pd.DataFrame(columns=["Line","Country 1", "Country 2", "Flow"])   # Interconnection matrix between countries
-    interconnections_T  = pd.DataFrame(columns=["Line","SO 1", "SO 2", "Flow"])           # Interconnection matrix between SOs
+    interconnections_T  = pd.DataFrame(columns=["Line","SO 1", "SO 2", "Flow"])             # Interconnection matrix between SOs
     ownership           = pd.DataFrame(lines_matrix["Line"],index = lines_matrix.index)
 
     if reactance:
-        react = lines_matrix["React"].to_numpy().tolist()  # The reactance matrix
+        react = attribute_matrix["React"].to_numpy().tolist()  # The reactance matrix
     else:
         react = []
 
     flows_matrix                    = np.zeros((nodes_matrix.shape[0], nodes_matrix.shape[0]))  # Flow matrix that shows the inflows (negative) and outflows (positive) of each node
     ownership["Country 1"]          = ownership["Country 2"] = ""
     if process_line_ownership and SO_owner:
         ownership["SO Owner 1"]     = ownership["SO Owner 2"]      = ""
         ownership["SO 1 Ownership"] = ownership["SO 2 Ownership"]  = 0.0
     
     for index in lines_matrix.index:
         node1, node2 = lines_matrix["Line"][index].split("-")
         node1, node2 =  int(node1), int(node2)
-        flows_matrix[get_node_index(node1, nodes_matrix) - 1, get_node_index(node2, nodes_matrix) - 1] = lines_matrix["Flow"][index]
-        flows_matrix[get_node_index(node2, nodes_matrix) - 1, get_node_index(node1, nodes_matrix) - 1] = -lines_matrix["Flow"][index]
+        flows_matrix[get_node_index(node1, nodes_matrix) - 1, get_node_index(node2, nodes_matrix) - 1] += lines_matrix["Flow"][index]
+        flows_matrix[get_node_index(node2, nodes_matrix) - 1, get_node_index(node1, nodes_matrix) - 1] -= lines_matrix["Flow"][index]
 
         # extracting interconnections and ownership
         country1                        = get_node_owner(node1, nodes_matrix, "Country")
         country2                        = get_node_owner(node2, nodes_matrix, "Country")
         ownership["Country 1"][index]   = country1
         ownership["Country 2"][index]   = country2
         if country1 != country2:
@@ -300,15 +299,15 @@
 def get_pout_pg_matrices(lines_matrix: pd.DataFrame, nodes_matrix: pd.DataFrame, flows: np.ndarray, gen: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
     "This function calculates the contribution of inflows to outflows"
 
     number_of_lines = int(lines_matrix.shape[0])
     pout            = np.zeros((number_of_lines, number_of_lines)).astype(float)
     pg              = np.zeros((number_of_lines, len(gen))).astype(float)
 
-    sum_of_outflows_and_withdrawals = ((flows < 0) * flows).sum(1) * -1.0
+    sum_of_inflows_and_injections = ((flows < 0) * flows).sum(1) * -1.0
 
     for index in lines_matrix.index:
         temp = lines_matrix["Line"][index].split("-")
         flow_on_the_line = 0.0
 
         if lines_matrix["Flow"][index] > 0:
             sending_node = int(temp[0])
@@ -318,38 +317,39 @@
             flow_on_the_line = -lines_matrix["Flow"][index]
 
         sending_node_index                  = get_node_index(sending_node, nodes_matrix)
         sending_nodes_indices               = np.nonzero((flows[sending_node_index - 1, :] < 0) * flows[sending_node_index - 1, :])[0]
         sending_nodes_indices               += 1  # adding +1 because these are matrix indices, starts from 0, from flows to indices in nodes_matrix, starts from 1.
         sending_nodes_of_line_sending_node  = nodes_matrix["Node"][sending_nodes_indices].tolist()
 
-        if sum_of_outflows_and_withdrawals[sending_node_index - 1] > 0:
-            contribution = flow_on_the_line/ sum_of_outflows_and_withdrawals[sending_node_index - 1]
+        if sum_of_inflows_and_injections[sending_node_index - 1] > 0:
+            contribution = flow_on_the_line/ sum_of_inflows_and_injections[sending_node_index - 1]
         else:
             contribution = 0.0
 
         for j in range(len(sending_nodes_of_line_sending_node)):
             if sending_node != sending_nodes_of_line_sending_node[j]:
                 temp_index = get_line_index(lines_matrix, sending_nodes_of_line_sending_node[j], sending_node)
-                pout[index - 1, temp_index - 1] = contribution
+                for i in temp_index:
+                    pout[index - 1, i - 1] = contribution
 
         if gen[sending_node_index - 1, 0] != 0:
             pg[index - 1, sending_node_index - 1] = contribution
 
     return pout, pg
 
 
 def get_pin_pd_matrices(lines_matrix: pd.DataFrame, nodes_matrix: pd.DataFrame, flows: np.ndarray, dem: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
     "This function calculates the contribution of outflows to inflows"
 
     number_of_lines = int(lines_matrix.shape[0])
     pin             = np.zeros((number_of_lines, number_of_lines)).astype(float)
     pd              = np.zeros((number_of_lines, len(dem))).astype(float)
-
-    sum_of_inflows_and_injections = ((flows > 0) * flows).sum(1)
+    
+    sum_of_outflows_and_withdrawals = ((flows > 0) * flows).sum(1)
 
     for index in lines_matrix.index:
         temp                = lines_matrix["Line"][index].split("-")
         flow_on_the_line    = 0.0
 
         if lines_matrix["Flow"][index] < 0:
             receiving_node      = int(temp[0])
@@ -359,23 +359,24 @@
             flow_on_the_line    = lines_matrix["Flow"][index]
 
         receiving_node_index                    = get_node_index(receiving_node, nodes_matrix)
         receiving_nodes_indices                 = np.nonzero((flows[receiving_node_index - 1, :] > 0) * flows[receiving_node_index - 1, :])[0]
         receiving_nodes_indices                 += 1
         receiving_nodes_of_line_receiving_node  = nodes_matrix["Node"][receiving_nodes_indices].tolist()
 
-        if sum_of_inflows_and_injections[receiving_node_index - 1] > 0:
-            contribution = flow_on_the_line/sum_of_inflows_and_injections[receiving_node_index - 1]
+        if sum_of_outflows_and_withdrawals[receiving_node_index - 1] > 0:
+            contribution = flow_on_the_line/sum_of_outflows_and_withdrawals[receiving_node_index - 1]
         else:
             contribution = 0.0
 
         for j in range(len(receiving_nodes_of_line_receiving_node)):
             if receiving_node != receiving_nodes_of_line_receiving_node[j]:
-                temp_index                      = get_line_index(lines_matrix, receiving_node, receiving_nodes_of_line_receiving_node[j])
-                pin[index - 1, temp_index - 1]  = contribution
+                temp_index                 = get_line_index(lines_matrix, receiving_node, receiving_nodes_of_line_receiving_node[j])
+                for i in temp_index:
+                    pin[index - 1, i - 1]  = contribution
 
         if dem[receiving_node_index - 1, 0] != 0:
             pd[index - 1, receiving_node_index - 1] = contribution
 
     return pin, pd
 
 
@@ -413,15 +414,15 @@
         Line_country_owner[group][country_line_indices]             = 1
         Line_country_owner[group][group_interconnections.index]     *= 0.5  
 
     countries_responsibility_matrix                     = pd.DataFrame(np.matmul(intermediate_matrix1.to_numpy().transpose(),Line_country_owner.to_numpy()), index=contribution_by_group_matrix.columns, columns=contribution_by_group_matrix.columns)
     diagonal                                            = np.diag(countries_responsibility_matrix)
     use_of                                              = countries_responsibility_matrix.sum(axis=1) - diagonal
     use_by                                              = countries_responsibility_matrix.sum() - diagonal
-    countries_responsibility_matrix["Use by others"]    = use_by
+    countries_responsibility_matrix["Used by others"]   = use_by
     countries_responsibility_matrix["Use of others"]    = use_of
     countries_responsibility_matrix["Net use"]          = use_by - use_of
 
     return countries_responsibility_matrix, Line_country_owner
 
 
 #%% running the model function
@@ -432,20 +433,35 @@
     start_time = time.time()
 
     #%% read inputs
     # data inputs
     input_file                  = os.path.join(directory_file, case_file + '.xlsx')
     nodes_sn                    = pd.read_excel(input_file, sheet_name ="Network", index_col=0) 
     lines_sn                    = pd.read_excel(input_file, sheet_name ="Flows", index_col=0)
-    lines_sn                    = lines_sn.groupby(["Line"]).sum()                              # removing double circuit lines
     lines_attributes            = pd.read_excel(input_file, sheet_name ="Assets attributes", index_col=0)
-    lines_attributes            = lines_attributes.set_index(["Line"])
-    lines_attributes.sort_index(inplace=True)                                                   # important in matrix multiplication, so that the order matches the lines matrix when later in the loop grouped by Line
+
+    # sort for easy calculation
+    if "ID" in lines_sn.columns and "ID" in lines_attributes.columns:
+        lines_sn                    = lines_sn.sort_values(by=['Line',"ID"])
+        lines_attributes            = lines_attributes.sort_values(by=['Line',"ID"])
+    elif "ID" in lines_attributes.columns:
+        lines_sn["ID"]              = lines_attributes["ID"]
+        lines_sn                    = lines_sn.sort_values(by=['Line',"ID"])
+        lines_attributes            = lines_attributes.sort_values(by=['Line',"ID"])
+    elif "ID" in lines_sn.columns:
+        lines_attributes["ID"]      = lines_sn["ID"]
+        lines_sn                    = lines_sn.sort_values(by=['Line',"ID"])
+        lines_attributes            = lines_attributes.sort_values(by=['Line',"ID"])
+    else:
+        lines_sn                    = lines_sn.sort_values(by=['Line'])
+        lines_attributes            = lines_attributes.sort_values(by=['Line'])
+    
+    lines_attributes.set_index(["Line"],inplace=True)
     lines_sn.reset_index(inplace=True)
-    lines_sn.index +=1
+    lines_sn.index              +=1
 
     # control inputs
     config_path                     = os.path.abspath(os.path.join(input_file, '..'))
     configuration_file              = os.path.join(config_path, config_file + '.xlsx')
     control_inputs                  = pd.read_excel(configuration_file, index_col=0) 
     control_inputs                  = control_inputs.set_index(["Inputs"])
     nodal_aggregation               = control_inputs.loc["Nodal Aggregation"][0]                                    # binary 0/1   
@@ -463,28 +479,49 @@
     show_snapshot_results           = control_inputs.loc["Snapshots Results"][0]                                    # binary 0/1
     show_agent_results              = control_inputs.loc["Agent Results"][0]                                        # binary 0/1
     show_country_results            = control_inputs.loc["Country Results"][0]                                      # binary 0/1
     show_SO_results                 = control_inputs.loc["SO Results"][0]                                           # binary 0/1
     show_aggregated_results         = control_inputs.loc["Aggregated Results"][0]                                   # binary 0/1
     show_intermediary_results       = control_inputs.loc["Intermediary Results"][0]                                 # binary 0/1
     cost_of_unused_capacity_op      = control_inputs.loc["Cost of Unused Capacity"][0]                              # integer equals 0 or 1 or 2 or 3
+    
+    # new inputs with exception handling to be compatible with the template of input variables of version 1.0.0 
+    try:   
+        losses_allocation_results   = control_inputs.loc["Losses Allocation Results"][0]                            # binary 0/1    
+    except KeyError:
+        losses_allocation_results   =  0
+    try:
+        demand_losses_weight        = control_inputs.loc["Demand Losses Responsibility (%)"][0]/100                 # percentage 0-100 
+    except KeyError:
+        demand_losses_weight        =  0
+    try:
+        generation_losses_weight    = control_inputs.loc["Generation Losses Responsibility (%)"][0]/100             # percentage 0-100
+    except KeyError:
+        generation_losses_weight    =  0
+    try:
+        losses_price                = control_inputs.loc["Losses price ($/MWh)"][0]                                 # float
+    except KeyError:
+        losses_price                =  0
+    try:
+        regional_losses             = control_inputs.loc["Regional losses"][0]                                      # float
+    except KeyError:
+        regional_losses             =  0
+    try:
+        regional_cost               = control_inputs.loc["Cost of regional assets"][0]                              # float
+    except KeyError:
+        regional_cost               =  0
+        
 
     # initializing control variables
-    remove_zero_values                      = False                                             # internal setting to input variable to remove the zero value from the results 
-    usage_result    = fraction_result       = cost_result       = False
+    remove_zero_values  = id_col            = Reactance_process = False                                             # internal setting to input variable to remove the zero value from the results 
+    usage_result   = fraction_result        = cost_result       = False
     ownership_processing                    = True
     SO_aggregation = category_aggregation   = asset_type_cost   = False
     asset_type_dic                          = {int(asset_types[i].split(":")[1]):asset_types[i].split(":")[0] for i in range(len(asset_types))} 
     snapshots_weights_dic                   = {int(snapshots_weights[i].split(":")[0]):int(snapshots_weights[i].split(":")[1]) for i in range(len(snapshots_weights))} 
-
-    # checking control inputs
-    if length_per_reactance == 0:
-        length_per_reactance = 1        # It doesn't have an effect on the calculation in this case
-    if cost_assignment_op == 1:
-        cost_of_unused_capacity_op = 0  # don't calculate the socialized cost if the full cost is allocated
     
     # checking the optional provided attributes
     attributes_provided = lines_attributes.columns
     if "Length" in attributes_provided and show_intermediary_results:
         usage_result                 = True                      # for calculating the usage MW*Km
         line_length_matrix           = lines_attributes['Length'].to_numpy()[None].transpose()
     if "Capacity" in attributes_provided:
@@ -507,39 +544,60 @@
     if "Exist/Planned" in attributes_provided:
         asset_type_cost              = True
         existing_assets              = (lines_attributes["Exist/Planned"]== 'Exist').astype(int).to_numpy()
     if "SO 1" in nodes_sn.columns:
         SO_aggregation               = True
         if "SO Owner 1" in attributes_provided and "SO 1 Ownership" in attributes_provided and "SO Owner 2" in attributes_provided and "SO 2 Ownership" in attributes_provided:
             ownership_processing     = False
+    if "ID" in attributes_provided:
+        id_col                      = True
+        id_column                   = lines_attributes["ID"]
+    if "Regional Assets" not in attributes_provided:
+        regional_losses             = 0
+        regional_cost               = 0
+    else:
+        regional_assets             = lines_attributes['Regional Assets'].to_numpy()[None].transpose()
     
-    show_SO_results = show_SO_results*SO_aggregation     # don't show SO results if it is not possible to aggregate results SO-wise
+    # checking control inputs
+    if length_per_reactance == 0:
+        length_per_reactance        = 1                 # It doesn't have an effect on the calculation in this case
+    elif "React" in attributes_provided:
+        Reactance_process           = True
+    if cost_assignment_op == 1:
+        cost_of_unused_capacity_op  = 0                 # don't calculate the socialized cost if the full cost is allocated
+
+    show_SO_results = show_SO_results*SO_aggregation    # don't show SO results if it is not possible to aggregate results SO-wise
 
     # initializing outputs from the snapshot loop
     gen_agent_flow_contribution_per_asset_overall   = np.zeros((int(nodes_sn.shape[0]),lines_sn.shape[0]))
     dem_agent_flow_contribution_per_asset_overall   = np.zeros((int(nodes_sn.shape[0]),lines_sn.shape[0]))
     line_flow_overall                               = np.zeros((int(lines_sn.shape[0]),1))
+    line_losses_overall                             = np.zeros((int(lines_sn.shape[0]),1))
     generation_overall                              = np.zeros((nodes_sn.shape[0],1))
     modified_generation_overall                     = np.zeros((nodes_sn.shape[0],1))
     positive_demand_overall                         = np.zeros((nodes_sn.shape[0],1))
     negative_demand_overall                         = np.zeros((nodes_sn.shape[0],1))
 
     #%% processing input data and basic results per snapshot
     for snapshot in range(1,n_snapshots+1):
-        output_file         = "Snapshot " + str(snapshot) +" results\\"
+        output_file         = "Scenario " + str(snapshot) +" results\\"
         output_file         = os.path.join(config_path, output_file)
         current_snapshot    = str(snapshot)
 
-        if "Losses"+current_snapshot in lines_sn.columns:   # checking if losses are provided
+        if "Losses sn"+current_snapshot in lines_sn.columns:   # checking if losses are provided
             lines           = lines_sn[["Line","Flow sn"+current_snapshot,"Losses sn"+current_snapshot]].copy()
             lines           = lines.rename(columns={"Flow sn"+current_snapshot:"Flow","Losses sn"+current_snapshot: "Losses"})
         else:
-            lines   = lines_sn[["Line","Flow sn"+current_snapshot]].copy()
-            lines   = lines.rename(columns={"Flow sn"+current_snapshot:"Flow"})
-        
+            lines                       = lines_sn[["Line","Flow sn"+current_snapshot]].copy()
+            lines                       = lines.rename(columns={"Flow sn"+current_snapshot:"Flow"})
+            losses_allocation_results   = 0
+
+        if id_col:
+            lines["ID"] = id_column.to_numpy()
+            
         other_attributes    = [i for i in nodes_sn.columns if "Generation" not in i]
         other_attributes    = [i for i in other_attributes if "Demand" not in i]
         nodes               = nodes_sn[["Generation sn"+current_snapshot,"Demand sn"+current_snapshot] + other_attributes].copy()
         nodes               = nodes.rename(columns={"Generation sn"+current_snapshot:"Generation","Demand sn"+current_snapshot: "Demand"})
 
         # aggregating generation and demand of the same node, case 2
         if nodal_aggregation:
@@ -552,15 +610,15 @@
                 if aggregation > 0:
                     nodes.loc[indices_of_nodes_with_generation_and_demand[i], "Generation"] = aggregation
                     nodes.loc[indices_of_nodes_with_generation_and_demand[i], "Demand"] = 0.0
                 else:
                     nodes.loc[indices_of_nodes_with_generation_and_demand[i], "Generation"] = 0.0
                     nodes.loc[indices_of_nodes_with_generation_and_demand[i], "Demand"] = abs(aggregation)
 
-        generation, demand, reactance, flows, phi, phiPositive, countries_interconnections, SOs_interconnections, Ownership_matrix = get_input_matrices(lines, nodes,lines_attributes,asset_type_dic,SO_aggregation, ownership_processing)
+        generation, demand, reactance, flows, phi, phiPositive, countries_interconnections, SOs_interconnections, Ownership_matrix = get_input_matrices(lines, nodes,lines_attributes,asset_type_dic,SO_aggregation, ownership_processing, Reactance_process)
         negative_demand, positive_demand    = extract_negative_demand(demand)
         modified_generation                 = generation - negative_demand
         is_all_ND_zeros                     = np.all(negative_demand == 0)
 
         # fill in the ownership matrix if given in the attribute file
         Ownership_matrix                       = Ownership_matrix.set_index(["Line"]) 
         if not ownership_processing:    
@@ -584,23 +642,27 @@
         generation_overall                              += generation*snapshots_weights_dic[snapshot]
         modified_generation_overall                     += modified_generation*snapshots_weights_dic[snapshot]
         positive_demand_overall                         += positive_demand*snapshots_weights_dic[snapshot]
         negative_demand_overall                         += negative_demand*snapshots_weights_dic[snapshot]
         line_flow                                       = lines["Flow"].to_numpy()[None].transpose()
         line_flow                                       = np.absolute(line_flow)
         line_flow_overall                               += line_flow*snapshots_weights_dic[snapshot]
+        if losses_allocation_results:
+            line_losses                                 = lines["Losses"].to_numpy()[None].transpose()
+            line_losses                                 = np.absolute(line_losses)
+            line_losses_overall                         += line_losses*snapshots_weights_dic[snapshot]
 
         # defining some matrices in advance
         x, country_nodes_matrix_G   = get_contribution_per_asset(gen_agent_flow_contribution_per_asset, nodes, lines, "Country")
         x, country_nodes_matrix_D   = get_contribution_per_asset(dem_agent_flow_contribution_per_asset, nodes, lines, "Country")
-        x, countries_lines          = get_contribution_per_group(x, reactance, length_per_reactance, Ownership_matrix, countries_interconnections, "Country")
+        x, countries_lines          = get_contribution_per_group(x, [], length_per_reactance, Ownership_matrix, countries_interconnections, "Country")
         if SO_aggregation:
             y, SO_nodes_matrix_G   = get_contribution_per_asset(gen_agent_flow_contribution_per_asset, nodes, lines, "SO 1")
             y, SO_nodes_matrix_D   = get_contribution_per_asset(dem_agent_flow_contribution_per_asset, nodes, lines, "SO 1")
-            y,   SOs_lines         = get_contribution_per_group(y, reactance, length_per_reactance, Ownership_matrix, SOs_interconnections, "SO Owner")
+            y,   SOs_lines         = get_contribution_per_group(y, [], length_per_reactance, Ownership_matrix, SOs_interconnections, "SO Owner")
     
 
         #%% calculating intermediary results per snapshot
         if show_snapshot_results:
             if not os.path.exists(output_file):
                 os.makedirs(output_file)
 
@@ -611,31 +673,31 @@
                 # calculating the contribution of each country to the flow of each line
                 gen_country_flow_contribution_per_asset, country_nodes_matrix_G = get_contribution_per_asset(gen_agent_flow_contribution_per_asset, nodes, lines, "Country")
                 dem_country_flow_contribution_per_asset, country_nodes_matrix_D = get_contribution_per_asset(dem_agent_flow_contribution_per_asset, nodes, lines, "Country")
                 # another way to calculate contribution_by_countries_G is through matrix multiplication = np.matmul(gen_agent_contribution_per_asset.transpose(),country_nodes_matrix_G.drop(columns=['Node']).to_numpy())
                 # but I decided to keep the function since I need the loop to calculate the nodal matrix anyway, so there is no efficiency gain from removing it. 
                 if show_aggregated_results:
                     # calculating the contribution of each country to the flow in other countries
-                    gen_country_flow_contribution_per_country, countries_lines  = get_contribution_per_group(gen_country_flow_contribution_per_asset, reactance, length_per_reactance, Ownership_matrix, countries_interconnections, "Country")
-                    dem_country_flow_contribution_per_country, countries_lines  = get_contribution_per_group(dem_country_flow_contribution_per_asset, reactance, length_per_reactance, Ownership_matrix, countries_interconnections, "Country")    
+                    gen_country_flow_contribution_per_country, countries_lines  = get_contribution_per_group(gen_country_flow_contribution_per_asset, [], length_per_reactance, Ownership_matrix, countries_interconnections, "Country")
+                    dem_country_flow_contribution_per_country, countries_lines  = get_contribution_per_group(dem_country_flow_contribution_per_asset, [], length_per_reactance, Ownership_matrix, countries_interconnections, "Country")    
                     if category_aggregation:
                         gen_country_flow_contribution_per_asset_category        = get_aggregation_per_category(gen_country_flow_contribution_per_asset, lines_attributes)
                         dem_country_flow_contribution_per_asset_category        = get_aggregation_per_category(dem_country_flow_contribution_per_asset, lines_attributes)
                       
             if show_SO_results:
                 # calculating the contribution of each SO to the flow of each line
                 gen_SO_flow_contribution_per_asset, SO_nodes_matrix_G = get_contribution_per_asset(gen_agent_flow_contribution_per_asset, nodes, lines, "SO 1")
                 dem_SO_flow_contribution_per_asset, SO_nodes_matrix_D = get_contribution_per_asset(dem_agent_flow_contribution_per_asset, nodes, lines, "SO 1")
                 if show_aggregated_results:
                     # calculating the contribution of each SO to the flow in other SOs
-                    gen_SO_flow_contribution_per_SO,   SOs_lines     = get_contribution_per_group(gen_SO_flow_contribution_per_asset, reactance, length_per_reactance, Ownership_matrix, SOs_interconnections, "SO Owner")
-                    dem_SO_flow_contribution_per_SO,   SOs_lines     = get_contribution_per_group(dem_SO_flow_contribution_per_asset, reactance, length_per_reactance, Ownership_matrix, SOs_interconnections, "SO Owner")
+                    gen_SO_flow_contribution_per_SO,   SOs_lines    = get_contribution_per_group(gen_SO_flow_contribution_per_asset, [], length_per_reactance, Ownership_matrix, SOs_interconnections, "SO Owner")
+                    dem_SO_flow_contribution_per_SO,   SOs_lines    = get_contribution_per_group(dem_SO_flow_contribution_per_asset, [], length_per_reactance, Ownership_matrix, SOs_interconnections, "SO Owner")
                     if category_aggregation:
-                        gen_SO_flow_contribution_per_asset_category    = get_aggregation_per_category(gen_SO_flow_contribution_per_asset, lines_attributes)
-                        dem_SO_flow_contribution_per_asset_category    = get_aggregation_per_category(dem_SO_flow_contribution_per_asset, lines_attributes)
+                        gen_SO_flow_contribution_per_asset_category = get_aggregation_per_category(gen_SO_flow_contribution_per_asset, lines_attributes)
+                        dem_SO_flow_contribution_per_asset_category = get_aggregation_per_category(dem_SO_flow_contribution_per_asset, lines_attributes)
 
             # here the order matters! because country_lines and SO_lines need to be calculated first
             if show_aggregated_results and show_agent_results:
                 # calculating the contribution of each agent to the flow in each country
                 gen_agent_flow_contribution_per_country   = np.matmul(gen_agent_flow_contribution_per_asset,countries_lines.to_numpy())
                 dem_agent_flow_contribution_per_country   = np.matmul(dem_agent_flow_contribution_per_asset,countries_lines.to_numpy())
                 if SO_aggregation:    
@@ -722,15 +784,99 @@
                     
                     if show_SO_results:
                         gen_SO_utilization_fraction_per_asset, SO_nodes_matrix_G  = get_contribution_per_asset(gen_agent_utilization_fraction_per_asset, nodes, lines, "SO 1")
                         dem_SO_utilization_fraction_per_asset, SO_nodes_matrix_D  = get_contribution_per_asset(dem_agent_utilization_fraction_per_asset, nodes, lines, "SO 1")
                         if category_aggregation and usage_result and show_aggregated_results:
                             gen_SO_utilization_fraction_per_asset_category        = get_utilization_per_category(gen_SO_flow_km_contribution_per_asset_category, gen_SO_flow_contribution_per_asset_category, flow_km_per_category, flow_per_category, asset_type_dic)
                             dem_SO_utilization_fraction_per_asset_category        = get_utilization_per_category(dem_SO_flow_km_contribution_per_asset_category, dem_SO_flow_contribution_per_asset_category, flow_km_per_category, flow_per_category, asset_type_dic)
+            #%% losses allocation
+            if losses_allocation_results:
+                gen_agent_losses_allocation_per_asset        = line_losses[:,0]*gen_agent_flow_contribution_per_asset/line_flow[:,0]
+                dem_agent_losses_allocation_per_asset        = line_losses[:,0]*dem_agent_flow_contribution_per_asset/line_flow[:,0]
+                
+                if regional_losses:
+                    gen_agent_losses_allocation_per_asset   = regional_assets[:,0]*gen_agent_losses_allocation_per_asset
+                    dem_agent_losses_allocation_per_asset   = regional_assets[:,0]*dem_agent_losses_allocation_per_asset
+
+                gen_agent_losses_allocation_per_asset[np.isnan(gen_agent_losses_allocation_per_asset)]    = 0
+                dem_agent_losses_allocation_per_asset[np.isnan(dem_agent_losses_allocation_per_asset)]    = 0
+                gen_agent_losses_allocation_per_asset[np.isinf(gen_agent_losses_allocation_per_asset)]    = 0
+                dem_agent_losses_allocation_per_asset[np.isinf(dem_agent_losses_allocation_per_asset)]    = 0      
+                
+                gen_agent_losses_allocation_per_asset       = gen_agent_losses_allocation_per_asset*generation_losses_weight
+                dem_agent_losses_allocation_per_asset       = dem_agent_losses_allocation_per_asset*demand_losses_weight
+
+                if show_agent_results and show_aggregated_results:
+                    gen_agent_losses_allocation_per_country = np.matmul(gen_agent_losses_allocation_per_asset,countries_lines.to_numpy())
+                    dem_agent_losses_allocation_per_country = np.matmul(dem_agent_losses_allocation_per_asset,countries_lines.to_numpy())
+                    gen_agent_total_losses_allocation       = np.sum(gen_agent_losses_allocation_per_asset, axis=1) 
+                    dem_agent_total_losses_allocation       = np.sum(dem_agent_losses_allocation_per_asset, axis=1)
+                    if SO_aggregation:
+                        gen_agent_losses_allocation_per_SO  = np.matmul(gen_agent_losses_allocation_per_asset,SOs_lines.to_numpy())
+                        dem_agent_losses_allocation_per_SO  = np.matmul(dem_agent_losses_allocation_per_asset,SOs_lines.to_numpy())
+                    if category_aggregation:
+                        gen_agent_losses_allocation_per_asset_category   = get_aggregation_per_category(pd.DataFrame(gen_agent_losses_allocation_per_asset.transpose(), index=lines["Line"], columns=nodes["Node"]), lines_attributes)
+                        dem_agent_losses_allocation_per_asset_category   = get_aggregation_per_category(pd.DataFrame(dem_agent_losses_allocation_per_asset.transpose(), index=lines["Line"], columns=nodes["Node"]), lines_attributes)
+                              
+                if show_country_results:
+                    gen_country_losses_allocation_per_asset, country_nodes_matrix_G = get_contribution_per_asset(gen_agent_losses_allocation_per_asset, nodes, lines, "Country")
+                    dem_country_losses_allocation_per_asset, country_nodes_matrix_D = get_contribution_per_asset(dem_agent_losses_allocation_per_asset, nodes, lines, "Country")
+                    if show_aggregated_results:
+                        gen_country_losses_allocation_per_country, countries_lines  = get_contribution_per_group(gen_country_losses_allocation_per_asset, [], length_per_reactance, Ownership_matrix, countries_interconnections, "Country")
+                        dem_country_losses_allocation_per_country, countries_lines  = get_contribution_per_group(dem_country_losses_allocation_per_asset, [], length_per_reactance, Ownership_matrix, countries_interconnections, "Country")
+                        if category_aggregation:
+                            gen_country_losses_allocation_per_asset_category        = get_aggregation_per_category(gen_country_losses_allocation_per_asset, lines_attributes)
+                            dem_country_losses_allocation_per_asset_category        = get_aggregation_per_category(dem_country_losses_allocation_per_asset, lines_attributes)
+                         
+                if show_SO_results:
+                    gen_SO_losses_allocation_per_asset, SO_nodes_matrix_G   = get_contribution_per_asset(gen_agent_losses_allocation_per_asset, nodes, lines, "SO 1")
+                    dem_SO_losses_allocation_per_asset, SO_nodes_matrix_D   = get_contribution_per_asset(dem_agent_losses_allocation_per_asset, nodes, lines, "SO 1")
+                    if show_aggregated_results:
+                        gen_SO_losses_allocation_per_SO,   SOs_lines        = get_contribution_per_group(gen_SO_losses_allocation_per_asset, [], length_per_reactance, Ownership_matrix, SOs_interconnections, "SO Owner")
+                        dem_SO_losses_allocation_per_SO,   SOs_lines        = get_contribution_per_group(dem_SO_losses_allocation_per_asset, [], length_per_reactance, Ownership_matrix, SOs_interconnections, "SO Owner")
+                        if category_aggregation:
+                            gen_SO_losses_allocation_per_asset_category     = get_aggregation_per_category(gen_SO_losses_allocation_per_asset, lines_attributes)
+                            dem_SO_losses_allocation_per_asset_category     = get_aggregation_per_category(dem_SO_losses_allocation_per_asset, lines_attributes)
+                
+                if losses_price:
+                    gen_agent_losses_allocation_cost_per_asset  = gen_agent_losses_allocation_per_asset*losses_price*snapshots_weights_dic[snapshot]*0.001
+                    dem_agent_losses_allocation_cost_per_asset  = dem_agent_losses_allocation_per_asset*losses_price*snapshots_weights_dic[snapshot]*0.001
+
+                    if show_agent_results and show_aggregated_results:
+                        gen_agent_losses_allocation_cost_per_country = gen_agent_losses_allocation_per_country*losses_price*snapshots_weights_dic[snapshot]*0.001
+                        dem_agent_losses_allocation_cost_per_country = dem_agent_losses_allocation_per_country*losses_price*snapshots_weights_dic[snapshot]*0.001
+                        gen_agent_total_losses_allocation_cost       = gen_agent_total_losses_allocation*losses_price*snapshots_weights_dic[snapshot]*0.001
+                        dem_agent_total_losses_allocation_cost       = dem_agent_total_losses_allocation*losses_price*snapshots_weights_dic[snapshot]*0.001
+                        if SO_aggregation:
+                            gen_agent_losses_allocation_cost_per_SO  = gen_agent_losses_allocation_per_SO*losses_price*snapshots_weights_dic[snapshot]*0.001
+                            dem_agent_losses_allocation_cost_per_SO  = dem_agent_losses_allocation_per_SO*losses_price*snapshots_weights_dic[snapshot]*0.001
+                        if category_aggregation:
+                            gen_agent_losses_allocation_cost_per_asset_category   = gen_agent_losses_allocation_per_asset_category*losses_price*snapshots_weights_dic[snapshot]*0.001
+                            dem_agent_losses_allocation_cost_per_asset_category   = dem_agent_losses_allocation_per_asset_category*losses_price*snapshots_weights_dic[snapshot]*0.001
                                 
+                    if show_country_results:
+                        gen_country_losses_allocation_cost_per_asset = gen_country_losses_allocation_per_asset*losses_price*snapshots_weights_dic[snapshot]*0.001
+                        dem_country_losses_allocation_cost_per_asset = dem_country_losses_allocation_per_asset*losses_price*snapshots_weights_dic[snapshot]*0.001
+                        if show_aggregated_results:
+                            gen_country_losses_allocation_cost_per_country  = gen_country_losses_allocation_per_country*losses_price*snapshots_weights_dic[snapshot]*0.001
+                            dem_country_losses_allocation_cost_per_country  = dem_country_losses_allocation_per_country*losses_price*snapshots_weights_dic[snapshot]*0.001
+                            if category_aggregation:
+                                gen_country_losses_allocation_cost_per_asset_category    = gen_country_losses_allocation_per_asset_category*losses_price*snapshots_weights_dic[snapshot]*0.001
+                                dem_country_losses_allocation_cost_per_asset_category    = dem_country_losses_allocation_per_asset_category*losses_price*snapshots_weights_dic[snapshot]*0.001
+                            
+                    if show_SO_results:
+                        gen_SO_losses_allocation_cost_per_asset = gen_SO_losses_allocation_per_asset*losses_price*snapshots_weights_dic[snapshot]*0.001
+                        dem_SO_losses_allocation_cost_per_asset = dem_SO_losses_allocation_per_asset*losses_price*snapshots_weights_dic[snapshot]*0.001
+                        if show_aggregated_results:
+                            gen_SO_losses_allocation_cost_per_SO = gen_SO_losses_allocation_per_SO*losses_price*snapshots_weights_dic[snapshot]*0.001
+                            dem_SO_losses_allocation_cost_per_SO = dem_SO_losses_allocation_per_SO*losses_price*snapshots_weights_dic[snapshot]*0.001
+                            if category_aggregation:
+                                gen_SO_losses_allocation_cost_per_asset_category = gen_SO_losses_allocation_per_asset_category*losses_price*snapshots_weights_dic[snapshot]*0.001
+                                dem_SO_losses_allocation_cost_per_asset_category = dem_SO_losses_allocation_per_asset_category*losses_price*snapshots_weights_dic[snapshot]*0.001
+
             #%% cost results kUS$
             if cost_result:
                 if cost_assignment_op == 1 or cost_assignment_op == 2:    
                     gen_agent_cost_per_asset    = gen_agent_utilization_fraction_per_asset*line_cost_matrix[:,0]/100
                     dem_agent_cost_per_asset    = dem_agent_utilization_fraction_per_asset*line_cost_matrix[:,0]/100
                 else:
                     if cost_assignment_op == 3: # full cost if the asset exist, used capacity cost if asset is planned
@@ -757,14 +903,18 @@
 
                     gen_agent_cost_per_asset    = (gen_agent_utilization_fraction_per_asset_partial + gen_agent_utilization_fraction_per_asset2)*line_cost_matrix[:,0]/100
                     dem_agent_cost_per_asset    = (dem_agent_utilization_fraction_per_asset_partial + dem_agent_utilization_fraction_per_asset2)*line_cost_matrix[:,0]/100
 
                 gen_agent_cost_per_asset = gen_agent_cost_per_asset*generation_weight
                 dem_agent_cost_per_asset = dem_agent_cost_per_asset*demand_weight 
                 
+                if regional_cost:
+                    gen_agent_cost_per_asset   = regional_assets[:,0]*gen_agent_cost_per_asset
+                    dem_agent_cost_per_asset   = regional_assets[:,0]*dem_agent_cost_per_asset
+
                 if not is_all_ND_zeros:
                     negative_dem_agent_cost_per_asset       = get_negative_demand_contribution(negative_demand, generation, gen_agent_cost_per_asset, nodes, lines)
 
                 if show_agent_results and show_aggregated_results:
                     gen_agent_cost_per_country              = np.matmul(gen_agent_cost_per_asset,countries_lines.to_numpy())
                     dem_agent_cost_per_country              = np.matmul(dem_agent_cost_per_asset,countries_lines.to_numpy())
                     gen_agent_total_cost                    = np.sum(gen_agent_cost_per_country, axis=1) 
@@ -780,29 +930,31 @@
                             gen_agent_network_utilization_fraction  = ((gen_agent_utilization_fraction_per_asset_category*cost_per_category.to_numpy().transpose()[:,0]).sum(axis=1)/cost_per_category.sum(axis=1)[0]).to_frame(name='Network Utilization %')              
                             dem_agent_network_utilization_fraction  = ((dem_agent_utilization_fraction_per_asset_category*cost_per_category.to_numpy().transpose()[:,0]).sum(axis=1)/cost_per_category.sum(axis=1)[0]).to_frame(name='Network Utilization %')
                             
                 if show_country_results:
                     gen_country_cost_per_asset, country_nodes_matrix_G      = get_contribution_per_asset(gen_agent_cost_per_asset, nodes, lines, "Country")
                     dem_country_cost_per_asset, country_nodes_matrix_D      = get_contribution_per_asset(dem_agent_cost_per_asset, nodes, lines, "Country")
                     if show_aggregated_results:
-                        gen_country_cost_per_country, countries_lines       = get_contribution_per_group(gen_country_cost_per_asset, reactance, length_per_reactance, Ownership_matrix, countries_interconnections, "Country")
-                        dem_country_cost_per_country, countries_lines       = get_contribution_per_group(dem_country_cost_per_asset, reactance, length_per_reactance, Ownership_matrix, countries_interconnections, "Country")
+                        gen_country_cost_per_country, countries_lines       = get_contribution_per_group(gen_country_cost_per_asset, [], length_per_reactance, Ownership_matrix, countries_interconnections, "Country")
+                        dem_country_cost_per_country, countries_lines       = get_contribution_per_group(dem_country_cost_per_asset, [], length_per_reactance, Ownership_matrix, countries_interconnections, "Country")
+                        country_cost_per_country                            = gen_country_cost_per_country + dem_country_cost_per_country
                         if category_aggregation:
                             gen_country_cost_per_asset_category             = get_aggregation_per_category(gen_country_cost_per_asset, lines_attributes)
                             dem_country_cost_per_asset_category             = get_aggregation_per_category(dem_country_cost_per_asset, lines_attributes)
                             if usage_result:
                                 gen_country_network_utilization_fraction    = ((gen_country_utilization_fraction_per_asset_category*cost_per_category.to_numpy().transpose()[:,0]).sum(axis=1)/cost_per_category.sum(axis=1)[0]).to_frame(name='Network Utilization %')
                                 dem_country_network_utilization_fraction    = ((dem_country_utilization_fraction_per_asset_category*cost_per_category.to_numpy().transpose()[:,0]).sum(axis=1)/cost_per_category.sum(axis=1)[0]).to_frame(name='Network Utilization %')
                         
                 if show_SO_results:
                     gen_SO_cost_per_asset, SO_nodes_matrix_G        = get_contribution_per_asset(gen_agent_cost_per_asset, nodes, lines, "SO 1")
                     dem_SO_cost_per_asset, SO_nodes_matrix_D        = get_contribution_per_asset(dem_agent_cost_per_asset, nodes, lines, "SO 1")
                     if show_aggregated_results:
-                        gen_SO_cost_per_SO,   SOs_lines             = get_contribution_per_group(gen_SO_cost_per_asset, reactance, length_per_reactance, Ownership_matrix, SOs_interconnections, "SO Owner")
-                        dem_SO_cost_per_SO,   SOs_lines             = get_contribution_per_group(dem_SO_cost_per_asset, reactance, length_per_reactance, Ownership_matrix, SOs_interconnections, "SO Owner")
+                        gen_SO_cost_per_SO,   SOs_lines             = get_contribution_per_group(gen_SO_cost_per_asset, [], length_per_reactance, Ownership_matrix, SOs_interconnections, "SO Owner")
+                        dem_SO_cost_per_SO,   SOs_lines             = get_contribution_per_group(dem_SO_cost_per_asset, [], length_per_reactance, Ownership_matrix, SOs_interconnections, "SO Owner")
+                        SO_cost_per_SO                              = dem_SO_cost_per_SO + gen_SO_cost_per_SO
                         if category_aggregation:
                             gen_SO_cost_per_asset_category          = get_aggregation_per_category(gen_SO_cost_per_asset, lines_attributes)
                             dem_SO_cost_per_asset_category          = get_aggregation_per_category(dem_SO_cost_per_asset, lines_attributes)
                             if usage_result:
                                 gen_SO_network_utilization_fraction = ((gen_SO_utilization_fraction_per_asset_category*cost_per_category.to_numpy().transpose()[:,0]).sum(axis=1)/cost_per_category.sum(axis=1)[0]).to_frame(name='Network Utilization %')
                                 dem_SO_network_utilization_fraction = ((dem_SO_utilization_fraction_per_asset_category*cost_per_category.to_numpy().transpose()[:,0]).sum(axis=1)/cost_per_category.sum(axis=1)[0]).to_frame(name='Network Utilization %')
 
@@ -871,15 +1023,15 @@
                     print_to_csv(output_file+"Demand agents flow contribution per country sn_"+current_snapshot, dem_agent_flow_contribution_per_country, index=nodes["Node"], columns=countries_lines.columns, total=False, remove_zeros=remove_zero_values)
                     if SO_aggregation:  
                         print_to_csv(output_file+"Generation agents flow contribution per SO sn_"+current_snapshot, gen_agent_flow_contribution_per_SO, index=nodes["Node"], columns=SOs_lines.columns, total=False, remove_zeros=remove_zero_values)
                         print_to_csv(output_file+"Demand agents flow contribution per SO sn_"+current_snapshot, dem_agent_flow_contribution_per_SO, index=nodes["Node"], columns=SOs_lines.columns, total=False, remove_zeros=remove_zero_values)
                     if category_aggregation:
                         remove_zero_rows_and_columns(gen_agent_flow_contribution_per_asset_category, remove_zero_values, remove_zero_values).to_csv(output_file+"Generation agents flow contribution per asset category sn_"+current_snapshot+".csv")
                         remove_zero_rows_and_columns(dem_agent_flow_contribution_per_asset_category, remove_zero_values, remove_zero_values).to_csv(output_file+"Demand agents flow contribution per asset category sn_"+current_snapshot+".csv")
-        
+            
             # countries flow results
             if show_country_results:
                 remove_zero_rows_and_columns(gen_country_flow_contribution_per_asset, remove_zero_values, remove_zero_values).to_csv(output_file+"Country generation flow contribution per asset sn_"+current_snapshot+".csv")
                 remove_zero_rows_and_columns(dem_country_flow_contribution_per_asset, remove_zero_values, remove_zero_values).to_csv(output_file+"Country demand flow contribution per asset sn_"+current_snapshot+".csv")
                 if show_aggregated_results:
                     remove_zero_rows_and_columns(gen_country_flow_contribution_per_country.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"Country generation flow contribution per country sn_"+current_snapshot+".csv")
                     remove_zero_rows_and_columns(dem_country_flow_contribution_per_country.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"Country demand flow contribution per country sn_"+current_snapshot+".csv")
@@ -951,14 +1103,87 @@
 
                 if show_SO_results:
                     remove_zero_rows_and_columns(gen_SO_utilization_fraction_per_asset, remove_zero_values, remove_zero_values).to_csv(output_file+"SO generation utilization fraction per asset sn_"+current_snapshot+".csv")
                     remove_zero_rows_and_columns(dem_SO_utilization_fraction_per_asset, remove_zero_values, remove_zero_values).to_csv(output_file+"SO demand utilization fraction per asset sn_"+current_snapshot+".csv")
                     if show_aggregated_results and category_aggregation and usage_result:
                         remove_zero_rows_and_columns(gen_SO_utilization_fraction_per_asset_category, remove_zero_values, remove_zero_values).to_csv(output_file+"SO generation utilization fraction per asset category sn_"+current_snapshot+".csv")
                         remove_zero_rows_and_columns(dem_SO_utilization_fraction_per_asset_category, remove_zero_values, remove_zero_values).to_csv(output_file+"SO demand utilization fraction per asset category sn_"+current_snapshot+".csv")
+            
+            # losses allocation results
+            if losses_allocation_results:
+                if show_agent_results:
+                    print_to_csv(output_file+"Generation agents losses allocation per asset sn_"+current_snapshot, gen_agent_losses_allocation_per_asset, index=nodes["Node"], columns=lines["Line"], total=True, remove_zeros=remove_zero_values)
+                    print_to_csv(output_file+"Demand agents losses allocation per asset sn_"+current_snapshot, dem_agent_losses_allocation_per_asset, index=nodes["Node"], columns=lines["Line"], total=True, remove_zeros=remove_zero_values)
+                    if show_aggregated_results:
+                        print_to_csv(output_file+"Generation agents losses allocation per country sn_"+current_snapshot, gen_agent_losses_allocation_per_country, index=nodes["Node"], columns=countries_lines.columns, total=False, remove_zeros=remove_zero_values)
+                        print_to_csv(output_file+"Demand agents losses allocation per country sn_"+current_snapshot, dem_agent_losses_allocation_per_country, index=nodes["Node"], columns=countries_lines.columns, total=False, remove_zeros=remove_zero_values)
+                        print_to_csv(output_file+"Generation agents total losses allocation sn_"+current_snapshot, gen_agent_total_losses_allocation, index=nodes["Node"], columns=['Total losses allocation MW'], total=True, remove_zeros=remove_zero_values)
+                        print_to_csv(output_file+"Demand agents total losses allocation sn_"+current_snapshot, dem_agent_total_losses_allocation, index=nodes["Node"], columns=['Total losses allocation'], total=True, remove_zeros=remove_zero_values)
+                        if SO_aggregation: 
+                            print_to_csv(output_file+"Generation agents losses allocation per SO sn_"+current_snapshot, gen_agent_losses_allocation_per_SO, index=nodes["Node"], columns=SOs_lines.columns, total=False, remove_zeros=remove_zero_values)
+                            print_to_csv(output_file+"Demand agents losses allocation per SO sn_"+current_snapshot, dem_agent_losses_allocation_per_SO, index=nodes["Node"], columns=SOs_lines.columns, total=False, remove_zeros=remove_zero_values)
+                        if category_aggregation:
+                            remove_zero_rows_and_columns(gen_agent_losses_allocation_per_asset_category, remove_zero_values, remove_zero_values).to_csv(output_file+"Generation agents losses allocation per asset category sn_"+current_snapshot+".csv")
+                            remove_zero_rows_and_columns(dem_agent_losses_allocation_per_asset_category, remove_zero_values, remove_zero_values).to_csv(output_file+"Demand agents losses allocation per asset category sn_"+current_snapshot+".csv")
+                
+                if show_country_results:
+                    remove_zero_rows_and_columns(gen_country_losses_allocation_per_asset, remove_zero_values, remove_zero_values).to_csv(output_file+"Country generation losses allocation per asset sn_"+current_snapshot+".csv")
+                    remove_zero_rows_and_columns(dem_country_losses_allocation_per_asset, remove_zero_values, remove_zero_values).to_csv(output_file+"Country demand losses allocation per asset sn_"+current_snapshot+".csv")
+                    if show_aggregated_results:
+                        remove_zero_rows_and_columns(gen_country_losses_allocation_per_country.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"Country generation losses allocation per country sn_"+current_snapshot+".csv")
+                        remove_zero_rows_and_columns(dem_country_losses_allocation_per_country.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"Country demand losses allocation per country sn_"+current_snapshot+".csv")
+                        if category_aggregation:
+                            remove_zero_rows_and_columns(gen_country_losses_allocation_per_asset_category, remove_zero_values, remove_zero_values).to_csv(output_file+"Country generation losses allocation per asset category sn_"+current_snapshot+".csv")
+                            remove_zero_rows_and_columns(dem_country_losses_allocation_per_asset_category, remove_zero_values, remove_zero_values).to_csv(output_file+"Country demand losses allocation per asset category sn_"+current_snapshot+".csv")
+
+                if show_SO_results:
+                    remove_zero_rows_and_columns(gen_SO_losses_allocation_per_asset, remove_zero_values, remove_zero_values).to_csv(output_file+"SO generation losses allocation per asset sn_"+current_snapshot+".csv")
+                    remove_zero_rows_and_columns(dem_SO_losses_allocation_per_asset, remove_zero_values, remove_zero_values).to_csv(output_file+"SO demand losses allocation per asset sn_"+current_snapshot+".csv")
+                    if show_aggregated_results:
+                        remove_zero_rows_and_columns(gen_SO_losses_allocation_per_SO.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"SO generation losses allocation per SO sn_"+current_snapshot+".csv")
+                        remove_zero_rows_and_columns(dem_SO_losses_allocation_per_SO.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"SO demand losses allocation per SO sn_"+current_snapshot+".csv")
+                        if category_aggregation:
+                            remove_zero_rows_and_columns(gen_SO_losses_allocation_per_asset_category, remove_zero_values, remove_zero_values).to_csv(output_file+"SO generation losses allocation per asset category sn_"+current_snapshot+".csv")
+                            remove_zero_rows_and_columns(dem_SO_losses_allocation_per_asset_category, remove_zero_values, remove_zero_values).to_csv(output_file+"SO demand losses allocation per asset category sn_"+current_snapshot+".csv")
+                
+                if losses_price:
+                    if show_agent_results:
+                        print_to_csv(output_file+"Generation agents losses allocation cost per asset sn_"+current_snapshot, gen_agent_losses_allocation_cost_per_asset, index=nodes["Node"], columns=lines["Line"], total=True, remove_zeros=remove_zero_values)
+                        print_to_csv(output_file+"Demand agents losses allocation cost per asset sn_"+current_snapshot, dem_agent_losses_allocation_cost_per_asset, index=nodes["Node"], columns=lines["Line"], total=True, remove_zeros=remove_zero_values)
+                        if show_aggregated_results:
+                            print_to_csv(output_file+"Generation agents losses allocation cost per country sn_"+current_snapshot, gen_agent_losses_allocation_cost_per_country, index=nodes["Node"], columns=countries_lines.columns, total=False, remove_zeros=remove_zero_values)
+                            print_to_csv(output_file+"Demand agents losses allocation cost per country sn_"+current_snapshot, dem_agent_losses_allocation_cost_per_country, index=nodes["Node"], columns=countries_lines.columns, total=False, remove_zeros=remove_zero_values)
+                            print_to_csv(output_file+"Generation agents total losses allocation cost sn_"+current_snapshot, gen_agent_total_losses_allocation_cost, index=nodes["Node"], columns=['Total losses allocation MW'], total=True, remove_zeros=remove_zero_values)
+                            print_to_csv(output_file+"Demand agents total losses allocation cost sn_"+current_snapshot, dem_agent_total_losses_allocation_cost, index=nodes["Node"], columns=['Total losses allocation'], total=True, remove_zeros=remove_zero_values)
+                            if SO_aggregation: 
+                                print_to_csv(output_file+"Generation agents losses allocation cost per SO sn_"+current_snapshot, gen_agent_losses_allocation_cost_per_SO, index=nodes["Node"], columns=SOs_lines.columns, total=False, remove_zeros=remove_zero_values)
+                                print_to_csv(output_file+"Demand agents losses allocation cost per SO sn_"+current_snapshot, dem_agent_losses_allocation_cost_per_SO, index=nodes["Node"], columns=SOs_lines.columns, total=False, remove_zeros=remove_zero_values)
+                            if category_aggregation:
+                                remove_zero_rows_and_columns(gen_agent_losses_allocation_cost_per_asset_category, remove_zero_values, remove_zero_values).to_csv(output_file+"Generation agents losses allocation cost per asset category sn_"+current_snapshot+".csv")
+                                remove_zero_rows_and_columns(dem_agent_losses_allocation_cost_per_asset_category, remove_zero_values, remove_zero_values).to_csv(output_file+"Demand agents losses allocation cost per asset category sn_"+current_snapshot+".csv")
+                    
+                    if show_country_results:
+                        remove_zero_rows_and_columns(gen_country_losses_allocation_cost_per_asset, remove_zero_values, remove_zero_values).to_csv(output_file+"Country generation losses allocation cost per asset sn_"+current_snapshot+".csv")
+                        remove_zero_rows_and_columns(dem_country_losses_allocation_cost_per_asset, remove_zero_values, remove_zero_values).to_csv(output_file+"Country demand losses allocation cost per asset sn_"+current_snapshot+".csv")
+                        if show_aggregated_results:
+                            remove_zero_rows_and_columns(gen_country_losses_allocation_cost_per_country.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"Country generation losses allocation cost per country sn_"+current_snapshot+".csv")
+                            remove_zero_rows_and_columns(dem_country_losses_allocation_cost_per_country.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"Country demand losses allocation cost per country sn_"+current_snapshot+".csv")
+                            if category_aggregation:
+                                remove_zero_rows_and_columns(gen_country_losses_allocation_cost_per_asset_category, remove_zero_values, remove_zero_values).to_csv(output_file+"Country generation losses allocation cost per asset category sn_"+current_snapshot+".csv")
+                                remove_zero_rows_and_columns(dem_country_losses_allocation_cost_per_asset_category, remove_zero_values, remove_zero_values).to_csv(output_file+"Country demand losses allocation cost per asset category sn_"+current_snapshot+".csv")
+
+                    if show_SO_results:
+                        remove_zero_rows_and_columns(gen_SO_losses_allocation_cost_per_asset, remove_zero_values, remove_zero_values).to_csv(output_file+"SO generation losses allocation cost per asset sn_"+current_snapshot+".csv")
+                        remove_zero_rows_and_columns(dem_SO_losses_allocation_cost_per_asset, remove_zero_values, remove_zero_values).to_csv(output_file+"SO demand losses allocation cost per asset sn_"+current_snapshot+".csv")
+                        if show_aggregated_results:
+                            remove_zero_rows_and_columns(gen_SO_losses_allocation_cost_per_SO.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"SO generation losses allocation cost per SO sn_"+current_snapshot+".csv")
+                            remove_zero_rows_and_columns(dem_SO_losses_allocation_cost_per_SO.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"SO demand losses allocation cost per SO sn_"+current_snapshot+".csv")
+                            if category_aggregation:
+                                remove_zero_rows_and_columns(gen_SO_losses_allocation_cost_per_asset_category, remove_zero_values, remove_zero_values).to_csv(output_file+"SO generation losses allocation cost per asset category sn_"+current_snapshot+".csv")
+                                remove_zero_rows_and_columns(dem_SO_losses_allocation_cost_per_asset_category, remove_zero_values, remove_zero_values).to_csv(output_file+"SO demand losses allocation cost per asset category sn_"+current_snapshot+".csv")
 
             # cost results
             if cost_result:
                 if show_agent_results:
                     print_to_csv(output_file+"Generation agents cost per asset sn_"+current_snapshot, gen_agent_cost_per_asset, index=nodes["Node"], columns=lines["Line"], total=True, remove_zeros=remove_zero_values)
                     print_to_csv(output_file+"Demand agents cost per asset sn_"+current_snapshot, dem_agent_cost_per_asset, index=nodes["Node"], columns=lines["Line"],total=True, remove_zeros=remove_zero_values)
                     if not is_all_ND_zeros:
@@ -983,41 +1208,44 @@
                     
                 if show_country_results:
                     remove_zero_rows_and_columns(gen_country_cost_per_asset, remove_zero_values, remove_zero_values).to_csv(output_file+"Country generation cost per asset sn_"+current_snapshot+".csv")
                     remove_zero_rows_and_columns(dem_country_cost_per_asset, remove_zero_values, remove_zero_values).to_csv(output_file+"Country demand cost per asset sn_"+current_snapshot+".csv")
                     if show_aggregated_results:
                         remove_zero_rows_and_columns(gen_country_cost_per_country.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"Country generation cost per country sn_"+current_snapshot+".csv")
                         remove_zero_rows_and_columns(dem_country_cost_per_country.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"Country demand cost per country sn_"+current_snapshot+".csv")
+                        remove_zero_rows_and_columns(country_cost_per_country.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"Country joint cost per country sn_"+current_snapshot+".csv")
                         if category_aggregation:
                             remove_zero_rows_and_columns(gen_country_cost_per_asset_category, remove_zero_values, remove_zero_values).to_csv(output_file+"Country generation cost per asset category sn_"+current_snapshot+".csv")
                             remove_zero_rows_and_columns(dem_country_cost_per_asset_category, remove_zero_values, remove_zero_values).to_csv(output_file+"Country demand cost per asset category sn_"+current_snapshot+".csv")
                             if usage_result:
                                 remove_zero_rows_and_columns(gen_country_network_utilization_fraction, remove_zero_values, remove_zero_values).to_csv(output_file+"Country generation network utilization sn_"+current_snapshot+".csv")
                                 remove_zero_rows_and_columns(dem_country_network_utilization_fraction, remove_zero_values, remove_zero_values).to_csv(output_file+"Country demand network utilization sn_"+current_snapshot+".csv")
 
                 if show_SO_results:
                     remove_zero_rows_and_columns(gen_SO_cost_per_asset, remove_zero_values, remove_zero_values).to_csv(output_file+"SO generation cost per asset sn_"+current_snapshot+".csv")
                     remove_zero_rows_and_columns(dem_SO_cost_per_asset, remove_zero_values, remove_zero_values).to_csv(output_file+"SO demand cost per asset sn_"+current_snapshot+".csv")
                     if show_aggregated_results:
                         remove_zero_rows_and_columns(gen_SO_cost_per_SO.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"SO generation cost per SO sn_"+current_snapshot+".csv")
                         remove_zero_rows_and_columns(dem_SO_cost_per_SO.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"SO demand cost per SO sn_"+current_snapshot+".csv")
+                        remove_zero_rows_and_columns(SO_cost_per_SO.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"SO joint cost per SO sn_"+current_snapshot+".csv")
                         if category_aggregation:
                             remove_zero_rows_and_columns(gen_SO_cost_per_asset_category, remove_zero_values, remove_zero_values).to_csv(output_file+"SO generation cost per asset category sn_"+current_snapshot+".csv")
                             remove_zero_rows_and_columns(dem_SO_cost_per_asset_category, remove_zero_values, remove_zero_values).to_csv(output_file+"SO demand cost per asset category sn_"+current_snapshot+".csv")
                             if usage_result:
                                 remove_zero_rows_and_columns(gen_SO_network_utilization_fraction, remove_zero_values, remove_zero_values).to_csv(output_file+"SO generation network utilization sn_"+current_snapshot+".csv")
                                 remove_zero_rows_and_columns(dem_SO_network_utilization_fraction, remove_zero_values, remove_zero_values).to_csv(output_file+"SO demand network utilization sn_"+current_snapshot+".csv")
 
     #%% overall results
     output_file         = "Overall results\\"
     output_file         = os.path.join(config_path, output_file)
     if not os.path.exists(output_file):
         os.makedirs(output_file)
 
     line_flow_overall                               = line_flow_overall/sum(snapshots_weights_dic.values())
+    line_losses_overall                             = line_losses_overall/sum(snapshots_weights_dic.values())
     modified_generation_overall                     = modified_generation_overall/sum(snapshots_weights_dic.values())
     generation_overall                              = generation_overall/sum(snapshots_weights_dic.values())
     positive_demand_overall                         = positive_demand_overall/sum(snapshots_weights_dic.values())
     negative_demand_overall                         = negative_demand_overall/sum(snapshots_weights_dic.values())
     is_all_ND_zeros                                 = np.all(negative_demand_overall == 0)
     gen_agent_flow_contribution_per_asset_overall   = gen_agent_flow_contribution_per_asset_overall/sum(snapshots_weights_dic.values())
     dem_agent_flow_contribution_per_asset_overall   = dem_agent_flow_contribution_per_asset_overall/sum(snapshots_weights_dic.values())
@@ -1025,26 +1253,26 @@
     if not is_all_ND_zeros:
         negative_dem_agent_contribution_per_asset_overall   = get_negative_demand_contribution(negative_demand_overall, generation_overall, gen_agent_flow_contribution_per_asset_overall, nodes_sn, lines_sn)
 
     if show_country_results:
         gen_country_flow_contribution_per_asset_overall, country_nodes_matrix_G = get_contribution_per_asset(gen_agent_flow_contribution_per_asset_overall, nodes, lines, "Country")
         dem_country_flow_contribution_per_asset_overall, country_nodes_matrix_D = get_contribution_per_asset(dem_agent_flow_contribution_per_asset_overall, nodes, lines, "Country")
         if show_aggregated_results:
-            gen_country_flow_contribution_per_country_overall, countries_lines  = get_contribution_per_group(gen_country_flow_contribution_per_asset_overall, reactance, length_per_reactance, Ownership_matrix, countries_interconnections, "Country")
-            dem_country_flow_contribution_per_country_overall, countries_lines  = get_contribution_per_group(dem_country_flow_contribution_per_asset_overall, reactance, length_per_reactance, Ownership_matrix, countries_interconnections, "Country")
+            gen_country_flow_contribution_per_country_overall, countries_lines  = get_contribution_per_group(gen_country_flow_contribution_per_asset_overall, [], length_per_reactance, Ownership_matrix, countries_interconnections, "Country")
+            dem_country_flow_contribution_per_country_overall, countries_lines  = get_contribution_per_group(dem_country_flow_contribution_per_asset_overall, [], length_per_reactance, Ownership_matrix, countries_interconnections, "Country")
             if category_aggregation:
                 gen_country_flow_contribution_per_asset_category_overall        = get_aggregation_per_category(gen_country_flow_contribution_per_asset_overall, lines_attributes)
                 dem_country_flow_contribution_per_asset_category_overall        = get_aggregation_per_category(dem_country_flow_contribution_per_asset_overall, lines_attributes)
                 
     if show_SO_results:
         gen_SO_flow_contribution_per_asset_overall, SO_nodes_matrix_G = get_contribution_per_asset(gen_agent_flow_contribution_per_asset_overall, nodes, lines, "SO 1")
         dem_SO_flow_contribution_per_asset_overall, SO_nodes_matrix_D = get_contribution_per_asset(dem_agent_flow_contribution_per_asset_overall, nodes, lines, "SO 1")
         if show_aggregated_results:
-            gen_SO_flow_contribution_per_SO_overall,   SOs_lines      = get_contribution_per_group(gen_SO_flow_contribution_per_asset_overall, reactance, length_per_reactance, Ownership_matrix, SOs_interconnections, "SO Owner")
-            dem_SO_flow_contribution_per_SO_overall,   SOs_lines      = get_contribution_per_group(dem_SO_flow_contribution_per_asset_overall, reactance, length_per_reactance, Ownership_matrix, SOs_interconnections, "SO Owner")
+            gen_SO_flow_contribution_per_SO_overall,   SOs_lines      = get_contribution_per_group(gen_SO_flow_contribution_per_asset_overall, [], length_per_reactance, Ownership_matrix, SOs_interconnections, "SO Owner")
+            dem_SO_flow_contribution_per_SO_overall,   SOs_lines      = get_contribution_per_group(dem_SO_flow_contribution_per_asset_overall, [], length_per_reactance, Ownership_matrix, SOs_interconnections, "SO Owner")
             if category_aggregation:
                 gen_SO_flow_contribution_per_asset_category_overall   = get_aggregation_per_category(gen_SO_flow_contribution_per_asset_overall, lines_attributes)
                 dem_SO_flow_contribution_per_asset_category_overall   = get_aggregation_per_category(dem_SO_flow_contribution_per_asset_overall, lines_attributes)
                 
     if show_agent_results and show_aggregated_results:
         gen_agent_flow_contribution_per_country_overall             = np.matmul(gen_agent_flow_contribution_per_asset_overall,countries_lines.to_numpy())
         dem_agent_flow_contribution_per_country_overall             = np.matmul(dem_agent_flow_contribution_per_asset_overall,countries_lines.to_numpy())
@@ -1106,23 +1334,26 @@
                 dem_agent_utilization_fraction_per_asset_overall_partial    = np.matmul(dem_agent_utilization_fraction_per_asset_overall,np.diag(1-line_above_UT_overall))
                 gen_agent_utilization_fraction_per_asset2_overall           = np.matmul(gen_agent_utilization_fraction_per_asset2_overall,np.diag(line_above_UT_overall))     # full cost for assets above the UT
                 dem_agent_utilization_fraction_per_asset2_overall           = np.matmul(dem_agent_utilization_fraction_per_asset2_overall,np.diag(line_above_UT_overall))
 
             gen_agent_cost_per_asset_overall    = (gen_agent_utilization_fraction_per_asset_overall_partial + gen_agent_utilization_fraction_per_asset2_overall)*line_cost_matrix[:,0]/100
             dem_agent_cost_per_asset_overall    = (dem_agent_utilization_fraction_per_asset_overall_partial + dem_agent_utilization_fraction_per_asset2_overall)*line_cost_matrix[:,0]/100
         
-        gen_agent_cost_per_asset_overall = gen_agent_cost_per_asset_overall*generation_weight
-        dem_agent_cost_per_asset_overall = dem_agent_cost_per_asset_overall*demand_weight 
+        gen_agent_cost_per_asset_overall        = gen_agent_cost_per_asset_overall*generation_weight
+        dem_agent_cost_per_asset_overall        = dem_agent_cost_per_asset_overall*demand_weight 
         
+        if regional_cost:
+            gen_agent_cost_per_asset_overall   = regional_assets[:,0]*gen_agent_cost_per_asset_overall
+            dem_agent_cost_per_asset_overall   = regional_assets[:,0]*dem_agent_cost_per_asset_overall
+
         if not is_all_ND_zeros:
             negative_dem_agent_cost_per_asset_overall = get_negative_demand_contribution(negative_demand_overall, generation_overall, gen_agent_cost_per_asset_overall, nodes_sn, lines_sn)
 
         # calculating the socialized cost of the grid
         if cost_of_unused_capacity_op:
-     
             gen_total_allocated_cost_per_asset_overall  = gen_agent_cost_per_asset_overall.sum(axis=0)[None].transpose()
             dem_total_allocated_cost_per_asset_overall  = dem_agent_cost_per_asset_overall.sum(axis=0)[None].transpose()
             total_cost_to_be_socialized_overall         = line_cost_matrix - gen_total_allocated_cost_per_asset_overall - dem_total_allocated_cost_per_asset_overall
             gen_cost_to_socialize_per_asset_overall     = total_cost_to_be_socialized_overall*generation_socialized_weight
             dem_cost_to_socialize_per_asset_overall     = total_cost_to_be_socialized_overall*demand_socialized_weight
             gen_cost_to_socialize_per_asset_overall     = np.where(gen_cost_to_socialize_per_asset_overall < 0, 0, gen_cost_to_socialize_per_asset_overall)
             dem_cost_to_socialize_per_asset_overall     = np.where(dem_cost_to_socialize_per_asset_overall < 0, 0, dem_cost_to_socialize_per_asset_overall)
@@ -1171,42 +1402,128 @@
                 dem_agent_socialized_cost_per_asset_overall     = dem_agent_socialized_weight_per_asset_overall*dem_cost_to_socialize_per_asset_overall[:,0]
     
         # the remaining cost results
         if show_country_results:
             gen_country_cost_per_asset_overall, country_nodes_matrix_G  = get_contribution_per_asset(gen_agent_cost_per_asset_overall, nodes, lines, "Country")
             dem_country_cost_per_asset_overall, country_nodes_matrix_D  = get_contribution_per_asset(dem_agent_cost_per_asset_overall, nodes, lines, "Country")
             if show_aggregated_results:
-                gen_country_cost_per_country_overall, countries_lines   = get_contribution_per_group(gen_country_cost_per_asset_overall, reactance, length_per_reactance, Ownership_matrix, countries_interconnections, "Country")
-                dem_country_cost_per_country_overall, countries_lines   = get_contribution_per_group(dem_country_cost_per_asset_overall, reactance, length_per_reactance, Ownership_matrix, countries_interconnections, "Country") 
+                gen_country_cost_per_country_overall, countries_lines   = get_contribution_per_group(gen_country_cost_per_asset_overall, [], length_per_reactance, Ownership_matrix, countries_interconnections, "Country")
+                dem_country_cost_per_country_overall, countries_lines   = get_contribution_per_group(dem_country_cost_per_asset_overall, [], length_per_reactance, Ownership_matrix, countries_interconnections, "Country") 
+                country_cost_per_country_overall                        = gen_country_cost_per_country_overall + dem_country_cost_per_country_overall
                 if category_aggregation:
                     gen_country_cost_per_asset_category_overall         = get_aggregation_per_category(gen_country_cost_per_asset_overall, lines_attributes)
                     dem_country_cost_per_asset_category_overall         = get_aggregation_per_category(dem_country_cost_per_asset_overall, lines_attributes)
 
         if show_SO_results:
-            gen_SO_cost_per_asset_overall, SO_nodes_matrix_G           = get_contribution_per_asset(gen_agent_cost_per_asset_overall, nodes, lines, "SO 1")
-            dem_SO_cost_per_asset_overall, SO_nodes_matrix_D           = get_contribution_per_asset(dem_agent_cost_per_asset_overall, nodes, lines, "SO 1")
+            gen_SO_cost_per_asset_overall, SO_nodes_matrix_G            = get_contribution_per_asset(gen_agent_cost_per_asset_overall, nodes, lines, "SO 1")
+            dem_SO_cost_per_asset_overall, SO_nodes_matrix_D            = get_contribution_per_asset(dem_agent_cost_per_asset_overall, nodes, lines, "SO 1")
             if show_aggregated_results:
-                gen_SO_cost_per_SO_overall,   SOs_lines                = get_contribution_per_group(gen_SO_cost_per_asset_overall, reactance, length_per_reactance, Ownership_matrix, SOs_interconnections, "SO Owner")
-                dem_SO_cost_per_SO_overall,   SOs_lines                = get_contribution_per_group(dem_SO_cost_per_asset_overall, reactance, length_per_reactance, Ownership_matrix, SOs_interconnections, "SO Owner")
+                gen_SO_cost_per_SO_overall,   SOs_lines                 = get_contribution_per_group(gen_SO_cost_per_asset_overall, [], length_per_reactance, Ownership_matrix, SOs_interconnections, "SO Owner")
+                dem_SO_cost_per_SO_overall,   SOs_lines                 = get_contribution_per_group(dem_SO_cost_per_asset_overall, [], length_per_reactance, Ownership_matrix, SOs_interconnections, "SO Owner")
+                SO_cost_per_SO_overall                                  = gen_SO_cost_per_SO_overall + dem_SO_cost_per_SO_overall
                 if category_aggregation:
-                    gen_SO_cost_per_asset_category_overall             = get_aggregation_per_category(gen_SO_cost_per_asset_overall, lines_attributes)
-                    dem_SO_cost_per_asset_category_overall             = get_aggregation_per_category(dem_SO_cost_per_asset_overall, lines_attributes)
+                    gen_SO_cost_per_asset_category_overall              = get_aggregation_per_category(gen_SO_cost_per_asset_overall, lines_attributes)
+                    dem_SO_cost_per_asset_category_overall              = get_aggregation_per_category(dem_SO_cost_per_asset_overall, lines_attributes)
 
         if show_agent_results and show_aggregated_results:
             gen_agent_cost_per_country_overall                          = np.matmul(gen_agent_cost_per_asset_overall,countries_lines.to_numpy())
             dem_agent_cost_per_country_overall                          = np.matmul(dem_agent_cost_per_asset_overall,countries_lines.to_numpy())
             gen_agent_total_cost_overall                                = np.sum(gen_agent_cost_per_country_overall, axis=1) 
             dem_agent_total_cost_overall                                = np.sum(dem_agent_cost_per_country_overall, axis=1)
             if SO_aggregation:  
                 gen_agent_cost_per_SO_overall                           = np.matmul(gen_agent_cost_per_asset_overall,SOs_lines.to_numpy())
                 dem_agent_cost_per_SO_overall                           = np.matmul(dem_agent_cost_per_asset_overall,SOs_lines.to_numpy())
             if category_aggregation:
                 gen_agent_cost_per_asset_category_overall               = get_aggregation_per_category(pd.DataFrame(gen_agent_cost_per_asset_overall.transpose(), index=lines["Line"], columns=nodes["Node"]), lines_attributes)
                 dem_agent_cost_per_asset_category_overall               = get_aggregation_per_category(pd.DataFrame(dem_agent_cost_per_asset_overall.transpose(), index=lines["Line"], columns=nodes["Node"]), lines_attributes)
-         
+
+    if losses_allocation_results:
+        gen_agent_losses_allocation_per_asset_overall   = line_losses_overall[:,0]*gen_agent_flow_contribution_per_asset_overall/line_flow_overall[:,0]
+        dem_agent_losses_allocation_per_asset_overall   = line_losses_overall[:,0]*dem_agent_flow_contribution_per_asset_overall/line_flow_overall[:,0]
+        
+        if regional_losses:
+            gen_agent_losses_allocation_per_asset_overall   = regional_assets[:,0]*gen_agent_losses_allocation_per_asset_overall
+            dem_agent_losses_allocation_per_asset_overall   = regional_assets[:,0]*dem_agent_losses_allocation_per_asset_overall
+
+        gen_agent_losses_allocation_per_asset_overall[np.isnan(gen_agent_losses_allocation_per_asset_overall)]    = 0
+        dem_agent_losses_allocation_per_asset_overall[np.isnan(dem_agent_losses_allocation_per_asset_overall)]    = 0
+        gen_agent_losses_allocation_per_asset_overall[np.isinf(gen_agent_losses_allocation_per_asset_overall)]    = 0
+        dem_agent_losses_allocation_per_asset_overall[np.isinf(dem_agent_losses_allocation_per_asset_overall)]    = 0     
+
+        gen_agent_losses_allocation_per_asset_overall   = gen_agent_losses_allocation_per_asset_overall*generation_losses_weight 
+        dem_agent_losses_allocation_per_asset_overall   = dem_agent_losses_allocation_per_asset_overall*demand_losses_weight
+
+        if show_agent_results and show_aggregated_results:
+            gen_agent_losses_allocation_per_country_overall = np.matmul(gen_agent_losses_allocation_per_asset_overall,countries_lines.to_numpy())
+            dem_agent_losses_allocation_per_country_overall = np.matmul(dem_agent_losses_allocation_per_asset_overall,countries_lines.to_numpy())
+            gen_agent_total_losses_allocation_overall       = np.sum(gen_agent_losses_allocation_per_asset_overall, axis=1) 
+            dem_agent_total_losses_allocation_overall       = np.sum(dem_agent_losses_allocation_per_asset_overall, axis=1)
+            if SO_aggregation:
+                gen_agent_losses_allocation_per_SO_overall  = np.matmul(gen_agent_losses_allocation_per_asset_overall,SOs_lines.to_numpy())
+                dem_agent_losses_allocation_per_SO_overall  = np.matmul(dem_agent_losses_allocation_per_asset_overall,SOs_lines.to_numpy())
+            if category_aggregation:
+                gen_agent_losses_allocation_per_asset_category_overall   = get_aggregation_per_category(pd.DataFrame(gen_agent_losses_allocation_per_asset_overall.transpose(), index=lines["Line"], columns=nodes["Node"]), lines_attributes)
+                dem_agent_losses_allocation_per_asset_category_overall   = get_aggregation_per_category(pd.DataFrame(dem_agent_losses_allocation_per_asset_overall.transpose(), index=lines["Line"], columns=nodes["Node"]), lines_attributes)
+                        
+        if show_country_results:
+            gen_country_losses_allocation_per_asset_overall, country_nodes_matrix_G = get_contribution_per_asset(gen_agent_losses_allocation_per_asset_overall, nodes, lines, "Country")
+            dem_country_losses_allocation_per_asset_overall, country_nodes_matrix_D = get_contribution_per_asset(dem_agent_losses_allocation_per_asset_overall, nodes, lines, "Country")
+            if show_aggregated_results:
+                gen_country_losses_allocation_per_country_overall, countries_lines  = get_contribution_per_group(gen_country_losses_allocation_per_asset_overall, [], length_per_reactance, Ownership_matrix, countries_interconnections, "Country")
+                dem_country_losses_allocation_per_country_overall, countries_lines  = get_contribution_per_group(dem_country_losses_allocation_per_asset_overall, [], length_per_reactance, Ownership_matrix, countries_interconnections, "Country")
+                if category_aggregation:
+                    gen_country_losses_allocation_per_asset_category_overall        = get_aggregation_per_category(gen_country_losses_allocation_per_asset_overall, lines_attributes)
+                    dem_country_losses_allocation_per_asset_category_overall        = get_aggregation_per_category(dem_country_losses_allocation_per_asset_overall, lines_attributes)
+                    
+        if show_SO_results:
+            gen_SO_losses_allocation_per_asset_overall, SO_nodes_matrix_G   = get_contribution_per_asset(gen_agent_losses_allocation_per_asset_overall, nodes, lines, "SO 1")
+            dem_SO_losses_allocation_per_asset_overall, SO_nodes_matrix_D   = get_contribution_per_asset(dem_agent_losses_allocation_per_asset_overall, nodes, lines, "SO 1")
+            if show_aggregated_results:
+                gen_SO_losses_allocation_per_SO_overall,   SOs_lines        = get_contribution_per_group(gen_SO_losses_allocation_per_asset_overall, [], length_per_reactance, Ownership_matrix, SOs_interconnections, "SO Owner")
+                dem_SO_losses_allocation_per_SO_overall,   SOs_lines        = get_contribution_per_group(dem_SO_losses_allocation_per_asset_overall, [], length_per_reactance, Ownership_matrix, SOs_interconnections, "SO Owner")
+                if category_aggregation:
+                    gen_SO_losses_allocation_per_asset_category_overall     = get_aggregation_per_category(gen_SO_losses_allocation_per_asset_overall, lines_attributes)
+                    dem_SO_losses_allocation_per_asset_category_overall     = get_aggregation_per_category(dem_SO_losses_allocation_per_asset_overall, lines_attributes)
+        
+        if losses_price:
+            gen_agent_losses_allocation_cost_per_asset_overall   = gen_agent_losses_allocation_per_asset_overall*losses_price*sum(snapshots_weights_dic.values())*0.001
+            dem_agent_losses_allocation_cost_per_asset_overall   = dem_agent_losses_allocation_per_asset_overall*losses_price*sum(snapshots_weights_dic.values())*0.001
+
+            if show_agent_results and show_aggregated_results:
+                gen_agent_losses_allocation_cost_per_country_overall = gen_agent_losses_allocation_per_country_overall*losses_price*sum(snapshots_weights_dic.values())*0.001
+                dem_agent_losses_allocation_cost_per_country_overall = dem_agent_losses_allocation_per_country_overall*losses_price*sum(snapshots_weights_dic.values())*0.001
+                gen_agent_total_losses_allocation_cost_overall       = gen_agent_total_losses_allocation_overall*losses_price*sum(snapshots_weights_dic.values())*0.001
+                dem_agent_total_losses_allocation_cost_overall       = dem_agent_total_losses_allocation_overall*losses_price*sum(snapshots_weights_dic.values())*0.001
+                if SO_aggregation:
+                    gen_agent_losses_allocation_cost_per_SO_overall  = gen_agent_losses_allocation_per_SO_overall*losses_price*sum(snapshots_weights_dic.values())*0.001
+                    dem_agent_losses_allocation_cost_per_SO_overall  = dem_agent_losses_allocation_per_SO_overall*losses_price*sum(snapshots_weights_dic.values())*0.001
+                if category_aggregation:
+                    gen_agent_losses_allocation_cost_per_asset_category_overall = gen_agent_losses_allocation_per_asset_category_overall*losses_price*sum(snapshots_weights_dic.values())*0.001
+                    dem_agent_losses_allocation_cost_per_asset_category_overall = dem_agent_losses_allocation_per_asset_category_overall*losses_price*sum(snapshots_weights_dic.values())*0.001
+                            
+            if show_country_results:
+                gen_country_losses_allocation_cost_per_asset_overall = gen_country_losses_allocation_per_asset_overall*losses_price*sum(snapshots_weights_dic.values())*0.001
+                dem_country_losses_allocation_cost_per_asset_overall = dem_country_losses_allocation_per_asset_overall*losses_price*sum(snapshots_weights_dic.values())*0.001
+                if show_aggregated_results:
+                    gen_country_losses_allocation_cost_per_country_overall   = gen_country_losses_allocation_per_country_overall*losses_price*sum(snapshots_weights_dic.values())*0.001
+                    dem_country_losses_allocation_cost_per_country_overall   = dem_country_losses_allocation_per_country_overall*losses_price*sum(snapshots_weights_dic.values())*0.001
+                    if category_aggregation:
+                        gen_country_losses_allocation_cost_per_asset_category_overall    = gen_country_losses_allocation_per_asset_category_overall*losses_price*sum(snapshots_weights_dic.values())*0.001
+                        dem_country_losses_allocation_cost_per_asset_category_overall    = dem_country_losses_allocation_per_asset_category_overall*losses_price*sum(snapshots_weights_dic.values())*0.001
+                        
+            if show_SO_results:
+                gen_SO_losses_allocation_cost_per_asset_overall  = gen_SO_losses_allocation_per_asset_overall*losses_price*sum(snapshots_weights_dic.values())*0.001
+                dem_SO_losses_allocation_cost_per_asset_overall  = dem_SO_losses_allocation_per_asset_overall*losses_price*sum(snapshots_weights_dic.values())*0.001
+                if show_aggregated_results:
+                    gen_SO_losses_allocation_cost_per_SO_overall = gen_SO_losses_allocation_per_SO_overall*losses_price*sum(snapshots_weights_dic.values())*0.001
+                    dem_SO_losses_allocation_cost_per_SO_overall = dem_SO_losses_allocation_per_SO_overall*losses_price*sum(snapshots_weights_dic.values())*0.001
+                    if category_aggregation:
+                        gen_SO_losses_allocation_cost_per_asset_category_overall = gen_SO_losses_allocation_per_asset_category_overall*losses_price*sum(snapshots_weights_dic.values())*0.001
+                        dem_SO_losses_allocation_cost_per_asset_category_overall = dem_SO_losses_allocation_per_asset_category_overall*losses_price*sum(snapshots_weights_dic.values())*0.001
+
     #%% overall intermediary results
     if show_intermediary_results:    
         if usage_result:
             gen_agent_flow_km_contribution_per_asset_overall                    = gen_agent_flow_contribution_per_asset_overall*line_length_matrix[:,0]
             dem_agent_flow_km_contribution_per_asset_overall                    = dem_agent_flow_contribution_per_asset_overall*line_length_matrix[:,0]
             if show_agent_results and show_aggregated_results:
                 gen_agent_flow_km_contribution_per_country_overall              = np.matmul(gen_agent_flow_km_contribution_per_asset_overall,countries_lines.to_numpy())
@@ -1297,15 +1614,87 @@
         remove_zero_rows_and_columns(dem_SO_flow_contribution_per_asset_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"SO demand overall flow contribution per asset.csv")
         if show_aggregated_results:
             remove_zero_rows_and_columns(gen_SO_flow_contribution_per_SO_overall.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"SO generation overall flow contribution per SO.csv")
             remove_zero_rows_and_columns(dem_SO_flow_contribution_per_SO_overall.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"SO demand overall flow contribution per SO.csv")
             if category_aggregation:
                 remove_zero_rows_and_columns(gen_SO_flow_contribution_per_asset_category_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"SO generation overall flow contribution per asset category.csv")
                 remove_zero_rows_and_columns(dem_SO_flow_contribution_per_asset_category_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"SO demand overall flow contribution per asset category.csv")
-                
+
+    if losses_allocation_results:
+        if show_agent_results:
+            print_to_csv(output_file+"Generation agents overall losses allocation per asset", gen_agent_losses_allocation_per_asset_overall, index=nodes["Node"], columns=lines["Line"], total=True, remove_zeros=remove_zero_values)
+            print_to_csv(output_file+"Demand agents overall losses allocation per asset", dem_agent_losses_allocation_per_asset_overall, index=nodes["Node"], columns=lines["Line"], total=True, remove_zeros=remove_zero_values)
+            if show_aggregated_results:
+                print_to_csv(output_file+"Generation agents overall losses allocation per country", gen_agent_losses_allocation_per_country_overall, index=nodes["Node"], columns=countries_lines.columns, total=False, remove_zeros=remove_zero_values)
+                print_to_csv(output_file+"Demand agents overall losses allocation per country", dem_agent_losses_allocation_per_country_overall, index=nodes["Node"], columns=countries_lines.columns, total=False, remove_zeros=remove_zero_values)
+                print_to_csv(output_file+"Generation agents overall total losses allocation", gen_agent_total_losses_allocation_overall, index=nodes["Node"], columns=['Total losses allocation MW'], total=True, remove_zeros=remove_zero_values)
+                print_to_csv(output_file+"Demand agents overall total losses allocation", dem_agent_total_losses_allocation_overall, index=nodes["Node"], columns=['Total losses allocation'], total=True, remove_zeros=remove_zero_values)
+                if SO_aggregation: 
+                    print_to_csv(output_file+"Generation agents overall losses allocation per SO", gen_agent_losses_allocation_per_SO_overall, index=nodes["Node"], columns=SOs_lines.columns, total=False, remove_zeros=remove_zero_values)
+                    print_to_csv(output_file+"Demand agents overall losses allocation per SO", dem_agent_losses_allocation_per_SO_overall, index=nodes["Node"], columns=SOs_lines.columns, total=False, remove_zeros=remove_zero_values)
+                if category_aggregation:
+                    remove_zero_rows_and_columns(gen_agent_losses_allocation_per_asset_category_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"Generation agents overall losses allocation per asset category.csv")
+                    remove_zero_rows_and_columns(dem_agent_losses_allocation_per_asset_category_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"Demand agents overall losses allocation per asset category.csv")
+        
+        if show_country_results:
+            remove_zero_rows_and_columns(gen_country_losses_allocation_per_asset_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"Country generation overall losses allocation per asset.csv")
+            remove_zero_rows_and_columns(dem_country_losses_allocation_per_asset_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"Country demand overall losses allocation per asset.csv")
+            if show_aggregated_results:
+                remove_zero_rows_and_columns(gen_country_losses_allocation_per_country_overall.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"Country generation overall losses allocation per country.csv")
+                remove_zero_rows_and_columns(dem_country_losses_allocation_per_country_overall.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"Country demand overall losses allocation per country.csv")
+                if category_aggregation:
+                    remove_zero_rows_and_columns(gen_country_losses_allocation_per_asset_category_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"Country generation overall losses allocation per asset category.csv")
+                    remove_zero_rows_and_columns(dem_country_losses_allocation_per_asset_category_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"Country demand overall losses allocation per asset category.csv")
+
+        if show_SO_results:
+            remove_zero_rows_and_columns(gen_SO_losses_allocation_per_asset_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"SO generation overall losses allocation per asset.csv")
+            remove_zero_rows_and_columns(dem_SO_losses_allocation_per_asset_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"SO demand overall losses allocation per asset.csv")
+            if show_aggregated_results:
+                remove_zero_rows_and_columns(gen_SO_losses_allocation_per_SO_overall.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"SO generation overall losses allocation per SO.csv")
+                remove_zero_rows_and_columns(dem_SO_losses_allocation_per_SO_overall.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"SO demand overall losses allocation per SO.csv")
+                if category_aggregation:
+                    remove_zero_rows_and_columns(gen_SO_losses_allocation_per_asset_category_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"SO generation overall losses allocation per asset category.csv")
+                    remove_zero_rows_and_columns(dem_SO_losses_allocation_per_asset_category_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"SO demand overall losses allocation per asset category.csv")
+
+        if losses_price:
+            if show_agent_results:
+                print_to_csv(output_file+"Generation agents overall losses allocation cost per asset", gen_agent_losses_allocation_cost_per_asset_overall, index=nodes["Node"], columns=lines["Line"], total=True, remove_zeros=remove_zero_values)
+                print_to_csv(output_file+"Demand agents overall losses allocation cost per asset", dem_agent_losses_allocation_cost_per_asset_overall, index=nodes["Node"], columns=lines["Line"], total=True, remove_zeros=remove_zero_values)
+                if show_aggregated_results:
+                    print_to_csv(output_file+"Generation agents overall losses allocation cost per country", gen_agent_losses_allocation_cost_per_country_overall, index=nodes["Node"], columns=countries_lines.columns, total=False, remove_zeros=remove_zero_values)
+                    print_to_csv(output_file+"Demand agents overall losses allocation cost per country", dem_agent_losses_allocation_cost_per_country_overall, index=nodes["Node"], columns=countries_lines.columns, total=False, remove_zeros=remove_zero_values)
+                    print_to_csv(output_file+"Generation agents overall total losses allocation cost", gen_agent_total_losses_allocation_cost_overall, index=nodes["Node"], columns=['Total losses allocation MW'], total=True, remove_zeros=remove_zero_values)
+                    print_to_csv(output_file+"Demand agents overall total losses allocation cost", dem_agent_total_losses_allocation_cost_overall, index=nodes["Node"], columns=['Total losses allocation'], total=True, remove_zeros=remove_zero_values)
+                    if SO_aggregation: 
+                        print_to_csv(output_file+"Generation agents overall losses allocation cost per SO", gen_agent_losses_allocation_cost_per_SO_overall, index=nodes["Node"], columns=SOs_lines.columns, total=False, remove_zeros=remove_zero_values)
+                        print_to_csv(output_file+"Demand agents overall losses allocation cost per SO", dem_agent_losses_allocation_cost_per_SO_overall, index=nodes["Node"], columns=SOs_lines.columns, total=False, remove_zeros=remove_zero_values)
+                    if category_aggregation:
+                        remove_zero_rows_and_columns(gen_agent_losses_allocation_cost_per_asset_category_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"Generation agents overall losses allocation cost per asset category.csv")
+                        remove_zero_rows_and_columns(dem_agent_losses_allocation_cost_per_asset_category_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"Demand agents overall losses allocation cost per asset category.csv")
+            
+            if show_country_results:
+                remove_zero_rows_and_columns(gen_country_losses_allocation_cost_per_asset_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"Country generation overall losses allocation cost per asset.csv")
+                remove_zero_rows_and_columns(dem_country_losses_allocation_cost_per_asset_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"Country demand overall losses allocation cost per asset.csv")
+                if show_aggregated_results:
+                    remove_zero_rows_and_columns(gen_country_losses_allocation_cost_per_country_overall.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"Country generation overall losses allocation cost per country.csv")
+                    remove_zero_rows_and_columns(dem_country_losses_allocation_cost_per_country_overall.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"Country demand overall losses allocation cost per country.csv")
+                    if category_aggregation:
+                        remove_zero_rows_and_columns(gen_country_losses_allocation_cost_per_asset_category_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"Country generation overall losses allocation cost per asset category.csv")
+                        remove_zero_rows_and_columns(dem_country_losses_allocation_cost_per_asset_category_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"Country demand overall losses allocation cost per asset category.csv")
+
+            if show_SO_results:
+                remove_zero_rows_and_columns(gen_SO_losses_allocation_cost_per_asset_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"SO generation overall losses allocation cost per asset.csv")
+                remove_zero_rows_and_columns(dem_SO_losses_allocation_cost_per_asset_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"SO demand overall losses allocation cost per asset.csv")
+                if show_aggregated_results:
+                    remove_zero_rows_and_columns(gen_SO_losses_allocation_cost_per_SO_overall.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"SO generation overall losses allocation cost per SO.csv")
+                    remove_zero_rows_and_columns(dem_SO_losses_allocation_cost_per_SO_overall.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"SO demand overall losses allocation cost per SO.csv")
+                    if category_aggregation:
+                        remove_zero_rows_and_columns(gen_SO_losses_allocation_cost_per_asset_category_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"SO generation overall losses allocation cost per asset category.csv")
+                        remove_zero_rows_and_columns(dem_SO_losses_allocation_cost_per_asset_category_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"SO demand overall losses allocation cost per asset category.csv")
+
     if cost_result:  
         if show_agent_results:
             print_to_csv(output_file+"Generation agents overall cost per asset", gen_agent_cost_per_asset_overall, index=nodes["Node"], columns=lines["Line"], total=True, remove_zeros=remove_zero_values)
             print_to_csv(output_file+"Demand agents overall cost per asset", dem_agent_cost_per_asset_overall, index=nodes["Node"], columns=lines["Line"],total=True, remove_zeros=remove_zero_values)
             if not is_all_ND_zeros:
                 remove_zero_rows_and_columns(negative_dem_agent_cost_per_asset_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"Negative demand agents overall cost per asset.csv")
             if cost_of_unused_capacity_op:
@@ -1325,24 +1714,26 @@
 
         if show_country_results:
             remove_zero_rows_and_columns(gen_country_cost_per_asset_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"Country generation overall cost per asset"+".csv")
             remove_zero_rows_and_columns(dem_country_cost_per_asset_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"Country demand overall cost per asset"+".csv")
             if show_aggregated_results:
                 remove_zero_rows_and_columns(gen_country_cost_per_country_overall.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"Country generation overall cost per country.csv")
                 remove_zero_rows_and_columns(dem_country_cost_per_country_overall.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"Country demand overall cost per country.csv")
+                remove_zero_rows_and_columns(country_cost_per_country_overall.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"Country joint overall cost per country.csv")
                 if category_aggregation:
                     remove_zero_rows_and_columns(gen_country_cost_per_asset_category_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"Country generation overall cost per asset category.csv")
                     remove_zero_rows_and_columns(dem_country_cost_per_asset_category_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"Country demand overall cost per asset category.csv")
 
         if show_SO_results:
             remove_zero_rows_and_columns(gen_SO_cost_per_asset_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"SO generation overall cost per asset.csv")
             remove_zero_rows_and_columns(dem_SO_cost_per_asset_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"SO demand overall cost per asset.csv")    
             if show_aggregated_results:
                 remove_zero_rows_and_columns(gen_SO_cost_per_SO_overall.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"SO generation overall cost per SO.csv")
                 remove_zero_rows_and_columns(dem_SO_cost_per_SO_overall.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"SO demand overall cost per SO.csv")
+                remove_zero_rows_and_columns(SO_cost_per_SO_overall.transpose(), remove_zero_values, remove_zero_values).to_csv(output_file+"SO joint overall cost per SO.csv")
                 if category_aggregation:
                     remove_zero_rows_and_columns(gen_SO_cost_per_asset_category_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"SO generation overall cost per asset category.csv")
                     remove_zero_rows_and_columns(dem_SO_cost_per_asset_category_overall, remove_zero_values, remove_zero_values).to_csv(output_file+"SO demand overall cost per asset category.csv")
     
     # other intermediary results
     if show_intermediary_results:
         if fraction_result:
@@ -1436,8 +1827,8 @@
     print('\n*************************************!RUNNING!*************************************')
     print(logo)
     execution_time = InfraFair_run(args.dir, args.case, args.config)
     print("*****************************!EXECUTION TIME %s!*****************************" % time.strftime('%H:%M:%S', time.gmtime(execution_time)))
     print('\n**************************!COST HAS BEEN FAIRLY ALLOCATED!*************************')
 
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `InfraFair-1.0.0/LICENSE` & `InfraFair-1.1.0/LICENSE.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,661 +1,661 @@
-                    GNU AFFERO GENERAL PUBLIC LICENSE
-                       Version 3, 19 November 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU Affero General Public License is a free, copyleft license for
-software and other kinds of works, specifically designed to ensure
-cooperation with the community in the case of network server software.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-our General Public Licenses are intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  Developers that use our General Public Licenses protect your rights
-with two steps: (1) assert copyright on the software, and (2) offer
-you this License which gives you legal permission to copy, distribute
-and/or modify the software.
-
-  A secondary benefit of defending all users' freedom is that
-improvements made in alternate versions of the program, if they
-receive widespread use, become available for other developers to
-incorporate.  Many developers of free software are heartened and
-encouraged by the resulting cooperation.  However, in the case of
-software used on network servers, this result may fail to come about.
-The GNU General Public License permits making a modified version and
-letting the public access it on a server without ever releasing its
-source code to the public.
-
-  The GNU Affero General Public License is designed specifically to
-ensure that, in such cases, the modified source code becomes available
-to the community.  It requires the operator of a network server to
-provide the source code of the modified version running there to the
-users of that server.  Therefore, public use of a modified version, on
-a publicly accessible server, gives the public access to the source
-code of the modified version.
-
-  An older license, called the Affero General Public License and
-published by Affero, was designed to accomplish similar goals.  This is
-a different license, not a version of the Affero GPL, but Affero has
-released a new version of the Affero GPL which permits relicensing under
-this license.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU Affero General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Remote Network Interaction; Use with the GNU General Public License.
-
-  Notwithstanding any other provision of this License, if you modify the
-Program, your modified version must prominently offer all users
-interacting with it remotely through a computer network (if your version
-supports such interaction) an opportunity to receive the Corresponding
-Source of your version by providing access to the Corresponding Source
-from a network server at no charge, through some standard or customary
-means of facilitating copying of software.  This Corresponding Source
-shall include the Corresponding Source for any work covered by version 3
-of the GNU General Public License that is incorporated pursuant to the
-following paragraph.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the work with which it is combined will remain governed by version
-3 of the GNU General Public License.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU Affero General Public License from time to time.  Such new versions
-will be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU Affero General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU Affero General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU Affero General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU Affero General Public License as published
-    by the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU Affero General Public License for more details.
-
-    You should have received a copy of the GNU Affero General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If your software can interact with users remotely through a computer
-network, you should also make sure that it provides a way for users to
-get its source.  For example, if your program is a web application, its
-interface could display a "Source" link that leads users to an archive
-of the code.  There are many ways you could offer source, and different
-solutions will be better for different programs; see section 13 for the
-specific requirements.
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU AGPL, see
-<https://www.gnu.org/licenses/>.
+                    GNU AFFERO GENERAL PUBLIC LICENSE
+                       Version 3, 19 November 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU Affero General Public License is a free, copyleft license for
+software and other kinds of works, specifically designed to ensure
+cooperation with the community in the case of network server software.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+our General Public Licenses are intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  Developers that use our General Public Licenses protect your rights
+with two steps: (1) assert copyright on the software, and (2) offer
+you this License which gives you legal permission to copy, distribute
+and/or modify the software.
+
+  A secondary benefit of defending all users' freedom is that
+improvements made in alternate versions of the program, if they
+receive widespread use, become available for other developers to
+incorporate.  Many developers of free software are heartened and
+encouraged by the resulting cooperation.  However, in the case of
+software used on network servers, this result may fail to come about.
+The GNU General Public License permits making a modified version and
+letting the public access it on a server without ever releasing its
+source code to the public.
+
+  The GNU Affero General Public License is designed specifically to
+ensure that, in such cases, the modified source code becomes available
+to the community.  It requires the operator of a network server to
+provide the source code of the modified version running there to the
+users of that server.  Therefore, public use of a modified version, on
+a publicly accessible server, gives the public access to the source
+code of the modified version.
+
+  An older license, called the Affero General Public License and
+published by Affero, was designed to accomplish similar goals.  This is
+a different license, not a version of the Affero GPL, but Affero has
+released a new version of the Affero GPL which permits relicensing under
+this license.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU Affero General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Remote Network Interaction; Use with the GNU General Public License.
+
+  Notwithstanding any other provision of this License, if you modify the
+Program, your modified version must prominently offer all users
+interacting with it remotely through a computer network (if your version
+supports such interaction) an opportunity to receive the Corresponding
+Source of your version by providing access to the Corresponding Source
+from a network server at no charge, through some standard or customary
+means of facilitating copying of software.  This Corresponding Source
+shall include the Corresponding Source for any work covered by version 3
+of the GNU General Public License that is incorporated pursuant to the
+following paragraph.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the work with which it is combined will remain governed by version
+3 of the GNU General Public License.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU Affero General Public License from time to time.  Such new versions
+will be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU Affero General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU Affero General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU Affero General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU Affero General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU Affero General Public License for more details.
+
+    You should have received a copy of the GNU Affero General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If your software can interact with users remotely through a computer
+network, you should also make sure that it provides a way for users to
+get its source.  For example, if your program is a web application, its
+interface could display a "Source" link that leads users to an archive
+of the code.  There are many ways you could offer source, and different
+solutions will be better for different programs; see section 13 for the
+specific requirements.
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU AGPL, see
+<https://www.gnu.org/licenses/>.
```

### Comparing `InfraFair-1.0.0/README.md` & `InfraFair-1.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 ![image](doc/Images/InfraFair_Logo.png)
-[![License](https://img.shields.io/badge/License-AGPL%20v3-blue.svg)](https://github.com/IIT-EnergySystemModels/InfraFair/blob/main/LICENSE)
-[![Documentation Status](https://readthedocs.org/projects/infrafair/badge/?version=latest)](https://infrafair.readthedocs.io/en/latest/?badge=latest)
 
 # InfraFair
 *"Fairness in allocating infrastructure cost"*   
 
 **InfraFair** has been developed at the [Instituto de Investigación Tecnológica (IIT)](https://www.iit.comillas.edu/index.php.en) 
 of the [Universidad Pontificia Comillas](https://www.comillas.edu/en/).
 
 The full documentation can be accessed [here](https://infrafair.readthedocs.io/en/latest/index.html)
 
 ## Description
-The InfraFair is a modelling tool aimed at computing the allocation of the cost of energy infrastructure according 
+The InfraFair modelling tool is aimed at computing the allocation of the cost of energy infrastructure according 
 to the economic use expected to be made by agents, driving efficient investment decisions. The modelling tool 
 employs the **Average Participations Method (APM)** that allocates the 
 cost based on the electrical usage that each agent makes of each infrastructure asset as a reasonable proxy 
 to the benefits, the former obtained from the latter. The basic intuition behind the APM is that 
 energy consumed by demands and produced by generators, as well as the responsibility for causing energy 
-flows, can be assigned by employing **a simple heuristic rule** that only uses the actual pattern of flows in 
-the infrastructure network. 
+flows, can be assigned by employing simple heuristic rules that only use the actual pattern of flows in 
+the infrastructure network.
 
-The rule assumes that energy flows can be traced by supposing that at any network node, the inflows are distributed proportionally among the outflows. This is the so-called **proportionality rule**. Implicit in this rule is the assumption that energy does not flow in the opposite direction to that of the prevalent (net) flow over each asset, which, according to this assumption, is the only existing flow. Based on these assumptions, the method traces the flow of energy from individual sources to individual sinks in all the network assets.
 
 ## Scope
 InfraFair determines the network utilisation of agents, system operators and countries. 
 Based on this utilisation and assuming that it reflects the economic benefits received by agents, 
 it determines the responsibility of each agent in the construction of each element in the network. 
 In order to reasonably reflect agent utilisation of infrastructure, multiple representative snapshots 
 of annual network usage should be provided. InfraFair presents a decision support tool for tariff 
@@ -32,15 +29,15 @@
 as well as other types of infrastructures operating on the same principle of flow (*flow-based infrastructure*), 
 such as gas and hydrogen infrastructure. 
 All assets that have a flow usage can be represented in the network model. For instance, the electrical network can include
 power lines, transformers, breaks, series capacitors and phase shifting transformers.
 
 
 ## Functionality
-Inputs to the model must consist of the **map of flows** in each of the assets as well as the **injections and withdrawals** of energy at each node. Additionally, the **rating capacity and the capital cost** of each asset must be provided for the model to be able to allocate costs to network users. Other information, such as the voltage and the length of each asset, can be provided to produce optional categorised results. When provided with hourly representative snapshots of these inputs, InfraFair can calculate (per snapshot and overall annual weighted average):
+When provided with hourly representative snapshots, InfraFair can calculate (per snapshot and overall annual weighted average):
 
 * Individual agent flow and cost contributions to each asset in the network.
 * Country flow and cost contributions to each asset in the network.
 * Individual agent and country utilisation of each asset in the network.
 * Individual Agent flow and cost contributions to similar aggregated assets.
 * Country flow and cost contributions to similar aggregated assets. 
 * Individual agent and country utilisation of similar aggregated assets.
@@ -79,17 +76,17 @@
 the following on the command prompt (Windows) or Terminal (Linux) (Depending on what your standard python version is, 
 you might need to call python3 instead of python)::
 
     > python InfraFair.py
 
 Then, three parameters (directory folder, and configuration file) will be asked for.
 
-**Remark**: at this step, only press enter for each input and InfraFair will be executed with the default parameters.
+**Remark**: at this step only press enter for each input and InfraFair will be executed with the default parameters.
 
-After this, in a directory of your choice, make a copy of the [Simple example](<https://github.com/IIT-EnergySystemModels/InfraFair/tree/main/Examples/Simple_ex>) or [EU example](<https://github.com/IIT-EnergySystemModels/InfraFair/tree/main/Examples/EU_ex>) case to create a new 
+After this in a directory of your choice, make a copy of the [Simple example](<https://github.com/IIT-EnergySystemModels/InfraFair/tree/master/Examples/Simple_ex>) or [EU example](<https://github.com/IIT-EnergySystemModels/InfraFair/tree/master/Examples/EU_ex>) case to create a new 
 case of your choice but using the current format of the .csv files.
 Proper execution of InfraFair.py can be made by introducing the new case and the directory of your choice. 
 
 Then, the output results should be written in the same folder as the case input. 
 
 **Note**: An alternative way to run the model is by creating a new script **script.py**, and writing the following::
         
@@ -104,12 +101,12 @@
 
 We strongly welcome anyone interested in contributing to this project.
 
 
 ## License
 Copyright 2023 [Universidad Pontificia Comillas](https://www.comillas.edu/en/)
 
-InfraFair is licensed under the open source [AGPL-3.0 license](https://github.com/IIT-EnergySystemModels/InfraFair/tree/main/LICENSE).
+InfraFair is licensed under the open source [AGPL-3.0 license](https://github.com/IIT-EnergySystemModels/InfraFair/tree/master/LICENSE.txt).
 
 
 ## Execution
-![image](doc/Images/InfraFair_execution.png)
+![image](doc/Images/InfraFair_execution.png)
```

### Comparing `InfraFair-1.0.0/setup.py` & `InfraFair-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,39 +13,39 @@
 \______|\__|  \__|\__|      \__|       \_______|\__|       \_______|\__|\__|      
 
 """
 print(logo)
 
 setup(
     name='InfraFair',
-    version='1.0.0',    
+    version='1.1.0',    
     description='A modelling tool for infrastructure cost allocation',
     url='https://github.com/IIT-EnergySystemModels/InfraFair',
     author='Mohamed A.Eltahir Elabbas',
     author_email='mohamed.a.eltahir@hotmail.com',
     license='GNU AFFERO General Public License v3',
     long_description = "README.md",
     packages=['InfraFair'],
     install_requires=['numpy>=1.21.4',
-                      'pandas>=1.3.4,<2.0.0',
+                      'pandas==1.3.4',
                       'matplotlib>=3.5.0',
-                      'openpyxl>=3.0.0',
+                      'openpyxl>=3.0.0',                  
                       ],
     dependency_links=[
         "http://pandas.pydata.org/",
         "http://www.numpy.org/",
         "https://matplotlib.org/",
     ],
-    python_requires= ">=3.8,<3.12",       
+    python_requires= ">=3.8,<3.12",     
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Science/Research',
         'Environment :: Console',
         'License :: OSI Approved :: GNU Affero General Public License v3',  
         'Operating System :: OS Independent',
         'Natural Language :: English',        
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],   
-)
+)
```

