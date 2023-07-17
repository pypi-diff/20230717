# Comparing `tmp/python_spectrometer-2023.6.1-py3-none-any.whl.zip` & `tmp/python_spectrometer-2023.7.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,17 @@
-Zip file size: 58829 bytes, number of entries: 14
+Zip file size: 59629 bytes, number of entries: 15
 -rw-r--r--  2.0 unx     4141 b- defN 20-Feb-02 00:00 python_spectrometer/__init__.py
--rw-r--r--  2.0 unx    77781 b- defN 20-Feb-02 00:00 python_spectrometer/core.py
+-rw-r--r--  2.0 unx    78709 b- defN 20-Feb-02 00:00 python_spectrometer/core.py
 -rw-r--r--  2.0 unx     1707 b- defN 20-Feb-02 00:00 python_spectrometer/daq/__init__.py
--rw-r--r--  2.0 unx     1148 b- defN 20-Feb-02 00:00 python_spectrometer/daq/__init__.pyi
--rw-r--r--  2.0 unx     3559 b- defN 20-Feb-02 00:00 python_spectrometer/daq/core.py
--rw-r--r--  2.0 unx     6806 b- defN 20-Feb-02 00:00 python_spectrometer/daq/qcodes.py
--rw-r--r--  2.0 unx    41672 b- defN 20-Feb-02 00:00 python_spectrometer/daq/settings.py
--rw-r--r--  2.0 unx     2275 b- defN 20-Feb-02 00:00 python_spectrometer/daq/simulator.py
--rw-r--r--  2.0 unx     3844 b- defN 20-Feb-02 00:00 python_spectrometer/daq/swabian_instruments.py
--rw-r--r--  2.0 unx    18418 b- defN 20-Feb-02 00:00 python_spectrometer/daq/zurich_instruments.py
-?rw-r--r--  2.0 unx     5649 b- defN 20-Feb-02 00:00 python_spectrometer-2023.6.1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 python_spectrometer-2023.6.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx    35168 b- defN 20-Feb-02 00:00 python_spectrometer-2023.6.1.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1292 b- defN 20-Feb-02 00:00 python_spectrometer-2023.6.1.dist-info/RECORD
-14 files, 203547 bytes uncompressed, 56651 bytes compressed:  72.2%
+-rw-r--r--  2.0 unx     1165 b- defN 20-Feb-02 00:00 python_spectrometer/daq/__init__.pyi
+-rw-r--r--  2.0 unx     5675 b- defN 20-Feb-02 00:00 python_spectrometer/daq/atsaverage.py
+-rw-r--r--  2.0 unx     3572 b- defN 20-Feb-02 00:00 python_spectrometer/daq/core.py
+-rw-r--r--  2.0 unx     6964 b- defN 20-Feb-02 00:00 python_spectrometer/daq/qcodes.py
+-rw-r--r--  2.0 unx    34491 b- defN 20-Feb-02 00:00 python_spectrometer/daq/settings.py
+-rw-r--r--  2.0 unx     2274 b- defN 20-Feb-02 00:00 python_spectrometer/daq/simulator.py
+-rw-r--r--  2.0 unx     3843 b- defN 20-Feb-02 00:00 python_spectrometer/daq/swabian_instruments.py
+-rw-r--r--  2.0 unx    18583 b- defN 20-Feb-02 00:00 python_spectrometer/daq/zurich_instruments.py
+?rw-r--r--  2.0 unx     5649 b- defN 20-Feb-02 00:00 python_spectrometer-2023.7.1.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 python_spectrometer-2023.7.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx    35168 b- defN 20-Feb-02 00:00 python_spectrometer-2023.7.1.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1386 b- defN 20-Feb-02 00:00 python_spectrometer-2023.7.1.dist-info/RECORD
+15 files, 203414 bytes uncompressed, 57301 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -6,14 +6,17 @@
 
 Filename: python_spectrometer/daq/__init__.py
 Comment: 
 
 Filename: python_spectrometer/daq/__init__.pyi
 Comment: 
 
+Filename: python_spectrometer/daq/atsaverage.py
+Comment: 
+
 Filename: python_spectrometer/daq/core.py
 Comment: 
 
 Filename: python_spectrometer/daq/qcodes.py
 Comment: 
 
 Filename: python_spectrometer/daq/settings.py
@@ -24,20 +27,20 @@
 
 Filename: python_spectrometer/daq/swabian_instruments.py
 Comment: 
 
 Filename: python_spectrometer/daq/zurich_instruments.py
 Comment: 
 
-Filename: python_spectrometer-2023.6.1.dist-info/METADATA
+Filename: python_spectrometer-2023.7.1.dist-info/METADATA
 Comment: 
 
-Filename: python_spectrometer-2023.6.1.dist-info/WHEEL
+Filename: python_spectrometer-2023.7.1.dist-info/WHEEL
 Comment: 
 
-Filename: python_spectrometer-2023.6.1.dist-info/licenses/LICENSE
+Filename: python_spectrometer-2023.7.1.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: python_spectrometer-2023.6.1.dist-info/RECORD
+Filename: python_spectrometer-2023.7.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## python_spectrometer/__init__.py

```diff
@@ -91,11 +91,11 @@
 
     spect.plot_raw = True  # Updates the figure accordingly
     spect.plot_timetrace = False
 
 See the documentation of :class:`~core.Spectrometer` and its methods
 for more information.
 """
-__version__ = '2023.6.1'
+__version__ = '2023.7.1'
 
 from . import daq
 from .core import Spectrometer
```

## python_spectrometer/core.py

```diff
@@ -3,17 +3,16 @@
 import inspect
 import os
 import shelve
 import warnings
 from datetime import datetime
 from pathlib import Path
 from pprint import pprint
-from typing import (Any, Callable, ContextManager, Dict, Generator, Iterable,
-                    Iterator, List, Literal, Mapping, Optional, Sequence,
-                    Tuple, Union)
+from typing import (Any, Callable, ContextManager, Dict, Generator, Iterable, Iterator, List,
+                    Literal, Mapping, Optional, Sequence, Tuple, Union)
 from unittest import mock
 
 import dill
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib import colors, gridspec
 from qutil import io
@@ -51,16 +50,17 @@
     def __init__(self, data: Dict[_keyT, Any], plot_raw: bool = False,
                  plot_timetrace: bool = False, plot_cumulative: bool = False,
                  plot_negative_frequencies: bool = True, plot_absolute_frequencies: bool = True,
                  plot_amplitude: bool = True, plot_density: bool = True,
                  plot_cumulative_normalized: bool = False, plot_style: _styleT = 'fast',
                  plot_update_mode: str = 'fast', plot_dB_scale: bool = False, prop_cycle=None,
                  raw_unit: str = 'V', processed_unit: str = 'V',
-                 figure_kw: Optional[Mapping] = None, subplot_kw: Optional[Mapping] = None,
-                 gridspec_kw: Optional[Mapping] = None, legend_kw: Optional[Mapping] = None):
+                 uses_windowed_estimator: bool = True, figure_kw: Optional[Mapping] = None,
+                 subplot_kw: Optional[Mapping] = None, gridspec_kw: Optional[Mapping] = None,
+                 legend_kw: Optional[Mapping] = None):
         """A helper class that manages plotting spectrometer data."""
         self._data = data
 
         # settable properties exposed to Spectrometer
         self._plot_raw = plot_raw
         self._plot_timetrace = plot_timetrace
         self._plot_cumulative = plot_cumulative
@@ -75,14 +75,15 @@
         self._processed_unit = processed_unit
 
         # For dB scale plots, default to the first spectrum acquired.
         self._reference_spectrum: Optional[_keyT] = None
 
         self.prop_cycle = prop_cycle or plt.rcParams['axes.prop_cycle']
         self.raw_unit = raw_unit
+        self.uses_windowed_estimator = uses_windowed_estimator
 
         self._leg = None
         self.axes = {key: dict.fromkeys(self.LINE_TYPES) for key in self.PLOT_TYPES}
         self.lines = dict()
         self.figure_kw = figure_kw or dict()
         self.subplot_kw = subplot_kw or dict()
         self.gridspec_kw = gridspec_kw or dict()
@@ -367,15 +368,15 @@
             line, = self.axes['cumulative'][line_type].plot(x, y, **self.line_props(key[0], d))
         self.update_line_attrs(['cumulative'], [line_type], [key], stale=False, line=line)
 
     def time_plot(self, key, line_type):
         y = self._data[key][f'timetrace_{line_type}'][-1]
         if np.iscomplexobj(y):
             y = np.abs(y)
-        x = np.arange(y.size) / self._data[key]['settings'].fs
+        x = np.arange(y.size) / self._data[key]['settings']['fs']
 
         d = self.lines[key]['time'][line_type]
         if line := d['line']:
             line.set_data(x, y)
             line.set_color(self.line_props(key[0], d)['color'])
             line.set_alpha(self.line_props(key[0], d)['alpha'])
             line.set_zorder(self.line_props(key[0], d)['zorder'])
@@ -557,32 +558,32 @@
     def set_subplotspec(self, plot: str, gs: gridspec.GridSpec):
         for line in self.lines_to_draw:
             self.axes[plot][line].set_subplotspec(gs)
 
     def set_xlims(self):
         # Frequency-axis plots
         right = max((
-            self._data[k]['settings'].f_max
+            self._data[k]['settings']['f_max']
             + (self._data[k]['settings'].get('freq', 0)
                if self.plot_absolute_frequencies else 0)
             for k in self.shown
         ), default=None)
         if (
                 not self.plot_negative_frequencies
                 or self.axes['main']['processed'].get_xscale() == 'log'
         ):
             left = min((
-                self._data[k]['settings'].f_min
+                self._data[k]['settings']['f_min']
                 + (self._data[k]['settings'].get('freq', 0)
                    if self.plot_absolute_frequencies else 0)
                 for k in self.shown
             ), default=None)
         else:
             left = min((
-                - self._data[k]['settings'].f_max
+                - self._data[k]['settings']['f_max']
                 + (self._data[k]['settings'].get('freq', 0)
                    if self.plot_absolute_frequencies else 0)
                 for k in self.shown
             ), default=None)
 
         with filter_warnings('ignore', UserWarning):
             # ignore warnings issued for empty plots with log scales
@@ -673,25 +674,27 @@
 
     def get_freq_data(self, key, line_type, dB, reference=False,
                       cumulative=False) -> Tuple[np.ndarray, np.ndarray]:
         x = self._data[key][f'f_{line_type}'].copy()
         if self.plot_absolute_frequencies:
             x += self._data[key]['settings'].get('freq', 0)
 
-        window = self._data[key]['settings'].get('window', 'hann')
-        nperseg = self._data[key]['settings'].nperseg
-        fs = self._data[key]['settings'].fs
+        window = self._data[key]['settings'].get(
+            'window', 'hann' if self.uses_windowed_estimator else 'boxcar'
+        )
+        nperseg = self._data[key]['settings']['nperseg']
+        fs = self._data[key]['settings']['fs']
 
         y = np.mean(self._data[key][f'S_{line_type}'], axis=0)
         if not self.plot_density or dB:
             # Need to calculate dB using the spectrum, not the density
             if isinstance(window, str) or isinstance(window, tuple):
-                window = signal.get_window(window, nperseg).astype(y.dtype)
+                window = signal.get_window(window, nperseg)
             else:
-                window = np.asarray(window, y.dtype)
+                window = np.asarray(window)
             y *= fs * (window ** 2).sum() / window.sum() ** 2
         if self.plot_amplitude and not cumulative:
             y **= 0.5
 
         if dB and not reference:
             _, y0 = self.get_freq_data(self.reference_spectrum, line_type, dB=True, reference=True)
             with np.errstate(divide='ignore', invalid='ignore'):
@@ -917,43 +920,50 @@
                  procfn: Optional[Union[Callable, Sequence[Callable]]] = None,
                  plot_raw: bool = False, plot_timetrace: bool = False,
                  plot_cumulative: bool = False, plot_negative_frequencies: bool = True,
                  plot_absolute_frequencies: bool = True, plot_amplitude: bool = True,
                  plot_density: bool = True, plot_cumulative_normalized: bool = True,
                  plot_style: _styleT = 'fast',
                  plot_update_mode: Literal['fast', 'always', 'never'] = 'fast',
-                 plot_dB_scale: bool = False, prop_cycle=None, savepath: _pathT = None,
+                 plot_dB_scale: bool = False, prop_cycle=None,
+                 purge_raw_data: bool = False, savepath: _pathT = None,
                  compress: bool = True, raw_unit: str = 'V', processed_unit: str = 'V',
                  figure_kw: Optional[Mapping] = None, subplot_kw: Optional[Mapping] = None,
                  gridspec_kw: Optional[Mapping] = None, legend_kw: Optional[Mapping] = None):
 
         self._data: Dict[Tuple[int, str], Dict] = {}
         self._savepath: Optional[Path] = None
 
         self.daq = daq
         self.procfn = chain(*procfn) if np.iterable(procfn) else chain(procfn or Id)
         self.savepath = savepath or '~/python_spectrometer/' + datetime.now().strftime('%Y-%m-%d')
         self.compress = compress
+        if purge_raw_data:
+            warnings.warn('Enabling purge raw data might break some plotting features!',
+                          UserWarning, stacklevel=2)
+        self.purge_raw_data = purge_raw_data
 
         if psd_estimator is None:
             psd_estimator = {}
         if callable(psd_estimator):
             self.psd_estimator = psd_estimator
         elif isinstance(psd_estimator, Mapping):
             self.psd_estimator = partial(welch, **psd_estimator)
         else:
-            raise TypeError('psd_estimator should be callable or kwarg_dict for welch().')
+            raise TypeError('psd_estimator should be callable or kwarg dict for welch().')
+        uses_windowed_estimator = 'window' in inspect.signature(self.psd_estimator).parameters
 
         self._plot_manager = _PlotManager(self._data, plot_raw, plot_timetrace,
                                           plot_cumulative, plot_negative_frequencies,
                                           plot_absolute_frequencies, plot_amplitude,
                                           plot_density, plot_cumulative_normalized,
                                           plot_style, plot_update_mode, plot_dB_scale,
-                                          prop_cycle, raw_unit, processed_unit, figure_kw,
-                                          subplot_kw, gridspec_kw, legend_kw)
+                                          prop_cycle, raw_unit, processed_unit,
+                                          uses_windowed_estimator, figure_kw, subplot_kw,
+                                          gridspec_kw, legend_kw)
 
     # Expose plot properties from plot manager
     _to_expose = ('fig', 'ax', 'ax_raw', 'leg', 'plot_raw', 'plot_timetrace', 'plot_cumulative',
                   'plot_negative_frequencies', 'plot_absolute_frequencies', 'plot_amplitude',
                   'plot_density', 'plot_cumulative_normalized', 'plot_style', 'plot_update_mode',
                   'plot_dB_scale', 'reference_spectrum', 'processed_unit')
     locals().update({attr: _forward_property(_PlotManager, '_plot_manager', attr)
@@ -1070,20 +1080,22 @@
         return parsed
 
     def _repr_keys(self, *keys) -> str:
         if not keys:
             keys = self.keys()
         return '\n'.join((str(key) for key in sorted(self.keys()) if key in keys))
 
+    @mock.patch.multiple('numpy.compat.py3k.pickle',
+                         Unpickler=dill.Unpickler, Pickler=dill.Pickler)
     def _savefn(self, file: _pathT, **kwargs):
         file = io.check_path_length(file)
         if self.compress:
             np.savez_compressed(str(file), **_to_native_types(kwargs))
         else:
-            np.save(str(file), **_to_native_types(kwargs))
+            np.savez(str(file), **_to_native_types(kwargs))
 
     @classmethod
     def _make_kwargs_compatible(cls, kwargs: Dict[str, Any]) -> Dict[str, Any]:
         compatible_kwargs = dict()
         signature = inspect.signature(cls)
 
         # Replace old param names by new ones ...
@@ -1162,36 +1174,42 @@
         self._plot_manager.add_new_line_entry(key)
 
         iterator = self.daq.acquire(**settings)
         for i in progressbar(count(), disable=not progress, total=settings.n_avg,
                              desc=f'Acquiring {settings.n_avg} spectra with key {key}'):
             # Promote warnings to errors during data acquisition since usually
             # something will go wrong at some point anyway.
-            with filter_warnings('error'):
-                try:
-                    fetched_data = next(iterator)
-                    processed_data = self._process_data(fetched_data, **settings)
-                except StopIteration as stop:
-                    measurement_metadata = stop.value
-                    break
-                except Exception as error:
-                    # Make sure we are left in a reproducible state
-                    self.drop(key)
-                    msg = 'Something went wrong during data acquisition'
-                    if 'fetched_data' in locals():
-                        msg = msg + (f'. {self.daq.acquire} last returned the following data:\n '
-                                     f'{fetched_data}')
-                    raise RuntimeError(msg) from error
+            try:
+                fetched_data = next(iterator)
+                processed_data = self._process_data(fetched_data, **settings)
+            except StopIteration as stop:
+                measurement_metadata = stop.value
+                break
+            except Exception as error:
+                # Make sure we are left in a reproducible state
+                self.drop(key)
+                msg = 'Something went wrong during data acquisition'
+                if 'fetched_data' in locals():
+                    msg = msg + (f'. {self.daq.acquire} last returned the following data:\n '
+                                 f'{fetched_data}')
+                raise RuntimeError(msg) from error
 
             # TODO: This could fail if the iterator was empty and processed_data was never assigned
             self._data[key].update(_merge_data_dicts(self._data[key], processed_data))
             self.set_reference_spectrum(self.reference_spectrum)
             self.show(key)
 
         self._data[key].update(measurement_metadata=measurement_metadata)
+        if self.purge_raw_data:
+            del self._data[key]['timetrace_raw']
+            del self._data[key]['timetrace_processed']
+            del self._data[key]['f_raw']
+            del self._data[key]['S_raw']
+            self._data[key]['S_processed'] = np.mean(self._data[key]['S_processed'], axis=0)[None]
+
         self._savefn(filepath, **self._data[key])
 
     take.__doc__ = (take.__doc__.replace(8*' ', '')
                     + '\n\nDAQ Parameters'
                     + '\n==============\n'
                     + '\n'.join((f'{key} : {val}' for key, val in daq_settings._doc_.items())))
```

## python_spectrometer/daq/__init__.pyi

```diff
@@ -1,17 +1,18 @@
-__all__ = ['qcodes', 'simulator', 'swabian_instruments', 'zurich_instruments', 'Keysight344xxA',
-           'NationalInstrumentsUSB6003', 'SwabianInstrumentsTimeTagger', 'DAQSettings',
-           'QoptColoredNoise', 'ZurichInstrumentsMFLIScope', 'ZurichInstrumentsMFLIDAQ']
+__all__ = ['atsaverage', 'qcodes', 'simulator', 'swabian_instruments', 'zurich_instruments',
+           'AlazarATS9xx0', 'Keysight344xxA', 'NationalInstrumentsUSB6003',
+           'SwabianInstrumentsTimeTagger', 'DAQSettings', 'QoptColoredNoise',
+           'ZurichInstrumentsMFLIScope', 'ZurichInstrumentsMFLIDAQ']
 
-from . import qcodes, simulator, swabian_instruments, zurich_instruments
+from . import atsaverage, qcodes, simulator, swabian_instruments, zurich_instruments
+from .atsaverage import AlazarATS9xx0
 from .qcodes import (Keysight344xxA, NationalInstrumentsUSB6003,
                      # Backwards "compatibility"
                      keysight_344xxA, national_instruments_daq)
-from .settings import (BoundedSet, ContinuousInterval, DAQSettings,
-                       DiscreteInterval)
+from .settings import DAQSettings
 from .simulator import (QoptColoredNoise,
                         # Backwards "compatibility"
                         qopt_colored_noise)
 from .swabian_instruments import (SwabianInstrumentsTimeTagger,
                                   # Backwards "compatibility"
                                   timetagger)
 from .zurich_instruments import (ZurichInstrumentsMFLIDAQ, ZurichInstrumentsMFLIScope,
```

## python_spectrometer/daq/core.py

```diff
@@ -1,19 +1,18 @@
 from __future__ import annotations
 
 import abc
 import warnings
 from abc import ABC
 from typing import Any, Dict, Iterator, Type
 
+from python_spectrometer.daq import DAQSettings
 from qutil.functools import cached_property
 from qutil.misc import filter_warnings
 
-from .settings import DAQSettings
-
 try:
     from numpy.typing import NDArray
 except ImportError:
     from numpy import ndarray as NDArray
 
 
 class DAQ(ABC):
```

## python_spectrometer/daq/qcodes.py

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
 import dataclasses
 from types import ModuleType
 from typing import Any, Dict, Iterator, Type
 
+from python_spectrometer.daq.core import DAQ
+from python_spectrometer.daq.settings import DAQSettings
+from qutil.domains import ContinuousInterval
 from qutil.functools import cached_property
 from qutil.misc import import_or_mock
 
-from python_spectrometer.daq.core import DAQ
-from python_spectrometer.daq.settings import ContinuousInterval, DAQSettings
-
 try:
     from numpy.typing import NDArray
 except ImportError:
     from numpy import ndarray as NDArray
 
 for name, package, local_name in [
     ('qcodes.instrument_drivers.Keysight.private.Keysight_344xxA_submodules', None,
@@ -44,25 +44,26 @@
     setup, acquire : Callable
 
     """
     dmm: _Keysight_344xxA = dataclasses.field()  # noqa
 
     @cached_property
     def DAQSettings(self) -> Type[DAQSettings]:
-        this = self
         class Keysight344xxASettings(DAQSettings):
             DEFAULT_FS = 1 / 3e-4
 
             @property
-            def ALLOWED_FS(self) -> ContinuousInterval:
+            def ALLOWED_FS(this) -> ContinuousInterval:
                 # timer_minimum is dynamic (depends on dmm.aperture_time() and others)
-                dt_min = this.dmm.aperture_time.vals.min_value
-                dt_max = this.dmm.aperture_time.vals.max_value
-                return (ContinuousInterval(upper=1 / this.dmm.sample.timer_minimum())
-                        & ContinuousInterval(lower=1 / dt_max, upper=1 / dt_min))
+                dt_min = self.dmm.aperture_time.vals.min_value
+                dt_max = self.dmm.aperture_time.vals.max_value
+                return (ContinuousInterval(upper=1 / self.dmm.sample.timer_minimum(),
+                                           precision=this.PRECISION)
+                        & ContinuousInterval(lower=1 / dt_max, upper=1 / dt_min,
+                                             precision=this.PRECISION))
 
         return Keysight344xxASettings
 
     def setup(self, **settings) -> Dict[str, Any]:
         """Sets up a Keysight DMM to acquire a timetrace for given parameters."""
         # Set the integration time (automatically selects aperture mode)
         self.dmm.aperture_time(1 / settings.get('fs', self.DAQSettings.DEFAULT_FS))
@@ -87,43 +88,39 @@
         for _ in range(n_avg):
             yield self.dmm.timetrace.get()
         return self.dmm.get_idn()
 
 
 @dataclasses.dataclass
 class NationalInstrumentsUSB(DAQ):
-    """Generates setup and acquisition functions for a NI DAQ.
+    """Handles data acquisition using a NI USB-DAQ.
 
     Requires the nidaqmx package.
 
     See :class:`~python_spectrometer.core.Spectrometer` for
     more details on usage and
     :class:`~python_spectrometer.daq.settings.DAQSettings`
     for more information on setup parameters.
 
     Parameters
     ----------
     ni_daq : DAQ.DAQAnalogInputs
         The qcodes DAQAnalogInputs instrument.
 
-    Returns
-    -------
-    setup, acquire : Callable
-
     Examples
     --------
     Use a NI DAQ to convert an analog input to a digital signal::
 
         from qcodes_contrib_drivers.drivers.NationalInstruments import DAQ
         import nidaqmx
         ni_daq = DAQ.DAQAnalogInputs('ni_daq', 'Dev1',
-                                     rate=1, channels={0: 3},
+                                     rate=1, channels={'mychan': 3},
                                      task=nidaqmx.Task(),
                                      samples_to_read=2)
-        setup, acquire = national_instruments_daq(ni_daq)
+        pyspec_daq = national_instruments_daq(ni_daq)
 
     """
     ni_daq: DAQAnalogInputs = dataclasses.field()  # noqa
 
     def __post_init__(self):
         if not isinstance(globals().get('nidaqmx'), ModuleType):
             raise ImportError(
@@ -173,15 +170,16 @@
 
 
 class NationalInstrumentsUSB6003(NationalInstrumentsUSB):
 
     @cached_property
     def DAQSettings(self) -> Type[DAQSettings]:
         class NationalInstrumentsDAQSettings(DAQSettings):
-            ALLOWED_FS = ContinuousInterval(lower=18.626450e-3, upper=100e3)
+            ALLOWED_FS = ContinuousInterval(lower=18.626450e-3, upper=100e3,
+                                            precision=DAQSettings.PRECISION)
 
         return NationalInstrumentsDAQSettings
 
 
 # Alias for backwards compatibility only.
 keysight_344xxA = Keysight344xxA
 national_instruments_daq = NationalInstrumentsUSB
```

## python_spectrometer/daq/settings.py

```diff
@@ -24,59 +24,49 @@
 properties. For instance, the highest frequency f_max cannot be larger
 than fs/2 by virtue of Nyquist's theorem. Hence, if there are
 conflicting parameters, the class tries to resolve them by adjusting
 one or the other and otherwise raising an error. Alternatively, a
 certain parameter might be constrained by hardware limitations. These
 can be implemented by subclassing :class:`.DAQSettings` and overriding
 the attributes :attr:`.DAQSettings.ALLOWED_FS` etc. There exist custom
-types for representing constraints. These are the classes
-:class:`.DiscreteInterval`, :class:`.ContinuousInterval`, and
-:class:`.BoundedSet`, whose purpose should be self-explanatory.
+types for representing constraints in :mod:`qutil:qutil.domains`.
 
 The method :meth:`.DAQSettings.to_consistent_dict` resolves all
 dictionary items into a :class:`dict` dictionary which contains all
 interdependent parameters validated for consistency.
 
 Internally, interdependent parameters are first cast to a value allowed
-by their :class:`.Domain` (which implements constraints both by
-hardware and other parameters) and then to the correct type. Finally,
-other parameters that depend on it are tried to be adjusted if
-necessary.
+by their :class:`qutil:~qutil.domains.Domain` (which implements
+constraints both by hardware and other parameters) and then to the
+correct type. Finally, other parameters that depend on it are tried to
+be adjusted if necessary.
 
 """
 from __future__ import annotations
 
-import abc
 import builtins
 import inspect
 import numbers
 import platform
 import textwrap
 import warnings
-from abc import ABC
 from collections import ChainMap
 from copy import copy
-from dataclasses import dataclass, field
-from math import ceil, floor, inf, isinf, nan
-from typing import (Any, Callable, Container, Dict, Generic, Iterable,
-                    Protocol, Tuple, TypeVar, Union)
+from math import ceil, floor, inf, isinf
+from typing import Any, Callable, Dict, Tuple, TypeVar
 
-from numpy import iterable as is_iterable
+from numpy import finfo
 from packaging import version
+from qutil.domains import BoundedSet, ContinuousInterval, DiscreteInterval, Domain, Interval
 from qutil.functools import wraps
-from qutil.itertools import next_closest, next_largest, next_smallest
 
 _T = TypeVar("_T")
 _KT = TypeVar("_KT")
 _VT = TypeVar("_VT")
 _RealT = TypeVar("_RealT", bound=numbers.Real)
-_IntegralT = TypeVar("_IntegralT", bound=numbers.Integral)
-_BoundT = Union[Callable[[], _RealT], _RealT]
-_BoundT = Union[Iterable[_BoundT], _BoundT]
-
 
 _doc_ = {
     'fs': "float.\n\tThe sampling rate. Default: ``2*f_max`` or :attr:`DEFAULT_FS`.",
     'df': "float.\n\t" r"The frequency spacing :math:`\Delta f`. If given, supersedes "
           ":attr:`f_min` for computing the total duration of the record. Default: :attr:`f_min` "
           "or :attr:`DEFAULT_DF`.",
     'f_max': "float.\n\tThe maximum frequency displayed. Also used for filters. Defaults to half "
@@ -110,208 +100,14 @@
         if value not in domain:
             raise ValueError(f'{param} must be in {domain}, not {value}.')
         f(self, value)
 
     return wrapper
 
 
-class Bound(Generic[_RealT]):
-    """A lazily evaluated bound."""
-
-    def __init__(self, default: _RealT):
-        self.default = default
-
-    def __set_name__(self, owner, name):
-        self._name = f'_{name}'
-
-    def __get__(self, instance, owner) -> _RealT:
-        value = getattr(instance, self._name, set())
-        evaluated = set()
-        for item in value:
-            if callable(item):
-                evaluated.add(item())
-            else:
-                evaluated.add(item)
-        if self._name.startswith('_lower'):
-            return max(evaluated, default=inf)
-        if self._name.startswith('_upper'):
-            return min(evaluated, default=-inf)
-        raise NameError('Bound descriptor instance name should start with lower or upper')
-
-    def __set__(self, instance, value):
-        if value is self:
-            value = self.default
-        if not is_iterable(value):
-            value = {value}
-        else:
-            value = set(value)
-        setattr(instance, self._name, value)
-
-
-class Bounded(Protocol[_RealT]):
-    """An object with bounds."""
-    lower: _BoundT
-    upper: _BoundT
-
-
-class Domain(Container[_RealT], Bounded[_RealT]):
-    """A domain that constrains the allowed values a parameter can take."""
-    lower: _BoundT[_RealT]
-    upper: _BoundT[_RealT]
-
-    def __lt__(self, value: _RealT) -> bool:
-        return self.max() < value
-
-    def __gt__(self, value: _RealT) -> bool:
-        return self.min() > value
-
-    @abc.abstractmethod
-    def __and__(self, other: object) -> Domain:
-        ...
-
-    def __contains__(self, value: object) -> True:
-        return isinstance(value, numbers.Real) and not (value > self or value < self)
-
-    @abc.abstractmethod
-    def min(self) -> _RealT:
-        ...
-
-    @abc.abstractmethod
-    def max(self) -> _RealT:
-        ...
-
-    @abc.abstractmethod
-    def next_closest(self, value: _RealT) -> _RealT:
-        ...
-
-    @abc.abstractmethod
-    def next_smallest(self, value: _RealT) -> _RealT:
-        ...
-
-    @abc.abstractmethod
-    def next_largest(self, value: _RealT) -> _RealT:
-        ...
-
-
-@dataclass
-class Interval(Domain[_RealT], Bounded[_RealT], ABC):
-    """An interval with lower and upper bounds."""
-    lower: _BoundT[_RealT] = field(default=Bound[_RealT](-inf))
-    upper: _BoundT[_RealT] = field(default=Bound[_RealT](inf))
-
-    def __and__(self, other: object) -> Domain:
-        if isinstance(other, Interval):
-            cls = type(self)
-            return cls(self._lower | other._lower, self._upper | other._upper)
-        if isinstance(other, Iterable):
-            return BoundedSet(other) & self
-        return NotImplemented
-
-    def min(self) -> _RealT:
-        return self.lower
-
-    def max(self) -> _RealT:
-        return self.upper
-
-
-@dataclass
-class DiscreteInterval(Interval[_IntegralT], Bounded[_IntegralT]):
-    """A discrete interval that only allows integral values."""
-    lower: _BoundT[_IntegralT] = field(default=Bound[_IntegralT](-inf))
-    upper: _BoundT[_IntegralT] = field(default=Bound[_IntegralT](inf))
-
-    def __contains__(self, value: object) -> bool:
-        return isinstance(value, numbers.Integral) and super().__contains__(value)
-
-    def next_closest(self, value: _RealT) -> int:
-        if value < self:
-            return ceil(self.min())
-        if value > self:
-            return floor(self.max())
-        return round(value)
-
-    def next_smallest(self, value: _RealT) -> int:
-        if value < self:
-            return ceil(self.min())
-        if value > self:
-            return floor(self.max())
-        return floor(value)
-
-    def next_largest(self, value: _RealT) -> int:
-        if value < self:
-            return ceil(self.min())
-        if value > self:
-            return floor(self.max())
-        return ceil(value)
-
-
-class ContinuousInterval(Interval[_RealT]):
-    """A continuous interval that allows any value within its bounds."""
-
-    def next_closest(self, value: _RealT) -> _RealT:
-        if value < self:
-            return self.min()
-        if value > self:
-            return self.max()
-        return value
-
-    def next_smallest(self, value: _RealT) -> _RealT:
-        return self.next_closest(value)
-
-    def next_largest(self, value: _RealT) -> _RealT:
-        return self.next_closest(value)
-
-
-class BoundedSet(Domain[_RealT], frozenset, Bounded[_RealT]):
-    """A finite set of numbers with lower and upper bounds."""
-    lower: _BoundT[_RealT] = Bound[_RealT](-inf)
-    upper: _BoundT[_RealT] = Bound[_RealT](inf)
-
-    def __init__(self, iterable: Iterable[_RealT] = ..., /, *,
-                 lower: _BoundT = -inf, upper: _BoundT[_RealT] = inf):
-        self.lower = lower
-        self.upper = upper
-        super().__init__(iterable)
-
-    def __repr__(self) -> str:
-        r = super().__repr__()
-        r = r.replace(')', f', lower={self.lower}, upper={self.upper})', 1)
-        return r
-
-    def __and__(self, other: object) -> Domain:
-        cls = type(self)
-        if isinstance(other, Domain) and not self:
-            return other
-        if isinstance(other, Interval):
-            return cls(self, lower=self._lower | other._lower, upper=self._upper | other._upper)
-        if isinstance(other, BoundedSet):
-            return cls(frozenset.intersection(self, other),
-                       lower=self._lower | other._lower, upper=self._upper | other._upper)
-        if isinstance(other, Iterable):
-            return cls(frozenset.intersection(self, other), lower=self._lower, upper=self._upper)
-        return NotImplemented
-
-    def min(self) -> _RealT:
-        # Can't use __contains__ here because that uses min in comparison
-        return min((item for item in self if self.lower <= item <= self.upper), default=nan)
-
-    def max(self) -> _RealT:
-        # Can't use __contains__ here because that uses max in comparison
-        return max((item for item in self if self.lower <= item <= self.upper), default=nan)
-
-    def next_closest(self, value: _RealT) -> _RealT:
-        return next_closest(self, value)
-
-    def next_smallest(self, value: _RealT) -> _RealT:
-        return next_smallest(self, value)
-
-    def next_largest(self, value: _RealT) -> _RealT:
-        return next_largest(self, value)
-
-
 class interdependent_daq_property(property):  # noqa
     """A property that modifies the getter and automatically generates
     the setter such that compatibility with other properties and
     constraints is checked at get-/set-time and values are coerced into
     the annotated return type."""
     def __init__(self, fget: Callable[[Any], Any] | None = ...):
         def _id(x: _T) -> _T:
@@ -445,29 +241,14 @@
             Traceback (most recent call last):
                 ...
             python_spectrometer.daq.settings.ResolutionError:
             Settings are inconsistent or not compatible with constraints.
             Parsed so far: {'nperseg': 500, 'n_pts': 400, 'fs': 231.5,
             'df': 3.2}
 
-            Test if there are no exceptions or infinite recursions for a consistent
-            set of parameters (only test up to 4 keyword parameters since the
-            product scales exponentially...):
-
-            >>> import qutil.itertools
-            >>> s = DAQSettings().to_consistent_dict()
-            >>> for kv in qutil.itertools.product(s.items(), repeat=4):
-            ...     t = DAQSettings(**dict(kv))
-            ...     d = t.to_consistent_dict()
-            ...     # Make sure this is reproducible
-            ...     _ = DAQSettings(d).to_consistent_dict()
-            ...     for k in set(s).difference(set(t)):
-            ...         # use setters for remaining parameters
-            ...         setattr(t, k, s[k])
-
             """
         )
     )
 
     # Rounding precision for comparing floating point values
     PRECISION: int = 10
 
@@ -481,55 +262,55 @@
     DEFAULT_N_AVG: int = 1
     # The default mapping to obtain noverlap from nperseg given as the
     # two-tuple (a, b) that fulfills nperseg = noverlap // a + b
     DEFAULT_NOVERLAP_MAPPING: Tuple[int, int] = (2, 0)
 
     # Override these to constrain parameters to certain sets allowed by hardware. An empty set
     # means no restrictions.
-    ALLOWED_FS: BoundedSet[float] | Interval[float] = BoundedSet()
-    ALLOWED_DF: BoundedSet[float] | Interval[float] = BoundedSet()
-    ALLOWED_F_MAX: BoundedSet[float] | Interval[float] = BoundedSet()
-    ALLOWED_F_MIN: BoundedSet[float] | Interval[float] = BoundedSet()
-    ALLOWED_NOVERLAP: BoundedSet[int] | Interval[int] = BoundedSet()
-    ALLOWED_N_PTS: BoundedSet[int] | Interval[int] = BoundedSet()
-    ALLOWED_N_SEG: BoundedSet[int] | Interval[int] = BoundedSet()
-    ALLOWED_N_AVG: BoundedSet[int] | Interval[int] = BoundedSet()
+    ALLOWED_FS: Domain[float] = BoundedSet(precision=PRECISION)
+    ALLOWED_DF: Domain[float] = BoundedSet(precision=PRECISION)
+    ALLOWED_F_MAX: Domain[float] = BoundedSet(precision=PRECISION)
+    ALLOWED_F_MIN: Domain[float] = BoundedSet(precision=PRECISION)
+    ALLOWED_NOVERLAP: Domain[int] = BoundedSet(precision=PRECISION)
+    ALLOWED_N_PTS: Domain[int] = BoundedSet(precision=PRECISION)
+    ALLOWED_N_SEG: Domain[int] = BoundedSet(precision=PRECISION)
+    ALLOWED_N_AVG: Domain[int] = BoundedSet(precision=PRECISION)
 
     @property
-    def ALLOWED_NPERSEG(self) -> BoundedSet[int] | Interval[int]:
+    def ALLOWED_NPERSEG(self) -> Domain[int]:
         return self.ALLOWED_N_PTS
 
     def _lower_bound_fs(self) -> float:
         return self._domain_f_max.min() * 2
 
     def _upper_bound_fs(self) -> float:
         return inf
 
     def _lower_bound_df(self) -> float:
-        return 0.
+        return finfo(float).eps
 
     def _upper_bound_df(self) -> float:
         return self._domain_f_min.max()
 
     def _lower_bound_f_max(self) -> float:
-        return self.get('f_min', self._infer_f_min()) or 0
+        return self.get('f_min', self._infer_f_min()) or finfo(float).eps
 
     def _upper_bound_f_max(self) -> float:
         fs = self.get('fs', self._infer_fs())
         return fs / 2 if fs is not None else inf
 
     def _lower_bound_f_min(self) -> float:
         df = self.get('df', self._infer_df())
-        return df if df is not None else 0
+        return df if df is not None else finfo(float).eps
 
     def _upper_bound_f_min(self) -> float:
         return self.get('f_max', self._infer_f_max()) or inf
 
     def _lower_bound_nperseg(self) -> int:
-        return floor(2 * (self.get('noverlap', self._infer_noverlap()) or 0.5))
+        return self.get('noverlap', 0) + 1
 
     def _upper_bound_nperseg(self) -> int | float:
         return self.get('n_pts', self._domain_n_pts.max())
 
     def _lower_bound_noverlap(self) -> int | float:
         ub_nperseg = self._domain_nperseg.max()
         nperseg = self.get('nperseg', self._infer_nperseg()) or ub_nperseg
@@ -537,15 +318,15 @@
         if 'n_seg' in self and self['n_seg'] > 2:
             return max(bound, nperseg - (ub_nperseg - nperseg) / (self['n_seg'] - 2))
         return bound
 
     def _upper_bound_noverlap(self) -> int | float:
         ub_nperseg = self._domain_nperseg.max()
         nperseg = self.get('nperseg', self._infer_nperseg()) or ub_nperseg
-        bound = nperseg // 2
+        bound = nperseg - 1
         if not isinf(ub_nperseg) and 'n_seg' in self:
             return min(bound, nperseg - (ub_nperseg - nperseg) // self['n_seg'])
         return bound
 
     def _lower_bound_n_pts(self) -> int:
         a, b = self.DEFAULT_NOVERLAP_MAPPING
         n_seg = self.get('n_seg', self._infer_n_seg()) or 1
@@ -568,54 +349,63 @@
     def _upper_bound_n_avg(self) -> int | float:
         return inf
 
     # The _domain_* properties cannot be cached because in principle both ALLOWED_* and Interval
     # can be dynamic.
     @property
     def _domain_fs(self) -> Domain[float]:
-        return self.ALLOWED_FS & ContinuousInterval(self._lower_bound_fs, self._upper_bound_fs)
+        return self.ALLOWED_FS & ContinuousInterval(self._lower_bound_fs, self._upper_bound_fs,
+                                                    self.PRECISION)
 
     @property
     def _domain_df(self) -> Domain[float]:
-        return self.ALLOWED_DF & ContinuousInterval(self._lower_bound_df, self._upper_bound_df)
+        return self.ALLOWED_DF & ContinuousInterval(self._lower_bound_df, self._upper_bound_df,
+                                                    self.PRECISION)
 
     @property
     def _domain_f_max(self) -> Domain[float]:
         return self.ALLOWED_F_MAX & ContinuousInterval(self._lower_bound_f_max,
-                                                       self._upper_bound_f_max)
+                                                       self._upper_bound_f_max,
+                                                       self.PRECISION)
 
     @property
     def _domain_f_min(self) -> Domain[float]:
         return self.ALLOWED_F_MIN & ContinuousInterval(self._lower_bound_f_min,
-                                                       self._upper_bound_f_min)
+                                                       self._upper_bound_f_min,
+                                                       self.PRECISION)
 
     @property
     def _domain_nperseg(self) -> Domain[int]:
         return self.ALLOWED_NPERSEG & DiscreteInterval(self._lower_bound_nperseg,
-                                                       self._upper_bound_nperseg)
+                                                       self._upper_bound_nperseg,
+                                                       self.PRECISION)
 
     @property
     def _domain_noverlap(self) -> Domain[int]:
         return self.ALLOWED_NOVERLAP & DiscreteInterval(self._lower_bound_noverlap,
-                                                        self._upper_bound_noverlap)
+                                                        self._upper_bound_noverlap,
+                                                        self.PRECISION)
 
     @property
     def _domain_n_pts(self) -> Domain[int]:
         return self.ALLOWED_N_PTS & DiscreteInterval(self._lower_bound_n_pts,
-                                                     self._upper_bound_n_pts)
+                                                     self._upper_bound_n_pts,
+                                                     self.PRECISION)
 
     @property
     def _domain_n_seg(self) -> Domain[int]:
         return self.ALLOWED_N_SEG & DiscreteInterval(self._lower_bound_n_seg,
-                                                     self._upper_bound_n_seg)
+                                                     self._upper_bound_n_seg,
+                                                     self.PRECISION)
 
     @property
     def _domain_n_avg(self) -> Domain[int]:
         return self.ALLOWED_N_AVG & DiscreteInterval(self._lower_bound_n_avg,
-                                                     self._upper_bound_n_avg)
+                                                     self._upper_bound_n_avg,
+                                                     self.PRECISION)
 
     @_validate_domain
     def _validate_fs(self, fs):
         if (inferred := self._infer_fs()) is not None and not self._isclose(inferred, fs):
             raise ValueError(f'fs not compatible with df and nperseg. actual = {fs}, inferred = '
                              f'{inferred}')
 
@@ -661,27 +451,25 @@
             return None
 
         fs_prev = fs
         if not isinf(df := self.get('df', self.get('f_min', inf))):
             # Constraints on nperseg constrain fs
             fs = df * self._domain_nperseg.next_largest(fs / df)
         if not self._isclose(fs, fs_prev):
-            # Chicken-egg problem here with nperseg and df, so cannot user setter
+            # Chicken-egg problem here with nperseg and df, so cannot use setter
             self['nperseg'] = self._domain_nperseg.next_largest(fs_prev / df)
             self._make_compatible_df(fs_prev / self['nperseg'])
-            fs = self['df'] * self._domain_nperseg.next_largest(fs_prev / self['df'])
-            return self._to_allowed_fs(fs)
+            return self._to_allowed_fs(fs_prev)
         if 'nperseg' in self:
             # Constraints on df constrain fs
             fs = self._domain_df.next_smallest(fs / self['nperseg']) * self['nperseg']
         if not self._isclose(fs, fs_prev):
             self['df'] = self._domain_df.next_closest(fs_prev / self['nperseg'])
             self._make_compatible_nperseg(ceil(fs_prev / self['df']))
-            fs = self._domain_df.next_smallest(fs_prev / self['nperseg']) * self['nperseg']
-            return self._to_allowed_fs(fs)
+            return self._to_allowed_fs(fs_prev)
         # Constraints on fs itself
         if not isinf(df) and not (fs / df) % 1:
             # fs might be due to ceil-ing when inferring nperseg. Use next_closest
             fs = self._domain_fs.next_closest(fs)
         else:
             fs = self._domain_fs.next_largest(fs)
         if not self._isclose(fs, fs_prev):
@@ -695,24 +483,23 @@
 
         df_prev = df
         if 'nperseg' in self:
             # Constraints on fs constrain df
             df = self._domain_fs.next_largest(df * self['nperseg']) / self['nperseg']
         if not self._isclose(df, df_prev):
             self['fs'] = self._domain_fs.next_closest(df_prev * self['nperseg'])
-            self._make_compatible_nperseg(ceil(self['fs'] / df_prev))
-            df = self._domain_fs.next_largest(df_prev * self['nperseg']) / self['nperseg']
+            # Use df instead of df_prev here because we preferentially adjust df over fs or nperseg
+            self._make_compatible_nperseg(ceil(self['fs'] / df))
             return self._to_allowed_df(df)
         if not isinf(fs := self.get('fs', self.get('f_max', inf) * 2)):
             # Constraints on nperseg constrain df
             df = fs / self._domain_nperseg.next_largest(fs / df)
         if not self._isclose(df, df_prev):
             self['nperseg'] = self._domain_nperseg.next_largest(fs / df_prev)
-            self._make_compatible_fs(df_prev * self['nperseg'])
-            df = self['fs'] / self._domain_nperseg.next_largest(self['fs'] / df_prev)
+            self._make_compatible_fs(df * self['nperseg'])
             return self._to_allowed_df(df)
         # Constraints on df itself
         df = self._domain_df.next_smallest(df)
         if not self._isclose(df, df_prev):
             self._make_compatible_df(df)
 
         return df
@@ -731,26 +518,24 @@
         nperseg_prev = nperseg
         fs = self.get('fs', self.get('f_max', inf) * 2)
         df = self.get('df', self.get('f_min', inf))
         if not isinf(df):
             # Constraints on fs constrain nperseg through df/f_min
             nperseg = ceil(self._domain_fs.next_largest(df * nperseg) / df)
         if nperseg != nperseg_prev:
-            self['fs'] = self._domain_fs.next_closest(fs if not isinf(fs) else df * nperseg_prev)
+            self['fs'] = self._domain_fs.next_largest(fs if not isinf(fs) else df * nperseg_prev)
             self._make_compatible_df(self['fs'] / nperseg_prev)
-            nperseg = ceil(self._domain_fs.next_largest(df * nperseg_prev) / df)
-            return self._to_allowed_nperseg(nperseg)
+            return self._to_allowed_nperseg(nperseg_prev)
         if not isinf(fs):
             # Constraints on df constrain nperseg through fs/f_max
             nperseg = ceil(fs / self._domain_df.next_smallest(fs / nperseg))
         if nperseg != nperseg_prev:
             self['df'] = self._domain_df.next_closest(df if not isinf(df) else fs * nperseg_prev)
             self._make_compatible_fs(self['df'] * nperseg_prev)
-            nperseg = ceil(self['fs'] / self._domain_df.next_smallest(self['fs'] / nperseg_prev))
-            return self._to_allowed_nperseg(nperseg)
+            return self._to_allowed_nperseg(nperseg_prev)
         # Constraints on nperseg itself
         nperseg = self._domain_nperseg.next_largest(nperseg)
         if nperseg != nperseg_prev:
             self._make_compatible_nperseg(nperseg)
 
         return nperseg
```

## python_spectrometer/daq/simulator.py

```diff
@@ -1,17 +1,16 @@
 """Provides a simulation backend for data acquisition."""
 from __future__ import annotations
 
 import dataclasses
 from typing import Callable, Iterator
 
 import numpy as np
-from qutil.functools import partial
-
 from python_spectrometer.daq.core import DAQ
+from qutil.functools import partial
 
 try:
     from numpy.typing import NDArray
 except ImportError:
     from numpy import ndarray as NDArray
 
 try:
```

## python_spectrometer/daq/swabian_instruments.py

```diff
@@ -1,17 +1,16 @@
 """Spectrometer driver for time tags using Swabian Instruments."""
 from __future__ import annotations
 
 import dataclasses
 import warnings
 from typing import Any, Dict, Iterable, Iterator, Sequence
 
-from qutil.misc import import_or_mock
-
 from python_spectrometer.daq.core import DAQ
+from qutil.misc import import_or_mock
 
 try:
     from numpy.typing import NDArray
 except ImportError:
     from numpy import ndarray as NDArray
 
 locals().update(import_or_mock('TimeTagger', None, 'tt'))
```

## python_spectrometer/daq/zurich_instruments.py

```diff
@@ -6,15 +6,15 @@
 Examples
 --------
 Start up a session and connect the device::
 
     from zhinst import toolkit
 
     session = toolkit.Session('localhost')
-    device = session.connect_device('dev5247')
+    device = session.connect_device('dev5247', interface='1gbe')
 
 Set up :class:`~python_spectrometer.core.Spectrometer`
 instances once using the DAQ module and once using the Scope module::
 
     from tempfile import mkdtemp
     from python_spectrometer import Spectrometer
     from python_spectrometer.daq import zurich_instruments
@@ -45,21 +45,20 @@
 import time
 import warnings
 from abc import ABC
 from typing import Any, Dict, Iterator, Mapping, Optional, Type, Union
 
 import numpy as np
 from packaging import version
+from python_spectrometer.daq.core import DAQ
+from python_spectrometer.daq.settings import DAQSettings
+from qutil.domains import BoundedSet, DiscreteInterval
 from scipy.special import gamma
 from zhinst import toolkit
 
-from python_spectrometer.daq.core import DAQ
-from python_spectrometer.daq.settings import (BoundedSet, DAQSettings,
-                                              DiscreteInterval)
-
 try:
     from numpy.typing import NDArray
 except ImportError:
     from numpy import ndarray as NDArray
 
 if version.parse(toolkit.__version__) < version.parse('0.5.0'):
     raise ImportError('This DAQ requires zhinst-toolkit >= 0.5.0. '
@@ -138,15 +137,16 @@
         ]
 
     @property
     def DAQSettings(self) -> Type[DAQSettings]:
         class MFLIDAQSettings(DAQSettings):
             CLOCKBASE = self.device.clockbase()
             # TODO: always the same for each instrument?
-            ALLOWED_FS = BoundedSet(CLOCKBASE / 70 / 2 ** np.arange(24))
+            ALLOWED_FS = BoundedSet(CLOCKBASE / 70 / 2 ** np.arange(24),
+                                    precision=DAQSettings.PRECISION)
             DEFAULT_FS = CLOCKBASE / 70 / 2**6
 
         return MFLIDAQSettings
 
     def setup(self, bandwidth: Union[str, float] = 'auto', filter_order: Optional[int] = None,
               freq: float = 0, **settings: Mapping) -> Dict[str, Any]:
         r"""Sets up the daq module to acquire time series data.
@@ -372,16 +372,17 @@
                 ), f"Scope record {index}/{num_records} size does not match totalsamples."
 
     @property
     def DAQSettings(self) -> Type[DAQSettings]:
         class MFLIScopeSettings(DAQSettings):
             CLOCKBASE = self.device.clockbase()
             # TODO: always the same for each instrument?
-            ALLOWED_N_PTS = DiscreteInterval(2 ** 12, 2 ** 14)
-            ALLOWED_FS = BoundedSet(CLOCKBASE / 2 ** np.arange(17))
+            ALLOWED_N_PTS = DiscreteInterval(2 ** 12, 2 ** 14, precision=DAQSettings.PRECISION)
+            ALLOWED_FS = BoundedSet(CLOCKBASE / 2 ** np.arange(17),
+                                    precision=DAQSettings.PRECISION)
             DEFAULT_FS = CLOCKBASE / 2 ** 8
 
         return MFLIScopeSettings
 
     def setup(self, **settings: Mapping) -> Dict[str, Any]:
         r"""Sets up the scope module to acquire time series data.
```

## Comparing `python_spectrometer-2023.6.1.dist-info/METADATA` & `python_spectrometer-2023.7.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-spectrometer
-Version: 2023.6.1
+Version: 2023.7.1
 Summary: Package to acquire time traces and compute and plot their power spectra
 Project-URL: Homepage, https://git.rwth-aachen.de/qutech/python-spectrometer
 Author: Quantum Technology Group, RWTH Aachen University
 License-Expression: GPL-3.0
 License-File: LICENSE
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -17,15 +17,15 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Requires-Dist: dill
 Requires-Dist: lazy-loader
 Requires-Dist: matplotlib>=3.7
 Requires-Dist: numpy
 Requires-Dist: packaging
-Requires-Dist: qutech-util>=2023.6.1
+Requires-Dist: qutech-util>=2023.7.1
 Requires-Dist: scipy
 Provides-Extra: complete
 Requires-Dist: python-spectrometer[doc]; extra == 'complete'
 Requires-Dist: python-spectrometer[qcodes]; extra == 'complete'
 Requires-Dist: python-spectrometer[simulator]; extra == 'complete'
 Requires-Dist: python-spectrometer[tests]; extra == 'complete'
 Requires-Dist: python-spectrometer[zurich-instruments]; extra == 'complete'
```

## Comparing `python_spectrometer-2023.6.1.dist-info/licenses/LICENSE` & `python_spectrometer-2023.7.1.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

