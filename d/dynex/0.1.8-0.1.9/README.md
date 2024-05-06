# Comparing `tmp/dynex-0.1.8.tar.gz` & `tmp/dynex-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynex-0.1.8.tar", last modified: Fri Oct  6 10:19:12 2023, max compression
+gzip compressed data, was "dynex-0.1.9.tar", last modified: Mon Oct 16 09:54:01 2023, max compression
```

## Comparing `dynex-0.1.8.tar` & `dynex-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-10-06 10:19:12.822509 dynex-0.1.8/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1522 2023-10-06 10:19:12.822509 dynex-0.1.8/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     9634 2023-09-04 09:37:45.000000 dynex-0.1.8/README.md
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-10-06 10:19:12.822509 dynex-0.1.8/dynex/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    84506 2023-10-06 10:18:37.000000 dynex-0.1.8/dynex/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-10-06 10:19:12.822509 dynex-0.1.8/dynex.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1522 2023-10-06 10:19:12.000000 dynex-0.1.8/dynex.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      180 2023-10-06 10:19:12.000000 dynex-0.1.8/dynex.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-10-06 10:19:12.000000 dynex-0.1.8/dynex.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       89 2023-10-06 10:19:12.000000 dynex-0.1.8/dynex.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        6 2023-10-06 10:19:12.000000 dynex-0.1.8/dynex.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-10-06 10:19:12.822509 dynex-0.1.8/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1892 2023-10-06 10:18:41.000000 dynex-0.1.8/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-10-16 09:54:01.395960 dynex-0.1.9/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1522 2023-10-16 09:54:01.395960 dynex-0.1.9/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     9634 2023-09-04 09:37:45.000000 dynex-0.1.9/README.md
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-10-16 09:54:01.395960 dynex-0.1.9/dynex/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   110270 2023-10-16 09:53:26.000000 dynex-0.1.9/dynex/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-10-16 09:54:01.395960 dynex-0.1.9/dynex.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1522 2023-10-16 09:54:01.000000 dynex-0.1.9/dynex.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      180 2023-10-16 09:54:01.000000 dynex-0.1.9/dynex.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-10-16 09:54:01.000000 dynex-0.1.9/dynex.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       89 2023-10-16 09:54:01.000000 dynex-0.1.9/dynex.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        6 2023-10-16 09:54:01.000000 dynex-0.1.9/dynex.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-10-16 09:54:01.395960 dynex-0.1.9/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1892 2023-10-16 09:53:55.000000 dynex-0.1.9/setup.py
```

### Comparing `dynex-0.1.8/PKG-INFO` & `dynex-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dynex
-Version: 0.1.8
+Version: 0.1.9
 Summary: Dynex SDK Neuromorphic Computing
 Home-page: https://github.com/dynexcoin/DynexSDK
 Author: Dynex Developers
 Author-email: office@dynexcoin.org
 License: GPLv3
 Description: The Dynex SDK provides a neuromorphic Ising/QUBO sampler which can be called from any Python code. Developers and application developers already familiar with the Dimod framework, PyQUBO or the Ocean SDK will find it very easy to run computations on the Dynex neuromorphic computing platform: The Dynex Sampler object can simply replace the default sampler object which typically is used to run computations on, for example, the D-Wave system – without the limitations of quantum machines. The Dynex SDK is a suite of open-source Python tools for solving hard problems with neuromorphic computing which helps reformulate your application’s problem for solution by the Dynex computing platform. It also handles communication between your application code and the Dynex neuromorphic computing platform automatically.
 Platform: UNKNOWN
```

### Comparing `dynex-0.1.8/README.md` & `dynex-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dynex-0.1.8/dynex/__init__.py` & `dynex-0.1.9/dynex/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,28 +22,41 @@
 SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT,
 STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF
 THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 __author__ = 'Dynex Developers'
 __credits__ = 'Dynex Developers, Contributors, Supporters and the Dynex Community'
 
 # Changelog 0.1.7:
-# - all internal funtions: prepend '_x' (and rebuild docs) 
-# - don't throw exeception on missing ini, just warning (import dynex issue) 
-# - test-net: automatically use max fitting chips; ignore num_reads 
-# - remove "boost job priority" for now 
+# + all internal funtions: prepend '_x' (and rebuild docs) 
+# + don't throw exeception on missing ini, just warning (import dynex issue) 
+# + test-net: automatically use max fitting chips; ignore num_reads 
+# + remove "boost job priority" for now 
 
 # Changelog 0.1.8:
-# - improved accuracy by validating solution file's reported energies with voltages and omitting incorrect reads
-# - improved sampling display (showing ground state and decluttered)
-# - default logging=False for CQM/BQM/SAT models
+# + improved accuracy by validating solution file's reported energies with voltages and omitting incorrect reads
+# + improved sampling display (showing ground state and decluttered)
+# + default logging=False for CQM/BQM/SAT models
+
+# Changelog 0.1.9:
+# + moved energy ground state calculation into _DynexSampler class
+# + improved debugging=True option for sampling
+# + new sampler parameter: bnb=True/False (testnet only; sampling method: branch-and-bound)
+# + new function dynex.sample(bqm, **parameters)
+# + new function dynex.sample_qubo(Q, offset, **parameters)
+# + new function dynex.sample_ising(h, j, **parameters)
+# + improved bqm2bin function:
+#    - faster: direct conversion from bqm (qubo step omitted)
+#    - rydberg hamiltonian formulation
+#    - reduction of linear terms
+    
 
 # Upcoming:
 # - Multi-model parallel sampling (f.e. for parameter tuning jobs, etc.)
 # - API call: encrypt file
 # - new encrypt / compress function
 
 ################################################################################################################################
@@ -645,95 +658,137 @@
         
             f.write(line_enc+"\n"); 
 
 ################################################################################################################################
 # calculate number of falsified clauses (loc) & Energy based on assignment and model
 ################################################################################################################################
 
-def _energy(model, sample, mapping=True):
+# moved into class DynexSampler
+            
+################################################################################################################################
+# functions to convert BQM to QUBO
+################################################################################################################################
+
+def max_precision(bqm):
+    max_abs_coeff = np.max(np.abs(bqm.to_numpy_matrix()))
+    if max_abs_coeff == 0:
+        print('[DYNEX] ERROR: AT LEAST ONE WEIGHT MUST BE > 0.0');
+        raise Exception("ERROR: AT LEAST ONE WEIGHT MUST BE > 0.0");
+    precision = 10 ** (np.floor(np.log10(max_abs_coeff)) - 4)
+    return precision
+
+def _convert_bqm_to_qubo_direct(bqm, relabel=True, logging=True):
     """
     `Internal Function`
+
+    Replacement for _convert_bqm_to_qubo with the following changes:
+    - direct conversion from bqm (qubo step omitted), faster
+    - rydberg hamiltonian formulation
+    - reduction of linear terms
     
-    Takes a model and dimod samples and calculates the energy and loc.
+    Converts a given Binary Quadratic Model (BQM) problem into a wncf file which is being used by the Dynex platform workers for the sampling process. Every BQM can be converted to a QUBO formulation in polynomial time (and vice-versa) without loss of functionality. During the process, variables are re-labeld and mapped to integer values in the range of [0, NUM_VARIABLES}. The mapping is being made available in sampler.variable_mappings and is used for constructing the returned sampleset object.
+
+    :Notes: 
+
+    - The BQM needs to have at least one defined weight, otherwise an exception is thrown
+    - Double values of weights are being converted to integer values with the factor 'PRECISION' 
+    - The value for PRECISION is determined automatically with function 10 ** (np.floor(np.log10(max_abs_coeff)) - 4)
+
+    :Parameters:
+
+    - :bqm: the Binary Quadratic Model to be converted (class:`dimod.BinaryQuadraticModel`)
+
+    :Returns:
+
+    - :clauses: A list of all clauses (`list`)
+    - :num_variables: number of variables (`int`)
+    - :num_clauses: number of clauses (`int`)
+    - :mappings: variable mappings original -> integer value (`dict`)
+    - :precision: precision of conversion (`double`)
+    - :bqm: class:`dimod.BinaryQuadraticModel`
+
+    """
     
-    Input: 
-    ======
+    # map variables to integers:
+    mappings = bqm.variables._relabel_as_integers();
+    
+    # define return set:
+    clauses = [];
+
+    # linear and quadratic terms of bqm:
+    linear = [v for i, v in sorted(bqm.linear.items(), key=lambda x: x[0])];
+    quadratic = [[i, j, v] for (i, j), v in bqm.quadratic.items()];
+    
+    # max precision to be applied:
+    precision = max_precision(bqm);
+    
+    # max precision is 1:
+    if precision>1:
+        if logging:
+            print("[ÐYNEX] PRECISION CUT FROM",precision,"TO 1");
+        precision = 1;
+
+    if logging:
+        print("[DYNEX] PRECISION SET TO", precision);
+
+    # linear terms:
+    linear_corr = np.round(np.array(linear) / precision);
+    _linear = {}
+    for i, _ in enumerate(linear):
+        if linear_corr[i] == 0:
+            continue
+        _linear[-np.sign(linear_corr[i]) * (i + 1)] = np.abs(linear_corr[i])
+        v = linear_corr[i];
+        
+    # reduce linear terms:
+    _linear_reduced = {}
+    for _, i in enumerate(_linear):
+        weight = _linear.get(i, 0) - _linear.get(-i, 0)
+        if weight > 0:
+            _linear_reduced[i] = weight
+            clauses.append([weight, i]);
+        elif weight < 0:
+            _linear_reduced[-i] = -weight
+            clauses.append([-weight, -i]);
+
+    num_variables = len(linear);
+    
+    # quadratic terms:
+    if quadratic:
+        quadratic_corr = np.round(np.array(quadratic)[:, 2] / precision)
+        _quadratic = {}
+        for edge, _ in enumerate(quadratic):
+            i = quadratic[edge][0] + 1
+            j = quadratic[edge][1] + 1
+
+            if quadratic[edge][2] > 0:
+                _quadratic[(-i, -j)] = _quadratic.get((i, j), 0) + quadratic_corr[edge]
+                v = np.abs(quadratic_corr[edge]);
+                if v != 0:
+                    clauses.append([v, -i, -j]);
+                
+            elif quadratic[edge][2] < 0:
+                _linear[i] = _linear.get(-i, 0) - quadratic_corr[edge]
+                _quadratic[(-i, j)] = _quadratic.get((i, -j), 0) - quadratic_corr[edge]
+                v = np.abs(quadratic_corr[edge]);
+                if v != 0:
+                    clauses.append([v, i, j]);
+                    clauses.append([v, -i, j]);
+                    clauses.append([v, i, -j]);
+                
+    # re-map variables:
+    bqm.variables._relabel(mappings);
+    num_clauses = len(clauses);
+
+    return clauses, num_variables, num_clauses, mappings, precision, bqm
     
-    - dimod sample (dict) with mapping = True
-      example: {0: 0, 1: 0, 2: 0, 3: 0, 4: 0, 5: 0, 6: 0, 7: 0, 8: 0, 9: 0, 10: 0, 11: 0, 12: 0, 13: 0, 14: 0}
-      
-    or
-      
-    - assignments (list) with mapping = False (raw solution file)
-      example: [1, 1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, 1, -1, -1]
-    """
-    # convert dimod sample to wcnf mapping:
-    wcnf_vars = []; 
-    if mapping:
-        for v in sample:
-            if v in model.var_mappings:
-                v_mapped = model.var_mappings[v];
-            else:
-                v_mapped = v;
-            wcnf_vars.append(sample[v_mapped])
-    # or convert solution file to 0/1:
-    else:
-        for v in sample:
-            if v>0:
-                wcnf_vars.append(1);
-            else:
-                wcnf_vars.append(0);
-        
-    loc = 0;
-    energy = 0.0;
-    for clause in model.clauses:
-        # 2 clause:
-        if len(clause)==2:
-            w = clause[0];
-            i = abs(clause[1]);
-            i_dir = np.sign(clause[1]);
-            if i_dir == -1:
-                i_dir = 0;
-            i_assign = wcnf_vars[i-1];
-            sat = False;
-            if (i_dir == i_assign):
-                sat = True;
-            if sat == False:
-                loc += 1;
-                energy += w;
-            
-        # 3 clause:
-        if len(clause)==3:
-            w = clause[0];
-            i = abs(clause[1]);
-            i_dir = np.sign(clause[1]);
-            if i_dir == -1:
-                i_dir = 0;
-            i_assign = wcnf_vars[i-1];
-            j = abs(clause[2]);
-            j_dir = np.sign(clause[2]);
-            if j_dir == -1:
-                j_dir = 0;
-            j_assign = wcnf_vars[j-1];
-            sat = False;
-            if (i_dir == i_assign) or (j_dir == j_assign):
-                sat = True;
-            if sat == False:
-                loc += 1;
-                energy += w;
-            
-    return loc, energy
-            
-################################################################################################################################
-# functions to convert BQM to QUBO
-################################################################################################################################
 
 def _convert_bqm_to_qubo(bqm, relabel=True, logging=True):
     """
-    `Internal Function`
+    `Internal Function - replaced by _convert_bqm_to_qubo_direct()`
 
     Converts a given Binary Quadratic Model (BQM) problem into a wncf file which is being used by the Dynex platform workers for the sampling process. Every BQM can be converted to a QUBO formulation in polynomial time (and vice-versa) without loss of functionality. During the process, variables are re-labeld and mapped to integer values in the range of [0, NUM_VARIABLES}. The mapping is being made available in sampler.variable_mappings and is used for constructing the returned sampleset object.
 
     :Notes: 
 
     - The BQM needs to have at least one defined weight, otherwise an exception is thrown
     - Double values of weights are being converted to integer values with the factor 'PRECISION' 
@@ -779,17 +834,14 @@
 
     # max precision is 1:
     if precision>1:
         if logging:
             print("[ÐYNEX] PRECISION CUT FROM",precision,"TO 1");
         precision = 1;
 
-    if logging:
-        print("[DYNEX] PRECISION SET TO", precision);
-
     # constant offset:
     W_add = Q[1]; 
     if logging:
         print("[DYNEX] QUBO: Constant offset of the binary quadratic model:", W_add);
 
     for i in range(0, len(Q_list)):
         touple = Q_list[i];
@@ -808,15 +860,15 @@
         # quadratic term:
         if i!=j:
             if w_int > 0:
                 clauses.append([w_int, -i, -j]);
             if w_int < 0:
                 clauses.append([-w_int, i, -j]);
                 clauses.append([-w_int, j]);
-        
+                
     num_variables = len(bqm.variables);
     num_clauses = len(clauses);
 
     # re-map variables from integer to original using self.var_mapping:
     bqm.variables._relabel(mappings)
     
     return clauses, num_variables, num_clauses, mappings, precision, bqm
@@ -880,17 +932,22 @@
 
         bqm = dimod.BinaryQuadraticModel({'x1': 1.0, 'x2': -1.5, 'x3': 2.0}, 
                                  {('x1', 'x2'): 1.0, ('x2', 'x3'): -2.0}, 
                                  0.0, dimod.BINARY)
         model = dynex.BQM(bqm)
 
     """
-    def __init__(self, bqm, relabel=True, logging=False):
-        self.clauses, self.num_variables, self.num_clauses, self.var_mappings, self.precision, self.bqm = _convert_bqm_to_qubo(bqm, relabel, logging);
+    def __init__(self, bqm, relabel=True, logging=False, formula=2):
+        if formula == 1:
+            self.clauses, self.num_variables, self.num_clauses, self.var_mappings, self.precision, self.bqm = _convert_bqm_to_qubo(bqm, relabel, logging);
+        if formula == 2:
+            self.clauses, self.num_variables, self.num_clauses, self.var_mappings, self.precision, self.bqm = _convert_bqm_to_qubo_direct(bqm, relabel, logging);
+            
         if self.num_clauses == 0 or self.num_variables == 0:
+            raise Exception('[DYNEX] ERROR: Could not initiate model - no variables & clauses');
             return;
         self.type = 'wcnf';
         self.logging = logging;
         self.typestr = 'BQM';
 
 class CQM():
     """
@@ -917,17 +974,24 @@
         cqm = dimod.ConstrainedQuadraticModel()
         cqm.set_objective(-3 * num_widget_a - 4 * num_widget_b)
         cqm.add_constraint(num_widget_a + num_widget_b <= 5, label='total widgets')
         model = dynex.CQM(cqm)
 
 
     """
-    def __init__(self, cqm, relabel=True, logging=False):
+    def __init__(self, cqm, relabel=True, logging=False, formula=2):
         bqm, self.invert = dimod.cqm_to_bqm(cqm)
-        self.clauses, self.num_variables, self.num_clauses, self.var_mappings, self.precision, self.bqm = _convert_bqm_to_qubo(bqm, relabel, logging);
+        if formula == 1:
+            self.clauses, self.num_variables, self.num_clauses, self.var_mappings, self.precision, self.bqm = _convert_bqm_to_qubo(bqm, relabel, logging);
+        if formula == 2:
+            self.clauses, self.num_variables, self.num_clauses, self.var_mappings, self.precision, self.bqm = _convert_bqm_to_qubo_direct(bqm, relabel, logging);
+            
+        if self.num_clauses == 0 or self.num_variables == 0:
+            raise Exception('[DYNEX] ERROR: Could not initiate model - no variables & clauses');
+            return;
         self.type = 'wcnf';
         self.logging = logging;
         self.typestr = 'CQM';
 
 ################################################################################################################################
 # Thread runner: sample clones
 ################################################################################################################################
@@ -939,15 +1003,221 @@
         print('[DYNEX] Clone '+str(x)+' started...'); 
     _sampler = _DynexSampler(model, False, True, description, False);
     _sampleset = _sampler.sample(num_reads, annealing_time, switchfraction, alpha, beta, gamma, delta, epsilon, zeta, minimum_stepsize, False);
     if logging:
         print('[DYNEX] Clone '+str(x)+' finished'); 
     q.put(_sampleset);
     return
+
+################################################################################################################################
+# Dynex sampling functions
+################################################################################################################################
+def sample_qubo(Q, offset=0.0, logging=True, formula=2, mainnet=False, description='Dynex SDK Job', test=False, bnb=False, num_reads = 32, annealing_time = 10, clones = 1, switchfraction = 0.0, alpha=20, beta=20, gamma=1, delta=1, epsilon=1, zeta=1, minimum_stepsize = 0.00000006, debugging=False):
+    """
+    Samples a Qubo problem.
+    
+    :Parameters:
+    
+    - :Q: The Qubo problem
+    
+    - :offset: The offset value of the Qubo problem
+    
+    - :logging: Defines if the sampling process should be quiet with no terminal output (FALSE) or if process updates are to be shown (`bool`)
+    
+    - :mainnet: Defines if the mainnet (Dynex platform sampling) or the testnet (local sampling) is being used for sampling (`bool`)
+    
+    - :description: Defines the description for the sampling, which is shown in Dynex job dashboards as well as in the market place  (`string`)
     
+    - :num_reads: Defines the number of parallel samples to be performed (`int` value in the range of [32, MAX_NUM_READS] as defined in your license)
+
+    - :annealing_time: Defines the number of integration steps for the sampling. Models are being converted into neuromorphic circuits, which are then simulated with ODE integration by the participating workers (`int` value in the range of [1, MAX_ANNEALING_TIME] as defined in your license)
+        
+    - :clones: Defines the number of clones being used for sampling. Default value is 1 which means that no clones are being sampled. Especially when all requested num_reads will fit on one worker, it is desired to also retrieve the optimum ground states found from more than just one worker. The number of clones runs the sampler for n clones in parallel and aggregates the samples. This ensures a broader spectrum of retrieved samples. Please note, it the number of clones is set higher than the number of available threads on your local machine, then the number of clones processed in parallel is being processed in batches. Clone sampling is only available when sampling on the mainnet. (`integer` value in the range of [1,128])
+
+    - :switchfraction: Defines the percentage of variables which are replaced by random values during warm start samplings (`double` in the range of [0.0, 1.0])
+
+    - :alpha: The ODE integration of the QUBU/Ising or SAT model based neuromorphic circuits is using automatic tuning of these parameters for the ODE integration. Setting values defines the upper bound for the automated parameter tuning (`double` value in the range of [0.00000001, 100.0] for alpha and beta, and [0.0 and 1.0] for gamma, delta and epsilon)
+
+    - :beta: The ODE integration of the QUBU/Ising or SAT model based neuromorphic circuits is using automatic tuning of these parameters for the ODE integration. Setting values defines the upper bound for the automated parameter tuning (`double` value in the range of [0.00000001, 100.0] for alpha and beta, and [0.0 and 1.0] for gamma, delta and epsilon)
+
+    - :gamma: The ODE integration of the QUBU/Ising or SAT model based neuromorphic circuits is using automatic tuning of these parameters for the ODE integration. Setting values defines the upper bound for the automated parameter tuning (`double` value in the range of [0.00000001, 100.0] for alpha and beta, and [0.0 and 1.0] for gamma, delta and epsilon)
+
+    - :delta: The ODE integration of the QUBU/Ising or SAT model based neuromorphic circuits is using automatic tuning of these parameters for the ODE integration. Setting values defines the upper bound for the automated parameter tuning (`double` value in the range of [0.00000001, 100.0] for alpha and beta, and [0.0 and 1.0] for gamma, delta and epsilon)
+
+    - :epsilon: The ODE integration of the QUBU/Ising or SAT model based neuromorphic circuits is using automatic tuning of these parameters for the ODE integration. Setting values defines the upper bound for the automated parameter tuning (`double` value in the range of [0.00000001, 100.0] for alpha and beta, and [0.0 and 1.0] for gamma, delta and epsilon)
+
+    - :zeta: The ODE integration of the QUBU/Ising or SAT model based neuromorphic circuits is using automatic tuning of these parameters for the ODE integration. Setting values defines the upper bound for the automated parameter tuning (`double` value in the range of [0.00000001, 100.0] for alpha and beta, and [0.0 and 1.0] for gamma, delta and epsilon)
+
+    - :minimum_stepsize: The ODE integration of the QUBU/Ising or SAT model based neuromorphic circuits is performig adaptive stepsizes for each ODE integration forward Euler step. This value defines the smallest step size for a single adaptive integration step (`double` value in the range of [0.0000000000000001, 1.0])
+
+    - :debugging: Only applicable for test-net sampling. Defines if the sampling process should be quiet with no terminal output (FALSE) or if process updates are to be shown (TRUE) (`bool`)
+
+    :bnb: Use alternative branch-and-bound sampling when in mainnet=False (`bool`)
+
+    :Returns:
+
+    - Returns a dimod sampleset object class:`dimod.sampleset`
+    
+    :Example:
+
+    .. code-block:: Python
+
+        from pyqubo import Array
+        N = 15
+        K = 3
+        numbers = [4.8097315016016315, 4.325157567810298, 2.9877429101815127,
+                   3.199880179616316, 0.5787939511978596, 1.2520928214246918,
+                   2.262867466401502, 1.2300003067401255, 2.1601079352817925,
+                   3.63753899583021, 4.598232793833491, 2.6215815162575646,
+                   3.4227134835783364, 0.28254151584552023, 4.2548151473817075]
+
+        q = Array.create('q', N, 'BINARY')
+        H = sum(numbers[i] * q[i] for i in range(N)) + 5.0 * (sum(q) - K)**2
+        model = H.compile()
+        Q, offset = model.to_qubo(index_label=True)
+        sampleset = dynex.sample_qubo(Q, offset, formula=2, annealing_time=200, bnb=True)
+        print(sampleset)
+           0  1  2  3  4  5  6  7  8  9 10 11 12 13 14   energy num_oc.
+        0  0  1  0  0  0  0  0  1  0  0  1  0  0  0  0 2.091336       1
+        ['BINARY', 1 rows, 1 samples, 15 variables]
+    
+    """
+    bqm = dimod.BinaryQuadraticModel.from_qubo(Q, offset)
+    model = BQM(bqm, logging=logging, formula=formula);
+    sampler = DynexSampler(model,  mainnet=mainnet, logging=logging, description=description, bnb=bnb);
+    sampleset = sampler.sample(num_reads=num_reads, annealing_time=annealing_time, clones=clones, switchfraction=switchfraction, alpha=alpha, beta=beta, gamma=gamma, delta=delta, epsilon=epsilon, zeta=zeta, minimum_stepsize=minimum_stepsize, debugging=debugging);
+    return sampleset
+    
+def sample_ising(h, j, logging=True, formula=2, mainnet=False, description='Dynex SDK Job', test=False, bnb=False, num_reads = 32, annealing_time = 10, clones = 1, switchfraction = 0.0, alpha=20, beta=20, gamma=1, delta=1, epsilon=1, zeta=1, minimum_stepsize = 0.00000006, debugging=False):
+    """
+    Samples an Ising problem.
+    
+    :Parameters:
+    
+    - :h: Linear biases of the Ising problem
+    
+    - :j: Quadratic biases of the Ising problem
+    
+    - :logging: Defines if the sampling process should be quiet with no terminal output (FALSE) or if process updates are to be shown (`bool`)
+    
+    - :mainnet: Defines if the mainnet (Dynex platform sampling) or the testnet (local sampling) is being used for sampling (`bool`)
+    
+    - :description: Defines the description for the sampling, which is shown in Dynex job dashboards as well as in the market place  (`string`)
+    
+    - :num_reads: Defines the number of parallel samples to be performed (`int` value in the range of [32, MAX_NUM_READS] as defined in your license)
+
+    - :annealing_time: Defines the number of integration steps for the sampling. Models are being converted into neuromorphic circuits, which are then simulated with ODE integration by the participating workers (`int` value in the range of [1, MAX_ANNEALING_TIME] as defined in your license)
+        
+    - :clones: Defines the number of clones being used for sampling. Default value is 1 which means that no clones are being sampled. Especially when all requested num_reads will fit on one worker, it is desired to also retrieve the optimum ground states found from more than just one worker. The number of clones runs the sampler for n clones in parallel and aggregates the samples. This ensures a broader spectrum of retrieved samples. Please note, it the number of clones is set higher than the number of available threads on your local machine, then the number of clones processed in parallel is being processed in batches. Clone sampling is only available when sampling on the mainnet. (`integer` value in the range of [1,128])
+
+    - :switchfraction: Defines the percentage of variables which are replaced by random values during warm start samplings (`double` in the range of [0.0, 1.0])
+
+    - :alpha: The ODE integration of the QUBU/Ising or SAT model based neuromorphic circuits is using automatic tuning of these parameters for the ODE integration. Setting values defines the upper bound for the automated parameter tuning (`double` value in the range of [0.00000001, 100.0] for alpha and beta, and [0.0 and 1.0] for gamma, delta and epsilon)
+
+    - :beta: The ODE integration of the QUBU/Ising or SAT model based neuromorphic circuits is using automatic tuning of these parameters for the ODE integration. Setting values defines the upper bound for the automated parameter tuning (`double` value in the range of [0.00000001, 100.0] for alpha and beta, and [0.0 and 1.0] for gamma, delta and epsilon)
+
+    - :gamma: The ODE integration of the QUBU/Ising or SAT model based neuromorphic circuits is using automatic tuning of these parameters for the ODE integration. Setting values defines the upper bound for the automated parameter tuning (`double` value in the range of [0.00000001, 100.0] for alpha and beta, and [0.0 and 1.0] for gamma, delta and epsilon)
+
+    - :delta: The ODE integration of the QUBU/Ising or SAT model based neuromorphic circuits is using automatic tuning of these parameters for the ODE integration. Setting values defines the upper bound for the automated parameter tuning (`double` value in the range of [0.00000001, 100.0] for alpha and beta, and [0.0 and 1.0] for gamma, delta and epsilon)
+
+    - :epsilon: The ODE integration of the QUBU/Ising or SAT model based neuromorphic circuits is using automatic tuning of these parameters for the ODE integration. Setting values defines the upper bound for the automated parameter tuning (`double` value in the range of [0.00000001, 100.0] for alpha and beta, and [0.0 and 1.0] for gamma, delta and epsilon)
+
+    - :zeta: The ODE integration of the QUBU/Ising or SAT model based neuromorphic circuits is using automatic tuning of these parameters for the ODE integration. Setting values defines the upper bound for the automated parameter tuning (`double` value in the range of [0.00000001, 100.0] for alpha and beta, and [0.0 and 1.0] for gamma, delta and epsilon)
+
+    - :minimum_stepsize: The ODE integration of the QUBU/Ising or SAT model based neuromorphic circuits is performig adaptive stepsizes for each ODE integration forward Euler step. This value defines the smallest step size for a single adaptive integration step (`double` value in the range of [0.0000000000000001, 1.0])
+
+    - :debugging: Only applicable for test-net sampling. Defines if the sampling process should be quiet with no terminal output (FALSE) or if process updates are to be shown (TRUE) (`bool`)
+
+    :bnb: Use alternative branch-and-bound sampling when in mainnet=False (`bool`)
+
+    :Returns:
+
+    - Returns a dimod sampleset object class:`dimod.sampleset`
+    
+    """
+    bqm = dimod.BinaryQuadraticModel.from_ising(h, j)
+    model = BQM(bqm, logging=logging, formula=formula);
+    sampler = DynexSampler(model,  mainnet=mainnet, logging=logging, description=description, bnb=bnb);
+    sampleset = sampler.sample(num_reads=num_reads, annealing_time=annealing_time, clones=clones, switchfraction=switchfraction, alpha=alpha, beta=beta, gamma=gamma, delta=delta, epsilon=epsilon, zeta=zeta, minimum_stepsize=minimum_stepsize, debugging=debugging);#
+    return sampleset
+
+def sample(bqm, logging=True, formula=2, mainnet=False, description='Dynex SDK Job', test=False, bnb=False, num_reads = 32, annealing_time = 10, clones = 1, switchfraction = 0.0, alpha=20, beta=20, gamma=1, delta=1, epsilon=1, zeta=1, minimum_stepsize = 0.00000006, debugging=False):
+    """
+    Samples a Binary Quadratic Model (bqm).
+    
+    :Parameters:
+    
+    - :bqm: Binary quadratic model to sample
+    
+    - :logging: Defines if the sampling process should be quiet with no terminal output (FALSE) or if process updates are to be shown (`bool`)
+    
+    - :mainnet: Defines if the mainnet (Dynex platform sampling) or the testnet (local sampling) is being used for sampling (`bool`)
+    
+    - :description: Defines the description for the sampling, which is shown in Dynex job dashboards as well as in the market place  (`string`)
+    
+    - :num_reads: Defines the number of parallel samples to be performed (`int` value in the range of [32, MAX_NUM_READS] as defined in your license)
+
+    - :annealing_time: Defines the number of integration steps for the sampling. Models are being converted into neuromorphic circuits, which are then simulated with ODE integration by the participating workers (`int` value in the range of [1, MAX_ANNEALING_TIME] as defined in your license)
+        
+    - :clones: Defines the number of clones being used for sampling. Default value is 1 which means that no clones are being sampled. Especially when all requested num_reads will fit on one worker, it is desired to also retrieve the optimum ground states found from more than just one worker. The number of clones runs the sampler for n clones in parallel and aggregates the samples. This ensures a broader spectrum of retrieved samples. Please note, it the number of clones is set higher than the number of available threads on your local machine, then the number of clones processed in parallel is being processed in batches. Clone sampling is only available when sampling on the mainnet. (`integer` value in the range of [1,128])
+
+    - :switchfraction: Defines the percentage of variables which are replaced by random values during warm start samplings (`double` in the range of [0.0, 1.0])
+
+    - :alpha: The ODE integration of the QUBU/Ising or SAT model based neuromorphic circuits is using automatic tuning of these parameters for the ODE integration. Setting values defines the upper bound for the automated parameter tuning (`double` value in the range of [0.00000001, 100.0] for alpha and beta, and [0.0 and 1.0] for gamma, delta and epsilon)
+
+    - :beta: The ODE integration of the QUBU/Ising or SAT model based neuromorphic circuits is using automatic tuning of these parameters for the ODE integration. Setting values defines the upper bound for the automated parameter tuning (`double` value in the range of [0.00000001, 100.0] for alpha and beta, and [0.0 and 1.0] for gamma, delta and epsilon)
+
+    - :gamma: The ODE integration of the QUBU/Ising or SAT model based neuromorphic circuits is using automatic tuning of these parameters for the ODE integration. Setting values defines the upper bound for the automated parameter tuning (`double` value in the range of [0.00000001, 100.0] for alpha and beta, and [0.0 and 1.0] for gamma, delta and epsilon)
+
+    - :delta: The ODE integration of the QUBU/Ising or SAT model based neuromorphic circuits is using automatic tuning of these parameters for the ODE integration. Setting values defines the upper bound for the automated parameter tuning (`double` value in the range of [0.00000001, 100.0] for alpha and beta, and [0.0 and 1.0] for gamma, delta and epsilon)
+
+    - :epsilon: The ODE integration of the QUBU/Ising or SAT model based neuromorphic circuits is using automatic tuning of these parameters for the ODE integration. Setting values defines the upper bound for the automated parameter tuning (`double` value in the range of [0.00000001, 100.0] for alpha and beta, and [0.0 and 1.0] for gamma, delta and epsilon)
+
+    - :zeta: The ODE integration of the QUBU/Ising or SAT model based neuromorphic circuits is using automatic tuning of these parameters for the ODE integration. Setting values defines the upper bound for the automated parameter tuning (`double` value in the range of [0.00000001, 100.0] for alpha and beta, and [0.0 and 1.0] for gamma, delta and epsilon)
+
+    - :minimum_stepsize: The ODE integration of the QUBU/Ising or SAT model based neuromorphic circuits is performig adaptive stepsizes for each ODE integration forward Euler step. This value defines the smallest step size for a single adaptive integration step (`double` value in the range of [0.0000000000000001, 1.0])
+
+    - :debugging: Only applicable for test-net sampling. Defines if the sampling process should be quiet with no terminal output (FALSE) or if process updates are to be shown (TRUE) (`bool`)
+
+    :bnb: Use alternative branch-and-bound sampling when in mainnet=False (`bool`)
+
+    :Returns:
+
+    - Returns a dimod sampleset object class:`dimod.sampleset`
+    
+    :Example:
+
+    .. code-block:: Python
+
+        from pyqubo import Array
+        N = 15
+        K = 3
+        numbers = [4.8097315016016315, 4.325157567810298, 2.9877429101815127,
+                   3.199880179616316, 0.5787939511978596, 1.2520928214246918,
+                   2.262867466401502, 1.2300003067401255, 2.1601079352817925,
+                   3.63753899583021, 4.598232793833491, 2.6215815162575646,
+                   3.4227134835783364, 0.28254151584552023, 4.2548151473817075]
+
+        q = Array.create('q', N, 'BINARY')
+        H = sum(numbers[i] * q[i] for i in range(N)) + 5.0 * (sum(q) - K)**2
+        model = H.compile()
+        Q, offset = model.to_qubo(index_label=True)
+        bqm = dimod.BinaryQuadraticModel.from_qubo(Q, offset)
+        sampleset = dynex.sample(bqm, offset, formula=2, annealing_time=200, bnb=True)
+        print(sampleset)
+           0  1  2  3  4  5  6  7  8  9 10 11 12 13 14   energy num_oc.
+        0  0  1  0  0  0  0  0  1  0  0  1  0  0  0  0 2.091336       1
+        ['BINARY', 1 rows, 1 samples, 15 variables]
+    
+    """
+    model = BQM(bqm, logging=logging, formula=formula);
+    sampler = DynexSampler(model,  mainnet=mainnet, logging=logging, description=description, bnb=bnb);
+    sampleset = sampler.sample(num_reads=num_reads, annealing_time=annealing_time, clones=clones, switchfraction=switchfraction, alpha=alpha, beta=beta, gamma=gamma, delta=delta, epsilon=epsilon, zeta=zeta, minimum_stepsize=minimum_stepsize, debugging=debugging);
+    return sampleset
+
         
 ################################################################################################################################
 # Dynex Sampler (public class)
 ################################################################################################################################
 class DynexSampler:
     """
     Initialises the sampler object given a model.
@@ -965,15 +1235,15 @@
     :Example:
 
     .. code-block:: Python
 
         sampler = dynex.DynexSampler(model)
 
     """
-    def __init__(self, model, logging=True, mainnet=True, description='Dynex SDK Job', test=False):
+    def __init__(self, model, logging=True, mainnet=True, description='Dynex SDK Job', test=False, bnb=False):
         
         # multi-model parallel sampling
         if isinstance(model, list):
             if mainnet==False:
                 raise Exception("[ÐYNEX] ERROR: Multi model parallel sampling is only supported on mainnet");
             if logging:
                 print("[ÐYNEX] MULTI-MODEL PARALLEL SAMPLING:",len(model),'MODELS');
@@ -981,14 +1251,15 @@
         self.state = 'initialised';
         self.model = model;
         self.logging = logging;
         self.mainnet = mainnet;
         self.description = description;
         self.test = test;
         self.dimod_assignments = {};
+        self.bnb = bnb; 
         
     def sample(self, num_reads = 32, annealing_time = 10, clones = 1, switchfraction = 0.0, alpha=20, beta=20, gamma=1, delta=1, epsilon=1, zeta=1, minimum_stepsize = 0.00000006, debugging=False):
         """
         The main sampling function:
 
         :Parameters:
 
@@ -1012,14 +1283,16 @@
 
         - :zeta: The ODE integration of the QUBU/Ising or SAT model based neuromorphic circuits is using automatic tuning of these parameters for the ODE integration. Setting values defines the upper bound for the automated parameter tuning (`double` value in the range of [0.00000001, 100.0] for alpha and beta, and [0.0 and 1.0] for gamma, delta and epsilon)
 
         - :minimum_stepsize: The ODE integration of the QUBU/Ising or SAT model based neuromorphic circuits is performig adaptive stepsizes for each ODE integration forward Euler step. This value defines the smallest step size for a single adaptive integration step (`double` value in the range of [0.0000000000000001, 1.0])
 
         - :debugging: Only applicable for test-net sampling. Defines if the sampling process should be quiet with no terminal output (FALSE) or if process updates are to be shown (TRUE) (`bool`)
 
+         :bnb: Use alternative branch-and-bound sampling when in mainnet=False (`bool`)
+
         :Returns:
 
         - Returns a dimod sampleset object class:`dimod.sampleset`
 
         :Example:
 
         .. code-block:: 
@@ -1067,15 +1340,15 @@
         if clones > 128:
             raise Exception("[DYNEX] ERROR: Value of clones must be in range [1,128]");
         if self.mainnet==False and clones > 1:
             raise Exception("[DYNEX] ERROR: Clone sampling is only supported on the mainnet");
         
         # sampling without clones: -------------------------------------------------------------------------------------------
         if clones == 1:
-            _sampler = _DynexSampler(self.model, self.logging, self.mainnet, self.description, self.test);
+            _sampler = _DynexSampler(self.model, self.logging, self.mainnet, self.description, self.test, self.bnb);
             _sampleset = _sampler.sample(num_reads, annealing_time, switchfraction, alpha, beta, gamma, delta, epsilon, zeta, minimum_stepsize, debugging);
             return _sampleset;
         
         # sampling with clones: ----------------------------------------------------------------------------------------------
         else:
             supported_threads = _getCoreCount() * 2;
             if clones > supported_threads:
@@ -1127,15 +1400,15 @@
 # Dynex Sampler class (private)
 ################################################################################################################################
 
 class _DynexSampler:
     """
     `Internal Class` which is called by public class `DynexSampler`
     """
-    def __init__(self, model, logging=True, mainnet=True, description='Dynex SDK Job', test=False):
+    def __init__(self, model, logging=True, mainnet=True, description='Dynex SDK Job', test=False, bnb=False):
         
         if not test and not _test_completed():
             raise Exception("CONFIGURATION TEST NOT COMPLETED. PLEASE RUN 'dynex.test()'");
         
         self.description = description;
 
         # parse config file:
@@ -1163,14 +1436,15 @@
         with open(tmppath, 'w') as f:
             f.write('0123456789ABCDEF')
         self.filepath = 'tmp/'
         self.filepath_full = os.getcwd()+'/tmp'
 
         # path to testnet
         self.solverpath = 'testnet/';
+        self.bnb = bnb;
 
         # multi-model parallel sampling?
         multi_model_mode = False;
         if isinstance(model, list):
             if mainnet == False:
                 raise Exception("[ÐYNEX] ERROR: Multi model parallel sampling is only supported on mainnet");
             multi_model_mode = True;
@@ -1352,14 +1626,83 @@
         except Exception as e:
             print(f"[DYNEX] An error occurred while sending the file: {str(e)}")
             raise Exception("ERROR: An error occurred while sending the file");
             retval = False;
         finally:
             ftp.quit();
         return retval;
+
+    # calculate ground state energy and numer of falsified softs from model ==========================================================
+    def _energy(self, sample, mapping=True):
+        """
+        `Internal Function`
+        
+        Takes a model and dimod samples and calculates the energy and loc.
+        
+        Input: 
+        ======
+        
+        - dimod sample (dict) with mapping = True
+          example: {0: 0, 1: 0, 2: 0, 3: 0, 4: 0, 5: 0, 6: 0, 7: 0, 8: 0, 9: 0, 10: 0, 11: 0, 12: 0, 13: 0, 14: 0}
+          
+        or
+          
+        - assignments (list) with mapping = False (raw solution file)
+          example: [1, 1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, 1, -1, -1]
+        """
+        # convert dimod sample to wcnf mapping:
+        wcnf_vars = []; 
+        if mapping:
+            for v in sample:
+                if v in self.model.var_mappings:
+                    v_mapped = self.model.var_mappings[v];
+                else:
+                    v_mapped = v;
+                wcnf_vars.append(sample[v_mapped])
+        # or convert solution file to 0/1:
+        else:
+            for v in sample:
+                if v>0:
+                    wcnf_vars.append(1);
+                else:
+                    wcnf_vars.append(0);
+            
+        loc = 0;
+        energy = 0.0;
+        for clause in self.model.clauses:
+            
+            if len(clause)==2:
+                # 2-lit clause:
+                w = clause[0];
+                i = abs(clause[1]);
+                i_dir = np.sign(clause[1]);
+                if i_dir == -1:
+                    i_dir = 0;
+                i_assign = wcnf_vars[i-1];
+                if (i_dir != i_assign):
+                    loc += 1;
+                    energy += w;
+            else:
+                # 3-lit clause:
+                w = clause[0];
+                i = abs(clause[1]);
+                i_dir = np.sign(clause[1]);
+                if i_dir == -1:
+                    i_dir = 0;
+                i_assign = wcnf_vars[i-1];
+                j = abs(clause[2]);
+                j_dir = np.sign(clause[2]);
+                if j_dir == -1:
+                    j_dir = 0;
+                j_assign = wcnf_vars[j-1];
+                if (i_dir != i_assign) and (j_dir != j_assign):
+                    loc += 1;
+                    energy += w;
+                
+        return loc, energy
             
     # list local available (downloaded) iles in /tmp =================================================================================
     def list_files_with_text_local(self):
         """
         `Internal Function`
 
         Scans the temporary directory for assignment files
@@ -1379,15 +1722,15 @@
             if filename.startswith(fn):
                 if os.path.getsize(directory+'/'+filename)>0:
                     filtered_files.append(filename)
 
         return filtered_files; 
     
     # verify correctness of downloaded file (loc and energy) ==========================================================================
-    def validate_file(self, file):
+    def validate_file(self, file, debugging=False):
         """
         `Internal Function`
         
         Validates loc and energy provided in filename with voltages. File not matching will be deleted on FTP and locally.
         """
         valid = False;
         
@@ -1415,28 +1758,38 @@
                 else:
                     voltages = ['NaN']; # invalid file received
             else: # test-net is not returning wallet
                 voltages = data.split(", ")[:-1];
                 
             # convert string voltages to list of floats:
             voltages = list(map(float, voltages));
+            if debugging:
+                print('DEBUG:');
+                print(voltages);
 
             # valid result? ignore Nan values and other incorrect data
             if len(voltages)>0 and voltages[0] != 'NaN' and self.num_variables == len(voltages):
-                val_loc, val_energy = _energy(self.model, voltages, mapping=False);
+                val_loc, val_energy = self._energy(voltages, mapping=False);
                 
                 # from later versions onwards, enforce also correctness of LOC (TBD):
                 if energy == val_energy:
                     valid = True;
+
+                if debugging:
+                    print('DEBUG:',self.filename,chips,steps,loc,energy,'=>',val_loc, val_energy, 'valid?',valid);
+
+            else:
+                if debugging:
+                    print('DEBUG:',self.filename,' NaN or num_variables =',len(voltages),' vs ',self.num_variables, 'valid?',valid);
                         
         return valid;
         
 
     # list and download solution files ================================================================================================
-    def list_files_with_text(self):
+    def list_files_with_text(self, debugging=False):
         """
         `Internal Function`
 
         Downloads assignment files from the FTP server specified in dynex.ini and stores them in /tmp as specified in dynex.ini
         Downloaded files are automatically deleted on the FTP server.
 
         :Returns:
@@ -1464,15 +1817,15 @@
                     # download file if not already local:
                     local_path = self.filepath+name;
                     if os.path.isfile(local_path)==False or os.path.getsize(local_path)==0:
                         with open(local_path, 'wb') as file:
                             ftp.retrbinary('RETR ' + name, file.write); 
                             file.close();
                         # correct file?
-                        if self.validate_file(name)==False:
+                        if self.validate_file(name, debugging)==False:
                             if self.logging:
                                 print('[DYNEX] REMOVING SOLUTION FILE',name,'(WRONG ENERGY REPORTED OR INCORRECT VOLTAGES)');
                             os.remove(local_path);
                             ftp.delete(name);
                         else:
                             # correctly downloaded?
                             cnt = 0;
@@ -1480,15 +1833,15 @@
                                 time.sleep(1);
                                 with open(local_path, 'wb') as file:
                                     if self.logging:
                                         print('[DYNEX] REDOWNLOADING FILE',name);
                                     ftp.retrbinary('RETR ' + name, file.write);
                                     file.close();
                                 # correct file?
-                                if self.validate_file(name) == False:
+                                if self.validate_file(name, debugging) == False:
                                     if self.logging:
                                         print('[DYNEX] REMOVING SOLUTION FILE',name,'(WRONG ENERGY REPORTED OR INCORRECT VOLTAGES)');
                                     os.remove(local_path);
                                     break;
                                 cnt += 1;
                                 if cnt>=10:
                                     break;
@@ -1692,32 +2045,35 @@
             else:
                 # run on test-net:
                 if self.type == 'wcnf':
                     localtype = 5;
                 if self.type == 'cnf':
                     localtype = 0;
                 JOB_ID = -1;
-                #command = self.solverpath+"np -t="+str(localtype)+" -ms="+str(annealing_time)+" -st=1 -msz="+str(minimum_stepsize)+" -c="+str(num_reads)+" --file='"+self.filepath_full+"/"+self.filename+"'";
-                # in test-net, we use the maximum fitting chips:
+                command = self.solverpath+"np -t="+str(localtype)+" -ms="+str(annealing_time)+" -st=1 -msz="+str(minimum_stepsize)+" -c="+str(num_reads)+" --file='"+self.filepath_full+"/"+self.filename+"'";
+                # in test-net, it cannot guaranteed that all requested chips are fitting:
                 num_reads = 0;
-                command = self.solverpath+"np -t="+str(localtype)+" -ms="+str(annealing_time)+" -st=1 -msz="+str(minimum_stepsize)+" --file='"+self.filepath_full+"/"+self.filename+"'";
-
+                
                 if alpha!=0:
                     command = command + " --alpha=" + str(alpha);
                 if beta!=0:
                     command = command + " --beta=" + str(beta);
                 if gamma!=0:
                     command = command + " --gamma=" + str(gamma);
                 if delta!=0:
                     command = command + " --delta=" + str(delta);
                 if epsilon!=0:
                     command = command + " --epsilon=" + str(epsilon);
                 if zeta!=0:
                     command = command + " --zeta=" + str(zeta);
 
+                # use branch-and-bound (testnet) sampler instead?:
+                if self.bnb:
+                    command = self.solverpath+"dynex-testnet-bnb "+self.filepath_full+"/"+self.filename;
+                
                 process = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE)
                 if debugging:
                     for c in iter(lambda: process.stdout.read(1), b""):
                         sys.stdout.write(c.decode('utf-8'))
                 else:
                     if self.logging:
                     	print("[DYNEX|TESTNET] *** WAITING FOR READS ***");
@@ -1734,15 +2090,15 @@
                 total_steps = 0;
                 lowest_energy = 1.7976931348623158e+308;
                 lowest_loc = 1.7976931348623158e+308;
 
                 # retrieve solutions
                 if mainnet:
                     try:
-                        files = self.list_files_with_text();
+                        files = self.list_files_with_text(debugging);
                         cnt_workers = len(files);
                     except Exception as e:
                         print('[DYNEX] CONNECTION TO FTP ENDPOINT FAILED:',e);
                         raise Exception('ERROR: CONNECTION TO FTP ENDPOINT FAILED')
                         files = []; 
                 else:
                     files = self.list_files_with_text_local(); 
@@ -1767,15 +2123,15 @@
                     if self.type=='cnf' and loc == 0:
                         finished = True;
                     if total_chips >= num_reads*0.90:
                         finished = True;
 
                 if cnt_workers<1:
                     if self.logging:
-                        if mainnet:
+                        if mainnet and debugging==False:
                             clear_output(wait=True);
                         if mainnet:
                             LOC_MIN, ENERGY_MIN, MALLOB_CHIPS, details = _get_status_details_api(JOB_ID);
                         else:
                             LOC_MIN, ENERGY_MIN, MALLOB_CHIPS = 0,0,0;
                             details = "";
                         elapsed_time = time.process_time() - t;
@@ -1785,15 +2141,15 @@
                         ta = tabulate(table, headers="firstrow", tablefmt='rounded_grid', floatfmt=".2f");
                         print(ta+'\n'+details);
                         
                     time.sleep(2); 
 
                 else:
                     if self.logging:
-                        if mainnet:
+                        if mainnet and debugging==False:
                             clear_output(wait=True);
                         if mainnet:
                             LOC_MIN, ENERGY_MIN, MALLOB_CHIPS, details = _get_status_details_api(JOB_ID);
                         else:
                             LOC_MIN, ENERGY_MIN, MALLOB_CHIPS = 0,0,0;
                             details = "";
                         elapsed_time = time.process_time() - t;
@@ -1812,15 +2168,15 @@
 
             # update mallob - job finished: -------------------------------------------------------------------------------------------------
             if mainnet:
                 _update_job_api(JOB_ID, 2, self.logging, workers=cnt_workers, lowest_loc=lowest_loc, lowest_energy=lowest_energy);
 
             # update final output (display all workers as stopped as well):
             if cnt_workers>0 and self.logging:
-                if mainnet:
+                if mainnet and debugging==False:
                     clear_output(wait=True);
                 if mainnet:
                     LOC_MIN, ENERGY_MIN, MALLOB_CHIPS, details = _get_status_details_api(JOB_ID, all_stopped = True);
                 else:
                     LOC_MIN, ENERGY_MIN, MALLOB_CHIPS = 0,0,0;
                     details = "";
                 elapsed_time = time.process_time() - t;
```

### Comparing `dynex-0.1.8/dynex.egg-info/PKG-INFO` & `dynex-0.1.9/dynex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dynex
-Version: 0.1.8
+Version: 0.1.9
 Summary: Dynex SDK Neuromorphic Computing
 Home-page: https://github.com/dynexcoin/DynexSDK
 Author: Dynex Developers
 Author-email: office@dynexcoin.org
 License: GPLv3
 Description: The Dynex SDK provides a neuromorphic Ising/QUBO sampler which can be called from any Python code. Developers and application developers already familiar with the Dimod framework, PyQUBO or the Ocean SDK will find it very easy to run computations on the Dynex neuromorphic computing platform: The Dynex Sampler object can simply replace the default sampler object which typically is used to run computations on, for example, the D-Wave system – without the limitations of quantum machines. The Dynex SDK is a suite of open-source Python tools for solving hard problems with neuromorphic computing which helps reformulate your application’s problem for solution by the Dynex computing platform. It also handles communication between your application code and the Dynex neuromorphic computing platform automatically.
 Platform: UNKNOWN
```

### Comparing `dynex-0.1.8/setup.py` & `dynex-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='dynex',
-    version='0.1.8',    
+    version='0.1.9',    
     description='Dynex SDK Neuromorphic Computing',
     url='https://github.com/dynexcoin/DynexSDK',
     author='Dynex Developers',
     author_email='office@dynexcoin.org',
     license='GPLv3',
     packages=['dynex'],
     install_requires=['pycryptodome>=3.18.0',
```

