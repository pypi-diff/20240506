# Comparing `tmp/fastatomstruct-0.7.0-cp39-none-win_amd64.whl.zip` & `tmp/fastatomstruct-0.7.1-cp39-cp39-manylinux_2_34_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 1207601 bytes, number of entries: 7
--rw-r--r--  4.6 unx     3486 b- defN 24-May-05 13:59 fastatomstruct-0.7.0.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 24-May-05 13:59 fastatomstruct-0.7.0.dist-info/WHEEL
--rw-r--r--  4.6 unx    35076 b- defN 24-May-05 13:59 fastatomstruct-0.7.0.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx    15219 b- defN 24-May-05 13:59 fastatomstruct/__init__.py
--rw-r--r--  4.6 unx   317713 b- defN 24-May-05 13:59 fastatomstruct/__init__.pyi
--rwxr-xr-x  4.6 unx  2912768 b- defN 24-May-05 13:59 fastatomstruct/fastatomstruct.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      615 b- defN 24-May-05 13:59 fastatomstruct-0.7.0.dist-info/RECORD
-7 files, 3284971 bytes uncompressed, 1206517 bytes compressed:  63.3%
+Zip file size: 782656 bytes, number of entries: 7
+-rw-r--r--  4.6 unx     3486 b- defN 24-May-06 16:38 fastatomstruct-0.7.1.dist-info/METADATA
+-rw-r--r--  4.6 unx      106 b- defN 24-May-06 16:38 fastatomstruct-0.7.1.dist-info/WHEEL
+-rw-r--r--  4.6 unx    35076 b- defN 24-May-06 16:38 fastatomstruct-0.7.1.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx    15222 b- defN 24-May-06 16:38 fastatomstruct/__init__.py
+-rw-r--r--  4.6 unx   337541 b- defN 24-May-06 16:38 fastatomstruct/__init__.pyi
+-rwxr-xr-x  4.6 unx  1710704 b- defN 24-May-06 16:38 fastatomstruct/fastatomstruct.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  4.6 unx      628 b- defN 24-May-06 16:38 fastatomstruct-0.7.1.dist-info/RECORD
+7 files, 2102763 bytes uncompressed, 781548 bytes compressed:  62.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: fastatomstruct-0.7.0.dist-info/METADATA
+Filename: fastatomstruct-0.7.1.dist-info/METADATA
 Comment: 
 
-Filename: fastatomstruct-0.7.0.dist-info/WHEEL
+Filename: fastatomstruct-0.7.1.dist-info/WHEEL
 Comment: 
 
-Filename: fastatomstruct-0.7.0.dist-info/license_files/LICENSE
+Filename: fastatomstruct-0.7.1.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: fastatomstruct/__init__.py
 Comment: 
 
 Filename: fastatomstruct/__init__.pyi
 Comment: 
 
-Filename: fastatomstruct/fastatomstruct.cp39-win_amd64.pyd
+Filename: fastatomstruct/fastatomstruct.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: fastatomstruct-0.7.0.dist-info/RECORD
+Filename: fastatomstruct-0.7.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fastatomstruct/__init__.py

```diff
@@ -249,17 +249,17 @@
 def mean_squared_displacement(atoms: List[Atoms]) -> np.ndarray:
     """Mean squared displacment of a trajectory.
     
     The MSD is calculated using the `tidynamics` package. It is defined as
 
     .. math::
 
-        \\mathrm{MSD} = \\frac{1}{N} \sum_{i = 1}^N |\vec{x}_i(t) - \vec{x}_i(0)|^2,
+        \\mathrm{MSD} = \\frac{1}{N} \sum_{i = 1}^N |\\vec{x}_i(t) - \\vec{x}_i(0)|^2,
 
-    where the :math:`\vec{x}_i(t)` are the atomic positions at time :math:`t`.
+    where the :math:`\\vec{x}_i(t)` are the atomic positions at time :math:`t`.
 
     Arguments:
         atoms (List[ase.Atoms]): Trajectory, atoms objects from ASE
 
     Returns:
         NumPy Array of floats containing the mean squared displacement
```

## fastatomstruct/__init__.pyi

```diff
@@ -564,15 +564,15 @@
     >>> fs.bond_length_ratio(atoms, 2.5, 4, 25)
     1.1065865743550205
     """
     ...
 
 
 def bond_length_ratio_list(atoms: Atoms, r_min: float, r_max: float,
-                           cutoff_angle: float, filter: Optional[fastatomstruct.Filter] = None]) -> NDArray:
+                           cutoff_angle: float, filter: Optional[fastatomstruct.Filter] = None) -> NDArray:
     """(Angular limited) bond length ratio for each set of atoms.
 
     The angular limited bond length ratio for a triplet of atoms
     :math:`i_1`, :math:`i_2`, and :math:`i_3` is defined as
 
     .. math::
 
@@ -707,15 +707,15 @@
            [  0.,   0.,   0., ..., 100.,  91.,  83.],
            [  0.,   0.,   0., ...,  91.,  74.,  80.],
            [  0.,   0.,   0., ...,  83.,  80.,  96.]])
     """
     ...
 
 
-def distances(atoms: Atoms, i: int, filter: Optional[fastatomstruct.Filter] = None]) -> NDArray:
+def distances(atoms: Atoms, i: int, filter: Optional[fastatomstruct.Filter] = None) -> NDArray:
     """Distances of one atom to all other atoms.
 
     Arguments:
         atoms (ase.Atoms): Atoms object from ASE
         i (int): Index of atom to calculate distances for
         filter (fastatomstruct.Filter): Filter instance
 
@@ -879,15 +879,15 @@
             13.02275278,  0.        ]])
     >>> d.shape
     (540, 540)
     """
     ...
 
 
-def distance_vectors(atoms: Atoms, i: int, filter: Optional[fastatomstruct.Filter] = None]) -> NDArray:
+def distance_vectors(atoms: Atoms, i: int, filter: Optional[fastatomstruct.Filter] = None) -> NDArray:
     """Distance vectors between one atom and all other atoms.
     
     Arguments:
         atoms (ase.Atoms): Atoms object from ASE
         i (int): Atom index
         filter (fastatomstruct.Filter): Filter instance
     
@@ -910,15 +910,15 @@
            [ -4.8092365 ,  -6.69770233,  -1.78779332],
            [ 12.63852603,   2.2464042 ,  -1.30209939],
            [  9.35835886,  -7.42100408,  -9.38750666]])
     """
     ...
 
 
-def all_distance_vectors(atoms: Atoms, i: int, filter: Optional[fastatomstruct.Filter] = None]) -> List[NDArray]:
+def all_distance_vectors(atoms: Atoms, i: int, filter: Optional[fastatomstruct.Filter] = None) -> List[NDArray]:
     """Distance vectors between all atoms and all other atoms.
     
     Arguments:
         atoms (ase.Atoms): Atoms object from ASE
         filter (fastatomstruct.Filter): Filter instance
     
     Returns:
@@ -1516,104 +1516,185 @@
            0.68408236, 0.49522574, 0.36855817, 0.33841338, 0.35511913,
            0.41287206, 0.55721067, 0.63542276, 0.75380977, 0.82271293,
            0.98696812, 0.97537108, 1.08549646, 1.19705248, 1.21846285,
            1.19599703, 1.29171737, 1.34423667, 1.40868964, 1.46559489]))
     """
 
 
-def mean_squared_displacement(atoms: List[Atoms]) -> NDArray:
-    """Mean squared displacement (MSD) with temporal averaging.
+def mean_squared_displacement_single(atoms: List[Atoms], timestep: float) -> NDArray:
+    """Mean squared displacement (MSD) without temporal averaging.
 
-    The (averaged) MSD is defined as
+    The (non-averaged) MSD is defined as
 
     .. math::
 
-        \mathrm{MSD} = \langle |\vec{x}(t) - \vec{x}(t_0)|^2 \rangle_{N, t_0} = \left\langle \frac{1}{N} \sum_{i = 1}^N |\vec{x}^i(t) - \vec{x}^i(t_0)|^2 \right\rangle_{t_0}
+        \mathrm{MSD} = \langle |\vec{x}(t) - \vec{x}(t_0)|^2 \rangle = \frac{1}{N} \sum_{i = 1}^N |\vec{x}^i(t) - \vec{x}^i(t_0)|^2.
 
     Arguments:
         atoms (List[ase.Atoms]): List of Atoms objects from ASE
+        timestep (float): Time step of the input trajectory (in fs)
 
     Returns:
-        1D array containing the MSD
-    """
-    ...
+        Two 1D arrays containing time and the MSD
 
+    Examples
+    --------
 
-def mean_squared_displacement_single(atoms: List[Atoms]) -> NDArray:
-    """Mean squared displacement (MSD) without temporal averaging.
-
-    The (non-averaged) MSD is defined as
-
-    .. math::
-
-        \mathrm{MSD} = \langle |\vec{x}(t) - \vec{x}(t_0)|^2 \rangle = \frac{1}{N} \sum_{i = 1}^N |\vec{x}^i(t) - \vec{x}^i(t_0)|^2
-
-    Arguments:
-        atoms (List[ase.Atoms]): List of Atoms objects from ASE
+    The exemplary file "Sb-1.00-300-100.traj" `can be found here <https://zivgitlab.uni-muenster.de/ag-salinga/fastatomstruct/-/raw/master/regressiontesting/Structures/Sb-1.00-300-100.traj>`_.
 
-    Returns:
-        1D array containing the MSD
+    >>> import fastatomstruct as fs
+    >>> from ase import io
+    >>> atoms = io.read("Sb-1.00-300-100.traj", index=":")
+    >>> fs.mean_squared_displacement_single(atoms, 2)
+    (array([0.00000000e+00, 2.00000000e+00, 4.50000000e+00, 7.62500000e+00,
+           1.15312500e+01, 1.64140625e+01, 2.25175781e+01, 3.01469727e+01,
+           3.96837158e+01, 5.16046448e+01, 6.65058060e+01, 8.51322575e+01,
+           1.08415322e+02, 1.37519152e+02, 1.73898940e+02, 2.19373675e+02,
+           2.76217094e+02, 3.47271368e+02, 4.36089210e+02, 5.47111512e+02,
+           6.85889390e+02, 8.59361738e+02, 1.07620217e+03, 1.34725272e+03,
+           1.68606589e+03, 2.10958237e+03]), array([0.        , 0.08570729, 0.14451626, 0.17254087, 0.18339419,
+           0.18973448, 0.22214894, 0.2472062 , 0.23734063, 0.26985745,
+           0.30982666, 0.33184891, 0.33978547, 0.38758629, 0.4960587 ,
+           0.56526925, 0.69970379, 0.84905888, 0.72705065, 0.83070123,
+           0.97334769, 1.25106927, 1.58822374, 1.89869893, 2.01082199,
+           2.03046029]))
     """
 
 
-def squared_displacement_single(atoms: List[Atoms]) -> NDArray:
+def squared_displacement_single(atoms: List[Atoms], timestep: float) -> NDArray:
     """Squared displacement (SD) for each atom without temporal averaging.
 
     The (non-averaged) SD is defined as
 
     .. math::
 
-        \mathrm{SD}_i = |\vec{x}^i(t) - \vec{x}^i(t_0)|^2 = |\vec{x}^i(t) - \vec{x}^i(t_0)|^2
+        \mathrm{SD}_i = |\vec{x}^i(t) - \vec{x}^i(t_0)|^2 = |\vec{x}^i(t) - \vec{x}^i(t_0)|^2.
 
     Arguments:
         atoms (List[ase.Atoms]): List of Atoms objects from ASE
+        timestep (float): Time step of the input trajectory (in fs)
 
     Returns:
-        2D array of shape (n_atoms, n_times) containing the SD
+        1D array of length n_times containing the times, 2D array of shape (n_atoms, n_times) containing the SD
+
+    Examples
+    --------
+
+    The exemplary file "Sb-1.00-300-100.traj" `can be found here <https://zivgitlab.uni-muenster.de/ag-salinga/fastatomstruct/-/raw/master/regressiontesting/Structures/Sb-1.00-300-100.traj>`_.
+
+    >>> import fastatomstruct as fs
+    >>> from ase import io
+    >>> atoms = io.read("Sb-1.00-300-100.traj", index=":")
+    >>> fs.squared_displacement_single(atoms, 2)
+    (array([0.00000000e+00, 2.00000000e+00, 4.50000000e+00, 7.62500000e+00,
+           1.15312500e+01, 1.64140625e+01, 2.25175781e+01, 3.01469727e+01,
+           3.96837158e+01, 5.16046448e+01, 6.65058060e+01, 8.51322575e+01,
+           1.08415322e+02, 1.37519152e+02, 1.73898940e+02, 2.19373675e+02,
+           2.76217094e+02, 3.47271368e+02, 4.36089210e+02, 5.47111512e+02,
+           6.85889390e+02, 8.59361738e+02, 1.07620217e+03, 1.34725272e+03,
+           1.68606589e+03, 2.10958237e+03]), array([[0.        , 0.01527723, 0.04965418, ..., 0.30716283, 0.74459351,
+            0.93403832],
+           [0.        , 0.10336262, 0.12957674, ..., 1.56028193, 0.69138778,
+            1.92792858],
+           [0.        , 0.02684147, 0.017915  , ..., 0.95177762, 0.65267762,
+            2.02677489],
+           ...,
+           [0.        , 0.09875333, 0.20993371, ..., 0.35825702, 0.41746509,
+            0.29975324],
+           [0.        , 0.01581711, 0.21283568, ..., 0.21601321, 0.63707872,
+            0.48397539],
+           [0.        , 0.06138846, 0.47158164, ..., 0.32970027, 0.18566879,
+            0.40088013]]))
     """
     ...
 
 
 def non_gaussian_alpha2(atoms: List[Atoms]) -> NDArray:
     """(Temporally averaged) non-Gaussian parameter.
 
     It is defined as
 
     .. math::
 
-        \alpha_2(t) = \left\langle \frac{3}{5} \frac{\sum_{i = 1}^N |\vec{x}^i(t) - \vec{x}^i(t_0)|^4}{(\sum_{i = 1}^N |\vec{x}^i(t) - \vec{x}^i(t_0)|^2)^2} \right\rangle_{t_0}
+        \alpha_2(t) = \left\langle \frac{3}{5} \frac{\sum_{i = 1}^N |\vec{x}^i(t) - \vec{x}^i(t_0)|^4}{(\sum_{i = 1}^N |\vec{x}^i(t) - \vec{x}^i(t_0)|^2)^2} \right\rangle_{t_0},
 
-    can be used to identify non-Gaussian behaviour in molecular dynamics.
+    and can be used to identify non-Gaussian behaviour in molecular dynamics.
 
     Arguments:
         atoms (List[ase.Atoms]): List of Atoms objects from ASE
+        timestep (float): Time step of the input trajectory (in fs)
 
     Returns:
-        1D array containing the non-Gaussian parameter for each time step
+        Two 1D arrays containing the times and the non-Gaussian parameter
+
+    Examples
+    --------
+
+    The exemplary file "Sb-1.00-300-100.traj" `can be found here <https://zivgitlab.uni-muenster.de/ag-salinga/fastatomstruct/-/raw/master/regressiontesting/Structures/Sb-1.00-300-100.traj>`_.
+
+    >>> import fastatomstruct as fs
+    >>> from ase import io
+    >>> atoms = io.read("Sb-1.00-300-100.traj", index=":")
+    >>> fs.non_gaussian_alpha2(atoms, 2)
+    (array([0.00000000e+00, 2.00000000e+00, 4.50000000e+00, 7.62500000e+00,
+           1.15312500e+01, 1.64140625e+01, 2.25175781e+01, 3.01469727e+01,
+           3.96837158e+01, 5.16046448e+01, 6.65058060e+01, 8.51322575e+01,
+           1.08415322e+02, 1.37519152e+02, 1.73898940e+02, 2.19373675e+02,
+           2.76217094e+02, 3.47271368e+02, 4.36089210e+02, 5.47111512e+02,
+           6.85889390e+02, 8.59361738e+02, 1.07620217e+03, 1.34725272e+03,
+           1.68606589e+03, 2.10958237e+03]), array([0.        , 0.05451509, 0.05746702, 0.03857166, 0.0436452 ,
+           0.13699174, 0.18596818, 0.13470472, 0.12885145, 0.15707456,
+           0.18798212, 0.1485821 , 0.21675234, 0.37810897, 0.30411076,
+           0.26653256, 0.18371315, 0.22608079, 0.40846979, 0.29919836,
+           0.29243173, 0.36112955, 0.22192952, 0.21543669, 0.45339333,
+           0.511548  ]))
     """
     ...
 
 
-def non_gaussian_alpha2_single(atoms: List[Atoms]) -> NDArray:
+def non_gaussian_alpha2_single(atoms: List[Atoms], timestep: float) -> NDArray:
     """(Non-averaged) non-Gaussian parameter.
 
     It is defined as
 
     .. math::
 
-        \alpha_2(t) = \frac{3}{5} \frac{\sum_{i = 1}^N |\vec{x}^i(t) - \vec{x}^i(t_0)|^4}{(\sum_{i = 1}^N |\vec{x}^i(t) - \vec{x}^i(t_0)|^2)^2}
+        \alpha_2(t) = \frac{3}{5} \frac{\sum_{i = 1}^N |\vec{x}^i(t) - \vec{x}^i(t_0)|^4}{(\sum_{i = 1}^N |\vec{x}^i(t) - \vec{x}^i(t_0)|^2)^2},
 
-    can be used to identify non-Gaussian behaviour in molecular dynamics.
+    and can be used to identify non-Gaussian behaviour in molecular dynamics.
 
     Arguments:
         atoms (List[ase.Atoms]): List of Atoms objects from ASE
+        timestep (float): Time step of the input trajectory (in fs)
 
     Returns:
-        2D array of shape (n_atoms, n_times) containing the non-Gaussian
-        parameter for each time step and atom
+        1D array of times, 2D array of shape (n_atoms, n_times) containing the non-Gaussian
+        parameter each time and atom
+
+    Examples
+    --------
+
+    The exemplary file "Sb-1.00-300-100.traj" `can be found here <https://zivgitlab.uni-muenster.de/ag-salinga/fastatomstruct/-/raw/master/regressiontesting/Structures/Sb-1.00-300-100.traj>`_.
+
+    >>> import fastatomstruct as fs
+    >>> from ase import io
+    >>> atoms = io.read("Sb-1.00-300-100.traj", index=":")
+    >>> fs.non_gaussian_alpha2_single(atoms, 2)
+    (array([0.00000000e+00, 2.00000000e+00, 4.50000000e+00, 7.62500000e+00,
+           1.15312500e+01, 1.64140625e+01, 2.25175781e+01, 3.01469727e+01,
+           3.96837158e+01, 5.16046448e+01, 6.65058060e+01, 8.51322575e+01,
+           1.08415322e+02, 1.37519152e+02, 1.73898940e+02, 2.19373675e+02,
+           2.76217094e+02, 3.47271368e+02, 4.36089210e+02, 5.47111512e+02,
+           6.85889390e+02, 8.59361738e+02, 1.07620217e+03, 1.34725272e+03,
+           1.68606589e+03, 2.10958237e+03]), array([       nan, 0.05451509, 0.08587094, 0.09528725, 0.16900584,
+           0.44242745, 0.50440087, 0.34962665, 0.26894454, 0.51749794,
+           0.45986851, 0.38946558, 0.3658462 , 0.49804137, 0.38984063,
+           0.35371946, 0.25276157, 0.1813512 , 0.47461673, 0.30959159,
+           0.24564468, 0.24307653, 0.15243596, 0.02262402, 0.06824235,
+           0.1051412 ]))
     """
     ...
 
 
 def overlap_q(atoms: List[Atoms], a: float, timestep: float) -> Tuple[NDArray, NDArray, NDArray, NDArray]:
     """Time-averaged overlap parameter.
 
@@ -1642,14 +1723,48 @@
     Arguments:
         atoms (List[ase.Atoms]): List of Atoms objects from ASE
         a (float): Cutoff for the overlap function
         timestep (float): Time step of the input trajectory (in fs)
 
     Returns:
         Four arrays of length n_times (time, full q, self part, distinct part)
+
+    Examples
+    --------
+
+    The exemplary file "Sb-1.00-300-100.traj" `can be found here <https://zivgitlab.uni-muenster.de/ag-salinga/fastatomstruct/-/raw/master/regressiontesting/Structures/Sb-1.00-300-100.traj>`_.
+
+    >>> import fastatomstruct as fs
+    >>> from ase import io
+    >>> atoms = io.read("Sb-1.00-300-100.traj", index=":")
+    >>> fs.overlap_q(atoms, 2, 200)
+    (array([0.00000000e+00, 2.00000000e+02, 4.50000000e+02, 7.62500000e+02,
+           1.15312500e+03, 1.64140625e+03, 2.25175781e+03, 3.01469727e+03,
+           3.96837158e+03, 5.16046448e+03, 6.65058060e+03, 8.51322575e+03,
+           1.08415322e+04, 1.37519152e+04, 1.73898940e+04, 2.19373675e+04,
+           2.76217094e+04, 3.47271368e+04, 4.36089210e+04, 5.47111512e+04,
+           6.85889390e+04, 8.59361738e+04, 1.07620217e+05, 1.34725272e+05,
+           1.68606589e+05, 2.10958237e+05]), array([  0.        , 728.        , 728.        , 728.        ,
+           728.        , 728.33333333, 728.22222222, 728.41666667,
+           728.8125    , 728.42857143, 728.96428571, 729.81081081,
+           729.22916667, 730.14516129, 734.1125    , 733.65686275,
+           738.43076923, 745.56363636, 742.38755981, 744.89015152,
+           745.996997  , 749.01431981, 758.91461101, 770.95468278,
+           773.55354994, 765.79654511]), array([  0.        , 728.        , 728.        , 728.        ,
+           728.        , 728.        , 728.        , 728.        ,
+           728.        , 727.95238095, 727.92857143, 727.97297297,
+           727.97916667, 727.08064516, 726.9375    , 726.23529412,
+           725.54615385, 723.93939394, 723.71291866, 723.51515152,
+           722.92192192, 717.01193317, 713.38519924, 709.77492447,
+           706.20336943, 701.01535509]), array([ 0.        ,  0.        ,  0.        ,  0.        ,  0.        ,
+            0.33333333,  0.22222222,  0.41666667,  0.8125    ,  0.47619048,
+            1.03571429,  1.83783784,  1.25      ,  3.06451613,  7.175     ,
+            7.42156863, 12.88461538, 21.62424242, 18.67464115, 21.375     ,
+           23.07507508, 32.00238663, 45.52941176, 61.17975831, 67.35018051,
+           64.78119002]))
     """
     ...
 
 
 def overlap_q_self(atoms: List[Atoms], a: float, timestep: float) -> Tuple[NDArray, NDArray]:
     """Self part of the overlap parameter.
 
@@ -1666,14 +1781,37 @@
     Arguments:
         atoms (List[ase.Atoms]): List of Atoms objects from ASE
         a (float): Cutoff for the overlap function
         timestep (float): Time step of the input trajectory (in fs)
 
     Returns:
         Two arrays of length n_times containing the self part of the overlap parameter (time, self part)
+
+    Examples
+    --------
+
+    The exemplary file "Sb-1.00-300-100.traj" `can be found here <https://zivgitlab.uni-muenster.de/ag-salinga/fastatomstruct/-/raw/master/regressiontesting/Structures/Sb-1.00-300-100.traj>`_.
+
+    >>> import fastatomstruct as fs
+    >>> from ase import io
+    >>> atoms = io.read("Sb-1.00-300-100.traj", index=":")
+    >>> fs.overlap_q_self(atoms, 2, 200)
+    (array([0.00000000e+00, 2.00000000e+02, 4.50000000e+02, 7.62500000e+02,
+           1.15312500e+03, 1.64140625e+03, 2.25175781e+03, 3.01469727e+03,
+           3.96837158e+03, 5.16046448e+03, 6.65058060e+03, 8.51322575e+03,
+           1.08415322e+04, 1.37519152e+04, 1.73898940e+04, 2.19373675e+04,
+           2.76217094e+04, 3.47271368e+04, 4.36089210e+04, 5.47111512e+04,
+           6.85889390e+04, 8.59361738e+04, 1.07620217e+05, 1.34725272e+05,
+           1.68606589e+05, 2.10958237e+05]), array([  0.        , 728.        , 728.        , 728.        ,
+           728.        , 728.        , 728.        , 728.        ,
+           728.        , 727.95238095, 727.92857143, 727.97297297,
+           727.97916667, 727.08064516, 726.9375    , 726.23529412,
+           725.54615385, 723.93939394, 723.71291866, 723.51515152,
+           722.92192192, 717.01193317, 713.38519924, 709.77492447,
+           706.20336943, 701.01535509]))
     """
     ...
 
 
 def overlap_q_self_atomic(atoms: List[Atoms], a: float) -> NDArray:
     """Self part of the overlap parameter for each individual atom.
 
@@ -1687,14 +1825,37 @@
 
     Arguments:
         atoms (List[ase.Atoms]): List of Atoms objects from ASE
         a (float): Cutoff for the overlap function
 
     Returns:
         Array of shape n_times and array of shape (n_atoms, n_times) containing the time and the self part of the overlap parameter
+
+    Examples
+    --------
+
+    The exemplary file "Sb-1.00-300-100.traj" `can be found here <https://zivgitlab.uni-muenster.de/ag-salinga/fastatomstruct/-/raw/master/regressiontesting/Structures/Sb-1.00-300-100.traj>`_.
+
+    >>> import fastatomstruct as fs
+    >>> from ase import io
+    >>> atoms = io.read("Sb-1.00-300-100.traj", index=":")
+    >>> fs.overlap_q_self_atomic(atoms, 2)
+    array([[0.        , 1.        , 1.        , ..., 1.        , 1.        ,
+            1.        ],
+           [0.        , 1.        , 1.        , ..., 1.        , 1.        ,
+            0.99906716],
+           [0.        , 1.        , 1.        , ..., 1.        , 1.        ,
+            1.        ],
+           ...,
+           [0.        , 1.        , 1.        , ..., 1.        , 1.        ,
+            1.        ],
+           [0.        , 1.        , 1.        , ..., 1.        , 1.        ,
+            1.        ],
+           [0.        , 1.        , 1.        , ..., 0.98878505, 1.        ,
+            0.9869403 ]])
     """
     ...
 
 
 def overlap_q_distinct(atoms: List[Atoms], a: float, timestep: float) -> Tuple[NDArray, NDArray]:
     """Distinct part of the overlap parameter.
 
@@ -1709,14 +1870,36 @@
     Arguments:
         atoms (List[ase.Atoms]): List of Atoms objects from ASE
         a (float): Cutoff for the overlap function
         timestep (float): Time step of the input trajectory (in fs)
 
     Returns:
         Two arrays of length n_times containing the time and the distinct part of the overlap parameter
+
+    Examples
+    --------
+
+    The exemplary file "Sb-1.00-300-100.traj" `can be found here <https://zivgitlab.uni-muenster.de/ag-salinga/fastatomstruct/-/raw/master/regressiontesting/Structures/Sb-1.00-300-100.traj>`_.
+
+    >>> import fastatomstruct as fs
+    >>> from ase import io
+    >>> atoms = io.read("Sb-1.00-300-100.traj", index=":")
+    >>> fs.overlap_q_distinct(atoms, 2, 200)
+    (array([0.00000000e+00, 2.00000000e+02, 4.50000000e+02, 7.62500000e+02,
+           1.15312500e+03, 1.64140625e+03, 2.25175781e+03, 3.01469727e+03,
+           3.96837158e+03, 5.16046448e+03, 6.65058060e+03, 8.51322575e+03,
+           1.08415322e+04, 1.37519152e+04, 1.73898940e+04, 2.19373675e+04,
+           2.76217094e+04, 3.47271368e+04, 4.36089210e+04, 5.47111512e+04,
+           6.85889390e+04, 8.59361738e+04, 1.07620217e+05, 1.34725272e+05,
+           1.68606589e+05, 2.10958237e+05]), array([ 0.        ,  0.        ,  0.        ,  0.        ,  0.        ,
+            0.33333333,  0.22222222,  0.41666667,  0.8125    ,  0.47619048,
+            1.03571429,  1.83783784,  1.25      ,  3.06451613,  7.175     ,
+            7.42156863, 12.88461538, 21.62424242, 18.67464115, 21.375     ,
+           23.07507508, 32.00238663, 45.52941176, 61.17975831, 67.35018051,
+           64.78119002]))
     """
     ...
 
 
 def overlap_q_single(atoms: List[Atoms], a: float, timestep: float) -> \
         Tuple[NDArray, NDArray, NDArray, NDArray]:
     """Non-averaged overlap parameter.
@@ -1745,14 +1928,37 @@
     Arguments:
         atoms (List[ase.Atoms]): List of Atoms objects from ASE
         a (float): Cutoff for the overlap function
         timestep (float): Time step of the input trajectory (in fs)
 
     Returns:
         Tuple of four arrays of length n_times (time, full q, self part, distinct part)
+
+    Examples
+    --------
+
+    The exemplary file "Sb-1.00-300-100.traj" `can be found here <https://zivgitlab.uni-muenster.de/ag-salinga/fastatomstruct/-/raw/master/regressiontesting/Structures/Sb-1.00-300-100.traj>`_.
+
+    >>> import fastatomstruct as fs
+    >>> from ase import io
+    >>> atoms = io.read("Sb-1.00-300-100.traj", index=":")
+    >>> fs.overlap_q_single(atoms, 2, 200)
+    (array([0.00000000e+00, 2.00000000e+02, 4.50000000e+02, 7.62500000e+02,
+           1.15312500e+03, 1.64140625e+03, 2.25175781e+03, 3.01469727e+03,
+           3.96837158e+03, 5.16046448e+03, 6.65058060e+03, 8.51322575e+03,
+           1.08415322e+04, 1.37519152e+04, 1.73898940e+04, 2.19373675e+04,
+           2.76217094e+04, 3.47271368e+04, 4.36089210e+04, 5.47111512e+04,
+           6.85889390e+04, 8.59361738e+04, 1.07620217e+05, 1.34725272e+05,
+           1.68606589e+05, 2.10958237e+05]), array([728., 728., 728., 728., 728., 729., 729., 729., 729., 729., 729.,
+           729., 733., 734., 749., 742., 742., 755., 753., 763., 766., 784.,
+           795., 810., 815., 807.]), array([728., 728., 728., 728., 728., 728., 728., 728., 728., 727., 727.,
+           727., 727., 727., 728., 724., 724., 718., 719., 718., 711., 696.,
+           680., 658., 646., 641.]), array([  0.,   0.,   0.,   0.,   0.,   1.,   1.,   1.,   1.,   2.,   2.,
+             2.,   6.,   7.,  21.,  18.,  18.,  37.,  34.,  45.,  55.,  88.,
+           115., 152., 169., 166.]))
     """
     ...
 
 
 def overlap_q_single_self(atoms: List[Atoms], a: float, timestep: float) -> Tuple[NDArray, NDArray]:
     """Self part of the overlap parameter.
 
@@ -1768,14 +1974,33 @@
     Arguments:
         atoms (List[ase.Atoms]): List of Atoms objects from ASE
         a (float): Cutoff for the overlap function
         timestep (float): Time step of the input trajectory (in fs)
 
     Returns:
         Two arrays of length n_times containing the time and the self part of the overlap parameter
+
+    Examples
+    --------
+
+    The exemplary file "Sb-1.00-300-100.traj" `can be found here <https://zivgitlab.uni-muenster.de/ag-salinga/fastatomstruct/-/raw/master/regressiontesting/Structures/Sb-1.00-300-100.traj>`_.
+
+    >>> import fastatomstruct as fs
+    >>> from ase import io
+    >>> atoms = io.read("Sb-1.00-300-100.traj", index=":")
+    >>> fs.overlap_q_single_self(atoms, 2, 200)
+    (array([0.00000000e+00, 2.00000000e+02, 4.50000000e+02, 7.62500000e+02,
+           1.15312500e+03, 1.64140625e+03, 2.25175781e+03, 3.01469727e+03,
+           3.96837158e+03, 5.16046448e+03, 6.65058060e+03, 8.51322575e+03,
+           1.08415322e+04, 1.37519152e+04, 1.73898940e+04, 2.19373675e+04,
+           2.76217094e+04, 3.47271368e+04, 4.36089210e+04, 5.47111512e+04,
+           6.85889390e+04, 8.59361738e+04, 1.07620217e+05, 1.34725272e+05,
+           1.68606589e+05, 2.10958237e+05]), array([728., 728., 728., 728., 728., 728., 728., 728., 728., 727., 727.,
+           727., 727., 727., 728., 724., 724., 718., 719., 718., 711., 696.,
+           680., 658., 646., 641.]))
     """
     ...
 
 
 def overlap_q_single_distinct(atoms: List[Atoms], a: float, timestep: float) -> Tuple[NDArray, NDArray]:
     """Distinct part of the overlap parameter.
 
@@ -1791,14 +2016,33 @@
     Arguments:
         atoms (List[ase.Atoms]): List of Atoms objects from ASE
         a (float): Cutoff for the overlap function
         timestep (float): Time step of the input trajectory (in fs)
 
     Returns:
         Two arrays of length n_times containing the time and the distinct part of the overlap parameter
+
+    Examples
+    --------
+
+    The exemplary file "Sb-1.00-300-100.traj" `can be found here <https://zivgitlab.uni-muenster.de/ag-salinga/fastatomstruct/-/raw/master/regressiontesting/Structures/Sb-1.00-300-100.traj>`_.
+
+    >>> import fastatomstruct as fs
+    >>> from ase import io
+    >>> atoms = io.read("Sb-1.00-300-100.traj", index=":")
+    >>> fs.overlap_q_single_distinct(atoms, 2, 200)
+    (array([0.00000000e+00, 2.00000000e+02, 4.50000000e+02, 7.62500000e+02,
+           1.15312500e+03, 1.64140625e+03, 2.25175781e+03, 3.01469727e+03,
+           3.96837158e+03, 5.16046448e+03, 6.65058060e+03, 8.51322575e+03,
+           1.08415322e+04, 1.37519152e+04, 1.73898940e+04, 2.19373675e+04,
+           2.76217094e+04, 3.47271368e+04, 4.36089210e+04, 5.47111512e+04,
+           6.85889390e+04, 8.59361738e+04, 1.07620217e+05, 1.34725272e+05,
+           1.68606589e+05, 2.10958237e+05]), array([  0.,   0.,   0.,   0.,   0.,   1.,   1.,   1.,   1.,   2.,   2.,
+             2.,   6.,   7.,  21.,  18.,  18.,  37.,  34.,  45.,  55.,  88.,
+           115., 152., 169., 166.]))
     """
     ...
 
 
 def fourpoint_susceptibility(
     atoms: List[Atoms], a: float, temperature: float, timestep: float
 ) -> Tuple[NDArray, NDArray, NDArray, NDArray, NDArray]:
@@ -1812,41 +2056,141 @@
 
     and gives information about dynamical heterogeneities. It can be split into three different parts
 
     .. math::
 
         \chi_4(t) = \chi_\mathrm{ss}(t) + \chi_\mathrm{dd}(t) + \chi_\mathrm{sd}(t),
 
-    (see Lacevic et al., "Spatially heterogeneous dynamics investigated via a time-dependent four-point density correlation function"), where :math:`\chi_\mathrm{ss}(t) \propto \langle Q_\mathrm{s}^2(t)\rangle - \langle Q_\mathrm{s}(t) \rangle^2`, :math:`\chi_\mathrm{dd}(t) \propto \langle Q_\mathrm{d}^2(t)\rangle - \langle Q_\mathrm{d}(t) \rangle^2`, and :math:`\chi_\mathrm{sd}(t) \propto \langle Q_\mathrm{s}(t) Q_\mathrm{d}(t) \rangle - \langle Q_\mathrm{s}(t) \rangle \langle Q_\mathrm{d}(t) \rangle`.
+    (see Lacevic et al., "Spatially heterogeneous dynamics investigated via a time-dependent four-point density correlation function"), where
+
+    .. math::
+
+        \begin{split}
+        \chi_\mathrm{ss}(t) &\propto \langle Q_\mathrm{s}^2(t)\rangle - \langle Q_\mathrm{s}(t) \rangle^2, \\
+        \chi_\mathrm{dd}(t) &\propto \langle Q_\mathrm{d}^2(t)\rangle - \langle Q_\mathrm{d}(t) \rangle^2\mathrm{, and} \\
+        \chi_\mathrm{sd}(t) &\propto \langle Q_\mathrm{s}(t) Q_\mathrm{d}(t) \rangle - \langle Q_\mathrm{s}(t) \rangle \langle Q_\mathrm{d}(t) \rangle.
+        \end{split}
+
+    :math:`Q(t)`, :math:`Q_\mathrm{s}(t)` and :math:`Q_\mathrm{d}(t)` are the overlap parameters defined as
+
+    .. math::
+
+        Q(t) = \sum_{i, j = 1}^N w(|\vec{r}_i(0) - \vec{r}_j(t)|),
+
+    with the self part
+
+    .. math::
+
+        Q_\mathrm{s}(t) = \sum_{i = 1}^N w(|\vec{r}_i(0) - \vec{r}_i(t)|),
+
+    and the distinct part
+
+    .. math::
+
+        Q_\mathrm{d}(t) = \sum_{i, j = 1, i \neq j}^N w(|\vec{r}_i(0) - \vec{r}_j(t)|)
+
+    (see Lacevic et al., "Spatially heterogeneous dynamics investigated via a time-dependent four-point density correlation function").
 
     Arguments:
         atoms (List[ase.Atoms]): List of Atoms objects from ASE
         a (float): Cutoff for the overlap function
         temperature (float): Temperature of the system (in K)
         timestep (float): Time step of the input trajectory (in fs)
 
     Returns:
         Five arrays of length n_times containing the time and four-point susceptibility (full, self part, distinct part, cross part)
+
+    Examples
+    --------
+
+    The exemplary file "Sb-1.00-300-100.traj" `can be found here <https://zivgitlab.uni-muenster.de/ag-salinga/fastatomstruct/-/raw/master/regressiontesting/Structures/Sb-1.00-300-100.traj>`_.
+
+    >>> import fastatomstruct as fs
+    >>> from ase import io
+    >>> atoms = io.read("Sb-1.00-300-100.traj", index=":")
+    >>> fs.fourpoint_susceptibility(atoms, 2, 300, 200)
+    (array([0.00000000e+00, 2.00000000e+02, 4.50000000e+02, 7.62500000e+02,
+           1.15312500e+03, 1.64140625e+03, 2.25175781e+03, 3.01469727e+03,
+           3.96837158e+03, 5.16046448e+03, 6.65058060e+03, 8.51322575e+03,
+           1.08415322e+04, 1.37519152e+04, 1.73898940e+04, 2.19373675e+04,
+           2.76217094e+04, 3.47271368e+04, 4.36089210e+04, 5.47111512e+04,
+           6.85889390e+04, 8.59361738e+04, 1.07620217e+05, 1.34725272e+05,
+           1.68606589e+05, 2.10958237e+05]), array([0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
+           0.00000000e+00, 3.67770417e-01, 2.86043658e-01, 4.02248894e-01,
+           1.49334902e+00, 6.83002204e-01, 1.82595198e+00, 3.21322276e+00,
+           3.76605527e+00, 8.19518588e+00, 3.76528238e+01, 5.12245972e+01,
+           1.58465429e+02, 4.72641884e+02, 3.07650655e+02, 3.49178041e+02,
+           6.51803710e+02, 1.12799195e+03, 2.11344492e+03, 3.62413461e+03,
+           3.97949143e+03, 2.89466312e+03]), array([0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
+           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
+           0.00000000e+00, 7.50551873e-02, 1.09768211e-01, 4.35199469e-02,
+           3.37601751e-02, 1.45735247e+00, 2.24842766e+00, 5.23022981e+00,
+           1.21477507e+01, 3.38154261e+01, 3.33430304e+01, 3.31992587e+01,
+           6.63575617e+01, 2.30103357e+02, 4.61289215e+02, 7.26624117e+02,
+           7.48902645e+02, 8.56246437e+02]), array([0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
+           0.00000000e+00, 3.67770417e-01, 2.86043658e-01, 4.02248894e-01,
+           1.49334902e+00, 7.28035316e-01, 1.83017383e+00, 3.17695614e+00,
+           3.89606786e+00, 9.65598261e+00, 4.21095979e+01, 5.95280642e+01,
+           1.89217064e+02, 5.66126085e+02, 3.74069040e+02, 4.23432522e+02,
+           8.06913757e+02, 1.46415590e+03, 2.75190309e+03, 4.63806120e+03,
+           5.08380153e+03, 3.80785978e+03]), array([ 0.00000000e+00,  0.00000000e+00,  0.00000000e+00,  0.00000000e+00,
+            0.00000000e+00,  0.00000000e+00,  0.00000000e+00, -9.40739754e-14,
+            0.00000000e+00, -1.20088300e-01, -1.13990066e-01, -7.25332452e-03,
+           -1.63772764e-01, -2.91814919e+00, -6.70520174e+00, -1.35336968e+01,
+           -4.28993855e+01, -1.27299627e+02, -9.97614155e+01, -1.07453740e+02,
+           -2.21467608e+02, -5.66267306e+02, -1.09974738e+03, -1.74055071e+03,
+           -1.85321275e+03, -1.76944310e+03]))
     """
     ...
 
 
 def fourpoint_susceptibility_self(
         atoms: List[Atoms], a: float, temperature: float, timestep: float) -> Tuple[NDArray]:
     """Self part of the four-point susceptibility.
 
     It is defined as
 
     .. math::
 
-        \chi_\mathrm{ss}(t) = \frac{\beta V}{N^2} \left[\langle Q_\mathrm{s}^2(t) \rangle - \langle Q_\mathrm{s}(t) \rangle^2\right]
+        \chi_\mathrm{ss}(t) = \frac{\beta V}{N^2} \left[\langle Q_\mathrm{s}^2(t) \rangle - \langle Q_\mathrm{s}(t) \rangle^2\right].
+
+    :math:`Q_\mathrm{s}(t)` is the self part of the overlap parameter, defined as
+
+    .. math::
+
+        Q_\mathrm{s}(t) = \sum_{i = 1}^N w(|\vec{r}_i(0) - \vec{r}_i(t)|)
 
+    (see Lacevic et al., "Spatially heterogeneous dynamics investigated via a time-dependent four-point density correlation function").
+    
     Arguments:
         atoms (List[ase.Atoms]): List of Atoms objects from ASE
         a (float): Cutoff for the overlap function
         temperature (float): Temperature of the system (in K)
         timestep (float): Time step of the input trajectory (in fs)
 
     Returns:
         Two arrays of length n_times containing the time and the self part of the four-point susceptibility
+
+    Examples
+    --------
+
+    The exemplary file "Sb-1.00-300-100.traj" `can be found here <https://zivgitlab.uni-muenster.de/ag-salinga/fastatomstruct/-/raw/master/regressiontesting/Structures/Sb-1.00-300-100.traj>`_.
+
+    >>> import fastatomstruct as fs
+    >>> from ase import io
+    >>> atoms = io.read("Sb-1.00-300-100.traj", index=":")
+    >>> fs.fourpoint_susceptibility_self(atoms, 2, 300, 200)
+    (array([0.00000000e+00, 2.00000000e+02, 4.50000000e+02, 7.62500000e+02,
+           1.15312500e+03, 1.64140625e+03, 2.25175781e+03, 3.01469727e+03,
+           3.96837158e+03, 5.16046448e+03, 6.65058060e+03, 8.51322575e+03,
+           1.08415322e+04, 1.37519152e+04, 1.73898940e+04, 2.19373675e+04,
+           2.76217094e+04, 3.47271368e+04, 4.36089210e+04, 5.47111512e+04,
+           6.85889390e+04, 8.59361738e+04, 1.07620217e+05, 1.34725272e+05,
+           1.68606589e+05, 2.10958237e+05]), array([0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
+           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
+           0.00000000e+00, 7.50551873e-02, 1.09768211e-01, 4.35199469e-02,
+           3.37601751e-02, 1.45735247e+00, 2.24842766e+00, 5.23022981e+00,
+           1.21477507e+01, 3.38154261e+01, 3.33430304e+01, 3.31992587e+01,
+           6.63575617e+01, 2.30103357e+02, 4.61289215e+02, 7.26624117e+02,
+           7.48902645e+02, 8.56246437e+02]))
     """
     ...
```

## Comparing `fastatomstruct-0.7.0.dist-info/METADATA` & `fastatomstruct-0.7.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fastatomstruct
-Version: 0.7.0
+Version: 0.7.1
 Requires-Dist: ase
 Requires-Dist: numpy
 Requires-Dist: tidynamics
 License-File: LICENSE
 Author: Nils Cedric Holle <nils.holle@uni-muenster.de>
 Author-email: Nils Cedric Holle <nils.holle@uni-muenster.de>
 License: GPL-3.0
```

## Comparing `fastatomstruct-0.7.0.dist-info/license_files/LICENSE` & `fastatomstruct-0.7.1.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

