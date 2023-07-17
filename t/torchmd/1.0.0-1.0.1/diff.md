# Comparing `tmp/torchmd-1.0.0.tar.gz` & `tmp/torchmd-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchmd-1.0.0.tar", last modified: Mon May 22 17:03:54 2023, max compression
+gzip compressed data, was "torchmd-1.0.1.tar", last modified: Mon Jul 17 13:17:51 2023, max compression
```

## Comparing `torchmd-1.0.0.tar` & `torchmd-1.0.1.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:03:54.839715 torchmd-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-22 17:03:11.000000 torchmd-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-22 17:03:11.000000 torchmd-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-22 17:03:54.839715 torchmd-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-22 17:03:11.000000 torchmd-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-22 17:03:11.000000 torchmd-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 17:03:54.839715 torchmd-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-22 17:03:11.000000 torchmd-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:03:54.831715 torchmd-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    19971 2023-05-22 17:03:12.000000 torchmd-1.0.0/tests/test_torchmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:03:54.839715 torchmd-1.0.0/torchmd/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-22 17:03:54.839715 torchmd-1.0.0/torchmd/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:03:54.839715 torchmd-1.0.0/torchmd/forcefields/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/forcefields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/forcefields/ff_parmed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/forcefields/ff_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/forcefields/forcefield.py
--rw-r--r--   0 runner    (1001) docker     (123)    22744 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/forces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/integrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/minimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/mycalc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/neighbourlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/systems.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-22 17:03:12.000000 torchmd-1.0.0/torchmd/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:03:54.839715 torchmd-1.0.0/torchmd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-22 17:03:54.000000 torchmd-1.0.0/torchmd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-22 17:03:54.000000 torchmd-1.0.0/torchmd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:03:54.000000 torchmd-1.0.0/torchmd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:03:54.000000 torchmd-1.0.0/torchmd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-22 17:03:54.000000 torchmd-1.0.0/torchmd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 17:03:54.000000 torchmd-1.0.0/torchmd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:17:51.059529 torchmd-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-17 13:17:19.000000 torchmd-1.0.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-17 13:17:19.000000 torchmd-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-17 13:17:51.059529 torchmd-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-17 13:17:19.000000 torchmd-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-17 13:17:19.000000 torchmd-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 13:17:51.059529 torchmd-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-17 13:17:19.000000 torchmd-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:17:51.055529 torchmd-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    19971 2023-07-17 13:17:19.000000 torchmd-1.0.1/tests/test_torchmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:17:51.059529 torchmd-1.0.1/torchmd/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-17 13:17:19.000000 torchmd-1.0.1/torchmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-17 13:17:51.059529 torchmd-1.0.1/torchmd/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:17:51.059529 torchmd-1.0.1/torchmd/forcefields/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:17:19.000000 torchmd-1.0.1/torchmd/forcefields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-07-17 13:17:19.000000 torchmd-1.0.1/torchmd/forcefields/ff_parmed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-17 13:17:19.000000 torchmd-1.0.1/torchmd/forcefields/ff_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-17 13:17:19.000000 torchmd-1.0.1/torchmd/forcefields/forcefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22744 2023-07-17 13:17:19.000000 torchmd-1.0.1/torchmd/forces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-17 13:17:19.000000 torchmd-1.0.1/torchmd/integrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-17 13:17:19.000000 torchmd-1.0.1/torchmd/minimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-17 13:17:19.000000 torchmd-1.0.1/torchmd/mycalc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-17 13:17:19.000000 torchmd-1.0.1/torchmd/neighbourlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-17 13:17:19.000000 torchmd-1.0.1/torchmd/npzMol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11010 2023-07-17 13:17:19.000000 torchmd-1.0.1/torchmd/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-07-17 13:17:19.000000 torchmd-1.0.1/torchmd/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-17 13:17:19.000000 torchmd-1.0.1/torchmd/systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-17 13:17:19.000000 torchmd-1.0.1/torchmd/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-17 13:17:19.000000 torchmd-1.0.1/torchmd/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:17:51.059529 torchmd-1.0.1/torchmd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-17 13:17:51.000000 torchmd-1.0.1/torchmd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-17 13:17:51.000000 torchmd-1.0.1/torchmd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:17:51.000000 torchmd-1.0.1/torchmd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:17:50.000000 torchmd-1.0.1/torchmd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-17 13:17:51.000000 torchmd-1.0.1/torchmd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 13:17:51.000000 torchmd-1.0.1/torchmd.egg-info/top_level.txt
```

### Comparing `torchmd-1.0.0/LICENSE.md` & `torchmd-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `torchmd-1.0.0/PKG-INFO` & `torchmd-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchmd
-Version: 1.0.0
+Version: 1.0.1
 Summary: TorchMD. Molecular dynamics with pytorch
 Author-email: Acellera <info@acellera.com>
 License: Copyright (c) 2020 Acellera
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `torchmd-1.0.0/README.md` & `torchmd-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `torchmd-1.0.0/pyproject.toml` & `torchmd-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `torchmd-1.0.0/tests/test_torchmd.py` & `torchmd-1.0.1/tests/test_torchmd.py`

 * *Files identical despite different names*

### Comparing `torchmd-1.0.0/torchmd/forcefields/ff_parmed.py` & `torchmd-1.0.1/torchmd/forcefields/ff_parmed.py`

 * *Files identical despite different names*

### Comparing `torchmd-1.0.0/torchmd/forcefields/ff_yaml.py` & `torchmd-1.0.1/torchmd/forcefields/ff_yaml.py`

 * *Files identical despite different names*

### Comparing `torchmd-1.0.0/torchmd/forcefields/forcefield.py` & `torchmd-1.0.1/torchmd/forcefields/forcefield.py`

 * *Files identical despite different names*

### Comparing `torchmd-1.0.0/torchmd/forces.py` & `torchmd-1.0.1/torchmd/forces.py`

 * *Files identical despite different names*

### Comparing `torchmd-1.0.0/torchmd/integrator.py` & `torchmd-1.0.1/torchmd/integrator.py`

 * *Files identical despite different names*

### Comparing `torchmd-1.0.0/torchmd/minimizers.py` & `torchmd-1.0.1/torchmd/minimizers.py`

 * *Files identical despite different names*

### Comparing `torchmd-1.0.0/torchmd/mycalc.py` & `torchmd-1.0.1/torchmd/mycalc.py`

 * *Files identical despite different names*

### Comparing `torchmd-1.0.0/torchmd/neighbourlist.py` & `torchmd-1.0.1/torchmd/neighbourlist.py`

 * *Files identical despite different names*

### Comparing `torchmd-1.0.0/torchmd/parameters.py` & `torchmd-1.0.1/torchmd/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,16 +109,19 @@
         return exclusions
 
     def build_parameters(self, ff, mol, terms):
         uqatomtypes, indexes = np.unique(mol.atomtype, return_inverse=True)
 
         self.mapped_atom_types = torch.tensor(indexes)
         self.charges = torch.tensor(mol.charge.astype(np.float64))
-        self.masses = self.make_masses(ff, mol.atomtype)
-        if "lj" in terms or "LJ" in terms:
+        if mol.masses is not None and isinstance(mol.masses, torch.Tensor):
+            self.masses = mol.masses
+        else:
+            self.masses = self.make_masses(ff, mol.atomtype)
+        if any(elem in terms for elem in ["lj", "repulsioncg", "repulsion"]):
             self.A, self.B = self.make_lj(ff, uqatomtypes)
         if "bonds" in terms and len(mol.bonds):
             uqbonds = np.unique([sorted(bb) for bb in mol.bonds], axis=0)
             self.bonds = torch.tensor(uqbonds.astype(np.int64))
             self.bond_params = self.make_bonds(ff, uqatomtypes[indexes[uqbonds]])
         if "angles" in terms and len(mol.angles):
             uqangles = np.unique(
```

### Comparing `torchmd-1.0.0/torchmd/run.py` & `torchmd-1.0.1/torchmd/run.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 from torchmd.parameters import Parameters
 from torchmd.forces import Forces
 from torchmd.integrator import Integrator
 from torchmd.wrapper import Wrapper
 import numpy as np
 from tqdm import tqdm
 import argparse
-import math
 import importlib
 from torchmd.integrator import maxwell_boltzmann
 from torchmd.utils import save_argparse, LogWriter, LoadFromFile
 from torchmd.minimizers import minimize_bfgs
+from npzMol import npzMolecule
+from utils import converter_xyz_output
 
 FS2NS = 1e-6
 
 
 def viewFrame(mol, pos, forces):
     from ffevaluation.ffevaluate import viewForces
 
@@ -120,14 +121,17 @@
     )
     parser.add_argument(
         "--exclusions",
         default=("bonds", "angles", "1-4"),
         type=tuple,
         help="exclusions for the LJ or repulsionCG term",
     )
+    parser.add_argument(
+        "--npz_file", default=None, type=str, help="Input file.npz with coord and z"
+    )
 
     args = parser.parse_args(args=arguments)
     os.makedirs(args.log_dir, exist_ok=True)
     save_argparse(args, os.path.join(args.log_dir, "input.yaml"), exclude="conf")
 
     if isinstance(args.forceterms, str):
         args.forceterms = [args.forceterms]
@@ -140,15 +144,15 @@
 
     return args
 
 
 precisionmap = {"single": torch.float, "double": torch.double}
 
 
-def setup(args):
+def setup(args, batch_comp=False):
     torch.manual_seed(args.seed)
     torch.cuda.manual_seed_all(args.seed)
     # We want to set TF32 to false by default to avoid precision problems
     torch.backends.cuda.matmul.allow_tf32 = False
     torch.backends.cudnn.allow_tf32 = False
     device = torch.device(args.device)
 
@@ -157,14 +161,17 @@
     elif args.structure is not None:
         mol = Molecule(args.structure)
         mol.box = (
             np.array([mol.crystalinfo["a"], mol.crystalinfo["b"], mol.crystalinfo["c"]])
             .reshape(3, 1)
             .astype(np.float32)
         )
+    elif args.npz_file is not None:
+        mol = npzMolecule(args.npz_file)
+        batch_comp = True
 
     if args.coordinates is not None:
         mol.read(args.coordinates)
 
     if args.extended_system is not None:
         mol.read(args.extended_system)
 
@@ -175,16 +182,28 @@
     parameters = Parameters(
         ff, mol, args.forceterms, precision=precision, device=device
     )
 
     external = None
     if args.external is not None:
         externalmodule = importlib.import_module(args.external["module"])
-        embeddings = torch.tensor(args.external["embeddings"]).repeat(args.replicas, 1)
-        external = externalmodule.External(args.external["file"], embeddings, device)
+        if batch_comp:
+            embeddings = torch.tensor(mol.embedding).repeat(args.replicas, 1)
+        else:
+            embeddings = torch.tensor(args.external["embeddings"]).repeat(
+                args.replicas, 1
+            )
+        output_transform = (
+            args.external["output_transform"]
+            if "output_transform" in args.external
+            else None
+        )
+        external = externalmodule.External(
+            args.external["file"], embeddings, device, output_transform
+        )
 
     system = System(mol.numAtoms, args.replicas, precision, device)
     system.set_positions(mol.coords)
     system.set_box(mol.box)
     system.set_velocities(
         maxwell_boltzmann(parameters.masses, args.temperature, args.replicas)
     )
@@ -201,15 +220,14 @@
     return mol, system, forces
 
 
 def dynamics(args, mol, system, forces):
     torch.manual_seed(args.seed)
     torch.cuda.manual_seed_all(args.seed)
     device = torch.device(args.device)
-
     integrator = Integrator(
         system,
         forces,
         args.timestep,
         device,
         gamma=args.langevin_gamma,
         T=args.langevin_temperature,
@@ -230,14 +248,15 @@
         trajs.append([])
 
     if args.minimize != None:
         minimize_bfgs(system, forces, steps=args.minimize)
 
     iterator = tqdm(range(1, int(args.steps / args.output_period) + 1))
     Epot = forces.compute(system.pos, system.box, system.forces)
+
     for i in iterator:
         # viewFrame(mol, system.pos, system.forces)
         Ekin, Epot, T = integrator.step(niter=args.output_period)
         wrapper.wrap(system.pos, system.box)
         currpos = system.pos.detach().cpu().numpy().copy()
         for k in range(args.replicas):
             trajs[k].append(currpos[k])
@@ -254,12 +273,18 @@
                     "epot": Epot[k],
                     "ekin": Ekin[k],
                     "etot": Epot[k] + Ekin[k],
                     "T": T[k],
                 }
             )
 
+    # new for on replicas because we start from .npy file saved in the previous step
+    for k in range(args.replicas):
+        npy_name = os.path.join(args.log_dir, args.output + f"_{k}.npy")
+        xyz_name = os.path.join(args.log_dir, args.output + f"_{k}.xyz")
+        converter_xyz_output(npy_name, xyz_name, mol.z)
+
 
 if __name__ == "__main__":
     args = get_args()
     mol, system, forces = setup(args)
     dynamics(args, mol, system, forces)
```

### Comparing `torchmd-1.0.0/torchmd/systems.py` & `torchmd-1.0.1/torchmd/systems.py`

 * *Files identical despite different names*

### Comparing `torchmd-1.0.0/torchmd/utils.py` & `torchmd-1.0.1/torchmd/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import csv
 import json
 import os
+import numpy as np
 import time
 import argparse
 import yaml
 
 
 class LogWriter(object):
     # kind of inspired form openai.baselines.bench.monitor
@@ -68,7 +69,29 @@
             yaml.dump(args, fout)
     else:
         with open(filename, "w") as f:
             for k, v in args.__dict__.items():
                 if k is exclude:
                     continue
                 f.write(f"{k}={v}\n")
+
+
+def converter_xyz_output(input_file, output_file, z=None):
+    from moleculekit.periodictable import periodictable_by_number
+    # it gets the embedding data from the mol.z attribute
+    mol_elements = np.array(z)
+    npy_file = np.load(input_file)
+    Nsteps = npy_file.shape[2]
+    Nats = npy_file.shape[0]
+    for i in range(Nsteps):
+        with open(output_file, "a") as f:
+            if "forces" not in input_file:
+                f.write(str(Nats))
+            f.write("\n\n")
+            for j in range(Nats):
+                if "forces" not in input_file:
+                    f.write(periodictable_by_number[mol_elements[j]].symbol)
+                    f.write(" ")
+                for k in range(3):
+                    f.write(str(npy_file[j, k, i]))
+                    f.write(" ")
+                f.write("\n")
```

### Comparing `torchmd-1.0.0/torchmd/wrapper.py` & `torchmd-1.0.1/torchmd/wrapper.py`

 * *Files identical despite different names*

### Comparing `torchmd-1.0.0/torchmd.egg-info/PKG-INFO` & `torchmd-1.0.1/torchmd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchmd
-Version: 1.0.0
+Version: 1.0.1
 Summary: TorchMD. Molecular dynamics with pytorch
 Author-email: Acellera <info@acellera.com>
 License: Copyright (c) 2020 Acellera
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `torchmd-1.0.0/torchmd.egg-info/SOURCES.txt` & `torchmd-1.0.1/torchmd.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 torchmd/__init__.py
 torchmd/_version.py
 torchmd/forces.py
 torchmd/integrator.py
 torchmd/minimizers.py
 torchmd/mycalc.py
 torchmd/neighbourlist.py
+torchmd/npzMol.py
 torchmd/parameters.py
 torchmd/run.py
 torchmd/systems.py
 torchmd/utils.py
 torchmd/wrapper.py
 torchmd.egg-info/PKG-INFO
 torchmd.egg-info/SOURCES.txt
```

