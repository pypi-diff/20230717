# Comparing `tmp/pylammpsmpi-0.1.2.tar.gz` & `tmp/pylammpsmpi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylammpsmpi-0.1.2.tar", last modified: Sun Jun 11 16:16:10 2023, max compression
+gzip compressed data, was "pylammpsmpi-0.2.0.tar", last modified: Mon Jul 17 21:17:25 2023, max compression
```

## Comparing `pylammpsmpi-0.1.2.tar` & `pylammpsmpi-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:16:10.906684 pylammpsmpi-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-11 16:16:07.000000 pylammpsmpi-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-11 16:16:07.000000 pylammpsmpi-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-11 16:16:10.906684 pylammpsmpi-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-11 16:16:07.000000 pylammpsmpi-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:16:10.906684 pylammpsmpi-0.1.2/pylammpsmpi/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-11 16:16:07.000000 pylammpsmpi-0.1.2/pylammpsmpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-11 16:16:10.906684 pylammpsmpi-0.1.2/pylammpsmpi/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-06-11 16:16:07.000000 pylammpsmpi-0.1.2/pylammpsmpi/lammps_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:16:10.906684 pylammpsmpi-0.1.2/pylammpsmpi/mpi/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 16:16:07.000000 pylammpsmpi-0.1.2/pylammpsmpi/mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13743 2023-06-11 16:16:07.000000 pylammpsmpi-0.1.2/pylammpsmpi/mpi/lmpmpi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:16:10.906684 pylammpsmpi-0.1.2/pylammpsmpi/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 16:16:07.000000 pylammpsmpi-0.1.2/pylammpsmpi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-11 16:16:07.000000 pylammpsmpi-0.1.2/pylammpsmpi/utils/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    19121 2023-06-11 16:16:07.000000 pylammpsmpi-0.1.2/pylammpsmpi/utils/lammps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:16:10.906684 pylammpsmpi-0.1.2/pylammpsmpi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-11 16:16:10.000000 pylammpsmpi-0.1.2/pylammpsmpi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-11 16:16:10.000000 pylammpsmpi-0.1.2/pylammpsmpi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 16:16:10.000000 pylammpsmpi-0.1.2/pylammpsmpi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-11 16:16:10.000000 pylammpsmpi-0.1.2/pylammpsmpi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-11 16:16:10.000000 pylammpsmpi-0.1.2/pylammpsmpi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-11 16:16:10.906684 pylammpsmpi-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-11 16:16:10.000000 pylammpsmpi-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:16:10.906684 pylammpsmpi-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-11 16:16:07.000000 pylammpsmpi-0.1.2/tests/test_pylammpsmpi_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-11 16:16:07.000000 pylammpsmpi-0.1.2/tests/test_pylammpsmpi_local.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-11 16:16:07.000000 pylammpsmpi-0.1.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:17:25.476988 pylammpsmpi-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-17 21:17:22.000000 pylammpsmpi-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-17 21:17:22.000000 pylammpsmpi-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-17 21:17:25.476988 pylammpsmpi-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-17 21:17:22.000000 pylammpsmpi-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:17:25.476988 pylammpsmpi-0.2.0/pylammpsmpi/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-17 21:17:22.000000 pylammpsmpi-0.2.0/pylammpsmpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-17 21:17:25.476988 pylammpsmpi-0.2.0/pylammpsmpi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:17:25.476988 pylammpsmpi-0.2.0/pylammpsmpi/mpi/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 21:17:22.000000 pylammpsmpi-0.2.0/pylammpsmpi/mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13805 2023-07-17 21:17:22.000000 pylammpsmpi-0.2.0/pylammpsmpi/mpi/lmpmpi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:17:25.476988 pylammpsmpi-0.2.0/pylammpsmpi/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:17:22.000000 pylammpsmpi-0.2.0/pylammpsmpi/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14979 2023-07-17 21:17:22.000000 pylammpsmpi-0.2.0/pylammpsmpi/wrapper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20729 2023-07-17 21:17:22.000000 pylammpsmpi-0.2.0/pylammpsmpi/wrapper/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-07-17 21:17:22.000000 pylammpsmpi-0.2.0/pylammpsmpi/wrapper/extended.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:17:25.476988 pylammpsmpi-0.2.0/pylammpsmpi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-17 21:17:25.000000 pylammpsmpi-0.2.0/pylammpsmpi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-17 21:17:25.000000 pylammpsmpi-0.2.0/pylammpsmpi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 21:17:25.000000 pylammpsmpi-0.2.0/pylammpsmpi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-17 21:17:25.000000 pylammpsmpi-0.2.0/pylammpsmpi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 21:17:25.000000 pylammpsmpi-0.2.0/pylammpsmpi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-17 21:17:25.476988 pylammpsmpi-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-17 21:17:25.000000 pylammpsmpi-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:17:25.476988 pylammpsmpi-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-17 21:17:22.000000 pylammpsmpi-0.2.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-17 21:17:22.000000 pylammpsmpi-0.2.0/tests/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-17 21:17:22.000000 pylammpsmpi-0.2.0/tests/test_pylammpsmpi_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-17 21:17:22.000000 pylammpsmpi-0.2.0/versioneer.py
```

### Comparing `pylammpsmpi-0.1.2/LICENSE` & `pylammpsmpi-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.1.2/PKG-INFO` & `pylammpsmpi-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylammpsmpi
-Version: 0.1.2
+Version: 0.2.0
 Summary: Parallel Lammps Python interface
 Home-page: https://github.com/pyiron/pylammpsmpi
 Author: Jan Janssen
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: lammps,mpi4py
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pylammpsmpi-0.1.2/README.md` & `pylammpsmpi-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.1.2/pylammpsmpi/mpi/lmpmpi.py` & `pylammpsmpi-0.2.0/pylammpsmpi/mpi/lmpmpi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 from ctypes import c_double, c_int
 from mpi4py import MPI
 import numpy as np
-import cloudpickle
 import sys
-import zmq
 from lammps import lammps
+from pympipool import (
+    connect_to_socket_interface,
+    send_result,
+    close_connection,
+    receive_instruction,
+)
 
 __author__ = "Sarath Menon, Jan Janssen"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
@@ -456,43 +460,41 @@
             for v in vl:
                 data.append(v)
         return data
 
 
 def _run_lammps_mpi(argument_lst):
     if MPI.COMM_WORLD.rank == 0:
-        context = zmq.Context()
-        socket = context.socket(zmq.PAIR)
         port_selected = argument_lst[argument_lst.index("--zmqport") + 1]
-        socket.connect("tcp://localhost:" + port_selected)
+        if "--host" in argument_lst:
+            host = argument_lst[argument_lst.index("--host") + 1]
+        else:
+            host = "localhost"
+        context, socket = connect_to_socket_interface(host=host, port=port_selected)
     else:
         context, socket = None, None
     # Lammps executable
     args = ["-screen", "none"]
     if len(argument_lst) > 3:
         args.extend(argument_lst[3:])
     job = lammps(cmdargs=args)
     while True:
         if MPI.COMM_WORLD.rank == 0:
-            input_dict = cloudpickle.loads(socket.recv())
-            # with open('process.txt', 'a') as file:
-            #     print('Input:', input_dict, file=file)
+            input_dict = receive_instruction(socket=socket)
         else:
             input_dict = None
         input_dict = MPI.COMM_WORLD.bcast(input_dict, root=0)
         if "shutdown" in input_dict.keys() and input_dict["shutdown"]:
-            if MPI.COMM_WORLD.rank == 0:
-                socket.close()
-                context.term()
             job.close()
+            if MPI.COMM_WORLD.rank == 0:
+                send_result(socket=socket, result_dict={"result": True})
+                close_connection(socket=socket, context=context)
             break
         output = select_cmd(input_dict["command"])(
             job=job, funct_args=input_dict["args"]
         )
         if MPI.COMM_WORLD.rank == 0 and output is not None:
-            # with open('process.txt', 'a') as file:
-            #     print('Output:', output, file=file)
-            socket.send(cloudpickle.dumps({"result": output}))
+            send_result(socket=socket, result_dict={"result": output})
 
 
 if __name__ == "__main__":
     _run_lammps_mpi(argument_lst=sys.argv)
```

### Comparing `pylammpsmpi-0.1.2/pylammpsmpi/utils/lammps.py` & `pylammpsmpi-0.2.0/pylammpsmpi/wrapper/concurrent.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,95 +1,135 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import os
-from pympipool import SocketInterface
+import socket
+from concurrent.futures import Future
+from queue import Queue
+from threading import Thread
+from pympipool import SocketInterface, cancel_items_in_queue
 
 
 __author__ = "Sarath Menon, Jan Janssen"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "production"
 __date__ = "Feb 28, 2020"
 
 
-class LammpsBase:
+def _initialize_socket(
+    interface, cmdargs, cwd, cores, oversubscribe=False, enable_flux_backend=False
+):
+    port_selected = interface.bind_to_random_port()
+    executable = os.path.join(
+        os.path.dirname(os.path.abspath(__file__)), "../mpi", "lmpmpi.py"
+    )
+    if enable_flux_backend:
+        cmds = ["flux", "run"]
+    else:
+        cmds = ["mpiexec"]
+    if oversubscribe:
+        cmds += ["--oversubscribe"]
+    cmds += [
+        "-n",
+        str(cores),
+        "python",
+        executable,
+        "--zmqport",
+        str(port_selected),
+    ]
+    if enable_flux_backend:
+        cmds += [
+            "--host",
+            socket.gethostname(),
+        ]
+    if cmdargs is not None:
+        cmds.extend(cmdargs)
+    interface.bootup(command_lst=cmds, cwd=cwd)
+    return interface
+
+
+def execute_async(
+    future_queue,
+    cmdargs,
+    cores,
+    oversubscribe=False,
+    enable_flux_backend=False,
+    cwd=None,
+    queue_adapter=None,
+    queue_adapter_kwargs=None,
+):
+    interface = _initialize_socket(
+        interface=SocketInterface(
+            queue_adapter=queue_adapter, queue_adapter_kwargs=queue_adapter_kwargs
+        ),
+        cmdargs=cmdargs,
+        cwd=cwd,
+        cores=cores,
+        enable_flux_backend=enable_flux_backend,
+        oversubscribe=oversubscribe,
+    )
+    while True:
+        task_dict = future_queue.get()
+        if "shutdown" in task_dict.keys() and task_dict["shutdown"]:
+            interface.shutdown(wait=task_dict["wait"])
+            break
+        elif "command" in task_dict.keys() and "future" in task_dict.keys():
+            f = task_dict.pop("future")
+            if f.set_running_or_notify_cancel():
+                f.set_result(interface.send_and_receive_dict(input_dict=task_dict))
+
+
+class LammpsConcurrent:
     def __init__(
-        self, cores=8, oversubscribe=False, working_directory=".", cmdargs=None
+        self,
+        cores=8,
+        oversubscribe=False,
+        enable_flux_backend=False,
+        working_directory=".",
+        cmdargs=None,
+        queue_adapter=None,
+        queue_adapter_kwargs=None,
     ):
         self.cores = cores
         self.working_directory = working_directory
-        self._interface = SocketInterface()
+        self._future_queue = Queue()
         self._process = None
         self._oversubscribe = oversubscribe
+        self._enable_flux_backend = enable_flux_backend
         self._cmdargs = cmdargs
+        self._queue_adapter = queue_adapter
+        self._queue_adapter_kwargs = queue_adapter_kwargs
 
     def start_process(self):
-        port_selected = self._interface.bind_to_random_port()
-        executable = os.path.join(
-            os.path.dirname(os.path.abspath(__file__)), "../mpi", "lmpmpi.py"
+        self._process = Thread(
+            target=execute_async,
+            kwargs={
+                "future_queue": self._future_queue,
+                "cmdargs": self._cmdargs,
+                "cores": self.cores,
+                "oversubscribe": self._oversubscribe,
+                "enable_flux_backend": self._enable_flux_backend,
+                "cwd": self.working_directory,
+                "queue_adapter": self._queue_adapter,
+                "queue_adapter_kwargs": self._queue_adapter_kwargs,
+            },
         )
-        cmds = ["mpiexec"]
-        if self._oversubscribe:
-            cmds += ["--oversubscribe"]
-        cmds += [
-            "-n",
-            str(self.cores),
-            "python",
-            executable,
-            "--zmqport",
-            str(port_selected),
-        ]
-        if self._cmdargs is not None:
-            cmds.extend(self._cmdargs)
-        self._interface.bootup(command_lst=cmds, cwd=self.working_directory)
+        self._process.start()
 
     def _send_and_receive_dict(self, command, data=None):
-        return self._interface.send_and_receive_dict(
-            input_dict={"command": command, "args": data}
-        )
-
-    def _send(self, command, data=None):
-        """
-        Send a command to the Lammps Library executable
-
-        Parameters
-        ----------
-        command : string
-            command to be send to the
-
-        data: optional, default None
-            data to be sent to the command
-
-        Returns
-        -------
-        None
-        """
-        self._interface.send_dict({"command": command, "args": data})
-
-    def _receive(self):
-        """
-        Receive data from the Lammps library
-
-        Parameters
-        ----------
-        None
-
-        Returns
-        -------
-        data : string
-            data from the command
-        """
-        return self._interface.receive_dict()
+        f = Future()
+        self._future_queue.put({"command": command, "args": data, "future": f})
+        return f
 
     @property
     def version(self):
         """
         Get the version of lammps
 
         Parameters
@@ -114,15 +154,15 @@
 
         Returns
         -------
         None
         """
         if not os.path.exists(inputfile):
             raise FileNotFoundError("Input file does not exist")
-        _ = self._send_and_receive_dict(command="get_file", data=[inputfile])
+        return self._send_and_receive_dict(command="get_file", data=[inputfile])
 
     # TODO
     def extract_setting(self, *args):
         return self._send_and_receive_dict(command="extract_setting", data=list(args))
 
     def extract_global(self, name):
         """
@@ -306,15 +346,15 @@
 
         boxhi: array of floats
             upper bound of box in three dimensions
 
         xy, yz, xz : floats
             box tilts
         """
-        _ = self._send_and_receive_dict(command="reset_box", data=list(args))
+        return self._send_and_receive_dict(command="reset_box", data=list(args))
 
     def generate_atoms(
         self, ids=None, type=None, x=None, v=None, image=None, shrinkexceed=False
     ):
         """
         Create atoms on all procs
 
@@ -340,15 +380,15 @@
             default False
 
         Returns
         -------
         None
 
         """
-        self.create_atoms(
+        return self.create_atoms(
             ids=ids, type=type, x=x, v=v, image=image, shrinkexceed=shrinkexceed
         )
 
     def create_atoms(self, n, id, type, x, v=None, image=None, shrinkexceed=False):
         """
         Create atoms on all procs
 
@@ -380,15 +420,15 @@
         -------
         None
 
         """
 
         if x is not None:
             funct_args = [n, id, type, x, v, image, shrinkexceed]
-            _ = self._send_and_receive_dict(command="create_atoms", data=funct_args)
+            return self._send_and_receive_dict(command="create_atoms", data=funct_args)
         else:
             raise TypeError("Value of x cannot be None")
 
     @property
     def has_exceptions(self):
         """Return whether the LAMMPS shared library was compiled with C++ exceptions handling enabled"""
         return self._send_and_receive_dict(command="has_exceptions", data=[])
@@ -410,15 +450,15 @@
         return self._send_and_receive_dict(command="has_ffmpeg_support", data=[])
 
     @property
     def installed_packages(self):
         return self._send_and_receive_dict(command="get_installed_packages", data=[])
 
     def set_fix_external_callback(self, *args):
-        _ = self._send_and_receive_dict(
+        return self._send_and_receive_dict(
             command="set_fix_external_callback", data=list(args)
         )
 
     def get_neighlist(self, *args):
         """Returns an instance of :class:`NeighList` which wraps access to the neighbor list with the given index
         :param idx: index of neighbor list
         :type  idx: int
@@ -503,21 +543,21 @@
             command to be sent
 
         Returns
         -------
         None
         """
         if isinstance(cmd, list):
-            for c in cmd:
-                _ = self._send_and_receive_dict(command="command", data=c)
+            return self._send_and_receive_dict(
+                command="commands_string", data="\n".join(cmd)
+            )
         elif len(cmd.split("\n")) > 1:
-            for c in cmd.split("\n"):
-                _ = self._send_and_receive_dict(command="command", data=c)
+            return self._send_and_receive_dict(command="commands_string", data=cmd)
         else:
-            _ = self._send_and_receive_dict(command="command", data=cmd)
+            return self._send_and_receive_dict(command="command", data=cmd)
 
     def gather_atoms(self, *args, concat=False, ids=None):
         """
         Gather atom properties
 
         Parameters
         ----------
@@ -568,17 +608,19 @@
             *args:
         """
         if ids is not None:
             lenids = len(ids)
             args = list(args)
             args.append(len(ids))
             args.append(ids)
-            _ = self._send_and_receive_dict(command="scatter_atoms_subset", data=args)
+            return self._send_and_receive_dict(
+                command="scatter_atoms_subset", data=args
+            )
         else:
-            _ = self._send_and_receive_dict(command="scatter_atoms", data=list(args))
+            return self._send_and_receive_dict(command="scatter_atoms", data=list(args))
 
     def get_thermo(self, *args):
         """
         Return current value of thermo keyword
 
         Parameters
         ----------
@@ -637,13 +679,16 @@
         ----------
         None
 
         Returns
         -------
         None
         """
-        self._interface.shutdown(wait=True)
+        cancel_items_in_queue(que=self._future_queue)
+        self._future_queue.put({"shutdown": True, "wait": True})
+        self._process.join()
+        self._process = None
 
     # TODO
     def __del__(self):
         if self._process is not None:
             self.close()
```

### Comparing `pylammpsmpi-0.1.2/pylammpsmpi.egg-info/PKG-INFO` & `pylammpsmpi-0.2.0/pylammpsmpi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylammpsmpi
-Version: 0.1.2
+Version: 0.2.0
 Summary: Parallel Lammps Python interface
 Home-page: https://github.com/pyiron/pylammpsmpi
 Author: Jan Janssen
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: lammps,mpi4py
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pylammpsmpi-0.1.2/setup.py` & `pylammpsmpi-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,11 +22,11 @@
                  'Programming Language :: Python :: 3.10',
                  'Programming Language :: Python :: 3.11'
                 ],
 
     keywords='lammps, mpi4py',
     packages=find_packages(exclude=["*tests*"]),
     install_requires=[
-        "cloudpickle>=2.2.1", "mpi4py>=3.1.4", "pympipool>=0.5.0", "pyzmq>=25.1.0",
+        "mpi4py>=3.1.4", "pympipool>=0.5.4", "numpy>=1.23.5"
     ],
     cmdclass=versioneer.get_cmdclass(),
 )
```

### Comparing `pylammpsmpi-0.1.2/tests/test_pylammpsmpi_cluster.py` & `pylammpsmpi-0.2.0/tests/test_concurrent.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,101 +1,99 @@
-# coding: utf-8
-# Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
-# Distributed under the terms of "New BSD License", see the LICENSE file.
-
 import unittest
-import os
 import numpy as np
-from pylammpsmpi import LammpsLibrary
-from dask.distributed import Client, LocalCluster
+import os
+from pylammpsmpi import LammpsConcurrent
 
 
-class TestLocalLammpsLibrary(unittest.TestCase):
+class TestLammpsConcurrent(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.execution_path = os.path.dirname(os.path.abspath(__file__))
         cls.citation_file = os.path.join(cls.execution_path, "citations.txt")
         cls.lammps_file = os.path.join(cls.execution_path, "in.simple")
-        cluster = LocalCluster(
-            n_workers=1,
-            threads_per_worker=2
-        )
-        client = Client(cluster)
-        cls.lmp = LammpsLibrary(
-            cores=2,
-            mode='dask',
-            cmdargs=["-cite", cls.citation_file],
-            client=client
+        cls.lmp = LammpsConcurrent(
+            cores=1,
+            oversubscribe=False,
+            enable_flux_backend=False,
+            working_directory=".",
+            cmdargs=["-cite", cls.citation_file]
         )
-        cls.lmp.file(cls.lammps_file)
+        cls.lmp.start_process()
+        cls.lmp.file(cls.lammps_file).result()
 
     @classmethod
     def tearDownClass(cls):
         cls.lmp.close()
 
     def test_extract_atom(self):
-        f = self.lmp.extract_atom("f")
+        f = self.lmp.extract_atom("f").result()
         self.assertEqual(len(f), 256)
         self.assertEqual(np.round(f[0][0], 2), -0.26)
 
-        ids = self.lmp.extract_atom("id")
+        ids = self.lmp.extract_atom("id").result()
         self.assertEqual(len(ids), 256)
 
+    def test_extract_compute_global(self):
+        compute_temp = self.lmp.extract_compute("1", 0, 0).result()
+        self.assertIsInstance(compute_temp, float)
+
+    def test_extract_compute_per_atom(self):
+        compute_ke_atom = self.lmp.extract_compute("ke", 1, 1).result()
+        self.assertEqual(len(compute_ke_atom), 256)
+
     def test_gather_atoms(self):
-        f = self.lmp.gather_atoms("f")
+        f = self.lmp.gather_atoms("f").result()
         self.assertEqual(len(f), 256)
         # this checks if info was gathered from
         # all processors
         self.assertEqual(np.round(f[-22][0], 2), 0.31)
 
-        ids = self.lmp.extract_atom("id")
+        ids = self.lmp.extract_atom("id").result()
         self.assertEqual(len(ids), 256)
 
     def test_extract_fix(self):
-        x = self.lmp.extract_fix("2", 0, 1, 1)
+        x = self.lmp.extract_fix("2", 0, 1, 1).result()
         self.assertEqual(np.round(x, 2), -2.61)
 
     def test_extract_variable(self):
-        x = self.lmp.extract_variable("tt", "all", 0)
+        x = self.lmp.extract_variable("tt", "all", 0).result()
         self.assertEqual(np.round(x, 2), 1.13)
-
-        x = self.lmp.extract_variable("fx", "all", 1)
+        x = self.lmp.extract_variable("fx", "all", 1).result()
         self.assertEqual(len(x), 256)
         self.assertEqual(np.round(x[0], 2), -0.26)
 
     def test_scatter_atoms(self):
-        f = self.lmp.gather_atoms("f")
+        f = self.lmp.gather_atoms("f").result()
         val = np.random.randint(0, 100)
         f[1][0] = val
-        self.lmp.scatter_atoms("f", f)
-        f1 = self.lmp.gather_atoms("f")
+        self.lmp.scatter_atoms("f", f).result()
+        f1 = self.lmp.gather_atoms("f").result()
         self.assertEqual(f1[1][0], val)
 
-        f = self.lmp.gather_atoms("f", ids=[1, 2])
+        f = self.lmp.gather_atoms("f", ids=[1, 2]).result()
         val = np.random.randint(0, 100)
         f[1][1] = val
-        self.lmp.scatter_atoms("f", f, ids=[1, 2])
-        f1 = self.lmp.gather_atoms("f", ids=[1, 2])
+        self.lmp.scatter_atoms("f", f, ids=[1, 2]).result()
+        f1 = self.lmp.gather_atoms("f", ids=[1, 2]).result()
         self.assertEqual(f1[1][1], val)
 
     def test_extract_box(self):
-        box = self.lmp.extract_box()
+        box = self.lmp.extract_box().result()
         self.assertEqual(len(box), 7)
 
         self.assertEqual(box[0][0], 0.0)
         self.assertEqual(np.round(box[1][0], 2), 6.72)
 
-        self.lmp.delete_atoms("group", "all")
-        self.lmp.reset_box([0.0, 0.0, 0.0], [8.0, 8.0, 8.0], 0.0, 0.0, 0.0)
-        box = self.lmp.extract_box()
+        self.lmp.command("delete_atoms group all").result()
+        self.lmp.reset_box([0.0, 0.0, 0.0], [8.0, 8.0, 8.0], 0.0, 0.0, 0.0).result()
+        box = self.lmp.extract_box().result()
         self.assertEqual(box[0][0], 0.0)
         self.assertEqual(np.round(box[1][0], 2), 8.0)
-        self.lmp.clear()
-        self.lmp.file(self.lammps_file)
+        self.lmp.command("clear")
+        self.lmp.file(self.lammps_file).result()
 
     def test_cmdarg_options(self):
         self.assertTrue(os.path.isfile(self.citation_file))
 
 
 if __name__ == "__main__":
     unittest.main()
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pylammpsmpi-0.1.2/tests/test_pylammpsmpi_local.py` & `pylammpsmpi-0.2.0/tests/test_pylammpsmpi_local.py`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.1.2/versioneer.py` & `pylammpsmpi-0.2.0/versioneer.py`

 * *Files identical despite different names*

