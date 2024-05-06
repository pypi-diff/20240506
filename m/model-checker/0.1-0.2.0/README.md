# Comparing `tmp/model_checker-0.1.tar.gz` & `tmp/model_checker-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_checker-0.1.tar", last modified: Fri Apr 26 20:37:06 2024, max compression
+gzip compressed data, was "model_checker-0.2.0.tar", last modified: Mon May  6 18:44:13 2024, max compression
```

## Comparing `model_checker-0.1.tar` & `model_checker-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-04-26 20:37:06.013812 model_checker-0.1/
--rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-04-26 19:58:45.000000 model_checker-0.1/LICENCE
--rw-r--r--   0 benjamin  (1000) users      (100)      670 2024-04-26 20:37:06.013812 model_checker-0.1/PKG-INFO
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-04-26 20:37:06.013812 model_checker-0.1/model_checker.egg-info/
--rw-r--r--   0 benjamin  (1000) users      (100)      670 2024-04-26 20:37:06.000000 model_checker-0.1/model_checker.egg-info/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)      346 2024-04-26 20:37:06.000000 model_checker-0.1/model_checker.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-04-26 20:37:06.000000 model_checker-0.1/model_checker.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-04-26 20:37:06.000000 model_checker-0.1/model_checker.egg-info/requires.txt
--rw-r--r--   0 benjamin  (1000) users      (100)        8 2024-04-26 20:37:06.000000 model_checker-0.1/model_checker.egg-info/top_level.txt
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-04-26 20:37:06.013812 model_checker-0.1/package/
--rw-r--r--   0 benjamin  (1000) users      (100)        0 2024-04-26 20:11:38.000000 model_checker-0.1/package/__init__.py
--rw-r--r--   0 benjamin  (1000) users      (100)    10290 2024-04-26 20:11:38.000000 model_checker-0.1/package/model_definitions.py
--rw-r--r--   0 benjamin  (1000) users      (100)    19408 2024-04-26 20:11:38.000000 model_checker-0.1/package/model_structure.py
--rw-r--r--   0 benjamin  (1000) users      (100)    19261 2024-04-26 20:11:38.000000 model_checker-0.1/package/semantics.py
--rw-r--r--   0 benjamin  (1000) users      (100)     6776 2024-04-26 20:11:38.000000 model_checker-0.1/package/syntax.py
--rw-r--r--   0 benjamin  (1000) users      (100)     3932 2024-04-26 20:15:00.000000 model_checker-0.1/package/test_complete.py
--rw-r--r--   0 benjamin  (1000) users      (100)      816 2024-04-26 20:10:17.000000 model_checker-0.1/pyproject.toml
--rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-04-26 20:37:06.013812 model_checker-0.1/setup.cfg
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 18:44:13.723148 model_checker-0.2.0/
+-rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-04-26 19:58:45.000000 model_checker-0.2.0/LICENCE
+-rw-r--r--   0 benjamin  (1000) users      (100)      673 2024-05-06 18:44:13.723148 model_checker-0.2.0/PKG-INFO
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 18:44:13.723148 model_checker-0.2.0/model_checker.egg-info/
+-rw-r--r--   0 benjamin  (1000) users      (100)      673 2024-05-06 18:44:13.000000 model_checker-0.2.0/model_checker.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)      402 2024-05-06 18:44:13.000000 model_checker-0.2.0/model_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-06 18:44:13.000000 model_checker-0.2.0/model_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-06 18:44:13.000000 model_checker-0.2.0/model_checker.egg-info/requires.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)        8 2024-05-06 18:44:13.000000 model_checker-0.2.0/model_checker.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 18:44:13.723148 model_checker-0.2.0/package/
+-rw-r--r--   0 benjamin  (1000) users      (100)      647 2024-04-28 01:38:31.000000 model_checker-0.2.0/package/__init__.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     5918 2024-05-06 18:32:01.000000 model_checker-0.2.0/package/examples.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    16022 2024-05-06 17:49:27.000000 model_checker-0.2.0/package/model_definitions.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    34588 2024-05-06 18:33:23.000000 model_checker-0.2.0/package/model_structure.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    19659 2024-05-04 18:05:09.000000 model_checker-0.2.0/package/semantics.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     7265 2024-05-03 14:48:57.000000 model_checker-0.2.0/package/syntax.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     5338 2024-05-06 18:33:30.000000 model_checker-0.2.0/package/test.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     5838 2024-05-02 19:11:05.000000 model_checker-0.2.0/package/test_complete.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     2070 2024-05-03 17:30:50.000000 model_checker-0.2.0/package/top_test.py
+-rw-r--r--   0 benjamin  (1000) users      (100)      819 2024-05-06 18:35:36.000000 model_checker-0.2.0/pyproject.toml
+-rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-06 18:44:13.723148 model_checker-0.2.0/setup.cfg
```

### Comparing `model_checker-0.1/LICENCE` & `model_checker-0.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `model_checker-0.1/PKG-INFO` & `model_checker-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: model_checker
-Version: 0.1
+Version: 0.2.0
 Summary: A hyperintensional model checker for counterfactual conditionals
-Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mfbuit46@mit.edu>
+Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
 Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
 Keywords: semantics,Z3,counterfactuals,model checker
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `model_checker-0.1/model_checker.egg-info/PKG-INFO` & `model_checker-0.2.0/model_checker.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: model_checker
-Version: 0.1
+Version: 0.2.0
 Summary: A hyperintensional model checker for counterfactual conditionals
-Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mfbuit46@mit.edu>
+Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
 Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
 Keywords: semantics,Z3,counterfactuals,model checker
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `model_checker-0.1/package/semantics.py` & `model_checker-0.2.0/package/semantics.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """
 contains all semantic functions
+this file defines the functions needed to generate Z3 constraints from
+input_sentences in infix form.
 """
 
 from z3 import (
     sat,
     Exists,
     ForAll,
     Implies,
@@ -13,19 +15,14 @@
     And,
     BitVec,
 )
 from syntax import Prefix
 
 # from sympy import symbols, Or, And, Implies, Not, to_cnf
 
-"""
-this file defines the functions needed to generate Z3 constraints from
-input_sentences in infix form.
-"""
-
 # def bit_vec_length():
 #     from test_complete import N
 #     return N
 # N = bit_vec_length()
 
 
 # NOTE: we used to have it where we declared a fixed set of variables.
@@ -35,63 +32,80 @@
 # x, y, z = BitVecs("x y z", N)
 
 # NOTE: variables are now declared inside each function where they are used.
 # QUESTIONS: is there a clear reason to prefer one way over the other?
 # is it possible/desirable to avoid use of 'Exists' entirely?
 
 
-def make_constraints(verify, falsify, possible, N, w):
+def make_constraints(verify, falsify, possible, assign, N, w):
+    '''function that makes the function to make the constraints (and list of sentence letters
+    and prefix sentences) This has to be done in order to define N in an input file—you'll see
+    here that N is passed in as a variable to the function, after which these 'make' a semantics
+    with that N (and the other inputs to this function also depend on N)
+    returns a function find_all_constraints that is used to find the constraints, the sentence letters,
+    and prefix sentences.. 
+    '''
     def non_null_verify(bit_s, atom):
-        """bit_s verifies atom and is not the null state"""
+        """bit_s verifies atom and is not the null state
+        returns a Z3 constraint"""
         return And(Not(bit_s == 0), verify(bit_s, atom))
 
     def non_null_falsify(bit_s, atom):
-        """bit_s verifies atom and is not the null state"""
+        """bit_s verifies atom and is not the null state
+        returns a Z3 constraint"""
         return And(Not(bit_s == 0), falsify(bit_s, atom))
 
     def non_triv_verify(bit_s, atom):
-        """bit_s verifies atom and is not the null state"""
+        """bit_s verifies atom and is not the null state
+        returns a Z3 constraint"""
         return And(non_null_verify(bit_s, atom), possible(bit_s))
 
     def non_triv_falsify(bit_s, atom):
-        """bit_s verifies atom and is not the null state"""
+        """bit_s verifies atom and is not the null state
+        returns a Z3 constraint"""
         return And(non_null_falsify(bit_s, atom), possible(bit_s))
 
     def fusion(bit_s, bit_t):
-        """the result of taking the maximum for each index in bit_s and bit_t"""
+        """the result of taking the maximum for each index in bit_s and bit_t
+        returns a Z3 constraint"""
         return bit_s | bit_t
 
     def is_part_of(bit_s, bit_t):
-        """the fusion of bit_s and bit_t is identical to bit_t"""
+        """the fusion of bit_s and bit_t is identical to bit_t
+        returns a Z3 constraint"""
         return fusion(bit_s, bit_t) == bit_t
 
     def compatible(bit_x, bit_y):
-        """the fusion of bit_x and bit_y is possible"""
+        """the fusion of bit_x and bit_y is possible
+        returns a Z3 constraint"""
         return possible(fusion(bit_x, bit_y))
 
     def maximal(bit_w):
-        """bit_w includes all compatible states as parts."""
+        """bit_w includes all compatible states as parts.
+        returns a Z3 constraint"""
         x = BitVec("max_dummy", N)
         return ForAll(
             x,
             Implies(
                 compatible(x, bit_w),
                 is_part_of(x, bit_w),
             ),
         )
 
     def is_world(bit_w):
-        """bit_w is both possible and maximal."""
+        """bit_w is both possible and maximal.
+        returns a Z3 constraint"""
         return And(
             possible(bit_w),
             maximal(bit_w),
         )
 
     def max_compatible_part(bit_x, bit_w, bit_y):
-        """bit_x is the biggest part of bit_w that is compatible with bit_y."""
+        """bit_x is the biggest part of bit_w that is compatible with bit_y.
+        returns a Z3 constraint"""
         z = BitVec("max_part_dummy", N)
         return And(
             is_part_of(bit_x, bit_w),
             compatible(bit_x, bit_y),
             ForAll(
                 z,
                 Implies(
@@ -101,43 +115,47 @@
                     bit_x == z,
                 ),
             ),
         )
 
     def is_alternative(bit_u, bit_y, bit_w):
         """
-        bit_u is a world that is the alternative that results from imposing state bit_y on world bit_w.
+        bit_u is a world that is the alternative that results from imposing state bit_y on
+        world bit_w.
+        returns a Z3 constraint
         """
         z = BitVec("alt_dummy", N)
         return And(
             is_world(bit_u),
             is_part_of(bit_y, bit_u),
             Exists(z, And(is_part_of(z, bit_u), max_compatible_part(z, bit_w, bit_y))),
         )
 
-    # NOTE: should throw error if boxright occurs in X
-    def extended_verify(state, ext_sent, evaluate=False):
-        """X is in prefix form. Same for extended_falsify"""
+    def extended_verify(state, ext_sent): # used to have default var evaluate=False, seems like
+        # it was unnecessary
+        """ext_sent is in prefix form. The state is the state that verifies ext_sent. 
+        evaluate is an optional bool to evaluate something (now unused).
+        returns a Z3 constraint"""
         if len(ext_sent) == 1:
-            # print(state,ext_sent,type(state),type(ext_sent))
             return verify(state, ext_sent[0])
         op = ext_sent[0]
         if "boxright" in op:
             raise ValueError(f"The sentence {ext_sent} is not extensional.")
         if "neg" in op:
             return extended_falsify(state, ext_sent[1])
         Y = ext_sent[1]  # should be a list itself
         Z = ext_sent[2]  # should be a list itself
         if "wedge" in op:
             y = BitVec("ex_ver_dummy_y", N)
             z = BitVec("ex_ver_dummy_z", N)
-            if evaluate is True:
-                return And(
-                    fusion(y, z) == state, extended_verify(y, Y), extended_verify(z, Z)
-                )
+            # if evaluate is True:
+            #     return And(
+            #         fusion(y, z) == state, extended_verify(y, Y), extended_verify(z, Z)
+            #     )
+            # had this in here for some reason. Don't remember why.
             return Exists(
                 [y, z],
                 And(
                     fusion(y, z) == state, extended_verify(y, Y), extended_verify(z, Z)
                 ),
             )
         if "vee" in op:
@@ -158,14 +176,16 @@
                 extended_verify(state, ["wedge", ["neg", Y], Z]),
             )
         raise ValueError(
             f"Something went wrong in extended_verify in evaluating the operator {op} in [{op}, {Y}, {Z}]"
         )
 
     def extended_falsify(state, ext_sent):
+        """ext_sent is in prefix form. The state is the state that falsifies ext_sent. 
+        returns a Z3 constraint"""
         if len(ext_sent) == 1:
             return falsify(state, ext_sent[0])
         op = ext_sent[0]
         if "boxright" in op:
             raise ValueError(f"The sentence {ext_sent} is not extensional.")
         if "neg" in op:
             return extended_verify(state, ext_sent[1])
@@ -175,15 +195,15 @@
             return Or(
                 extended_falsify(state, Y),
                 extended_falsify(state, Z),
                 extended_falsify(state, ["vee", Y, Z]),
             )
         y = BitVec("ex_fal_dummy_y", N)
         z = BitVec("ex_fal_dummy_z", N)
-        # both used in vee and rightarrow cases, but usage is mutually exclusive so can define up here
+        # usage of these two in vee and right arrow is mutually exclusive, so can define uphere
         if "vee" in op:
             return Exists(
                 [y, z],
                 And(
                     state == fusion(y, z),
                     extended_falsify(y, Y),
                     extended_falsify(z, Z),
@@ -204,25 +224,39 @@
         raise ValueError(
             f"Something went wrong in extended_verify in evaluating the operator {op} in [{op}, {Y}, {Z}]"
         )
 
     # NOTE: the true_at/false-at definitions are bilateral to accommodate the fact
     # that the exhaustivity constraint is not included in the definition of props
     # this should avoid the need for specific clauses for (un)negated CFs
-    # TODO: linter says all or none of the returns should be an expression
     def true_at(sentence, world):
-        """sentence is a sentence in prefix notation"""
+        """sentence is a sentence in prefix notation
+        returns a Z3 constraint"""
         x = BitVec("t_dummy_x", N)
         u = BitVec("t_dummy_u", N)
+        y = BitVec("t_dummy_y", N)
         if len(sentence) == 1:
             sent = sentence[0]
+            if 'top' in str(sent)[0]:
+                raise ValueError('This is raised in principle when top is a proposition. @B, what should we do?')
+                # if top is a sentence letter, its constraint is already in the model.
+                # It wouldn't hurt to add it again I think in principle, but if there's something
+                # else that should go here when top is passed in by itself then it would go here
+                # return ForAll(x, And(verify(x, sent),Not(falsify(x, sent)))) # this is the top constraint
             return Exists(x, And(is_part_of(x, world), verify(x, sent)))
         op = sentence[0]
         if "neg" in op:
             return false_at(sentence[1], world)
+        if len(sentence) == 2 and 'Box' in op:
+            return ForAll(u, Implies(is_world(u), true_at(sentence[1], u)))
+            # return ForAll(x, Implies(possible(x), Exists(y, And(extended_verify(y,sentence[1]), compatible(x,y)))))
+        if len(sentence) == 2 and 'Diamond' in op:
+            # print(sentence)
+            return Exists(u, And(is_world(u), true_at(sentence[1], u)))
+            # return Exists(x, And(possible(x), extended_verify(x,sentence[1])))
         Y = sentence[1]
         Z = sentence[2]
         if "wedge" in op:
             return And(true_at(Y, world), true_at(Z, world))
         if "vee" in op:
             return Or(true_at(Y, world), true_at(Z, world))
         if "leftrightarrow" in op:
@@ -236,26 +270,35 @@
             return ForAll(
                 [x, u],
                 Implies(
                     And(extended_verify(x, Y), is_alternative(u, x, world)),
                     true_at(Z, u),
                 ),
             )
+        raise ValueError(f'No if statements triggered— true_at for {sentence} at world {world}')
 
-    # TODO: linter says all or none of the returns should be an expression
     def false_at(sentence, world):
-        """X is a sentence in prefix notation"""
+        """X is a sentence in prefix notation
+        returns a Z3 constraint"""
         x = BitVec("f_dummy_x", N)
         u = BitVec("f_dummy_u", N)
         if len(sentence) == 1:
             sent = sentence[0]
+            # if str(sent) == "\\top":
+            #     return ForAll(x, And(verify(x, sent),Not(falsify(x, sent))))
             return Exists(x, And(is_part_of(x, world), falsify(x, sent)))
         op = sentence[0]
         if "neg" in op:
             return true_at(sentence[1], world)
+        if len(sentence) == 2 and 'Box' in op:
+            # print(sentence)
+            return Exists(u, And(is_world(u), false_at(sentence[1], u)))
+        if len(sentence) == 2 and 'Diamond' in op:
+            # print(sentence)
+            return ForAll(u, Implies(is_world(u), false_at(sentence[1], u)))
         Y = sentence[1]
         Z = sentence[2]
         if "wedge" in op:
             return Or(false_at(Y, world), false_at(Z, world))
         if "vee" in op:
             return And(false_at(Y, world), false_at(Z, world))
         if "leftrightarrow" in op:
@@ -266,76 +309,83 @@
         if "rightarrow" in op:
             return And(true_at(Y, world), false_at(Z, world))
         if "boxright" in op:
             return Exists(
                 [x, u],
                 And(extended_verify(x, Y), is_alternative(u, x, world), false_at(Z, u)),
             )
+        raise ValueError(f'No if statements triggered— false_at for {sentence} at world {world}')
 
     def prop_const(atom):
         """
         atom is a proposition since its verifiers and falsifiers are closed under
         fusion respectively, and the verifiers and falsifiers for atom are
         incompatible (exclusivity). NOTE: exhaustivity crashes Z3 so left off.
+        returns a Z3 constraint for the proposition atom
         """
         x = BitVec("prop_dummy_x", N)
         y = BitVec("prop_dummy_y", N)
         sent_to_prop = [
-            Exists(x, non_triv_verify(x, atom)),
-            Exists(y, non_triv_falsify(y, atom)),
+            Not(verify(0, atom)),
+            Not(falsify(0, atom)),
+            # Exists(x, non_null_verify(x, atom)),
+            # Exists(y, non_null_falsify(y, atom)),
+            # Exists(x, non_triv_verify(x, atom)),
+            # Exists(y, non_triv_falsify(y, atom)),
             ForAll(
                 [x, y],
                 Implies(
                     And(verify(x, atom), verify(y, atom)), verify(fusion(x, y), atom)
                 ),
             ),
             ForAll(
                 [x, y],
                 Implies(
                     And(falsify(x, atom), falsify(y, atom)), falsify(fusion(x, y), atom)
                 ),
             ),
             ForAll(
                 [x, y],
-                Implies(
-                    And(falsify(x, atom), falsify(y, atom)), falsify(fusion(x, y), atom)
-                ),
+                Implies(And(verify(x, atom), falsify(y, atom)), Not(compatible(x, y))),
             ),
             ForAll(
                 [x, y],
-                Implies(And(verify(x, atom), falsify(y, atom)), Not(compatible(x, y))),
+                Implies(
+                    And(possible(x), assign(x, atom) == y),
+                    And(
+                        compatible(x, y),
+                        Or(verify(y, atom), falsify(y, atom)),
+                    ),
+                ),
             ),
-            # ForAll( #exhaustivity
-            #     x,
-            #     Implies(
-            #         possible(x),
-            #         Exists(
-            #             y,
-            #             And(
-            #                 compatible(x,y),
-            #                 Or(verify(y, atom), falsify(y, atom)),
-            #             ),
-            #         ),
-            #     ),
-            # ),
         ]
         return sent_to_prop
 
     def find_frame_constraints():
         """find the constraints that depend only on the sentence letters
         returns a list of Z3 constraints"""
         x = BitVec("frame_dummy_x", N)
         y = BitVec("frame_dummy_y", N)
         z = BitVec("frame_dummy_z", N)
         frame_constraints = [
             ForAll([x, y], Implies(And(possible(y), is_part_of(x, y)), possible(x))),
             ForAll([x, y], Exists(z, fusion(x, y) == z)),
             is_world(w),
         ]
-        return frame_constraints
+        # test_atom = [Const("test_atom", AtomSort)]
+        # test_constraints = [
+        #     Exists(x,
+        #         And(
+        #            is_world(x),
+        #            Not(true_at(test_atom, x)),
+        #            Not(false_at(test_atom, x)),
+        #         )
+        #     ),
+        # ]
+        return frame_constraints # + test_constraints
 
     # def add_general_constraints(solv, input_sentence_letters):
     #     """adds the constraints that go in every solver"""
     #     possible_part = ForAll(
     #         [x, y], Implies(And(possible(y), is_part_of(x, y)), possible(x))
     #     )
     #     solv.add(possible_part)
@@ -351,140 +401,90 @@
     #     for sent_letter in input_sentence_letters:
     #         print(f"\nSentence {sent_letter} yields the general constraints:\n")
     #         for const in prop_const(sent_letter):
     #             solv.add(const)
     #             print(f"{const}\n")
 
     def find_model_constraints(prefix_sents,input_sentence_letters):
-        """find constraints corresponding to the input sentences"""
+        """find constraints corresponding to the input sentences
+        returns a list of Z3 constraints"""
         prop_constraints = []
+        input_constraints = []
         for sent_letter in input_sentence_letters:
-            for const in prop_const(sent_letter):
-                prop_constraints.append(const)
-        input_const = []
+            if 'top' in str(sent_letter):
+                x = BitVec("top_x", N)
+                top_constraint = ForAll(x,
+                    And(
+                        verify(x,sent_letter),
+                        Not(falsify(x,sent_letter))
+                    )
+                )
+                prop_constraints.append(top_constraint)
+                continue
+            for constraint in prop_const(sent_letter):
+                prop_constraints.append(constraint)
         for sentence in prefix_sents:
             sentence_constraint = true_at(sentence, w)
-            input_const.append(sentence_constraint)
-        model_constraints = prop_constraints + input_const
+            input_constraints.append(sentence_constraint)
+        model_constraints = prop_constraints + input_constraints
         return model_constraints
 
     # def add_input_constraints(solv, prefix_sentences):
     #     """add input-specific constraints to the solver"""
     #     for sentence in prefix_sentences:
     #         print(sentence)
     #         sentence_constraint = true_at(sentence, w)
     #         print(
     #             f"Sentence {sentence} yields the model constraint:\n {sentence_constraint}\n"
     #         )
     #         solv.add(sentence_constraint)
 
-    def is_counterfactual(prefix_sentence):
-        """returns a boolean to say whether a given sentence is a counterfactual
-        used in find_extensional_subsentences"""
-        if len(prefix_sentence) == 1:
-            return False
-        if len(prefix_sentence) == 2:
-            return is_counterfactual(prefix_sentence[1])
-        if "boxright" in prefix_sentence[0]:
-            return True
-        return is_counterfactual(prefix_sentence[1]) or is_counterfactual(
-            prefix_sentence[2]
-        )
-
-    # TODO: linter says all or none of the returns should be an expression
-    def all_subsentences_of_a_sentence(prefix_sentence, progress=False):
-        """finds all the subsentence of a prefix sentence
-        returns these as a set
-        used in find_extensional_subsentences"""
-        if progress is False:
-            progress = []
-        # TODO: linter says cannot access member "append" for type "Literal[True]" Member "append" is unknown
-        progress.append(prefix_sentence)
-        if len(prefix_sentence) == 1:
-            return progress
-        if len(prefix_sentence) == 2:
-            # TODO: linter says cannot access member "append" for type "Literal[True]" Member "append" is unknown
-            return all_subsentences_of_a_sentence(prefix_sentence[1], progress)
-        if len(prefix_sentence) == 3:
-            # TODO: linter says cannot access member "append" for type "Literal[True]" Member "append" is unknown
-            left_subsentences = all_subsentences_of_a_sentence(
-                prefix_sentence[1], progress
-            )
-            # TODO: linter says cannot access member "append" for type "Literal[True]" Member "append" is unknown
-            right_subsentences = all_subsentences_of_a_sentence(
-                prefix_sentence[2], progress
-            )
-            all_subsentences = left_subsentences + right_subsentences
-            return all_subsentences
-
-    def find_extensional_subsentences(prefix_sentences):
-        """finds all the extensional subsentences in a list of prefix sentences
-        used in find_all_constraints"""
-        # all_subsentences = [all_subsentences_of_a_sentence(sent) for sent in prefix_sentences]
-        all_subsentences = []
-        for prefix_sent in prefix_sentences:
-            # TODO: linter says cannot access member "append" for type "Literal[True]" Member "append" is unknown
-            all_subsentences.extend(all_subsentences_of_a_sentence(prefix_sent))
-        extensional_subsentences = [
-            sent for sent in all_subsentences if not is_counterfactual(sent)
-        ]
-        return extensional_subsentences
-
-    def repeats_removed(L):
-        """takes a list and removes the repeats in it.
-        used in find_all_constraints"""
-        seen = []
-        for obj in L:
-            if obj not in seen:
-                seen.append(obj)
-        return seen
-
     def sentence_letters_in_compound(prefix_input_sentence):
         """finds all the sentence letters in ONE input sentence. returns a list. WILL HAVE REPEATS
-        used in all_sentence_letters"""
+        used in all_sentence_letters
+        returns a list of AtomSorts. CRUCIAL: IN THAT SENSE DOES NOT FOLLOW SYNTAX OF PREFIX SENTS.
+        But that's ok, just relevant to know"""
         if len(prefix_input_sentence) == 1:  # base case: atomic sentence
             return prefix_input_sentence
-        # recursive case: complex sentence as input. Should have max 3 elems (binary operator) in this list, but figured eh why not not check, above code should ensure that never happens
         return_list = []
         for part in prefix_input_sentence[1:]:
             return_list.extend(sentence_letters_in_compound(part))
         return return_list
 
     def all_sentence_letters(prefix_input_sentences):
-        """finds all the sentence letters in a list of input sentences. returns as a list with no repeats (sorted for consistency)
+        """finds all the sentence letters in a list of input sentences.
+        returns as a list with no repeats (sorted for consistency)
         used in find_all_constraints"""
         sentence_letters = set()
-        for input in prefix_input_sentences:
-            sentence_letters_in_input = sentence_letters_in_compound(input)
+        for prefix_input in prefix_input_sentences:
+            sentence_letters_in_input = sentence_letters_in_compound(prefix_input)
             for sentence_letter in sentence_letters_in_input:
                 sentence_letters.add(sentence_letter)
         return list(sentence_letters)
         # sort just to make every output the same, given sets aren't hashable
 
     def find_all_constraints(infix_input_sentences):
         """find Z3 constraints for input sentences
-        input_sents are a list of infix sentences"""
-        # prefix_premises = [Prefix(input_sent) for input_sent in infix_premises]  # this works
-        # prefix_conclusions = [Prefix(input_sent) for input_sent in infix_conclusions]
-        # prefix_sentences = prefix_combine(prefix_premises, prefix_conclusions)
+        input_sents are a list of infix sentences
+        returns a tuple with all Z3 constraints, for the model, the sentence letters
+        (a list of AtomSorts), and the prefix_sentences (a list of lists, since prefix
+        sentences are lists)"""
         prefix_sentences = [Prefix(input_sent) for input_sent in infix_input_sentences]
         sentence_letters = all_sentence_letters(prefix_sentences)  # this works
         input_const = find_model_constraints(prefix_sentences, sentence_letters)
-        # print(sentence_letters)
-        # print([type(let) for let in sentence_letters])
         gen_const = find_frame_constraints()
         const = gen_const + input_const
-        raw_ext_subsentences = find_extensional_subsentences(prefix_sentences)
-        ext_subsentences = repeats_removed(raw_ext_subsentences)
-        return (const, sentence_letters, ext_subsentences)
+        return (const, sentence_letters, prefix_sentences)
 
     return find_all_constraints
 
 
 def solve_constraints(all_constraints): # all_constraints is a list
-    """find model for the input constraints if there is any"""
+    """find model for the input constraints if there is any
+    returns a tuple with a boolean representing if the constraints were solved or not
+    and, if True, the model, if False the unsatisfiable core of the constraints"""
     solver = Solver()
     solver.add(all_constraints)
     result = solver.check(*[all_constraints])
     if result == sat:
         return (True, solver.model())
     return (False, solver.unsat_core())
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `model_checker-0.1/package/syntax.py` & `model_checker-0.2.0/package/syntax.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-'''
+"""
 file contains all syntactic definitions
 
 NOTES:
 All sentence letters are capital letters.
 All commands must be strictly in lowercase; they can have double backslash, a forward slash, or nothing (nothing so long as the first letter is lowercase).
 The unary operators are defined in a separate set for clarity in the code.
-'''
-import doctest
-from z3 import (
-    Const, DeclareSort
-)
+"""
+from z3 import Const, DeclareSort
 
 
 AtomSort = DeclareSort("AtomSort")
 # sentence_stuff = {'A','B','C','D','E','F','G','H','I','J','K','L','M','N','O','P','Q','R','S','T','U','V','Z','W','Y','Z'}
 # operator_stuff = {'\\','/','a','b','c','d','e','f','g','h','i','j','k','l','m','n','o','p','q','r','s','t','u','v','w','x','y','z'}
-unary_operators = {'\\neg', '/neg', 'neg'}
+unary_operators = {"\\neg", "/neg", "neg", "box", "Box", "\\Box", "\\box", "Diamond", "diamond", "\\diamond", "\\Diamond"}
+
+
 def tokenize(str_exp):
     """
     >>> tokenize("(A /wedge (B /vee C))")
     ['(', 'A', '/wedge', '(', 'B', '/vee', 'C', ')', ')']
 
     >>> tokenize("(/neg A /wedge (B /vee C))")
     ['(', '/neg', 'A', '/wedge', '(', 'B', '/vee', 'C', ')', ')']
@@ -40,15 +39,15 @@
                 tokenized_l = ["("]
                 tokenized_l.extend(tokenize_improved_input([base_string[1:]]))
                 return tokenized_l
             if ")" in base_string:  # right parentheses in base_string
                 tokenized_l = tokenize_improved_input([base_string[:-1]])
                 tokenized_l.append(")")
                 return tokenized_l
-            return split_str # else case: covers sentence letter case and latex operator case
+            return split_str  # else case: covers sentence letter case and latex operator case
         tokenized_l = tokenize_improved_input([split_str[0]])
         tokenized_l.extend(tokenize_improved_input(split_str[1:]))
         return tokenized_l
 
     return tokenize_improved_input(split_str)
 
 
@@ -63,15 +62,14 @@
 
     >>> binary_comp(tokenize('/neg (A /wedge (B /vee C))'))
     2
     """
     return len([char for char in tokenized_expression if char == "("])
 
 
-# TODO: linter says all or none of the returns should be an expression
 def main_op_index(tokenized_expression):
     """
     given an expression with complexity > 0, finds the index of the main operator.
     Starting after the expression's initial parenthesis, the point
     at which the number of left parentheses equals the number of right is the
     first expression (as it is closed there)
     ASSUMES FIRST CHAR IS LEFT PARENTH. IF NOT CASE, EQN PROLLY SHOULDN'T BE HERE
@@ -88,75 +86,95 @@
     7
 
     >>> main_op_index(tokenize('((A \\op (B \\op C)) \\op (D \\op E))'))
     10
     """
     left_parentheses = 0
     right_parentheses = 0
-    if tokenized_expression[0] != '(':
-        raise ValueError(tokenized_expression, 'this case probably shouldnt be being raised by this function')
-    for i, token in enumerate(tokenized_expression[1:]): # [1:] to exclude the left parenth (thus complexity) of the main operator
+    if tokenized_expression[0] != "(":
+        raise ValueError(tokenized_expression, "Error: parentheses unmatched")
+    # [1:] to exclude the left parens (thus complexity) of the main operator
+    for i, token in enumerate(tokenized_expression[1:]):
         if token == "(":
             left_parentheses += 1
         elif token == ")":
             right_parentheses += 1
-        elif token in unary_operators: # ignore this case since we care about binary complexity
+        # ignore this case since we care about binary complexity
+        elif token in unary_operators:
             continue
         if left_parentheses == right_parentheses:
-            return i + 2 # +1 bc list is [1:] and we want original index, and +1 bc it's next elem where the main op is
+            # +1 bc list is [1:] and we want original index, and +1 bc it's next
+            # elem where the main op is
+            return i + 2
+    raise ValueError(tokenized_expression, f"Error: looks like nothing was passed into main_op_index ({tokenized_expression})")
 
 
 def parse(tokens):
     """
     >>> parse(tokenize("(A /wedge (B /lor C))"))
     ['/wedge', ['A'], ['/lor', ['B'], ['C']]]
 
     >>> parse(tokenize("/neg A"))
     ['/neg', ['A']]
-    
+
     >>> parse(tokenize("A")) # note: atomic sentence should return a single element list
     ['A']
 
     >>> parse(tokenize('((A /op (B /op C)) /op (D /op E))'))
     ['/op', ['/op', ['A'], ['/op', ['B'], ['C']]], ['/op', ['D'], ['E']]]
     """
     bin_comp_tokens = binary_comp(tokens)
+    # if tokens[0] == "\\top":
+    #     return ["\\top"]
+    #     return [Const(token, AtomSort)]
     if tokens[0] in unary_operators:
         return [tokens[0], parse(tokens[1:])]
     if bin_comp_tokens == 0:
         token = tokens[0]
-        return [Const(token, AtomSort)] # Const is a function to make a constant
+        # Const is a function to make a constant
+        return [Const(token, AtomSort)]
     main_operator_index = main_op_index(tokens)
-    op_str = tokens[main_operator_index]  # determines how far the operation is
-    left_expression = tokens[1 : main_operator_index]  # start 1 (exclude first parenthesis), stop at same pos of above (exclusive)
-    right_expression = tokens[main_operator_index + 1 : -1]  # from pos of op plus 1 to the penultimate, thus excluding the last parentheses, which belongs to the main expression
+    # determines how far the operation is
+    op_str = tokens[main_operator_index]
+    # start 1 (exclude first parenthesis), stop at same pos of above (exclusive)
+    left_expression = tokens[1:main_operator_index]
+    # from pos of op plus 1 to the penultimate, thus excluding the last
+    # parentheses, which belongs to the main expression
+    if main_operator_index is None:
+        raise SyntaxError("Error: 'main_operator_index' is not set.")
+    right_expression = tokens[main_operator_index + 1 : -1]
     return [op_str, parse(left_expression), parse(right_expression)]
 
 
 def Prefix(A):
     """takes a sentence in Infix notation and translates it to Prefix notation"""
     return parse(tokenize(A))
 
 
 def Infix(A):
     """takes a sentence in Prefix notation and translates it to infix notation"""
     if len(A) == 1:
         return str(A[0])
     if len(A) == 2:
-        return f'\\neg {Infix(A[1])}'
+        if 'neg' in A[0]:
+            return f"\\neg {Infix(A[1])}"
+        if 'iamond' in A[0]:
+            return f"\\Diamond {Infix(A[1])}"
+        return f"\\Box {Infix(A[1])}"
     op = A[0]
     left_expr = A[1]
     right_expr = A[2]
-    return f'({Infix(left_expr)} {op} {Infix(right_expr)})'
+    return f"({Infix(left_expr)} {op} {Infix(right_expr)})"
+
 
 # doctest.testmod()
 # print(tokenize("(A \\wedge (B \\vee C))")) # the doctests fail, but this works. Need to do double backslash for abfnrtv.
 # print(Prefix("(A \\wedge (B \\vee \\neg C))")) # ['\\wedge', ['A'], ['\\vee', ['B'], ['\\neg', ['C']]]]
-# print(Prefix("A")) 
+# print(Prefix("A"))
 # print(Prefix('((A \\op (B \\op C)) \\op (D \\op E))')) # ['\\op', ['\\op', ['A'], ['\\op', ['B'], ['C']]], ['\\op', ['D'], ['E']]]
 
 # sentences = [Prefix("(A \\wedge (B \\vee \\neg C))"), Prefix("A"), Prefix('((A \\op (B \\op Z)) \\op (D \\op E))')]
 # print(all_sentence_letters(sentences)) # correctly prints ['A', 'B', 'C', 'D', 'E', 'Z']
 # print(Prefix("\\neg (A \\boxright B)"))
 # print(all_sentence_letters([Prefix("\\neg (A \\boxright B)")]))
 
-# moved unused prefix_combine to the boneyard
+# moved unused prefix_combine to the boneyard
```

### Comparing `model_checker-0.1/pyproject.toml` & `model_checker-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "model_checker"
-version = "0.1"
+version = "0.2.0"
 description = "A hyperintensional model checker for counterfactual conditionals"
 authors = [
     { name = "Benjamin Brast-McKie", email = "benbrastmckie@gmail.com" },
-    { name = "Miguel Buitrago", email = "mfbuit46@mit.edu" },
+    { name = "Miguel Buitrago", email = "mbuit82@gmail.com" },
 ]
 license = { text = "MIT" }
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

