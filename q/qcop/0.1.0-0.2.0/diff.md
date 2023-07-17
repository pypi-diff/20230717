# Comparing `tmp/qcop-0.1.0.tar.gz` & `tmp/qcop-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcop-0.1.0.tar", max compression
+gzip compressed data, was "qcop-0.2.0.tar", max compression
```

## Comparing `qcop-0.1.0.tar` & `qcop-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0     1079 2023-06-30 03:15:39.777848 qcop-0.1.0/LICENSE
--rw-r--r--   0        0        0      851 2023-06-30 03:15:39.777848 qcop-0.1.0/README.md
--rw-r--r--   0        0        0     1336 2023-06-30 03:15:39.777848 qcop-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       40 2023-06-30 03:15:39.777848 qcop-0.1.0/qcop/__init__.py
--rw-r--r--   0        0        0      153 2023-06-30 03:15:39.777848 qcop-0.1.0/qcop/adapters/__init__.py
--rw-r--r--   0        0        0     4560 2023-06-30 03:15:39.777848 qcop-0.1.0/qcop/adapters/base.py
--rw-r--r--   0        0        0     1381 2023-06-30 03:15:39.777848 qcop-0.1.0/qcop/adapters/file.py
--rw-r--r--   0        0        0     4495 2023-06-30 03:15:39.777848 qcop-0.1.0/qcop/adapters/terachem.py
--rw-r--r--   0        0        0      164 2023-06-30 03:15:39.777848 qcop-0.1.0/qcop/adapters/xtb.py
--rw-r--r--   0        0        0     3338 2023-06-30 03:15:39.781848 qcop-0.1.0/qcop/exceptions.py
--rw-r--r--   0        0        0     7855 2023-06-30 03:15:39.781848 qcop-0.1.0/qcop/main.py
--rw-r--r--   0        0        0     6485 2023-06-30 03:15:39.781848 qcop-0.1.0/qcop/utils.py
--rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 qcop-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-07-17 21:30:07.975420 qcop-0.2.0/LICENSE
+-rw-r--r--   0        0        0      851 2023-07-17 21:30:07.975420 qcop-0.2.0/README.md
+-rw-r--r--   0        0        0     1336 2023-07-17 21:30:07.975420 qcop-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       40 2023-07-17 21:30:07.975420 qcop-0.2.0/qcop/__init__.py
+-rw-r--r--   0        0        0      182 2023-07-17 21:30:07.975420 qcop-0.2.0/qcop/adapters/__init__.py
+-rw-r--r--   0        0        0     4409 2023-07-17 21:30:07.975420 qcop-0.2.0/qcop/adapters/base.py
+-rw-r--r--   0        0        0     1317 2023-07-17 21:30:07.975420 qcop-0.2.0/qcop/adapters/file.py
+-rw-r--r--   0        0        0     1924 2023-07-17 21:30:07.975420 qcop-0.2.0/qcop/adapters/qcengine.py
+-rw-r--r--   0        0        0     4058 2023-07-17 21:30:07.975420 qcop-0.2.0/qcop/adapters/terachem.py
+-rw-r--r--   0        0        0     4039 2023-07-17 21:30:07.975420 qcop-0.2.0/qcop/adapters/utils.py
+-rw-r--r--   0        0        0      164 2023-07-17 21:30:07.975420 qcop-0.2.0/qcop/adapters/xtb.py
+-rw-r--r--   0        0        0     3324 2023-07-17 21:30:07.975420 qcop-0.2.0/qcop/exceptions.py
+-rw-r--r--   0        0        0     8354 2023-07-17 21:30:07.975420 qcop-0.2.0/qcop/main.py
+-rw-r--r--   0        0        0     5044 2023-07-17 21:30:07.975420 qcop-0.2.0/qcop/utils.py
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 qcop-0.2.0/PKG-INFO
```

### Comparing `qcop-0.1.0/LICENSE` & `qcop-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qcop-0.1.0/README.md` & `qcop-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `qcop-0.1.0/pyproject.toml` & `qcop-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "qcop"
-version = "0.1.0"
+version = "0.2.0"
 description = "A package for operating Quantum Chemistry programs using qcio standardized data structures."
 authors = ["Colton Hicks <github@coltonhicks.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
-qcio = ">=0.2.1"
-qcparse = ">=0.3.1"
+qcio = ">=0.3.0"
+qcparse = ">=0.4.0"
 qcengine = { extras = ["qcengine"], version = ">=0.26.0" }
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 mypy = "^1.3.0"
 pytest = "^7.3.2"
```

### Comparing `qcop-0.1.0/qcop/adapters/base.py` & `qcop-0.2.0/qcop/adapters/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from abc import ABC, abstractmethod
-from typing import Callable, List, Optional
+from typing import Callable, List, Optional, Tuple
 
-from qcio.models.base_io import ComputedPropertiesBase, InputBase
-from qcio.models.single_point import SinglePointComputedProperties
+from qcio import InputBase, ResultsBase
 
 from qcop.exceptions import UnsupportedCalcTypeError
 
 __all__ = ["BaseAdapter", "registry"]
 
 # Registry for all Adaptors
 registry = {}
@@ -25,15 +24,15 @@
 
     @abstractmethod
     def compute(
         self,
         inp_obj: InputBase,
         update_func: Optional[Callable] = None,
         update_interval: Optional[float] = None,
-    ) -> ComputedPropertiesBase:
+    ) -> Tuple[ResultsBase, str]:
         """Compute the given program on the given files.
 
         Implementations of this function can assume:
             - All input files have already been written to the working directory.
             - Output files requested as output will be collected automatically.
 
         Args:
@@ -42,79 +41,75 @@
                 take the entire stdout/stderr output as a string for its first
                     argument.
             update_interval: The minimum time in seconds between calls to the
                 update_func.
 
 
         Returns:
-            The computed properties object for a computation.
+            Tuple of ResultsBase object and stdout from the program.
         """
 
 
-class QCOPProgramAdapter(BaseAdapter):
-    """Base adapter for all program adapters."""
+class ProgramAdapter(BaseAdapter):
+    """Base adapter for all program adapters (all but FileAdaptor)."""
 
     program: str  # All subclasses must specify program name
+    supported_calctypes: List[str]  # All subclasses must specify supported calctypes
 
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
         # Ensure that subclasses define the required class attributes
         if not getattr(cls, "program", None):
             raise NotImplementedError(
-                f"Subclasses of QCOPProgramAdapter must define a program string. "
-                f"{cls.__name__} does not meet this requirement."
+                f"Subclasses of {ProgramAdapter.__name__} must define a program "
+                f"string. {cls.__name__} does not meet this requirement."
             )
 
         # Automatically register all subclasses
         registry[cls.program] = cls
 
+        if not getattr(cls, "supported_calctypes", None):
+            raise NotImplementedError(
+                f"Subclasses of {ProgramAdapter.__name__} must define a nonempty "
+                f"supported_calctypes list. {cls.__name__} does not meet this "
+                "requirement."
+            )
+
     @abstractmethod
     def program_version(self, stdout: Optional[str]) -> str:
         """Get the version of the program.
 
         Args:
             stdout: The stdout from the program. Because running "program --version"
                 can be extremely slow for some programs, the stdout from the program
                 is passed in here so that the version can be extracted from it if
                 possible. If the version cannot be extracted from the stdout, then
-                this function should extract the program version in some other way.
+                this function should return the program version in some other way.
         """
 
-
-class QCOPSinglePointAdapter(QCOPProgramAdapter):
-    # TODO: This is a hack. Remove!
-    program = "fake program"
-    supported_calc_types: List[str]  # All subclasses must specify supported drivers
-
-    def __init_subclass__(cls, **kwargs):
-        super().__init_subclass__(**kwargs)
-
-        if not getattr(cls, "supported_calc_types", None):
-            raise NotImplementedError(
-                f"Subclasses of QCOPProgramAdapter must define a nonempty "
-                f"supported_calc_types list. {cls.__name__} does not meet this "
-                "requirement."
-            )
-
     def compute(
         self,
         inp_obj: InputBase,
         update_func: Optional[Callable] = None,
         update_interval: Optional[float] = None,
-    ) -> SinglePointComputedProperties:
-        """Single point compute method."""
-        if inp_obj.program_args.calc_type not in self.supported_calc_types:
+    ) -> Tuple[ResultsBase, str]:
+        """Top level compute method used by external calls.
+
+        Performs all necessary checks and then calls the _compute method which is
+        bespoke to each adapter.
+        """
+        if inp_obj.calctype not in self.supported_calctypes:
             raise UnsupportedCalcTypeError(
                 program=self.program,
-                calc_type=inp_obj.program_args.calc_type,
-                supported_calc_types=self.supported_calc_types,
+                calctype=inp_obj.calctype,
+                supported_calctypes=self.supported_calctypes,
             )
         return self._compute(inp_obj, update_func, update_interval)
 
     @abstractmethod
     def _compute(
         self,
         inp_obj: InputBase,
         update_func: Optional[Callable] = None,
         update_interval: Optional[float] = None,
-    ) -> SinglePointComputedProperties:
+    ) -> Tuple[ResultsBase, str]:
         """Subclasses should implement this method with custom compute logic."""
```

### Comparing `qcop-0.1.0/qcop/adapters/file.py` & `qcop-0.2.0/qcop/adapters/file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,43 @@
-from typing import Callable, Optional
+from typing import Callable, Optional, Tuple
 
-from qcio import FileInput, FileSuccessfulOutput
+from qcio import FileInput, FileOutput
 
 from qcop.adapters.base import BaseAdapter
-from qcop.utils import execute_subprocess
+
+from .utils import execute_subprocess
 
 
 class FileAdapter(BaseAdapter):
     """adapter for running a program on files."""
 
     def __init__(self, program: str) -> None:
         super().__init__()
         self.program = program
 
     def compute(
         self,
         inp_obj: FileInput,
         update_func: Optional[Callable] = None,
         update_interval: Optional[float] = None,
-    ) -> FileSuccessfulOutput:
+    ) -> Tuple[FileOutput, str]:
         """Compute the given program on the given files.
 
         Args:
             inp_obj: The qcio FileInput object for a computation.
             update_func: A callback function to call as the program executes.
             update_interval: The minimum time in seconds between calls to the
             update_func.
 
         Returns:
-            Tuple of None and FileSuccessfulOutput object for a computation. None is
+            Tuple of None and FileOutput object for a computation. None is
                 returned because no computed properties are returned for a file
                 computation.
 
         Raises:
             ProgramNotFoundException: If the program is not found.
 
         """
         stdout = execute_subprocess(
-            self.program,
-            inp_obj.program_args.cmdline_args,
-            update_func,
-            update_interval,
+            self.program, inp_obj.cmdline_args, update_func, update_interval
         )
         return None, stdout
```

### Comparing `qcop-0.1.0/qcop/adapters/terachem.py` & `qcop-0.2.0/qcop/adapters/terachem.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 from typing import Callable, Optional, Tuple
 
-from qcio.models.single_point import (
-    SinglePointComputedProperties,
-    SinglePointInput,
-    SPCalcType,
-)
-from qcparse import parse_computed_props
+from qcio import CalcType, ProgramInput, SinglePointResults
+from qcparse import parse_results
 from qcparse.parsers.terachem import parse_version_string
 
 from qcop.exceptions import AdapterInputError
-from qcop.utils import execute_subprocess
 
-from .base import QCOPSinglePointAdapter
+from .base import ProgramAdapter
+from .utils import execute_subprocess
 
 
-class TeraChemAdapter(QCOPSinglePointAdapter):
+class TeraChemAdapter(ProgramAdapter):
     """Adapter for TeraChem."""
 
-    supported_calc_types = [SPCalcType.energy, SPCalcType.gradient, SPCalcType.hessian]
+    supported_calctypes = [CalcType.energy, CalcType.gradient, CalcType.hessian]
     program = "terachem"
     padding = 20  # padding between keyword and value in tc.in
 
     def program_version(self, stdout: Optional[str] = None) -> str:
         """Get the program version.
 
         Args:
@@ -32,54 +28,54 @@
         """
         if stdout:
             return parse_version_string(stdout)
         else:
             # Cut out "TeraChem version " (17 chars) from the output
             return execute_subprocess(self.program, ["--version"])[17:]
 
-    def prepare_inputs(self, inp_obj: SinglePointInput) -> str:
+    def prepare_inputs(self, inp_obj: ProgramInput) -> str:
         """Translate qcio objects into TeraChem inputs files. Write files to disk.
 
         Args:
-            inp_obj: The qcio SinglePointInput object for a computation.
+            inp_obj: The qcio ProgramInput object for a computation.
 
         Returns:
             Filename of input file (tc.in).
         """
         # Write molecule to disk
         xyz_filename = "geom.xyz"
         inp_obj.molecule.save(xyz_filename)
 
         # Write input file
         inp_filename = "tc.in"
 
         with open(inp_filename, "w") as f:
-            # calc_type
-            if inp_obj.program_args.calc_type == "hessian":
-                calc_type = "frequencies"
+            # calctype
+            if inp_obj.calctype == "hessian":
+                calctype = "frequencies"
             else:
-                calc_type = inp_obj.program_args.calc_type
-            f.write(f"{'run':<{self.padding}} {calc_type}\n")
+                calctype = inp_obj.calctype
+            f.write(f"{'run':<{self.padding}} {calctype}\n")
             # Molecule
             f.write(f"{'coordinates':<{self.padding}} {xyz_filename}\n")
             f.write(f"{'charge':<{self.padding}} {inp_obj.molecule.charge}\n")
             f.write(f"{'spinmult':<{self.padding}} {inp_obj.molecule.multiplicity}\n")
             # Model
-            f.write(f"{'method':<{self.padding}} {inp_obj.program_args.model.method}\n")
-            f.write(f"{'basis':<{self.padding}} {inp_obj.program_args.model.basis}\n")
+            f.write(f"{'method':<{self.padding}} {inp_obj.model.method}\n")
+            f.write(f"{'basis':<{self.padding}} {inp_obj.model.basis}\n")
 
             # Keywords
             non_keywords = {
                 "charge": ".molecule.charge",
                 "spinmult": ".molecule.multiplicity",
-                "run": ".program_args.calc_type",
-                "basis": ".program_args.model.basis",
-                "method": ".program_args.model.method",
+                "run": ".calctype",
+                "basis": ".model.basis",
+                "method": ".model.method",
             }
-            for key, value in inp_obj.program_args.keywords.items():
+            for key, value in inp_obj.keywords.items():
                 # Check for keywords that should be passed as structured data
                 if key in non_keywords:
                     raise AdapterInputError(
                         program=self.program,
                         message=f"Keyword '{key}' should not be set as a keyword. It "
                         f"should be set at '{non_keywords[key]}'",
                     )
@@ -90,30 +86,23 @@
     # TODO: Need command line options for TeraChem e.g., -g 1 for GPUs MAYBE?
     # Try using it for a while without and see what roadblocks we run into
     def _compute(
         self,
         inp_obj,
         update_func: Optional[Callable] = None,
         update_interval: Optional[float] = None,
-    ) -> Tuple[SinglePointComputedProperties, str]:
+    ) -> Tuple[SinglePointResults, str]:
         """Execute TeraChem on the given input.
 
         Args:
-            inp_obj: The qcio SinglePointInput object for a computation.
+            inp_obj: The qcio ProgramInput object for a computation.
             update_func: A callback function to call as the program executes.
             update_interval: The minimum time in seconds between calls to the
                 update_func.
 
         Returns:
-            A tuple of SinglePointComputedProperties and the stdout str.
+            A tuple of SinglePointComputedProps and the stdout str.
         """
         tc_in = self.prepare_inputs(inp_obj)
         stdout = execute_subprocess(self.program, [tc_in], update_func, update_interval)
-        # Hardcoding "terachem" so "terachemd" isn't passed to parse
-        parsed_output = parse_computed_props(stdout, "terachem", "stdout")
+        parsed_output = parse_results(stdout, self.program, "stdout")
         return parsed_output, stdout
-
-
-class TeraChemDockerAdapter(TeraChemAdapter):
-    """Adapter for TeraChem executable running in Docker."""
-
-    program = "terachemd"
```

### Comparing `qcop-0.1.0/qcop/exceptions.py` & `qcop-0.2.0/qcop/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Experimental exception hierarchy. This may be too complex and unhelpful for now"""
 
 from subprocess import CalledProcessError
 from typing import List, Optional
 
-from qcio import SPCalcType
+from qcio import CalcType
 
 
 class QCOPBaseError(Exception):
     """Base class for exceptions in qcop. All custom exceptions should inherit from
     this class."""
 
     pass
@@ -56,24 +56,24 @@
         driver: driver which is not supported
         message: explanation of the error
     """
 
     def __init__(
         self,
         program: str,
-        calc_type: SPCalcType,
-        supported_calc_types: List[SPCalcType],
+        calctype: CalcType,
+        supported_calctypes: List[CalcType],
     ):
         self.program = program
-        self.calc_type = calc_type
-        self.supported_calc_types = supported_calc_types
+        self.calctype = calctype
+        self.supported_calctypes = supported_calctypes
         self.message = (
             f"The {self.program} adapter does not yet support "
-            f"'{self.calc_type.value}' calculations. This adaptor can compute: "
-            f"{[i.value for i in self.supported_calc_types]}"
+            f"'{self.calctype.value}' calculations. This adaptor can compute: "
+            f"{[i.value for i in self.supported_calctypes]}"
         )
         super().__init__(self.message)
 
 
 class QCEngineError(QCOPBaseError):
     """Exception raised when any part of qcengine execution fails."""
```

### Comparing `qcop-0.1.0/qcop/main.py` & `qcop-0.2.0/qcop/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 """Top level compute functions for qcop."""
-import os
-import platform
+import traceback
 from time import time
-from typing import Callable, Optional
+from typing import Any, Callable, Dict, Optional, Union
 
-from qcio import FileInput
+from qcio import (
+    CalcType,
+    FileInput,
+    Files,
+    Model,
+    Molecule,
+    ProgramFailure,
+    ResultsBase,
+)
 from qcio.helper_types import StrOrPath
-from qcio.models.base_io import InputBase, OutputBase, Provenance
+from qcio.models import InputBase, OutputBase
+from qcio.utils import calctype_to_output
 
-from .adapters import FileAdapter, registry
-from .exceptions import AdapterNotFoundError, QCEngineError, QCOPBaseError
-from .utils import tmpdir
+from .exceptions import QCOPBaseError
+from .utils import construct_provenance, get_adapter, tmpdir
 
 
 def compute(
-    inp_obj: InputBase,
     program: str,
+    inp_obj: InputBase,
     *,
     working_dir: Optional[StrOrPath] = None,
     rm_working_dir: bool = True,
     collect_stdout: bool = True,
     collect_files: bool = False,
     update_func: Optional[Callable] = None,
     update_interval: Optional[float] = None,
@@ -41,154 +48,170 @@
         collect_stdout: Whether to collect stdout/stderr from the program as output.
             Failed computations will always collect stdout/stderr.
         collect_files: Whether to collect all files from the calc_dir as output.
         update_func: A function to call as the program executes. The function must
             accept the in-process stdout/stderr output as a string for its first
             argument.
         update_interval: The minimum time in seconds between calls to the update_func.
-        print_stdout: Whether to print stdout/stderr to the terminal as the program
-            executes. Will be ignored if update_func passed
+        print_stdout: Whether to print stdout/stderr to the terminal in real time as
+            the program executes. Will be ignored if an update_func passed.
         raise_exc: If False, qcop will return a subclass of the FailedComputation object
             when the QC program fails rather than raise an exception. qcop exceptions
             not related external program failure will always be raised.
         qcng_fallback: Whether to fall back to qcengine if qcop doesn't have an
             adapter for the program.
-        **kwargs: Additional keyword arguments to pass to the adapter.
+        **kwargs: Additional keyword arguments to pass to the adapter or qcng.compute().
 
     Returns:
         The qcio output object for a computation. A subclass of OutputBase. Will either
         be a FailedComputation object or the corresponding output object for the input
         type. E.g., SinglePointInput -> SinglePointOutput.
 
     Raises:
         AdapterNotFoundException: If the program is not supported (i.e., no Adapter is
             implemented for it in qcop or qcengine).
         ProgramNotFoundException: If the program executable is not found on the system
             at execution time. This likely means the program is not installed on the
             system.
-        UnsupportedCalcTypeError: If the program is supported but the calc_type is not.
+        UnsupportedCalcTypeError: If the program is supported but the calctype is not.
         ExecutionFailedException: If the program fails during execution and
             raise_exc=True.
         QCEngineException: If QCEngine performed the computation, fails and
             raise_exc=True.
     """
-    # Get adapter to execute program
-    if isinstance(inp_obj, FileInput):
-        adapter = FileAdapter(program)
-    else:
-        try:
-            adapter = registry[program]()
-        except KeyError:
-            # Use QCEngine as a fallback, if requested.
-            if qcng_fallback:
-                try:  # Import QCEngine
-                    from qcengine import compute as qcng_compute
-                    from qcengine.exceptions import QCEngineException
-
-                    from .utils import qcng_get_program
-                except ModuleNotFoundError as e:
-                    raise ModuleNotFoundError(
-                        "QCEngine not installed. To use qcengine as a fallback, "
-                        "install it by running 'python -m pip install "
-                        "qcop[qcengine]'."
-                    ) from e
-
-                # Check for QCEngine harness and that program is installed
-                qcng_get_program(program)
-
-                try:
-                    return inp_obj.to_output_from_qcel(
-                        qcng_compute(
-                            inp_obj.to_qcel(),
-                            program,
-                            raise_error=raise_exc,
-                            return_dict=True,  # qcio works with dicts for qcel i/o
-                            **kwargs,
-                        ),
-                    )
-
-                except QCEngineException as e:  # Base exception for all QCEngine
-                    raise QCEngineError(
-                        "Something went wrong with QCEngine. See the traceback above "
-                        "for details."
-                    ) from e
-            else:
-                raise AdapterNotFoundError(program)
-
     # Set update_func if print_stdout is True and update_func is None
     if print_stdout and update_func is None:
         update_func, update_interval = (lambda _, stdout_new: print(stdout_new), 0.1)
 
     # Change cwd to a temporary directory to run the program.
     with tmpdir(working_dir, rm_working_dir) as calc_dir:
+        # Get adapter to execute program
+        adapter = get_adapter(program, inp_obj, qcng_fallback)
+
         if adapter.write_files:  # Write non structured input files to disk.
-            inp_obj.program_args.write_files()
+            inp_obj.write_files()
+
+        output_dict: Dict[str, Optional[str]] = {}
+        stdout: Optional[str]
 
         start = time()
         try:
             # Execute the program.
-            computed_properties, stdout = adapter.compute(
+            results, stdout = adapter.compute(
                 inp_obj, update_func, update_interval, **kwargs
             )
-            output_constructor = inp_obj.to_success
+            # getattr covers FileInput
+            output_cls = calctype_to_output(getattr(inp_obj, "calctype", None))
         except QCOPBaseError as e:
             if raise_exc:
                 raise e
             else:
-                # Return a FailedOutput object.
-                output_constructor = inp_obj.to_failure
-                stdout = getattr(e, "stdout", None)
-                exception = e
+                # Return a ProgramFailure object.
+                output_cls = ProgramFailure
+                # Someday may may put half-completed results here
+                results, stdout = None, getattr(e, "stdout", None)
+                # For mypy because e.stdout is not of a a known type
+                stdout = str(stdout) if stdout is not None else None
+                output_dict["traceback"] = traceback.format_exc()
 
         # Construct Provenance object
-        wall_time = time() - start
-        if hasattr(adapter, "program_version"):
-            version = adapter.program_version(stdout)
-        else:
-            version = None
-
-        provenance = Provenance(
-            program=program,
-            program_version=version,
-            working_dir=str(calc_dir),
-            wall_time=round(wall_time, 6),
-            hostname=platform.node(),
-            hostcpus=os.cpu_count(),
-        )
+        provenance = construct_provenance(program, adapter, calc_dir, start, stdout)
 
         # Construct output object
-        if output_constructor == inp_obj.to_failure:  # Failure
-            output: OutputBase = output_constructor(provenance, exception)
-        else:  # Success
-            # Remove stdout if not requested
-            stdout = stdout if collect_stdout else None
-            output = output_constructor(provenance, computed_properties, stdout)
+        stdout = stdout if collect_stdout and output_cls != ProgramFailure else None
+        # Ensure results is not None to maintain interface
+        results = results if results is not None else ResultsBase()
+        output_dict.update(
+            {
+                "input_data": inp_obj,
+                "stdout": stdout,
+                "results": results,
+                "provenance": provenance,
+            }
+        )
+
+        output_obj = output_cls(**output_dict)
 
         # Optionally collect output files
         if collect_files or isinstance(inp_obj, FileInput):
             # Collect output files from the calc_dir
-            output.add_files(
-                calc_dir, recursive=True, exclude=inp_obj.program_args.files.keys()
-            )
+            output_obj.add_files(calc_dir, recursive=True, exclude=inp_obj.files.keys())
 
-    return output
+    return output_obj
+
+
+def compute_args(
+    program: str,
+    molecule: Molecule,
+    *,
+    calctype: Union[str, CalcType],
+    model: Union[Dict[str, str], Model],
+    keywords: Optional[Dict[str, Any]] = None,
+    files: Optional[Union[Dict[str, Union[str, bytes]], Files]] = None,
+    extras: Optional[Dict[str, Any]] = None,
+    **kwargs,
+) -> OutputBase:
+    """An alternative to the compute function that accepts independent argument for
+    SinglePointInput.
+
+    Args:
+        program: The program to run.
+        molecule: The molecule to use.
+        calctype: The type of calculation to run.
+        model: The model to use for the calculation.
+        keywords: The keywords to use for the calculation.
+        files: The files to use for the calculation. Either a qcio.Files object or a
+            dict mapping file names to file contents (bytes or str).
+        extras: Extra arguments to pass to the adapter.
+        **kwargs: Extra arguments to pass to the compute function.
+
+    Returns:
+        The output of the computation.
+
+    Raises:
+        AdapterNotFoundError: If no adapter is found for the given program.
+        AdapterInputError: If the adapter raises an exception when generating input
+            files.
+        QCEngineError: If the adapter raises an exception when running the program.
+    """
+    if isinstance(files, Files):  # Check in case Files object is passed instead of dict
+        files = files.files
+
+    inp_obj = SinglePointInput(
+        calctype=calctype,
+        molecule=molecule,
+        model=model,
+        keywords=keywords or {},
+        files=files or {},
+        extras=extras or {},
+    )
+
+    return compute(program, inp_obj, **kwargs)
 
 
 if __name__ == "__main__":  # pragma: no cover
     from qcio import Molecule, SinglePointInput
 
     h2 = Molecule(
         symbols=["H", "H"],
         geometry=[[0, 0, 0], [0, 0, 0.7414]],
         charge=0,
         multiplicity=1,
     )
     sp_energy = SinglePointInput(
         molecule=h2,
-        program_args={
-            "model": {"method": "HF", "basis": "6-31g"},
-            "calc_type": "gradient",
-            "keywords": {"purify": "no"},
-        },
+        model={"method": "HF", "basis": "6-31g"},
+        calctype="gradient",
+        keywords={"purify": "no"},
+    )
+    files = Files(files={"file1": "string data"})
+    files = {"file1": "string data"}
+    # output = compute("terachemd", sp_energy, collect_stdout=False, collect_files=True)
+    output = compute_args(
+        "terachemd",
+        h2,
+        calctype="energy",
+        model={"method": "HF", "basis": "6-31g"},
+        files=files,
+        keywords={"purify": "no"},
+        collect_files=True,
     )
-    output = compute(sp_energy, "terachemd", collect_stdout=False, collect_files=True)
-    print(output.__repr__())
```

### Comparing `qcop-0.1.0/PKG-INFO` & `qcop-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: qcop
-Version: 0.1.0
+Version: 0.2.0
 Summary: A package for operating Quantum Chemistry programs using qcio standardized data structures.
 License: MIT
 Author: Colton Hicks
 Author-email: github@coltonhicks.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: qcengine[qcengine] (>=0.26.0)
-Requires-Dist: qcio (>=0.2.1)
-Requires-Dist: qcparse (>=0.3.1)
+Requires-Dist: qcio (>=0.3.0)
+Requires-Dist: qcparse (>=0.4.0)
 Description-Content-Type: text/markdown
 
 # Quantum Chemistry Operate
 
 A package for operating Quantum Chemistry programs using [qcio](https://github.com/coltonbh/qcio) standardized data structures.
 
 [![image](https://img.shields.io/pypi/v/qcop.svg)](https://pypi.python.org/pypi/qcop)
```

