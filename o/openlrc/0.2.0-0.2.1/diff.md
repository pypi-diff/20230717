# Comparing `tmp/openlrc-0.2.0.tar.gz` & `tmp/openlrc-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlrc-0.2.0.tar", max compression
+gzip compressed data, was "openlrc-0.2.1.tar", max compression
```

## Comparing `openlrc-0.2.0.tar` & `openlrc-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1083 2023-05-10 10:20:06.659160 openlrc-0.2.0/LICENSE
--rw-r--r--   0        0        0      106 2023-06-09 13:01:57.605311 openlrc-0.2.0/openlrc/__init__.py
--rw-r--r--   0        0        0     6642 2023-07-01 13:36:53.572387 openlrc-0.2.0/openlrc/chatbot.py
--rw-r--r--   0        0        0     2761 2023-07-12 18:58:48.074505 openlrc-0.2.0/openlrc/context.py
--rw-r--r--   0        0        0     1424 2023-07-12 19:00:10.406166 openlrc-0.2.0/openlrc/defaults.py
--rw-r--r--   0        0        0      966 2023-07-05 20:31:15.832362 openlrc-0.2.0/openlrc/exceptions.py
--rw-r--r--   0        0        0      597 2023-06-15 20:08:22.292558 openlrc-0.2.0/openlrc/logger.py
--rw-r--r--   0        0        0    12901 2023-07-12 18:58:48.075680 openlrc-0.2.0/openlrc/openlrc.py
--rw-r--r--   0        0        0     5165 2023-07-12 18:58:48.076238 openlrc-0.2.0/openlrc/opt.py
--rw-r--r--   0        0        0     7702 2023-07-12 18:58:48.076743 openlrc-0.2.0/openlrc/prompter.py
--rw-r--r--   0        0        0     6372 2023-06-29 05:51:12.383562 openlrc-0.2.0/openlrc/subtitle.py
--rw-r--r--   0        0        0     6729 2023-07-12 18:58:48.076743 openlrc-0.2.0/openlrc/transcribe.py
--rw-r--r--   0        0        0     5735 2023-07-12 18:58:48.077748 openlrc-0.2.0/openlrc/translate.py
--rw-r--r--   0        0        0     6552 2023-07-06 13:45:34.300323 openlrc-0.2.0/openlrc/utils.py
--rw-r--r--   0        0        0     1654 2023-07-12 19:02:49.168288 openlrc-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5572 2023-07-12 19:02:30.593756 openlrc-0.2.0/README.md
--rw-r--r--   0        0        0     7019 1970-01-01 00:00:00.000000 openlrc-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-05-10 10:20:06.659160 openlrc-0.2.1/LICENSE
+-rw-r--r--   0        0        0      106 2023-06-09 13:01:57.605311 openlrc-0.2.1/openlrc/__init__.py
+-rw-r--r--   0        0        0     6643 2023-07-14 13:02:05.768264 openlrc-0.2.1/openlrc/chatbot.py
+-rw-r--r--   0        0        0     2761 2023-07-12 18:58:48.074505 openlrc-0.2.1/openlrc/context.py
+-rw-r--r--   0        0        0     2164 2023-07-13 10:41:08.371996 openlrc-0.2.1/openlrc/defaults.py
+-rw-r--r--   0        0        0      966 2023-07-05 20:31:15.832362 openlrc-0.2.1/openlrc/exceptions.py
+-rw-r--r--   0        0        0      597 2023-06-15 20:08:22.292558 openlrc-0.2.1/openlrc/logger.py
+-rw-r--r--   0        0        0    13617 2023-07-17 08:20:23.713740 openlrc-0.2.1/openlrc/openlrc.py
+-rw-r--r--   0        0        0     5147 2023-07-16 07:28:45.850524 openlrc-0.2.1/openlrc/opt.py
+-rw-r--r--   0        0        0     3920 2023-07-17 08:05:53.681548 openlrc-0.2.1/openlrc/preprocess.py
+-rw-r--r--   0        0        0     7702 2023-07-12 18:58:48.076743 openlrc-0.2.1/openlrc/prompter.py
+-rw-r--r--   0        0        0     6736 2023-07-16 07:46:51.494326 openlrc-0.2.1/openlrc/subtitle.py
+-rw-r--r--   0        0        0     6614 2023-07-13 15:11:24.766191 openlrc-0.2.1/openlrc/transcribe.py
+-rw-r--r--   0        0        0     5867 2023-07-17 07:58:32.297546 openlrc-0.2.1/openlrc/translate.py
+-rw-r--r--   0        0        0     7332 2023-07-14 03:29:48.721545 openlrc-0.2.1/openlrc/utils.py
+-rw-r--r--   0        0        0     1733 2023-07-17 08:24:48.610852 openlrc-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5712 2023-07-17 08:30:54.378527 openlrc-0.2.1/README.md
+-rw-r--r--   0        0        0     7296 1970-01-01 00:00:00.000000 openlrc-0.2.1/PKG-INFO
```

### Comparing `openlrc-0.2.0/LICENSE` & `openlrc-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openlrc-0.2.0/openlrc/chatbot.py` & `openlrc-0.2.1/openlrc/chatbot.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
                 )
                 self.update_fee(response)
                 if response.choices[0].finish_reason == 'length':
                     raise ChatBotException(
                         f'Failed to get completion. Exceed max token length. '
                         f'Prompt tokens: {response.usage["prompt_tokens"]}, '
                         f'Completion tokens: {response.usage["completion_tokens"]}, '
-                        f'Total tokens: {response.usage["total_tokens"]}'
+                        f'Total tokens: {response.usage["total_tokens"]} '
                         f'Reduce chunk_size may help.'
                     )
                 if not output_checker(messages, response.choices[0].message.content):
                     logger.warning(f'Invalid response format. Retry num: {i + 1}.')
                     continue
 
                 break
```

### Comparing `openlrc-0.2.0/openlrc/context.py` & `openlrc-0.2.1/openlrc/context.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.2.0/openlrc/exceptions.py` & `openlrc-0.2.1/openlrc/exceptions.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.2.0/openlrc/logger.py` & `openlrc-0.2.1/openlrc/logger.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.2.0/openlrc/openlrc.py` & `openlrc-0.2.1/openlrc/openlrc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 #  Copyright (C) 2023. Hao Zheng
 #  All rights reserved.
 
 import concurrent.futures
 import json
+import shutil
 from pathlib import Path
 from pprint import pformat
 from queue import Queue
 from threading import Lock
 from typing import List
 
 from faster_whisper.transcribe import Segment
 
 from openlrc.context import Context
 from openlrc.defaults import default_asr_options, default_vad_options
 from openlrc.logger import logger
 from openlrc.opt import SubtitleOptimizer
+from openlrc.preprocess import Preprocessor
 from openlrc.subtitle import Subtitle
 from openlrc.transcribe import Transcriber
 from openlrc.translate import GPTTranslator
 from openlrc.utils import Timer, extend_filename, get_audio_duration, format_timestamp, extract_audio, \
     get_file_type
 
 
@@ -29,16 +31,16 @@
                     from the Hugging Face Hub.
                     Default: ``large-v2``
     :param compute_type: The type of computation to use. Can be ``int8``, ``int8_float16``, ``int16``,
                     ``float16`` or ``float32``.
                     Default: ``float16``
     :param fee_limit: The maximum fee you are willing to pay for one translation call. Default: ``0.1``
     :param consumer_thread: To prevent exceeding the RPM and TPM limits set by OpenAI, the default is TPM/MAX_TOKEN.
-    :param asr_options: parameters for whisper model.
-    :param vad_options: parameters for VAD model.
+    :param asr_options: Parameters for whisper model.
+    :param vad_options: Parameters for VAD model.
     """
 
     def __init__(self, model_name='large-v2', compute_type='float16', fee_limit=0.1, consumer_thread=11,
                  asr_options=None, vad_options=None):
         self.fee_limit = fee_limit
         self.api_fee = 0  # Can be updated in different thread, operation should be thread-safe
         self.from_video = set()
@@ -116,27 +118,30 @@
             transcribed_opt_sub = self.post_process(transcribed_sub, update_name=True)
             audio_name = transcribed_path.stem.replace('_transcribed', '')
 
             # xxx_transcribed_optimized_translated.json
             translated_path = extend_filename(transcribed_opt_sub.filename, '_translated')
 
             final_subtitle = transcribed_opt_sub
-            if not skip_trans:
+            final_subtitle.filename = Path(translated_path.parent / f'{audio_name}.json')
+            if not skip_trans and not final_subtitle.exists():
                 with Timer('Translation process'):
                     try:
                         final_subtitle = self._translate(audio_name, prompter, target_lang, transcribed_opt_sub,
                                                          translated_path)
                     except Exception as e:
                         self.exception = e
 
-            final_subtitle.filename = Path(translated_path.parent / f'{audio_name}.json')
-
-            final_subtitle.to_lrc()
+            # Copy preprocessed/xxx_preprocessed.lrc or preprocessed/xxx_preprocessed.srt to xxx.lrc or xxx.srt
+            lrc_path = final_subtitle.to_lrc()
+            shutil.copy(lrc_path, lrc_path.parents[1] / lrc_path.name.replace('_preprocessed.lrc', '.lrc'))
             if audio_name in self.from_video:
-                final_subtitle.to_srt()
+                srt_path = final_subtitle.to_srt()
+                shutil.copy(srt_path, srt_path.parents[1] / srt_path.name.replace('_preprocessed.srt', '.srt'))
+
             logger.info(f'Translation fee til now: {self.api_fee:.4f} USD')
 
     def _translate(self, audio_name, prompter, target_lang, transcribed_opt_sub, translated_path):
         json_filename = Path(translated_path.parent / (audio_name + '.json'))
         compare_path = Path(translated_path.parent, f'{audio_name}_compare.json')
         if not translated_path.exists():
             if not compare_path.exists():
@@ -168,58 +173,61 @@
 
             # xxx_transcribed_optimized_translated.json
             transcribed_opt_sub.save(translated_path, update_name=True)
         else:
             logger.info(f'Found translated json file: {translated_path}')
         translated_sub = Subtitle.from_json(translated_path)
 
-        final_subtitle = self.post_process(translated_sub, output_name=json_filename, t2m=target_lang == 'zh-cn',
-                                           update_name=True)  # xxx.json
+        final_subtitle = self.post_process(translated_sub, output_name=json_filename, update_name=True)  # xxx.json
+
         return final_subtitle
 
     def run(self, paths, src_lang=None, target_lang='zh-cn', prompter='base_trans', context_path=None,
-            skip_trans=False):
+            skip_trans=False, noise_suppress=False):
         """
         Split the translation into 2 phases: transcription and translation. They're running in parallel.
         Firstly, transcribe the audios one-by-one. At the same time, translation threads are created and waiting for
         the transcription results. After all the transcriptions are done, the translation threads will start to
         translate the transcribed texts.
 
         :param paths: Audio/Video paths, can be a list or a single path.
-        :param src_lang: Language of the audio, default to auto detect.
+        :param src_lang: Language of the audio, default to auto-detect.
         :param target_lang: Target language, default to Mandarin Chinese.
         :param prompter: Currently, only `base_trans` is supported.
         :param context_path: path to context config file. (Default to use `context.yaml` in the first audio's directory)
-        :param skip_trans: Skip the translation process if True.
+        :param skip_trans: Whether to skip the translation process. (Default to False)
+        :param noise_suppress: Whether to suppress the noise in the audio. (Default to False)
         """
         if not paths:
             logger.warning('No audio/video file given. Skip LRCer.run()')
             return
 
         if isinstance(paths, str) or isinstance(paths, Path):
             paths = [paths]
 
-        audio_paths = self.pre_process(paths)
-
-        logger.info(f'Working on {len(audio_paths)} audio files: {pformat(audio_paths)}')
+        paths = list(map(Path, paths))
 
         if context_path:
             context_path = Path(context_path)
             self.context.load_config(context_path)
             logger.info(f'Found context config: {context_path}')
             logger.debug(f'Context: {self.context}')
         else:
             # Try to find the default `context.yaml` in the first audio's directory
             try:
-                context_path = audio_paths[0].parent / 'context.yaml'
+                context_path = paths[0].parent / 'context.yaml'
                 self.context.load_config(context_path)
                 logger.info(f'Found context config file: {context_path}')
             except FileNotFoundError:
                 logger.info(f'Default context config not found: {self.context}, using default context.')
 
+        audio_paths = self.pre_process(paths, noise_suppress=noise_suppress)
+
+        logger.info(f'Working on {len(audio_paths)} audio files: {pformat(audio_paths)}')
+
         transcription_queue = Queue()
 
         with Timer('Transcription (Producer) and Translation (Consumer) process'):
             consumer = concurrent.futures.ThreadPoolExecutor(thread_name_prefix='Consumer') \
                 .submit(self.transcription_consumer, transcription_queue, target_lang, prompter, skip_trans)
             producer = concurrent.futures.ThreadPoolExecutor(thread_name_prefix='Producer') \
                 .submit(self.transcription_producer, transcription_queue, audio_paths, src_lang)
@@ -251,34 +259,38 @@
         with open(name, 'w', encoding='utf-8') as f:
             json.dump(result, f, ensure_ascii=False, indent=4)
 
         logger.info(f'File saved to {name}')
 
         return result
 
-    def pre_process(self, paths):
+    def pre_process(self, paths, noise_suppress=False):
         paths = [Path(path) for path in paths]
 
         # Check if path is audio or video
         for i, path in enumerate(paths):
             if not path.exists() or not path.is_file():
                 raise FileNotFoundError(f'File not found: {path}')
 
             paths[i] = extract_audio(path)
 
             if get_file_type(path) == 'video':
                 self.from_video.add(path.name)
 
+        # Audio-based process
+        preprocessor = Preprocessor(paths)
+        paths = preprocessor.run(noise_suppress)
+
         return paths
 
     @staticmethod
-    def post_process(transcribed_sub: Path, output_name: Path = None, remove_files: List[Path] = None, t2m=False,
+    def post_process(transcribed_sub: Path, output_name: Path = None, remove_files: List[Path] = None,
                      update_name=False):
         optimizer = SubtitleOptimizer(transcribed_sub)
-        optimizer.perform_all(t2m=t2m)
+        optimizer.perform_all()
         optimizer.save(output_name, update_name=update_name)
 
         # Remove intermediate files
         if remove_files:
             _ = [file.unlink() for file in remove_files if file.is_file()]
 
         return optimizer.subtitle
```

### Comparing `openlrc-0.2.0/openlrc/opt.py` & `openlrc-0.2.1/openlrc/opt.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,23 +126,23 @@
             new_elements[i].text = element.text.replace('<unk>', '')
 
         self.subtitle.segments = new_elements
 
     def remove_empty(self):
         self.subtitle.segments = [element for element in self.subtitle.segments if element.text]
 
-    def perform_all(self, t2m=False):
+    def perform_all(self):
         for _ in range(2):
             self.merge_same()
             self.merge_short()
             self.merge_repeat()
             self.cut_long()
             self.remove_unk()
             self.remove_empty()
 
-            if t2m or self.subtitle.lang.lower() == 'zh-cn':
+            if self.subtitle.lang.lower() == 'zh-cn':
                 self.traditional2mandarin()
 
     def save(self, output_name=None, update_name=False):
         optimized_name = extend_filename(self.filename, '_optimized') if not output_name else output_name
         self.subtitle.save(optimized_name, update_name=update_name)
         logger.info(f'Optimized json file saved to {optimized_name}')
```

### Comparing `openlrc-0.2.0/openlrc/prompter.py` & `openlrc-0.2.1/openlrc/prompter.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.2.0/openlrc/subtitle.py` & `openlrc-0.2.1/openlrc/subtitle.py`

 * *Files 17% similar despite different names*

```diff
@@ -89,47 +89,61 @@
             json.dump(results, f, ensure_ascii=False, indent=4)
 
         if update_name:
             self.filename = filename
 
         return filename
 
+    def exists(self):
+        """
+        Check if the .lrc/.srt/.json file exist.
+        :return:
+        """
+        lrc_path = self.filename.with_suffix('.lrc')
+        srt_path = self.filename.with_suffix('.srt')
+
+        return lrc_path.exists() or srt_path.exists() or self.filename.exists()
+
     def to_lrc(self):
         # If duration larger than 1 hour, use srt file instead
         if self.segments[-1].end >= 3600:
             logger.warning('Duration larger than 1 hour, use srt file instead')
             self.to_srt()
             return
 
-        lrc_name = self.filename.with_suffix('.lrc')
+        lrc_path = self.filename.with_suffix('.lrc')
         fmt = partial(format_timestamp, fmt='lrc')
-        with open(lrc_name, 'w', encoding='utf-8') as f:
+        with open(lrc_path, 'w', encoding='utf-8') as f:
             print(f'# LRC generated by https://github.com/zh-plus/Open-Lyrics, lang={self.lang}', file=f, flush=True)
             for i, segment in enumerate(self.segments):
                 print(
                     f'[{fmt(segment.start)}] {segment.text}',
                     file=f,
                     flush=True,
                 )
                 if i == len(self.segments) - 1 or segment.end != self.segments[i + 1].start:
                     print(f'[{fmt(segment.end)}]', file=f, flush=True)
 
-        logger.info(f'File saved to {lrc_name}')
+        logger.info(f'File saved to {lrc_path}')
+
+        return lrc_path
 
     def to_srt(self):
-        srt_name = self.filename.with_suffix('.srt')
+        srt_path = self.filename.with_suffix('.srt')
         fmt = partial(format_timestamp, fmt='srt')
-        with open(srt_name, 'w', encoding='utf-8') as f:
+        with open(srt_path, 'w', encoding='utf-8') as f:
             print(f'# LRC generated by https://github.com/zh-plus/Open-Lyrics, lang={self.lang}', file=f, flush=True)
             for i, segment in enumerate(self.segments, start=1):
                 print(f'{i}\n'
                       f'{fmt(segment.start)} --> {fmt(segment.end)}\n'
                       f'{segment.text}\n', file=f, flush=True)
 
-        logger.info(f'File saved to {srt_name}')
+        logger.info(f'File saved to {srt_path}')
+
+        return srt_path
 
     @classmethod
     def from_lrc(cls, filename):
         filename = Path(filename)
         with open(filename, encoding='utf-8') as f:
             lines = f.readlines()
```

### Comparing `openlrc-0.2.0/openlrc/transcribe.py` & `openlrc-0.2.1/openlrc/transcribe.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 #  Copyright (C) 2023. Hao Zheng
 #  All rights reserved.
 
 from pathlib import Path
 from typing import NamedTuple, Union, List
 
 import pysbd
-import spacy
 from faster_whisper.transcribe import WhisperModel, Segment
 from pysbd.languages import LANGUAGE_CODES
 from tqdm import tqdm
 
 from openlrc.defaults import default_asr_options, default_vad_options
-from openlrc.exceptions import DependencyException
 from openlrc.logger import logger
-from openlrc.utils import Timer, get_audio_duration, get_spacy_lib
+from openlrc.utils import Timer, get_audio_duration, spacy_load
 
 
 class TranscriptionInfo(NamedTuple):
     language: str
     duration: float
 
 
@@ -59,21 +57,15 @@
         return result, info
 
     def sentence_split(self, segments: List[Segment], lang):
         if lang not in LANGUAGE_CODES.keys():
             logger.warning(f'Language {lang} not supported. Skip sentence split.')
             return segments
 
-        lib_name = get_spacy_lib(lang)
-        try:
-            nlp = spacy.load(lib_name)
-        except (IOError, ImportError, OSError):
-            raise DependencyException(
-                f'Try `spacy download {lib_name}` to fix.'
-                f'Check https://spacy.io/usage for more instruction.')
+        nlp = spacy_load(lang)
 
         def seg_from_words(seg: Segment, seg_id, words, tokens):
             text = ''.join([word.word for word in words])
             return Segment(seg_id, seg.seek, words[0].start, words[-1].end, text, tokens,
                            seg.temperature, seg.avg_logprob, seg.compression_ratio, seg.no_speech_prob, words)
 
         def mid_split(seg_entry):
@@ -133,14 +125,19 @@
                         break
                     if split_words_len >= len(split.rstrip()):
                         break
 
                 if split_words_len >= len(split.rstrip()) + 2:
                     logger.warning(
                         f'Extracted split words len mismatch: {split_words_len} >= {len(split)} + 2')
+                if split_words_len == 0:
+                    logger.warning(
+                        f'Extracted zero split words: {split_words_len} == 0, for split: {split}, skip'
+                    )
+                    continue
 
                 word_start += len(split_words)
 
                 entry = seg_from_words(segment, id_cnt, split_words,
                                        segment.tokens[word_start: word_start + len(split_words)])
 
                 if len(split) < (50 if lang in self.non_word_boundary else 100):
```

### Comparing `openlrc-0.2.0/openlrc/translate.py` & `openlrc-0.2.1/openlrc/translate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #  Copyright (C) 2023. Hao Zheng
 #  All rights reserved.
 
 import json
 import os
 import re
 import uuid
+from typing import Union, List
 
 import requests
 
 from openlrc.chatbot import GPTBot
 from openlrc.logger import logger
 from openlrc.prompter import prompter_map, BaseTranslatePrompter
 
@@ -67,16 +68,19 @@
 
             return summary.strip(), scene.strip(), [t.strip() for t in translation]
 
         except Exception as e:
             logger.error(f'Failed to extract contents from response: {content}')
             raise e
 
-    def translate(self, texts, src_lang, target_lang, audio_type='Anime', title='', background='', description='',
-                  compare_path='test_intermediate.json'):
+    def translate(self, texts: Union[str, List[str]], src_lang, target_lang, audio_type='Anime', title='',
+                  background='', description='', compare_path='translate_intermediate.json'):
+        if not isinstance(texts, list):
+            texts = [texts]
+
         prompter: BaseTranslatePrompter = prompter_map[self.prompter](
             src_lang, target_lang, audio_type, title=title, background=background, description=description)
         translate_bot = GPTBot(fee_limit=self.fee_limit)
         translate_bot.update(temperature=0.7)
 
         chunks = self.make_chunks(texts, chunk_size=self.chunk_size)
         logger.info(f'Translating {title}: {len(chunks)} chunks, {len(texts)} lines in total.')
```

### Comparing `openlrc-0.2.0/openlrc/utils.py` & `openlrc-0.2.1/openlrc/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,19 +7,22 @@
 from pathlib import Path
 from typing import List, Dict, Any, Union
 
 import audioread
 import ffmpeg
 import filetype
 import jaconvV2
+import langcodes
+import spacy
 import tiktoken
 import torch
 import unicodedata
-from langcodes import Language
 from lingua import LanguageDetectorBuilder
+
+from openlrc.defaults import supported_languages_lingua
 from openlrc.logger import logger
 
 
 def extract_audio(path: Path) -> Path:
     """
     Extract audio from video.
     :return: Audio path
@@ -72,20 +75,20 @@
     del model
 
 
 def normalize(text):
     """
     Normalize strings using str.lower(), and unicodedata.normalize
     """
-    text = unicodedata.normalize('NFKC', text.lower())
-
     # unicodedata cant handel quotes as expected'’'
-    quotes_table = str.maketrans('“”‘’', '""\'\'')
+    quotes_table = str.maketrans('〈〉゛“”‘’', '<>"""\'\'')
     text = text.translate(quotes_table)
 
+    text = unicodedata.normalize('NFKC', text.lower())
+
     # unicodedata cant handel kana
     text = jaconvV2.z2h(text)
 
     # Special case
     special_table = str.maketrans('〇①②③④⑤⑥⑦⑧⑨', '0123456789')
     text = text.translate(special_table)
 
@@ -194,17 +197,17 @@
     elif fmt == 'srt':
         return f"{hours:02d}:{minutes:02d}:{seconds:02d},{milliseconds:03d}"
     else:
         raise ValueError(f"Unsupported timestamp format: {fmt}")
 
 
 def detect_lang(text):
-    detector = LanguageDetectorBuilder.from_all_languages().build()
+    detector = LanguageDetectorBuilder.from_languages(*supported_languages_lingua).build()
     name = detector.detect_language_of(' '.join(text)).name.lower()
-    lang_code = Language.find(name).language
+    lang_code = langcodes.Language.find(name).language
     return lang_code
 
 
 def get_spacy_lib(lang):
     special_case = {
         'core_web': ['zh', 'en'],
         'ent_wiki': ['xx']
@@ -212,7 +215,34 @@
 
     mid_str = 'core_news'
     for k, v in special_case.items():
         if lang in v:
             mid_str = k
 
     return f'{lang}_{mid_str}_sm'
+
+
+def spacy_load(lang) -> spacy.Language:
+    lib_name = get_spacy_lib(lang)
+    try:
+        nlp = spacy.load(lib_name)
+    except (IOError, ImportError, OSError):
+        logger.warning(f'Spacy model {lib_name} missed, downloading')
+        spacy.cli.download(lib_name)
+        nlp = spacy.load(lib_name)
+
+    return nlp
+
+
+def get_similarity(text1, text2):
+    lang1 = detect_lang(text1)
+    lang2 = detect_lang(text2)
+
+    if lang1 != lang2:
+        raise ValueError(f'language of {text1} ({lang1}) is not the same as {text2} ({lang2})')
+
+    nlp = spacy_load(lang1)
+
+    doc1 = nlp(text1)
+    doc2 = nlp(text2)
+
+    return doc1.similarity(doc2)
```

### Comparing `openlrc-0.2.0/pyproject.toml` & `openlrc-0.2.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [virtualenvs]
 create = true
 in-project = true
 
 [tool.poetry]
 name = "openlrc"
-version = "0.2.0"
+version = "0.2.1"
 description = "Transcribe (whisper) and translate (gpt) voice into LRC file."
 license = "MIT"
 authors = [
     "Hao Zheng <zhenghaosustc@gmail.com>"
 ]
 readme = "README.md"
 homepage = "https://github.com/zh-plus/Open-Lyrics"
@@ -48,14 +48,17 @@
 lingua-language-detector = "^1.3.2"
 pandas = "^2.0.2"
 filetype = "^1.2.0"
 jaconvV2 = "^0.4"
 spacy = "^3.5.4"
 pysbd = "^0.3.4"
 faster-whisper = "^0.6.0"
+soundfile = "^0.12.1"
+ffmpeg-normalize = "^1.27.5"
+deepfilternet = "^0.5.3"
 #torch = { version = "2.0.1", source = "torch" }
 #torchaudio = { version = "2.0.2", source = "torch" }
 #torchvision = { version = "0.15.2", source = "torch" }
 
 
 [[tool.poetry.source]]
 name = "PyPI"
```

### Comparing `openlrc-0.2.0/README.md` & `openlrc-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,17 @@
 # To skip translation process
 lrcer.run('./data/test.mp3', target_lang='en', skip_trans=True)
 
 # Change asr_options or vad_options, check openlrc.defaults for details
 vad_options = {"threshold": 0.1}
 lrcer = LRCer(vad_options=vad_options)
 lrcer.run('./data/test.mp3', target_lang='zh-cn')
+
+# Enhance the audio using noise suppression (consume more time).
+lrcer.run('./data/test.mp3', target_lang='zh-cn', noise_suppress=True)
 ```
 
 ### Context
 
 Utilize the available context to enhance the quality of your translation.
 Save them as `context.yaml` in the same directory as your audio file.
```

### Comparing `openlrc-0.2.0/PKG-INFO` & `openlrc-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlrc
-Version: 0.2.0
+Version: 0.2.1
 Summary: Transcribe (whisper) and translate (gpt) voice into LRC file.
 Home-page: https://github.com/zh-plus/Open-Lyrics
 License: MIT
 Keywords: openai-gpt3,whisper,voice transcribe,lrc
 Author: Hao Zheng
 Author-email: zhenghaosustc@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -15,25 +15,28 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: audioread (>=3.0.0,<4.0.0)
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
+Requires-Dist: deepfilternet (>=0.5.3,<0.6.0)
 Requires-Dist: faster-whisper (>=0.6.0,<0.7.0)
+Requires-Dist: ffmpeg-normalize (>=1.27.5,<2.0.0)
 Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
 Requires-Dist: filetype (>=1.2.0,<2.0.0)
 Requires-Dist: jaconvV2 (>=0.4,<0.5)
 Requires-Dist: langcodes (>=3.3.0,<4.0.0)
 Requires-Dist: language-data (>=1.1,<2.0)
 Requires-Dist: lingua-language-detector (>=1.3.2,<2.0.0)
 Requires-Dist: openai (>=0.27.6,<0.28.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: punctuators (>=0.0.5,<0.0.6)
 Requires-Dist: pysbd (>=0.3.4,<0.4.0)
+Requires-Dist: soundfile (>=0.12.1,<0.13.0)
 Requires-Dist: spacy (>=3.5.4,<4.0.0)
 Requires-Dist: tiktoken (>=0.3.1,<0.4.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: zhconv (>=1.4.3,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/zh-plus/Open-Lyrics/issues
 Description-Content-Type: text/markdown
 
@@ -107,14 +110,17 @@
 # To skip translation process
 lrcer.run('./data/test.mp3', target_lang='en', skip_trans=True)
 
 # Change asr_options or vad_options, check openlrc.defaults for details
 vad_options = {"threshold": 0.1}
 lrcer = LRCer(vad_options=vad_options)
 lrcer.run('./data/test.mp3', target_lang='zh-cn')
+
+# Enhance the audio using noise suppression (consume more time).
+lrcer.run('./data/test.mp3', target_lang='zh-cn', noise_suppress=True)
 ```
 
 ### Context
 
 Utilize the available context to enhance the quality of your translation.
 Save them as `context.yaml` in the same directory as your audio file.
```

