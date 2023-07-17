# Comparing `tmp/qcio-0.2.1.tar.gz` & `tmp/qcio-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcio-0.2.1.tar", max compression
+gzip compressed data, was "qcio-0.3.0.tar", max compression
```

## Comparing `qcio-0.2.1.tar` & `qcio-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0     1079 2023-06-30 03:01:39.044386 qcio-0.2.1/LICENSE
--rw-r--r--   0        0        0      898 2023-06-30 03:01:39.044386 qcio-0.2.1/README.md
--rw-r--r--   0        0        0     1246 2023-06-30 03:01:39.044386 qcio-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      560 2023-06-30 03:01:39.044386 qcio-0.2.1/qcio/__init__.py
--rw-r--r--   0        0        0       89 2023-06-30 03:01:39.044386 qcio-0.2.1/qcio/constants.py
--rw-r--r--   0        0        0      346 2023-06-30 03:01:39.044386 qcio-0.2.1/qcio/helper_types.py
--rw-r--r--   0        0        0     3671 2023-06-30 03:01:39.044386 qcio-0.2.1/qcio/mixins.py
--rw-r--r--   0        0        0      151 2023-06-30 03:01:39.044386 qcio-0.2.1/qcio/models/__init__.py
--rw-r--r--   0        0        0     8112 2023-06-30 03:01:39.044386 qcio-0.2.1/qcio/models/base_io.py
--rw-r--r--   0        0        0     4447 2023-06-30 03:01:39.044386 qcio-0.2.1/qcio/models/base_model.py
--rw-r--r--   0        0        0     3350 2023-06-30 03:01:39.044386 qcio-0.2.1/qcio/models/file.py
--rw-r--r--   0        0        0     7534 2023-06-30 03:01:39.044386 qcio-0.2.1/qcio/models/molecule.py
--rw-r--r--   0        0        0    12500 2023-06-30 03:01:39.044386 qcio-0.2.1/qcio/models/single_point.py
--rw-r--r--   0        0        0      190 2023-06-30 03:01:39.044386 qcio-0.2.1/qcio/utils.py
--rw-r--r--   0        0        0     1623 1970-01-01 00:00:00.000000 qcio-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-07-17 21:07:13.766101 qcio-0.3.0/LICENSE
+-rw-r--r--   0        0        0      898 2023-07-17 21:07:13.766101 qcio-0.3.0/README.md
+-rw-r--r--   0        0        0     1246 2023-07-17 21:07:13.766101 qcio-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      573 2023-07-17 21:07:13.766101 qcio-0.3.0/qcio/__init__.py
+-rw-r--r--   0        0        0       89 2023-07-17 21:07:13.766101 qcio-0.3.0/qcio/constants.py
+-rw-r--r--   0        0        0      346 2023-07-17 21:07:13.766101 qcio-0.3.0/qcio/helper_types.py
+-rw-r--r--   0        0        0      272 2023-07-17 21:07:13.770101 qcio-0.3.0/qcio/models/__init__.py
+-rw-r--r--   0        0        0     9738 2023-07-17 21:07:13.770101 qcio-0.3.0/qcio/models/base_models.py
+-rw-r--r--   0        0        0     3082 2023-07-17 21:07:13.770101 qcio-0.3.0/qcio/models/inputs.py
+-rw-r--r--   0        0        0     2236 2023-07-17 21:07:13.770101 qcio-0.3.0/qcio/models/inputs_base.py
+-rw-r--r--   0        0        0     7511 2023-07-17 21:07:13.770101 qcio-0.3.0/qcio/models/molecule.py
+-rw-r--r--   0        0        0     3585 2023-07-17 21:07:13.770101 qcio-0.3.0/qcio/models/outputs.py
+-rw-r--r--   0        0        0     1935 2023-07-17 21:07:13.770101 qcio-0.3.0/qcio/models/outputs_base.py
+-rw-r--r--   0        0        0     4462 2023-07-17 21:07:13.770101 qcio-0.3.0/qcio/models/results.py
+-rw-r--r--   0        0        0     4253 2023-07-17 21:07:13.770101 qcio-0.3.0/qcio/qcel.py
+-rw-r--r--   0        0        0      793 2023-07-17 21:07:13.770101 qcio-0.3.0/qcio/utils.py
+-rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 qcio-0.3.0/PKG-INFO
```

### Comparing `qcio-0.2.1/LICENSE` & `qcio-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qcio-0.2.1/README.md` & `qcio-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `qcio-0.2.1/pyproject.toml` & `qcio-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "qcio"
-version = "0.2.1"
+version = "0.3.0"
 description = "Beautiful and user friendly data structures for quantum chemistry."
 authors = ["Colton Hicks <github@coltonhicks.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = ">=1.7.4,!=1.8,!=1.8.1,<2.0.0"
 numpy = ">=1.20"
 toml = "^0.10.2"
 pyyaml = "^6.0"
+typing-extensions = "^4.7.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 mypy = "^1.1.1"
 pytest = "^7.2.2"
 pre-commit = "^3.2.1"
 pytest-cov = "^4.0.0"
 ruff = "^0.0.260"
 isort = "^5.12.0"
-typing-extensions = "^4.5.0"
 qcelemental = "^0.25.1"
 types-toml = "^0.10.8.6"
 types-pyyaml = "^6.0.12.10"
 
 [tool.black]
 line-length = 88
```

### Comparing `qcio-0.2.1/qcio/models/file.py` & `qcio-0.3.0/qcio/models/outputs.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,94 +1,99 @@
-"""Basic file I/O objects for calculations."""
-from pathlib import Path
-from typing import List, Type, Union
+"""End user output objects from a calculation."""
+from typing import Literal, Optional, Union
 
-from typing_extensions import Self
+from qcio.helper_types import ArrayLike2D
 
-from ..mixins import Files
-from .base_io import FailedOutputBase, InputBase, ProgramArgsBase, SuccessfulOutputBase
+from .inputs import DualProgramInput, FileInput, ProgramInput
+from .molecule import Molecule
+from .outputs_base import OutputBase, SuccessfulOutputBase
+from .results import OptimizationResults, SinglePointResults
 
-__all__ = ["FileArgs", "FileInput", "FileSuccessfulOutput", "FileFailedOutput"]
+__all__ = ["FileOutput", "SinglePointOutput", "OptimizationOutput", "ProgramFailure"]
 
 
-class FileArgs(ProgramArgsBase):
-    """Program arguments for a FileInput.
+class FileOutput(SuccessfulOutputBase):
+    """Generic output class for pure file based I/O.
 
     Attributes:
-        cmdline_args: A list of command line arguments to be passed to the program.
+        input_data: The FileInput object used for the computation.
         files: A dict mapping filename to str or bytes data.
+        success: A boolean indicator that the operation succeeded (always True)
+        stdout: The primary logging output of the program. Contains a union of stdout
+            and stderr.
+        provenance: An object containing the provenance information for the results.
         extras: Additional information to bundle with the object. Use for schema
             development and scratch space.
-    """
-
-    cmdline_args: List[str] = []
-
 
-class FileInput(InputBase):
-    """File and command line argument inputs for a calculation.
-
-    Attributes:
-        program_args: Files and command line arguments for the program.
-        extras: Additional information to bundle with the object. Use for schema
-            development and scratch space.
     """
 
-    program_args: FileArgs = FileArgs()
-
-    @classmethod
-    def from_directory(cls, directory: Union[Path, str], **kwargs) -> Self:
-        """Collect all files from directory and instantiate an object."""
-        obj = cls(**kwargs)
-        directory = Path(directory)
-        obj.program_args.add_files(directory)
-        return obj
-
-    def get_failed_output_class(self) -> Type["FileFailedOutput"]:
-        return FileFailedOutput
+    input_data: FileInput
 
-    def get_successful_output_class(self) -> Type["FileSuccessfulOutput"]:
-        return FileSuccessfulOutput
 
+class SinglePointOutput(SuccessfulOutputBase):
+    """Output from a successful single point calculation.
 
-class FileOutputMixin(Files):
-    """Mixin for file based output objects.
     Attributes:
-        input_data: The input data for the computation.
+        input_data: The SinglePointInput object for the computation.
+        success: Always True for a successful computation.
+        results: The results computed by the program.
         files: A dict mapping filename to str or bytes data.
-        extras: Additional information to bundle with the object. Use for schema
-            development and scratch space.
-        success: A boolean indicator that the operation succeeded (always True)
         stdout: The primary logging output of the program. Contains a union of stdout
             and stderr.
+        provenance: An object containing the provenance information for the results.
+        extras: Additional information to bundle with the object. Use for schema
+            development and scratch space.
     """
 
-    input_data: FileInput
+    input_data: ProgramInput
+    results: SinglePointResults
 
+    @property
+    def return_result(self) -> Union[float, ArrayLike2D]:
+        """Return the result of the calculation.
+
+        Returns:
+            The explicitly requested result of the calculation, i.e., the energy,
+                gradient, or hessian.
+        """
+        return getattr(self.results, self.input_data.calctype.value)
 
-class FileSuccessfulOutput(SuccessfulOutputBase, FileOutputMixin):
-    """Generic output class for pure file based I/O.
+
+class OptimizationOutput(SuccessfulOutputBase):
+    """Output from a successful optimization.
 
     Attributes:
-        input_data: The FileInput object used for the computation.
-        files: A dict mapping filename to str or bytes data.
-        extras: Additional information to bundle with the object. Use for schema
-            development and scratch space.
-        success: A boolean indicator that the operation succeeded (always True)
-        stdout: The primary logging output of the program. Contains a union of stdout
-            and stderr.
+        input_data: The OptimizationInput object for the computation.
+        results: The results computed by the program.
     """
 
-    input_data: FileInput
+    input_data: Union[DualProgramInput, ProgramInput]
+    results: OptimizationResults
 
+    @property
+    def final_molecule(self) -> Molecule:
+        """Return the final molecule in the optimization."""
+        return self.results.molecules[-1]
 
-class FileFailedOutput(FailedOutputBase, FileOutputMixin):
-    """Generic output class for pure file based I/O.
+
+class ProgramFailure(OutputBase):
+    """A object containing details about a failed calculation.
 
     Attributes:
-        input_data: input_data: The FileInput object used for the computation.
-        files: A dict mapping filename to str or bytes data.
-        extras: Additional information to bundle with the object. Use for schema
-            development and scratch space.
+        input_data: The input object for the computation.
         success: Always False for a Failed output.
+        traceback: String representation of the traceback of the exception that caused
+            the failure.
+        results: Any compted data that was able to be extracted before program failed.
         stdout: The primary logging output of the program. Contains a union of stdout
             and stderr.
+        provenance: An object containing the provenance information for the output.
     """
+
+    input_data: Union[DualProgramInput, ProgramInput, FileInput]
+    success: Literal[False] = False
+    traceback: Optional[str] = None
+
+    @property
+    def ptraceback(self) -> None:
+        """Print the traceback text"""
+        print(self.traceback)
```

### Comparing `qcio-0.2.1/qcio/models/molecule.py` & `qcio-0.3.0/qcio/models/molecule.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy as np
 from pydantic import validator
 from typing_extensions import Self
 
 from qcio.constants import BOHR_TO_ANGSTROM
 from qcio.helper_types import ArrayLike2D
 
-from .base_model import QCIOModelBase
+from .base_models import QCIOModelBase
 
 if TYPE_CHECKING:
     from pydantic.typing import ReprArgs
 
 __all__ = ["Molecule", "Identifiers"]
 
 
@@ -83,16 +83,16 @@
     """
 
     symbols: List[str]
     geometry: ArrayLike2D
     charge: int = 0
     multiplicity: int = 1
     identifiers: Identifiers = Identifiers()
-    # masses: Optional[List[float]] = None
-    # connectivity: Optional[List[Bond]] = None
+    # masses: List[float] = []
+    # connectivity: List[Bond] = []
 
     def __repr_args__(self) -> "ReprArgs":
         """A helper for __repr__ that returns a list of tuples of the form
         (name, value).
         """
         return [  # pragma: no cover
             ("name", self.identifiers.name_common),
```

### Comparing `qcio-0.2.1/PKG-INFO` & `qcio-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcio
-Version: 0.2.1
+Version: 0.3.0
 Summary: Beautiful and user friendly data structures for quantum chemistry.
 License: MIT
 Author: Colton Hicks
 Author-email: github@coltonhicks.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.20)
 Requires-Dist: pydantic (>=1.7.4,!=1.8,!=1.8.1,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: typing-extensions (>=4.7.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Quantum Chemistry I/O
 
 [![image](https://img.shields.io/pypi/v/qcio.svg)](https://pypi.python.org/pypi/qcio)
 [![image](https://img.shields.io/pypi/l/qcio.svg)](https://pypi.python.org/pypi/qcio)
 [![image](https://img.shields.io/pypi/pyversions/qcio.svg)](https://pypi.python.org/pypi/qcio)
```

