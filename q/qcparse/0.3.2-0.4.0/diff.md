# Comparing `tmp/qcparse-0.3.2.tar.gz` & `tmp/qcparse-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcparse-0.3.2.tar", max compression
+gzip compressed data, was "qcparse-0.4.0.tar", max compression
```

## Comparing `qcparse-0.3.2.tar` & `qcparse-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     3993 2023-06-30 03:20:35.137518 qcparse-0.3.2/README.md
--rw-r--r--   0        0        0     1196 2023-06-30 03:20:35.141518 qcparse-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      312 2023-06-30 03:20:35.141518 qcparse-0.3.2/qcparse/__init__.py
--rw-r--r--   0        0        0      879 2023-06-30 03:20:35.141518 qcparse-0.3.2/qcparse/cli.py
--rw-r--r--   0        0        0      475 2023-06-30 03:20:35.141518 qcparse-0.3.2/qcparse/exceptions.py
--rw-r--r--   0        0        0     6793 2023-06-30 03:20:35.141518 qcparse-0.3.2/qcparse/main.py
--rw-r--r--   0        0        0     2418 2023-06-30 03:20:35.141518 qcparse-0.3.2/qcparse/models.py
--rw-r--r--   0        0        0       74 2023-06-30 03:20:35.141518 qcparse-0.3.2/qcparse/parsers/__init__.py
--rw-r--r--   0        0        0     9189 2023-06-30 03:20:35.141518 qcparse-0.3.2/qcparse/parsers/terachem.py
--rw-r--r--   0        0        0     2701 2023-06-30 03:20:35.141518 qcparse-0.3.2/qcparse/parsers/utils.py
--rw-r--r--   0        0        0     3995 2023-06-30 03:20:35.141518 qcparse-0.3.2/qcparse/registry.py
--rw-r--r--   0        0        0     1193 2023-06-30 03:20:35.141518 qcparse-0.3.2/qcparse/utils.py
--rw-r--r--   0        0        0     4630 1970-01-01 00:00:00.000000 qcparse-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     3107 2023-07-17 21:17:54.733668 qcparse-0.4.0/README.md
+-rw-r--r--   0        0        0     1195 2023-07-17 21:17:54.733668 qcparse-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      298 2023-07-17 21:17:54.733668 qcparse-0.4.0/qcparse/__init__.py
+-rw-r--r--   0        0        0      851 2023-07-17 21:17:54.737668 qcparse-0.4.0/qcparse/cli.py
+-rw-r--r--   0        0        0      475 2023-07-17 21:17:54.737668 qcparse-0.4.0/qcparse/exceptions.py
+-rw-r--r--   0        0        0     6676 2023-07-17 21:17:54.737668 qcparse-0.4.0/qcparse/main.py
+-rw-r--r--   0        0        0     2338 2023-07-17 21:17:54.737668 qcparse-0.4.0/qcparse/models.py
+-rw-r--r--   0        0        0       74 2023-07-17 21:17:54.737668 qcparse-0.4.0/qcparse/parsers/__init__.py
+-rw-r--r--   0        0        0     9105 2023-07-17 21:17:54.737668 qcparse-0.4.0/qcparse/parsers/terachem.py
+-rw-r--r--   0        0        0     2693 2023-07-17 21:17:54.737668 qcparse-0.4.0/qcparse/parsers/utils.py
+-rw-r--r--   0        0        0     3968 2023-07-17 21:17:54.737668 qcparse-0.4.0/qcparse/registry.py
+-rw-r--r--   0        0        0     1193 2023-07-17 21:17:54.737668 qcparse-0.4.0/qcparse/utils.py
+-rw-r--r--   0        0        0     3744 1970-01-01 00:00:00.000000 qcparse-0.4.0/PKG-INFO
```

### Comparing `qcparse-0.3.2/pyproject.toml` & `qcparse-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [tool.poetry]
 name = "qcparse"
-version = "0.3.2"
+version = "0.4.0"
 description = "A package for parsing Quantum Chemistry program file outputs into structured qcio data objects."
 authors = ["Colton Hicks <github@coltonhicks.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 pydantic = ">=1.7.4,!=1.8,!=1.8.1,<2.0.0"
-qcio = ">=0.2.0"
-
+qcio = ">=0.3.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.1.1"
 isort = "^5.12.0"
 pytest = "^7.2.2"
 pre-commit = "^3.2.0"
 pytest-cov = "^4.0.0"
```

### Comparing `qcparse-0.3.2/qcparse/cli.py` & `qcparse-0.4.0/qcparse/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 import json
 from pathlib import Path
 
-from .main import parse_computed_props
+from .main import parse_results
 
 
 def main():
     parser = argparse.ArgumentParser(
         description="Parse Quantum Chemistry output files into structured JSON or "
         "Python objects."
     )
@@ -14,14 +14,12 @@
     parser.add_argument("filepath", help="Path to the file")
     parser.add_argument(
         "--filetype", help="Type of file. Defaults to 'stdout'", default="stdout"
     )
 
     args = parser.parse_args()
 
-    computed_props = parse_computed_props(
-        Path(args.filepath), args.program, args.filetype
-    )
+    computed_props = parse_results(Path(args.filepath), args.program, args.filetype)
     # Hacking in pretty print since probably preferred for most users
     # Can update to result.json(indent=4) when this PR accepted
     # https://github.com/MolSSI/QCElemental/pull/307
     print(json.dumps(computed_props.dict(), indent=4))
```

### Comparing `qcparse-0.3.2/qcparse/main.py` & `qcparse-0.4.0/qcparse/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,72 +1,69 @@
 """Top level functions for the tcparse library"""
 
 from importlib import import_module
 from pathlib import Path
 from typing import List, Optional, Union
 
-from qcio import (
-    SinglePointComputedProperties,
-    SinglePointFailedOutput,
-    SinglePointInput,
-    SinglePointSuccessfulOutput,
-)
+from qcio import ProgramFailure, ProgramInput, SinglePointOutput, SinglePointResults
 
 from .exceptions import MatchNotFoundError
 from .models import single_point_data_collector
 from .parsers import *  # noqa: F403 Ensure all parsers get registered
 from .registry import ParserSpec, registry
 from .utils import get_file_content
 
-__all__ = ["parse", "parse_computed_props", "registry"]
+__all__ = ["parse", "parse_results", "registry"]
 
 
-def parse_computed_props(
+def parse_results(
     data_or_path: Union[str, bytes, Path],
     program: str,
     filetype: str = "stdout",
-) -> SinglePointComputedProperties:
+) -> SinglePointResults:
     """Parse a file using the parsers registered for the given program.
 
+    Can expand function to return other Results objects in the future.
+
     Args:
         data_or_path: File contents (str or bytes) or path to the file to parse.
         program: The QC program that generated the output file.
             To see the available programs run:
             >>> from qcparse import registry
             >>> registry.supported_programs()
         filetype: The type of file to parse (e.g. 'stdout' for the log output).
             To see the available filetypes for a given program run
             >>> from qcparse import registry
             >>> registry.supported_filetypes('program_name')
 
     Returns:
-        A SinglePointComputedProperties object containing the parsed data.
+        A SinglePointResults object containing the parsed data.
 
     Raises:
         MatchNotFoundError: If a required parser fails to parse its data.
     """
     file_content, _ = get_file_content(data_or_path)
 
     # Create a data collector object to store the parsed data
     data_collector = single_point_data_collector(collect_inputs=False)
 
     # Get the calculation type if filetype is 'stdout'
     if filetype == "stdout":
-        parse_calc_type = import_module(f"qcparse.parsers.{program}").parse_calc_type
-        calc_type = parse_calc_type(file_content)
+        parse_calctype = import_module(f"qcparse.parsers.{program}").parse_calctype
+        calctype = parse_calctype(file_content)
 
     else:
-        calc_type = None
+        calctype = None
 
     # Get all the parsers for the program and filetype
     parsers: List[ParserSpec] = registry.get_parsers(
         program,
         filetype=filetype,
         collect_inputs=False,
-        calc_type=calc_type,
+        calctype=calctype,
     )
 
     # Apply parsers to the file content.
     for parser_info in parsers:
         try:
             # This will raise a MatchNotFound error if the parser can't find its data
             parser_info.parser(file_content, data_collector)
@@ -76,26 +73,26 @@
             else:
                 # Parser didn't find anything, but it wasn't required
                 pass
 
     # Remove scratch data
     del data_collector.scratch
 
-    return SinglePointComputedProperties(**data_collector.computed.dict())
+    return SinglePointResults(**data_collector.computed.dict())
 
 
 # TODO: Finish out this function for parsing full inputs, outputs, and failures
 # for now going to skip failing tests and just focus on simpler parse_computed_props
 # function.
 def parse(
     data_or_path: Union[str, bytes, Path],
     program: str,
     filetype: str = "stdout",
-    input_data: Optional[SinglePointInput] = None,
-) -> Union[SinglePointSuccessfulOutput, SinglePointFailedOutput]:
+    input_data: Optional[ProgramInput] = None,
+) -> Union[SinglePointOutput, ProgramFailure]:
     """Parse a file using the parsers registered for the given program.
 
     Args:
         data_or_path: File contents (str or bytes) or path to the file to parse.
         program: The QC program that generated the output file.
             To see the available programs run:
             >>> from qcparse import registry
@@ -106,49 +103,49 @@
             >>> registry.supported_filetypes('program_name')
         input_data: An optional SinglePointInput object containing the input data
             for the calculation. This will be added to the SinglePointOutput object
             returned by this function and no input data will be parsed from the file.
 
 
     Returns:
-        SinglePointOutput or SinglePointFailure object encapsulating the parsed data.
+        SinglePointOutput or ProgramFailure object encapsulating the parsed data.
     """
     raise NotImplementedError("This function needs work before it is ready to use.")
     # file_content, filepath = get_file_content(data_or_path)
 
     # # Create a data collector object to store the parsed data
     # # Don't collect inputs if input_data is passed
     # collect_inputs = input_data is None
     # # TODO: Handle failed calculations
     # data_collector = single_point_data_collector(collect_inputs)
 
     # # Get the calculation type if filetype is 'stdout'
     # if filetype == "stdout":
-    #     parse_calc_type = import_module(f"qcparse.parsers.{program}").parse_calc_type
-    #     calc_type = parse_calc_type(file_content)
-    #     data_collector.input_data.program_args.calc_type = calc_type
+    #     parse_calctype = import_module(f"qcparse.parsers.{program}").parse_calctype
+    #     calctype = parse_calctype(file_content)
+    #     data_collector.input_data.calctype = calctype
 
     #     # Determine if calculation succeeded
     #     parse_calculation_succeeded = import_module(
     #         f"qcparse.parsers.{program}"
     #     ).calculation_succeeded
     #     if not parse_calculation_succeeded(file_content):
     #         # TODO: Handle failed calculations
     #         pass
 
     #     data_collector.stdout = file_content
     # else:
-    #     calc_type = None
+    #     calctype = None
 
     # # Get all the parsers for the program and filetype
     # parsers: List[ParserSpec] = registry.get_parsers(
     #     program,
     #     filetype=filetype,
     #     collect_inputs=collect_inputs,
-    #     calc_type=calc_type,
+    #     calctype=calctype,
     # )
 
     # # Apply parsers to the file content.
     # for parser_info in parsers:
     #     try:
     #         # This will raise a MatchNotFound error if the parser can't find its data
     #         parser_info.parser(file_content, data_collector)
@@ -171,16 +168,14 @@
     # )
     # if post_process:
     #     post_process(data_collector, file_content, filetype, filepath, input_data)
 
     # # Remove scratch data
     # del data_collector.scratch
 
-    # return SinglePointSuccessfulOutput(**data_collector.dict())
+    # return SinglePointOutput(**data_collector.dict())
 
 
 if __name__ == "__main__":
     # output = parse("./tests/data/water.gradient.out", "terachem", "stdout")
-    props, prov = parse_computed_props(
-        "./tests/data/water.gradient.out", "terachem", "stdout"
-    )
+    props, prov = parse_results("./tests/data/water.gradient.out", "terachem", "stdout")
     print(props)
```

### Comparing `qcparse-0.3.2/qcparse/models.py` & `qcparse-0.4.0/qcparse/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,16 +51,15 @@
 
 def single_point_data_collector(collect_inputs: bool = True) -> ParsedDataCollector:
     """Create a namespace for a single point result."""
     output_obj = ParsedDataCollector()
     if collect_inputs:
         # Input Objects
         output_obj.input_data = ParsedDataCollector()
-        output_obj.input_data.program_args = ParsedDataCollector()
-        output_obj.input_data.program_args.model = ParsedDataCollector()
+        output_obj.input_data.model = ParsedDataCollector()
 
     # Output Objects
     output_obj.computed = ParsedDataCollector()
     output_obj.provenance = ParsedDataCollector()
     output_obj.extras = ParsedDataCollector()
 
     # Scratch space for parsers
```

### Comparing `qcparse-0.3.2/qcparse/parsers/terachem.py` & `qcparse-0.4.0/qcparse/parsers/terachem.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,46 +14,46 @@
 """
 
 import re
 from enum import Enum
 from pathlib import Path
 from typing import Optional, Union
 
-from qcio import Molecule, SinglePointInput, SPCalcType
+from qcio import CalcType, Molecule, ProgramInput
 
 from qcparse.exceptions import MatchNotFoundError
 from qcparse.models import ParsedDataCollector
 
 from .utils import parser, regex_search
 
 
 class FileType(str, Enum):
     stdout = "stdout"
 
 
-def parse_calc_type(string: str) -> SPCalcType:
-    """Parse the calc_type from TeraChem stdout."""
-    calc_types = (
-        (SPCalcType.energy, r"SINGLE POINT ENERGY CALCULATIONS"),
-        (SPCalcType.gradient, r"SINGLE POINT GRADIENT CALCULATIONS"),
-        (SPCalcType.hessian, r"FREQUENCY ANALYSIS"),
+def parse_calctype(string: str) -> CalcType:
+    """Parse the calctype from TeraChem stdout."""
+    calctypes = (
+        (CalcType.energy, r"SINGLE POINT ENERGY CALCULATIONS"),
+        (CalcType.gradient, r"SINGLE POINT GRADIENT CALCULATIONS"),
+        (CalcType.hessian, r"FREQUENCY ANALYSIS"),
     )
-    for calc_type, regex in calc_types:
+    for calctype, regex in calctypes:
         match = re.search(regex, string)
         if match:
-            return calc_type
+            return calctype
     raise MatchNotFoundError(regex, string)
 
 
 def post_process(
     data_collector: ParsedDataCollector,
     file_content: Union[str, bytes],
     filetype: str,
     filepath: Optional[Path] = None,
-    input_data: Optional[SinglePointInput] = None,
+    input_data: Optional[ProgramInput] = None,
 ):
     """Any post processing required after parsing is done here.
 
     Args:
         Must accept 'output' and then all args passed to parse().
     """
 
@@ -81,33 +81,29 @@
     data_collector.computed.energy = float(regex_search(regex, string).group(1))
 
 
 @parser(filetype=FileType.stdout, input_data=True)
 def parse_method(string: str, data_collector: ParsedDataCollector):
     """Parse the method from TeraChem stdout."""
     regex = r"Method: (\S+)"
-    data_collector.input_data.program_args.model.method = regex_search(
-        regex, string
-    ).group(1)
+    data_collector.input_data.model.method = regex_search(regex, string).group(1)
 
 
 @parser(filetype=FileType.stdout)
 def parse_working_directory(string: str, data_collector: ParsedDataCollector):
     """Parse the scratch directory from TeraChem stdout."""
     regex = r"Scratch directory: (.*?)\n"
     data_collector.provenance.working_dir = regex_search(regex, string).group(1)
 
 
 @parser(filetype=FileType.stdout, input_data=True)
 def parse_basis(string: str, data_collector: ParsedDataCollector):
     """Parse the basis from TeraChem stdout."""
     regex = r"Using basis set: (\S+)"
-    data_collector.input_data.program_args.model.basis = regex_search(
-        regex, string
-    ).group(1)
+    data_collector.input_data.model.basis = regex_search(regex, string).group(1)
 
 
 def parse_git_commit(string: str) -> str:
     """Parse TeraChem git commit from TeraChem stdout."""
     regex = r"Git Version: (\S*)"
     return regex_search(regex, string).group(1)
 
@@ -145,15 +141,15 @@
     for regex in FAILURE_REGEXPS:
         if re.search(regex, string):
             # If any match for a failure regex is found, the calculation failed
             return False
     return True
 
 
-@parser(filetype=FileType.stdout, only=[SPCalcType.gradient, SPCalcType.hessian])
+@parser(filetype=FileType.stdout, only=[CalcType.gradient, CalcType.hessian])
 def parse_gradient(string: str, data_collector: ParsedDataCollector):
     """Parse gradient from TeraChem stdout."""
     # This will match all floats after the dE/dX dE/dY dE/dZ header and stop at the
     # terminating ---- line
     regex = r"(?<=dE\/dX\s{12}dE\/dY\s{12}dE\/dZ\n)[\d\.\-\s]+(?=\n-{2,})"
     gradient_string = regex_search(regex, string).group()
 
@@ -164,15 +160,15 @@
     gradient = []
     for i in range(0, len(values), 3):
         gradient.append(values[i : i + 3])
 
     data_collector.computed.gradient = gradient
 
 
-@parser(filetype=FileType.stdout, only=[SPCalcType.hessian])
+@parser(filetype=FileType.stdout, only=[CalcType.hessian])
 def parse_hessian(string: str, data_collector: ParsedDataCollector):
     """Parse Hessian Matrix from TeraChem stdout
 
     Notes:
         This function searches the entire document N times for all regex matches where
         N is the number of atoms. This makes the function's code easy to reason about.
         If performance becomes an issues for VERY large Hessians (unlikely) you can
```

### Comparing `qcparse-0.3.2/qcparse/parsers/utils.py` & `qcparse-0.4.0/qcparse/parsers/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 import importlib
 import inspect
 import re
 from typing import List, Optional
 
-from qcio import SPCalcType
+from qcio import CalcType
 
 from qcparse.exceptions import MatchNotFoundError
 from qcparse.registry import registry
 
 
 def parser(
     filetype: str,
     *,
     required: bool = True,
     input_data: bool = False,
-    only: Optional[List[SPCalcType]] = None,
+    only: Optional[List[CalcType]] = None,
 ):
     """Decorator to register a function as a parser for program output filetype.
 
     Args:
         filetype: The filetype the parser operates on.
         required: If True and the parser fails a MatchNotFoundError will be raised.
             If False and the parser fails the value will be ignored.
         input_data: Whether the parser is for input data, such as method, basis, or a
             molecular structure, instead of computed output data. If True the parser
             will be not be called if a SinglePointInput object is passed as input_data
             to the top-level parse function.
-        only: Only register the parser on these SPCalcTypes. If None the parser will be
-            registered for all SPCalcTypes.
+        only: Only register the parser on these CalcTypes. If None the parser will be
+            registered for all CalcTypes.
     """
 
     def decorator(func):
         # Get the current module name. Should match program name.
         module = inspect.getmodule(func).__name__
         program_name = module.split(".")[-1]
```

### Comparing `qcparse-0.3.2/qcparse/registry.py` & `qcparse-0.4.0/qcparse/registry.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from collections import defaultdict
 from typing import Callable, Dict, List, Optional
 
 from pydantic import BaseModel
-from qcio import SPCalcType
+from qcio import CalcType
 
 from .exceptions import RegistryError
 
 
 class ParserSpec(BaseModel):
     """Information about a parser function.
 
     Attributes:
         parser: The parser function.
         filetype: The filetype that the parser is for.
         required: Whether the parser is required to be successful for the parsing to
             be considered successful. If True and the parser fails a MatchNotFoundError
             will be raised. If False and the parser fails the value will be ignored.
-        calc_types: The calculation types that the parser work on.
+        calctypes: The calculation types that the parser work on.
     """
 
     parser: Callable
     filetype: str
     required: bool
     input_data: bool = False
-    calc_types: List[SPCalcType]
+    calctypes: List[CalcType]
 
 
 class ParserRegistry(BaseModel):
     """Registry for parser functions."""
 
     registry: Dict[str, List[ParserSpec]] = defaultdict(list)
 
     def register(
         self,
         program: str,
         parser: Callable,
         filetype: str,
         required: bool,
         input_data: bool,
-        only: Optional[List[SPCalcType]],
+        only: Optional[List[CalcType]] = None,
     ) -> None:
         """Register a new parser function.
 
         Args:
             program: The program that the parser is for.
             parser: The parser function.
             filetype: The filetype that the parser is for.
@@ -55,33 +55,32 @@
         """
         parser_info = ParserSpec(
             parser=parser,
             filetype=filetype,
             required=required,
             input_data=input_data,
             # If only not passed then register for all calculation types
-            calc_types=only
-            or [SPCalcType.energy, SPCalcType.gradient, SPCalcType.hessian],
+            calctypes=only or [CalcType.energy, CalcType.gradient, CalcType.hessian],
         )
         self.registry[program].append(parser_info)
 
     def get_parsers(
         self,
         program: str,
         filetype: Optional[str] = None,
         collect_inputs: bool = True,
-        calc_type: Optional[SPCalcType] = None,
+        calctype: Optional[CalcType] = None,
     ) -> List[ParserSpec]:
         """Get all parser functions for a given program.
 
         Args:
             program: The program to get parsers for.
             filetype: If given only return parsers for this filetype.
             collect_inputs: If False return only parsers for output data.
-            calc_type: Filter parsers for a given calculation type.
+            calctype: Filter parsers for a given calculation type.
 
         Returns:
             List of ParserSpec objects.
 
         """
 
         parsers: List[ParserSpec] = self.registry[program]
@@ -90,16 +89,16 @@
 
         if filetype:
             parsers = [p_spec for p_spec in parsers if p_spec.filetype == filetype]
 
         if not collect_inputs:
             parsers = [p_spec for p_spec in parsers if not p_spec.input_data]
 
-        if calc_type:
-            parsers = [p_spec for p_spec in parsers if calc_type in p_spec.calc_types]
+        if calctype:
+            parsers = [p_spec for p_spec in parsers if calctype in p_spec.calctypes]
         return parsers
 
     def supported_programs(self) -> List[str]:
         """Get all programs with registered parsers.
 
         Returns:
             List of program names.
```

### Comparing `qcparse-0.3.2/qcparse/utils.py` & `qcparse-0.4.0/qcparse/utils.py`

 * *Files identical despite different names*

