# Comparing `tmp/deep_utils-1.2.1.tar.gz` & `tmp/deep_utils-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep_utils-1.2.1.tar", last modified: Sat May 27 18:34:14 2023, max compression
+gzip compressed data, was "deep_utils-1.2.2.tar", last modified: Mon Jul 17 18:18:42 2023, max compression
```

## Comparing `deep_utils-1.2.1.tar` & `deep_utils-1.2.2.tar`

### file list

```diff
@@ -1,655 +1,655 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.277540 deep_utils-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-27 18:34:03.000000 deep_utils-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26630 2023-05-27 18:34:14.277540 deep_utils-1.2.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.233540 deep_utils-1.2.1/deep_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/audio/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/audio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/audio/asr/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/audio/asr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/audio/asr/wave2vec2/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/audio/asr/wave2vec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/audio/classification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/audio/classification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/audio/classification/wav2vec2/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/audio/classification/wav2vec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/audio/diarization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/audio/diarization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/audio/diarization/pyannote/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/audio/diarization/pyannote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/audio/utils_/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/audio/utils_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/audio/vad/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/audio/vad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/audio/vad/pyannote/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/audio/vad/pyannote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/augmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/augmentation/cutmix/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/augmentation/cutmix/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/blocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/blocks/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/blocks/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/callbacks/tf_keras/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/callbacks/tf_keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/cv2_dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/dummy_framework/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/dummy_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/dummy_framework/dummy_framework.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/glide_text2im_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/groundingdino_torch_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/requests_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/tf_cv2_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/tf_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/torch_cv2_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/torch_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/torch_monai_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/torchvision_torch_timm_transformers_fairscale_dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/utils/git_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/utils/git_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/utils/memory_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/utils/memory_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/utils/sqlalchemy_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/utils/sqlalchemy_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/utils/torch_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/utils/torch_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/vision/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/vision/face_detection/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/vision/face_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/vision/face_recognition/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/vision/face_recognition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/vision/object_detection/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/vision/object_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/vision/object_tracker/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/vision/object_tracker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/vision/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/vision/ocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/vision/ocr/crnn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/vision/ocr/crnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils/_dummy_objects/vision/ocr/crnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/vision/ocr/crnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.241540 deep_utils-1.2.1/deep_utils/_dummy_objects/vision/torch_vision/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/vision/torch_vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.241540 deep_utils-1.2.1/deep_utils/_dummy_objects/vision/vision_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/vision/vision_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.241540 deep_utils-1.2.1/deep_utils/_dummy_objects/vision/vision_utils/torch_vision_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/_dummy_objects/vision/vision_utils/torch_vision_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.241540 deep_utils-1.2.1/deep_utils/audio/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/audio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.241540 deep_utils-1.2.1/deep_utils/audio/asr/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/audio/asr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.241540 deep_utils-1.2.1/deep_utils/audio/asr/wav2vec2/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/audio/asr/wav2vec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.241540 deep_utils-1.2.1/deep_utils/audio/asr/wav2vec2/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/audio/asr/wav2vec2/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/audio/asr/wav2vec2/torch/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.241540 deep_utils-1.2.1/deep_utils/audio/audio_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/audio/audio_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/audio/audio_utils/librosa_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/audio/audio_utils/torchaudio_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/audio/audio_utils/vox_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.241540 deep_utils-1.2.1/deep_utils/audio/classification/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/audio/classification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.241540 deep_utils-1.2.1/deep_utils/audio/classification/wav2vec2/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/audio/classification/wav2vec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.241540 deep_utils-1.2.1/deep_utils/audio/classification/wav2vec2/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/audio/classification/wav2vec2/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/audio/classification/wav2vec2/torch/audio_classification_wav2vec2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.241540 deep_utils-1.2.1/deep_utils/audio/diarization/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/audio/diarization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.241540 deep_utils-1.2.1/deep_utils/audio/diarization/pyannote/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/audio/diarization/pyannote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/audio/diarization/pyannote/pyannote_audio_diarization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.241540 deep_utils-1.2.1/deep_utils/audio/vad/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/audio/vad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.241540 deep_utils-1.2.1/deep_utils/audio/vad/pyannote/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/audio/vad/pyannote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/audio/vad/pyannote/pyannote_audio_vad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.241540 deep_utils-1.2.1/deep_utils/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/augmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.241540 deep_utils-1.2.1/deep_utils/augmentation/cutmix/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/augmentation/cutmix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/augmentation/cutmix/cutmix_tf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/augmentation/cutmix/cutmix_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.241540 deep_utils-1.2.1/deep_utils/augmentation/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/augmentation/torch/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8071 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/augmentation/torch/augmentation_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.241540 deep_utils-1.2.1/deep_utils/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/blocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.241540 deep_utils-1.2.1/deep_utils/blocks/tf/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/blocks/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/blocks/tf/blocks_tf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.241540 deep_utils-1.2.1/deep_utils/blocks/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/blocks/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/blocks/torch/blocks_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.241540 deep_utils-1.2.1/deep_utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.241540 deep_utils-1.2.1/deep_utils/callbacks/tf_keras/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/callbacks/tf_keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/callbacks/tf_keras/lr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.241540 deep_utils-1.2.1/deep_utils/callbacks/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/callbacks/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/callbacks/torch/torch_csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/callbacks/torch/torch_model_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/callbacks/torch/torch_tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.241540 deep_utils-1.2.1/deep_utils/design_patterns/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/design_patterns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.245540 deep_utils-1.2.1/deep_utils/design_patterns/chain_of_responsibility/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/design_patterns/chain_of_responsibility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/design_patterns/chain_of_responsibility/chain_of_responsibilities_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.245540 deep_utils-1.2.1/deep_utils/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/elasticsearch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.245540 deep_utils-1.2.1/deep_utils/elasticsearch/search_engine/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/elasticsearch/search_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23209 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/elasticsearch/search_engine/elasticsearch_search_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.245540 deep_utils-1.2.1/deep_utils/gis/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/gis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.245540 deep_utils-1.2.1/deep_utils/gis/projection/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/gis/projection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/gis/projection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.245540 deep_utils-1.2.1/deep_utils/main_abs/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/main_abs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.245540 deep_utils-1.2.1/deep_utils/main_abs/cv2/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/main_abs/cv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/main_abs/cv2/cv2_caffe.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/main_abs/cv2/cv2_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/main_abs/cv2/cv2_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/main_abs/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/main_abs/main_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.245540 deep_utils-1.2.1/deep_utils/multi_modals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/multi_modals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.245540 deep_utils-1.2.1/deep_utils/multi_modals/_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/multi_modals/_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.245540 deep_utils-1.2.1/deep_utils/multi_modals/_models/blip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/multi_modals/_models/blip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.245540 deep_utils-1.2.1/deep_utils/multi_modals/_models/blip/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/multi_modals/_models/blip/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.245540 deep_utils-1.2.1/deep_utils/multi_modals/_models/blip/torch/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/multi_modals/_models/blip/torch/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10566 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/multi_modals/_models/blip/torch/models/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)    41523 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/multi_modals/_models/blip/torch/models/med.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/multi_modals/_models/blip/torch/models/med_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/multi_modals/_models/blip/torch/models/vit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.245540 deep_utils-1.2.1/deep_utils/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/nlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.245540 deep_utils-1.2.1/deep_utils/nlp/ner/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/nlp/ner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10689 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/nlp/ner/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/nlp/ner/base_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/nlp/ner/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/nlp/ner/taggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/nlp/ner/utils_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.245540 deep_utils-1.2.1/deep_utils/nlp/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/nlp/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.245540 deep_utils-1.2.1/deep_utils/nlp/utils/multi_lang_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/nlp/utils/multi_lang_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/nlp/utils/multi_lang_utils/multi_lang_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.245540 deep_utils-1.2.1/deep_utils/nlp/utils/persian/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/nlp/utils/persian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/nlp/utils/persian/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.245540 deep_utils-1.2.1/deep_utils/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.245540 deep_utils-1.2.1/deep_utils/preprocessing/monai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/preprocessing/monai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/preprocessing/monai/monai_segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.245540 deep_utils-1.2.1/deep_utils/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.249540 deep_utils-1.2.1/deep_utils/utils/algorithm_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/algorithm_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/algorithm_utils/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.249540 deep_utils-1.2.1/deep_utils/utils/box_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/box_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/box_utils/box_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)    36114 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/box_utils/boxes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.249540 deep_utils-1.2.1/deep_utils/utils/coco_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/coco_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/coco_utils/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.249540 deep_utils-1.2.1/deep_utils/utils/color_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/color_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/color_utils/color_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.249540 deep_utils-1.2.1/deep_utils/utils/compress_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/compress_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/compress_utils/zip_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.249540 deep_utils-1.2.1/deep_utils/utils/ctc_decoder/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/ctc_decoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/ctc_decoder/ctc_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.249540 deep_utils-1.2.1/deep_utils/utils/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/decorators/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.249540 deep_utils-1.2.1/deep_utils/utils/dict_named_tuple_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/dict_named_tuple_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/dict_named_tuple_utils/dictnamedtuple_37.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/dict_named_tuple_utils/dictnamedtuple_38.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.249540 deep_utils-1.2.1/deep_utils/utils/dict_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/dict_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/dict_utils/dict_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.249540 deep_utils-1.2.1/deep_utils/utils/dir_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/dir_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17058 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/dir_utils/dir_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.249540 deep_utils-1.2.1/deep_utils/utils/download_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/download_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/download_utils/download_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.249540 deep_utils-1.2.1/deep_utils/utils/encodes/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/encodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/encodes/b64.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/encodes/web_inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.249540 deep_utils-1.2.1/deep_utils/utils/gif_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/gif_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/gif_utils/gif_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.249540 deep_utils-1.2.1/deep_utils/utils/hash_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/hash_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/hash_utils/hash_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.249540 deep_utils-1.2.1/deep_utils/utils/image_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/image_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/image_utils/image_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.249540 deep_utils-1.2.1/deep_utils/utils/json_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/json_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/json_utils/json_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.249540 deep_utils-1.2.1/deep_utils/utils/kafka_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/kafka_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/kafka_utils/kafka_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.249540 deep_utils-1.2.1/deep_utils/utils/lib_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/lib_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/lib_utils/download_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/lib_utils/lib_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/lib_utils/main_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.253540 deep_utils-1.2.1/deep_utils/utils/list_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/list_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/list_utils/list_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.253540 deep_utils-1.2.1/deep_utils/utils/logging_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/logging_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/logging_utils/logging_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.253540 deep_utils-1.2.1/deep_utils/utils/lr_scheduler_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/lr_scheduler_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/lr_scheduler_utils/warmup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.253540 deep_utils-1.2.1/deep_utils/utils/matplotlib_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/matplotlib_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/matplotlib_utils/bar_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/matplotlib_utils/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.253540 deep_utils-1.2.1/deep_utils/utils/memory_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/memory_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/memory_utils/torch_memory_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.253540 deep_utils-1.2.1/deep_utils/utils/minio_lib/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/minio_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/minio_lib/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.253540 deep_utils-1.2.1/deep_utils/utils/multi_label_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/multi_label_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.253540 deep_utils-1.2.1/deep_utils/utils/multi_label_utils/stratify/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/multi_label_utils/stratify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/multi_label_utils/stratify/stratify_train_test_split.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.253540 deep_utils-1.2.1/deep_utils/utils/np_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/np_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/np_utils/main_np.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.253540 deep_utils-1.2.1/deep_utils/utils/object_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/object_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/object_utils/object_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.253540 deep_utils-1.2.1/deep_utils/utils/opencv_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/opencv_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/opencv_utils/opencv_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.253540 deep_utils-1.2.1/deep_utils/utils/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/optimizers/tf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.253540 deep_utils-1.2.1/deep_utils/utils/os_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/os_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/os_utils/os_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.253540 deep_utils-1.2.1/deep_utils/utils/pickle_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/pickle_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/pickle_utils/pickle_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.253540 deep_utils-1.2.1/deep_utils/utils/postgresql_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/postgresql_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/postgresql_utils/postgresql_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.253540 deep_utils-1.2.1/deep_utils/utils/random_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/random_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/random_utils/random_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.253540 deep_utils-1.2.1/deep_utils/utils/re_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/re_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/re_utils/re_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.253540 deep_utils-1.2.1/deep_utils/utils/requests_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/requests_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/requests_utils/requests_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.253540 deep_utils-1.2.1/deep_utils/utils/resize_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/resize_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/resize_utils/main_resize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.253540 deep_utils-1.2.1/deep_utils/utils/shutil_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/shutil_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/shutil_utils/shutil_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.257540 deep_utils-1.2.1/deep_utils/utils/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/sqlalchemy/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/sqlalchemy/insert.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/sqlalchemy/sqlalchemy_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.257540 deep_utils-1.2.1/deep_utils/utils/tensorboard_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/tensorboard_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/tensorboard_utils/tesnsorboard_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.257540 deep_utils-1.2.1/deep_utils/utils/tf_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/tf_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/tf_utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/tf_utils/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.257540 deep_utils-1.2.1/deep_utils/utils/torch_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/torch_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/torch_utils/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.257540 deep_utils-1.2.1/deep_utils/utils/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/utils/arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/utils/hyper_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/utils/shuffle_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/utils/str_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/utils/yaml_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.257540 deep_utils-1.2.1/deep_utils/utils/variable_naming_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/variable_naming_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/utils/variable_naming_utils/variable_naming_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.257540 deep_utils-1.2.1/deep_utils/vision/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.257540 deep_utils-1.2.1/deep_utils/vision/color_recognition/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/color_recognition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.257540 deep_utils-1.2.1/deep_utils/vision/color_recognition/cnn_color/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/color_recognition/cnn_color/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.257540 deep_utils-1.2.1/deep_utils/vision/color_recognition/cnn_color/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/color_recognition/cnn_color/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/color_recognition/cnn_color/torch/color_cnn_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/color_recognition/cnn_color/torch/color_cnn_torch_pred.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.257540 deep_utils-1.2.1/deep_utils/vision/face_detection/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.257540 deep_utils-1.2.1/deep_utils/vision/face_detection/haarcascade/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/haarcascade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.257540 deep_utils-1.2.1/deep_utils/vision/face_detection/haarcascade/cv2_/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/haarcascade/cv2_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/haarcascade/cv2_/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/haarcascade/cv2_/haarcascade_cv2_face_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.257540 deep_utils-1.2.1/deep_utils/vision/face_detection/main/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/main/main_face_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.257540 deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.257540 deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/tf/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/tf/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/tf/mtcnn_tf_face_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.257540 deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/tf/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/tf/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/tf/src/box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/tf/src/first_stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/tf/src/get_nets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.257540 deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/torch/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/torch/mtcnn_torch_face_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.261540 deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/torch/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/torch/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/torch/src/box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/torch/src/first_stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/torch/src/get_nets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.261540 deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.261540 deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/retinaface_torch_face_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.261540 deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.261540 deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/src/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/src/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.261540 deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/src/layers/functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/src/layers/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/src/layers/functions/prior_box.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.261540 deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/src/layers/modules/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/src/layers/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/src/layers/modules/multibox_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/src/load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/src/net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/src/retinaface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.261540 deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/src/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13383 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/src/utils/box_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.261540 deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/src/utils/nms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/src/utils/nms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/src/utils/nms/py_cpu_nms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/src/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.261540 deep_utils-1.2.1/deep_utils/vision/face_detection/ssd/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/ssd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.261540 deep_utils-1.2.1/deep_utils/vision/face_detection/ssd/cv2/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/ssd/cv2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.261540 deep_utils-1.2.1/deep_utils/vision/face_detection/ssd/cv2/caffe/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/ssd/cv2/caffe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/ssd/cv2/caffe/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/ssd/cv2/caffe/ssd_cv2_caffe_face_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.261540 deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.261540 deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/tf/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/tf/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/tf/ultralight_tf_face_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.261540 deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/tf/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/tf/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/tf/utils/op.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/tf/utils/rfb_320.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/tf/utils/slim_320.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/tf/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.261540 deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/ultralight_torch_face_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.265540 deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/utils/box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/utils/data_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/utils/fd_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_RFB.py
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_RFB_fd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_fd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/utils/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/utils/ssd.py
--rw-r--r--   0 runner    (1001) docker     (123)    18077 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/utils/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.265540 deep_utils-1.2.1/deep_utils/vision/face_recognition/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_recognition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.265540 deep_utils-1.2.1/deep_utils/vision/face_recognition/main/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_recognition/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_recognition/main/main_face_recognition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.265540 deep_utils-1.2.1/deep_utils/vision/face_recognition/vggface2/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_recognition/vggface2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.265540 deep_utils-1.2.1/deep_utils/vision/face_recognition/vggface2/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_recognition/vggface2/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_recognition/vggface2/torch/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.265540 deep_utils-1.2.1/deep_utils/vision/face_recognition/vggface2/torch/src/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_recognition/vggface2/torch/src/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5859 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_recognition/vggface2/torch/src/senet_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/face_recognition/vggface2/torch/vggface2_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.265540 deep_utils-1.2.1/deep_utils/vision/image_caption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/image_caption/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.265540 deep_utils-1.2.1/deep_utils/vision/image_caption/blip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/image_caption/blip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.265540 deep_utils-1.2.1/deep_utils/vision/image_caption/blip/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/image_caption/blip/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/image_caption/blip/torch/blip_torch_image_caption.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/image_caption/image_caption.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.265540 deep_utils-1.2.1/deep_utils/vision/image_editing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/image_editing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.265540 deep_utils-1.2.1/deep_utils/vision/image_editing/glide/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/image_editing/glide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13150 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/image_editing/glide/glide_image_editing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.265540 deep_utils-1.2.1/deep_utils/vision/object_detection/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.265540 deep_utils-1.2.1/deep_utils/vision/object_detection/main/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/main/main_object_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.265540 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.265540 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.265540 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.269540 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/models/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    42372 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/models/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4435 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/models/experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)    27031 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/models/tf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18183 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/models/yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolo_v5_torch_object_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.269540 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)    17021 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/augmentations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/autoanchor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/autobatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    55706 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    48196 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)    46792 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/google_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    14576 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    24456 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.269540 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/augmentations.py
--rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/triton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.269540 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.269540 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.269540 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/models/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    84416 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/models/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/models/experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)    40059 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/models/yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/yolo_v7_torch_object_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.273540 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/add_nms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/autoanchor.py
--rw-r--r--   0 runner    (1001) docker     (123)    56265 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    36907 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/google_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    75043 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    10167 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    20998 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    15474 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19151 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/yolo_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.273540 deep_utils-1.2.1/deep_utils/vision/object_tracker/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_tracker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.273540 deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.273540 deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.273540 deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/deep/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/deep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/deep_sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.273540 deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/sort/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/sort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/sort/detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/sort/iou_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     8059 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/sort/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/sort/linear_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/sort/nn_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/sort/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/sort/track.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/sort/tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.273540 deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/utils/asserts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/utils/draw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/utils/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    12138 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/utils/json_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/utils/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/utils/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.273540 deep_utils-1.2.1/deep_utils/vision/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/ocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.273540 deep_utils-1.2.1/deep_utils/vision/ocr/crnn/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/ocr/crnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.273540 deep_utils-1.2.1/deep_utils/vision/ocr/crnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/ocr/crnn/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/ocr/crnn/torch/crnn_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/ocr/crnn/torch/crnn_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.273540 deep_utils-1.2.1/deep_utils/vision/text2box_visual_grounding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/text2box_visual_grounding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.273540 deep_utils-1.2.1/deep_utils/vision/text2box_visual_grounding/dino/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/text2box_visual_grounding/dino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/text2box_visual_grounding/dino/visual_grounding_dino_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.277540 deep_utils-1.2.1/deep_utils/vision/torch_vision/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/torch_vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.277540 deep_utils-1.2.1/deep_utils/vision/torch_vision/torch_vision_inference/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/torch_vision/torch_vision_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/torch_vision/torch_vision_inference/torch_vision_inference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.277540 deep_utils-1.2.1/deep_utils/vision/torch_vision/torch_vision_models/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/torch_vision/torch_vision_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/torch_vision/torch_vision_models/torch_vision_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.277540 deep_utils-1.2.1/deep_utils/vision/vision_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/vision_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.277540 deep_utils-1.2.1/deep_utils/vision/vision_utils/torch_vision_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/vision_utils/torch_vision_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-27 18:34:03.000000 deep_utils-1.2.1/deep_utils/vision/vision_utils/torch_vision_utils/torch_vision_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.237540 deep_utils-1.2.1/deep_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26630 2023-05-27 18:34:14.000000 deep_utils-1.2.1/deep_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23773 2023-05-27 18:34:14.000000 deep_utils-1.2.1/deep_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 18:34:14.000000 deep_utils-1.2.1/deep_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-27 18:34:14.000000 deep_utils-1.2.1/deep_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-27 18:34:14.000000 deep_utils-1.2.1/deep_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-27 18:34:14.277540 deep_utils-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-27 18:34:03.000000 deep_utils-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.277540 deep_utils-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-27 18:34:03.000000 deep_utils-1.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.277540 deep_utils-1.2.1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-27 18:34:03.000000 deep_utils-1.2.1/tests/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.277540 deep_utils-1.2.1/tests/utils/encoding_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/tests/utils/encoding_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-27 18:34:03.000000 deep_utils-1.2.1/tests/utils/encoding_utils/encoding_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.277540 deep_utils-1.2.1/tests/utils/np_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-27 18:34:03.000000 deep_utils-1.2.1/tests/utils/np_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-27 18:34:03.000000 deep_utils-1.2.1/tests/utils/np_utils/np_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.277540 deep_utils-1.2.1/tests/utils/resize_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-27 18:34:03.000000 deep_utils-1.2.1/tests/utils/resize_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-27 18:34:03.000000 deep_utils-1.2.1/tests/utils/resize_utils/resize_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.277540 deep_utils-1.2.1/tests/utils/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/tests/utils/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.277540 deep_utils-1.2.1/tests/vision/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/tests/vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.277540 deep_utils-1.2.1/tests/vision/face_detection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/tests/vision/face_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.277540 deep_utils-1.2.1/tests/vision/face_detection/mtcnn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/tests/vision/face_detection/mtcnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.277540 deep_utils-1.2.1/tests/vision/face_detection/mtcnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/tests/vision/face_detection/mtcnn/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-27 18:34:03.000000 deep_utils-1.2.1/tests/vision/face_detection/mtcnn/torch/mtcnn_torch_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.277540 deep_utils-1.2.1/tests/vision/face_detection/ultralight/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/tests/vision/face_detection/ultralight/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.277540 deep_utils-1.2.1/tests/vision/face_detection/ultralight/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/tests/vision/face_detection/ultralight/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-27 18:34:03.000000 deep_utils-1.2.1/tests/vision/face_detection/ultralight/torch/ultralight_torch_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.277540 deep_utils-1.2.1/tests/vision/object_detection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/tests/vision/object_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.277540 deep_utils-1.2.1/tests/vision/object_detection/yolo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/tests/vision/object_detection/yolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.277540 deep_utils-1.2.1/tests/vision/object_detection/yolo/v5/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/tests/vision/object_detection/yolo/v5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.277540 deep_utils-1.2.1/tests/vision/object_detection/yolo/v5/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/tests/vision/object_detection/yolo/v5/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-27 18:34:03.000000 deep_utils-1.2.1/tests/vision/object_detection/yolo/v5/torch/yolov5_detection_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.277540 deep_utils-1.2.1/tests/vision/vision_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/tests/vision/vision_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:14.277540 deep_utils-1.2.1/tests/vision/vision_utils/torch_vision_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:03.000000 deep_utils-1.2.1/tests/vision/vision_utils/torch_vision_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-27 18:34:03.000000 deep_utils-1.2.1/tests/vision/vision_utils/torch_vision_utils/torch_vision_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.630346 deep_utils-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-17 18:18:31.000000 deep_utils-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26630 2023-07-17 18:18:42.630346 deep_utils-1.2.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.590346 deep_utils-1.2.2/deep_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/audio/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/audio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/audio/asr/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/audio/asr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/audio/asr/wave2vec2/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/audio/asr/wave2vec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/audio/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/audio/classification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/audio/classification/wav2vec2/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/audio/classification/wav2vec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/audio/diarization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/audio/diarization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/audio/diarization/pyannote/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/audio/diarization/pyannote/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/audio/utils_/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/audio/utils_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/audio/vad/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/audio/vad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/audio/vad/pyannote/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/audio/vad/pyannote/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/augmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/augmentation/cutmix/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/augmentation/cutmix/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/blocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/blocks/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/blocks/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/callbacks/tf_keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/callbacks/tf_keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/cv2_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/dummy_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/dummy_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/dummy_framework/dummy_framework.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/glide_text2im_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/groundingdino_torch_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/requests_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/tf_cv2_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/tf_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/torch_cv2_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/torch_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/torch_monai_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/torchvision_torch_timm_transformers_fairscale_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/utils/git_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/utils/git_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/utils/memory_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/utils/memory_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/utils/sqlalchemy_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/utils/sqlalchemy_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/utils/torch_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/utils/torch_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/vision/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/vision/face_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/vision/face_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/vision/face_recognition/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/vision/face_recognition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/vision/object_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/vision/object_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/vision/object_tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/vision/object_tracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/vision/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/vision/ocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/vision/ocr/crnn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/vision/ocr/crnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/vision/ocr/crnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/vision/ocr/crnn/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/vision/torch_vision/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/vision/torch_vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/vision/vision_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/vision/vision_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/_dummy_objects/vision/vision_utils/torch_vision_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/_dummy_objects/vision/vision_utils/torch_vision_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/audio/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/audio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/audio/asr/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/audio/asr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/audio/asr/wav2vec2/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/audio/asr/wav2vec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/audio/asr/wav2vec2/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/audio/asr/wav2vec2/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/audio/asr/wav2vec2/torch/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.594346 deep_utils-1.2.2/deep_utils/audio/audio_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/audio/audio_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/audio/audio_utils/librosa_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/audio/audio_utils/torchaudio_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/audio/audio_utils/vox_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.598346 deep_utils-1.2.2/deep_utils/audio/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/audio/classification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.598346 deep_utils-1.2.2/deep_utils/audio/classification/wav2vec2/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/audio/classification/wav2vec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.598346 deep_utils-1.2.2/deep_utils/audio/classification/wav2vec2/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/audio/classification/wav2vec2/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/audio/classification/wav2vec2/torch/audio_classification_wav2vec2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.598346 deep_utils-1.2.2/deep_utils/audio/diarization/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/audio/diarization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.598346 deep_utils-1.2.2/deep_utils/audio/diarization/pyannote/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/audio/diarization/pyannote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/audio/diarization/pyannote/pyannote_audio_diarization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.598346 deep_utils-1.2.2/deep_utils/audio/vad/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/audio/vad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.598346 deep_utils-1.2.2/deep_utils/audio/vad/pyannote/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/audio/vad/pyannote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/audio/vad/pyannote/pyannote_audio_vad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.598346 deep_utils-1.2.2/deep_utils/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/augmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.598346 deep_utils-1.2.2/deep_utils/augmentation/cutmix/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/augmentation/cutmix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/augmentation/cutmix/cutmix_tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/augmentation/cutmix/cutmix_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.598346 deep_utils-1.2.2/deep_utils/augmentation/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/augmentation/torch/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8071 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/augmentation/torch/augmentation_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.598346 deep_utils-1.2.2/deep_utils/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/blocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.598346 deep_utils-1.2.2/deep_utils/blocks/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/blocks/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/blocks/tf/blocks_tf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.598346 deep_utils-1.2.2/deep_utils/blocks/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/blocks/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/blocks/torch/blocks_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.598346 deep_utils-1.2.2/deep_utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.598346 deep_utils-1.2.2/deep_utils/callbacks/tf_keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/callbacks/tf_keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/callbacks/tf_keras/lr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.598346 deep_utils-1.2.2/deep_utils/callbacks/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/callbacks/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/callbacks/torch/torch_csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/callbacks/torch/torch_model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/callbacks/torch/torch_tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.598346 deep_utils-1.2.2/deep_utils/design_patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/design_patterns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.598346 deep_utils-1.2.2/deep_utils/design_patterns/chain_of_responsibility/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/design_patterns/chain_of_responsibility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/design_patterns/chain_of_responsibility/chain_of_responsibilities_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.598346 deep_utils-1.2.2/deep_utils/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/elasticsearch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.598346 deep_utils-1.2.2/deep_utils/elasticsearch/search_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/elasticsearch/search_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23209 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/elasticsearch/search_engine/elasticsearch_search_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.598346 deep_utils-1.2.2/deep_utils/gis/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/gis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.598346 deep_utils-1.2.2/deep_utils/gis/projection/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/gis/projection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/gis/projection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.598346 deep_utils-1.2.2/deep_utils/main_abs/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/main_abs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.598346 deep_utils-1.2.2/deep_utils/main_abs/cv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/main_abs/cv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/main_abs/cv2/cv2_caffe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/main_abs/cv2/cv2_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/main_abs/cv2/cv2_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/main_abs/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/main_abs/main_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.598346 deep_utils-1.2.2/deep_utils/multi_modals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/multi_modals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.602346 deep_utils-1.2.2/deep_utils/multi_modals/_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/multi_modals/_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.602346 deep_utils-1.2.2/deep_utils/multi_modals/_models/blip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/multi_modals/_models/blip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.602346 deep_utils-1.2.2/deep_utils/multi_modals/_models/blip/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/multi_modals/_models/blip/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.602346 deep_utils-1.2.2/deep_utils/multi_modals/_models/blip/torch/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/multi_modals/_models/blip/torch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10566 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/multi_modals/_models/blip/torch/models/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41523 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/multi_modals/_models/blip/torch/models/med.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/multi_modals/_models/blip/torch/models/med_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/multi_modals/_models/blip/torch/models/vit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.602346 deep_utils-1.2.2/deep_utils/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/nlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.602346 deep_utils-1.2.2/deep_utils/nlp/ner/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/nlp/ner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10689 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/nlp/ner/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/nlp/ner/base_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/nlp/ner/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/nlp/ner/taggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/nlp/ner/utils_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.602346 deep_utils-1.2.2/deep_utils/nlp/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/nlp/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.602346 deep_utils-1.2.2/deep_utils/nlp/utils/multi_lang_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/nlp/utils/multi_lang_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/nlp/utils/multi_lang_utils/multi_lang_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.602346 deep_utils-1.2.2/deep_utils/nlp/utils/persian/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/nlp/utils/persian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/nlp/utils/persian/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.602346 deep_utils-1.2.2/deep_utils/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.602346 deep_utils-1.2.2/deep_utils/preprocessing/monai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/preprocessing/monai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/preprocessing/monai/monai_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.602346 deep_utils-1.2.2/deep_utils/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.602346 deep_utils-1.2.2/deep_utils/utils/algorithm_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/algorithm_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/algorithm_utils/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.602346 deep_utils-1.2.2/deep_utils/utils/box_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/box_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/box_utils/box_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36114 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/box_utils/boxes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.602346 deep_utils-1.2.2/deep_utils/utils/coco_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/coco_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/coco_utils/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.602346 deep_utils-1.2.2/deep_utils/utils/color_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/color_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/color_utils/color_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.602346 deep_utils-1.2.2/deep_utils/utils/compress_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/compress_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/compress_utils/zip_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.602346 deep_utils-1.2.2/deep_utils/utils/ctc_decoder/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/ctc_decoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/ctc_decoder/ctc_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.602346 deep_utils-1.2.2/deep_utils/utils/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/decorators/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.602346 deep_utils-1.2.2/deep_utils/utils/dict_named_tuple_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/dict_named_tuple_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/dict_named_tuple_utils/dictnamedtuple_37.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/dict_named_tuple_utils/dictnamedtuple_38.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.602346 deep_utils-1.2.2/deep_utils/utils/dict_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/dict_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/dict_utils/dict_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.606346 deep_utils-1.2.2/deep_utils/utils/dir_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/dir_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17058 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/dir_utils/dir_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.606346 deep_utils-1.2.2/deep_utils/utils/download_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/download_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/download_utils/download_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.606346 deep_utils-1.2.2/deep_utils/utils/encodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/encodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/encodes/b64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/encodes/web_inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.606346 deep_utils-1.2.2/deep_utils/utils/gif_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/gif_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/gif_utils/gif_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.606346 deep_utils-1.2.2/deep_utils/utils/hash_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/hash_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/hash_utils/hash_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.606346 deep_utils-1.2.2/deep_utils/utils/image_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/image_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/image_utils/image_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.606346 deep_utils-1.2.2/deep_utils/utils/json_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/json_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/json_utils/json_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.606346 deep_utils-1.2.2/deep_utils/utils/kafka_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/kafka_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/kafka_utils/kafka_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.606346 deep_utils-1.2.2/deep_utils/utils/lib_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/lib_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/lib_utils/download_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/lib_utils/lib_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/lib_utils/main_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.606346 deep_utils-1.2.2/deep_utils/utils/list_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/list_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/list_utils/list_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.606346 deep_utils-1.2.2/deep_utils/utils/logging_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/logging_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/logging_utils/logging_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.606346 deep_utils-1.2.2/deep_utils/utils/lr_scheduler_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/lr_scheduler_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/lr_scheduler_utils/warmup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.606346 deep_utils-1.2.2/deep_utils/utils/matplotlib_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/matplotlib_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/matplotlib_utils/bar_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/matplotlib_utils/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.606346 deep_utils-1.2.2/deep_utils/utils/memory_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/memory_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/memory_utils/torch_memory_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.606346 deep_utils-1.2.2/deep_utils/utils/minio_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/minio_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/minio_lib/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.606346 deep_utils-1.2.2/deep_utils/utils/multi_label_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/multi_label_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.606346 deep_utils-1.2.2/deep_utils/utils/multi_label_utils/stratify/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/multi_label_utils/stratify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/multi_label_utils/stratify/stratify_train_test_split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.606346 deep_utils-1.2.2/deep_utils/utils/np_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/np_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/np_utils/main_np.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.606346 deep_utils-1.2.2/deep_utils/utils/object_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/object_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/object_utils/object_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.606346 deep_utils-1.2.2/deep_utils/utils/opencv_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/opencv_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/opencv_utils/opencv_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.606346 deep_utils-1.2.2/deep_utils/utils/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/optimizers/tf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.606346 deep_utils-1.2.2/deep_utils/utils/os_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/os_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/os_utils/os_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.610346 deep_utils-1.2.2/deep_utils/utils/pickle_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/pickle_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/pickle_utils/pickle_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.610346 deep_utils-1.2.2/deep_utils/utils/postgresql_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/postgresql_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/postgresql_utils/postgresql_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.610346 deep_utils-1.2.2/deep_utils/utils/random_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/random_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/random_utils/random_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.610346 deep_utils-1.2.2/deep_utils/utils/re_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/re_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/re_utils/re_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.610346 deep_utils-1.2.2/deep_utils/utils/requests_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/requests_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/requests_utils/requests_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.610346 deep_utils-1.2.2/deep_utils/utils/resize_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/resize_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/resize_utils/main_resize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.610346 deep_utils-1.2.2/deep_utils/utils/shutil_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/shutil_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/shutil_utils/shutil_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.610346 deep_utils-1.2.2/deep_utils/utils/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/sqlalchemy/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/sqlalchemy/insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/sqlalchemy/sqlalchemy_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.610346 deep_utils-1.2.2/deep_utils/utils/tensorboard_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/tensorboard_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/tensorboard_utils/tesnsorboard_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.610346 deep_utils-1.2.2/deep_utils/utils/tf_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/tf_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/tf_utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/tf_utils/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.610346 deep_utils-1.2.2/deep_utils/utils/torch_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/torch_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/torch_utils/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.610346 deep_utils-1.2.2/deep_utils/utils/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/utils/arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/utils/hyper_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/utils/shuffle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/utils/str_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/utils/yaml_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.610346 deep_utils-1.2.2/deep_utils/utils/variable_naming_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/variable_naming_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/utils/variable_naming_utils/variable_naming_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.610346 deep_utils-1.2.2/deep_utils/vision/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.610346 deep_utils-1.2.2/deep_utils/vision/color_recognition/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/color_recognition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.610346 deep_utils-1.2.2/deep_utils/vision/color_recognition/cnn_color/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/color_recognition/cnn_color/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.610346 deep_utils-1.2.2/deep_utils/vision/color_recognition/cnn_color/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/color_recognition/cnn_color/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/color_recognition/cnn_color/torch/color_cnn_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/color_recognition/cnn_color/torch/color_cnn_torch_pred.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.610346 deep_utils-1.2.2/deep_utils/vision/face_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.610346 deep_utils-1.2.2/deep_utils/vision/face_detection/haarcascade/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/haarcascade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.610346 deep_utils-1.2.2/deep_utils/vision/face_detection/haarcascade/cv2_/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/haarcascade/cv2_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/haarcascade/cv2_/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/haarcascade/cv2_/haarcascade_cv2_face_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.610346 deep_utils-1.2.2/deep_utils/vision/face_detection/main/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/main/main_face_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.614346 deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.614346 deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/tf/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/tf/mtcnn_tf_face_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.614346 deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/tf/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/tf/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/tf/src/box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/tf/src/first_stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/tf/src/get_nets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.614346 deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/torch/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/torch/mtcnn_torch_face_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.614346 deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/torch/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/torch/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/torch/src/box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/torch/src/first_stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/torch/src/get_nets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.614346 deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.614346 deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/retinaface_torch_face_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.614346 deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.614346 deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/src/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/src/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.614346 deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/src/layers/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/src/layers/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/src/layers/functions/prior_box.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.614346 deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/src/layers/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/src/layers/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/src/layers/modules/multibox_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/src/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/src/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/src/retinaface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.614346 deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/src/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13383 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/src/utils/box_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.614346 deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/src/utils/nms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/src/utils/nms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/src/utils/nms/py_cpu_nms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/src/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.614346 deep_utils-1.2.2/deep_utils/vision/face_detection/ssd/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/ssd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.614346 deep_utils-1.2.2/deep_utils/vision/face_detection/ssd/cv2/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/ssd/cv2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.614346 deep_utils-1.2.2/deep_utils/vision/face_detection/ssd/cv2/caffe/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/ssd/cv2/caffe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/ssd/cv2/caffe/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/ssd/cv2/caffe/ssd_cv2_caffe_face_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.614346 deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.614346 deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/tf/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/tf/ultralight_tf_face_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.614346 deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/tf/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/tf/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/tf/utils/op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/tf/utils/rfb_320.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/tf/utils/slim_320.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/tf/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.618346 deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/ultralight_torch_face_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.618346 deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/utils/box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/utils/data_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/utils/fd_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_RFB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_RFB_fd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_fd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/utils/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/utils/ssd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18077 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/utils/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.618346 deep_utils-1.2.2/deep_utils/vision/face_recognition/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_recognition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.618346 deep_utils-1.2.2/deep_utils/vision/face_recognition/main/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_recognition/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_recognition/main/main_face_recognition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.618346 deep_utils-1.2.2/deep_utils/vision/face_recognition/vggface2/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_recognition/vggface2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.618346 deep_utils-1.2.2/deep_utils/vision/face_recognition/vggface2/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_recognition/vggface2/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_recognition/vggface2/torch/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.618346 deep_utils-1.2.2/deep_utils/vision/face_recognition/vggface2/torch/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_recognition/vggface2/torch/src/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5859 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_recognition/vggface2/torch/src/senet_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/face_recognition/vggface2/torch/vggface2_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.618346 deep_utils-1.2.2/deep_utils/vision/image_caption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/image_caption/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.618346 deep_utils-1.2.2/deep_utils/vision/image_caption/blip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/image_caption/blip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.618346 deep_utils-1.2.2/deep_utils/vision/image_caption/blip/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/image_caption/blip/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/image_caption/blip/torch/blip_torch_image_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/image_caption/image_caption.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.618346 deep_utils-1.2.2/deep_utils/vision/image_editing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/image_editing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.618346 deep_utils-1.2.2/deep_utils/vision/image_editing/glide/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/image_editing/glide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13150 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/image_editing/glide/glide_image_editing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.618346 deep_utils-1.2.2/deep_utils/vision/object_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.618346 deep_utils-1.2.2/deep_utils/vision/object_detection/main/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/main/main_object_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.618346 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.618346 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.618346 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.622346 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/models/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42372 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/models/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4435 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/models/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27031 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/models/tf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18183 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/models/yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolo_v5_torch_object_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.622346 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17021 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/autoanchor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/autobatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55706 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48196 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46792 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/google_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14576 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24456 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.622346 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/triton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.622346 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.622346 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.622346 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84416 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/models/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40059 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/models/yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/yolo_v7_torch_object_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.626346 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/add_nms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/autoanchor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56265 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36907 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/google_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75043 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10167 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20998 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15474 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19151 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/yolo_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.626346 deep_utils-1.2.2/deep_utils/vision/object_tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_tracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.626346 deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.626346 deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.626346 deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/deep/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/deep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/deep_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.626346 deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/iou_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8059 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/linear_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/nn_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.626346 deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/asserts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12138 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/json_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.626346 deep_utils-1.2.2/deep_utils/vision/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/ocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.626346 deep_utils-1.2.2/deep_utils/vision/ocr/crnn/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/ocr/crnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.626346 deep_utils-1.2.2/deep_utils/vision/ocr/crnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/ocr/crnn/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/ocr/crnn/torch/crnn_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/ocr/crnn/torch/crnn_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.626346 deep_utils-1.2.2/deep_utils/vision/text2box_visual_grounding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/text2box_visual_grounding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.626346 deep_utils-1.2.2/deep_utils/vision/text2box_visual_grounding/dino/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/text2box_visual_grounding/dino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/text2box_visual_grounding/dino/visual_grounding_dino_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.626346 deep_utils-1.2.2/deep_utils/vision/torch_vision/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/torch_vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.626346 deep_utils-1.2.2/deep_utils/vision/torch_vision/torch_vision_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/torch_vision/torch_vision_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/torch_vision/torch_vision_inference/torch_vision_inference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.626346 deep_utils-1.2.2/deep_utils/vision/torch_vision/torch_vision_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/torch_vision/torch_vision_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/torch_vision/torch_vision_models/torch_vision_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.626346 deep_utils-1.2.2/deep_utils/vision/vision_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/vision_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.626346 deep_utils-1.2.2/deep_utils/vision/vision_utils/torch_vision_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/vision_utils/torch_vision_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-17 18:18:31.000000 deep_utils-1.2.2/deep_utils/vision/vision_utils/torch_vision_utils/torch_vision_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.590346 deep_utils-1.2.2/deep_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26630 2023-07-17 18:18:42.000000 deep_utils-1.2.2/deep_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23773 2023-07-17 18:18:42.000000 deep_utils-1.2.2/deep_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 18:18:42.000000 deep_utils-1.2.2/deep_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-17 18:18:42.000000 deep_utils-1.2.2/deep_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-17 18:18:42.000000 deep_utils-1.2.2/deep_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-17 18:18:42.630346 deep_utils-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-17 18:18:31.000000 deep_utils-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.626346 deep_utils-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-17 18:18:31.000000 deep_utils-1.2.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.626346 deep_utils-1.2.2/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-17 18:18:31.000000 deep_utils-1.2.2/tests/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.626346 deep_utils-1.2.2/tests/utils/encoding_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/tests/utils/encoding_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-17 18:18:31.000000 deep_utils-1.2.2/tests/utils/encoding_utils/encoding_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.626346 deep_utils-1.2.2/tests/utils/np_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-17 18:18:31.000000 deep_utils-1.2.2/tests/utils/np_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-17 18:18:31.000000 deep_utils-1.2.2/tests/utils/np_utils/np_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.630346 deep_utils-1.2.2/tests/utils/resize_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-17 18:18:31.000000 deep_utils-1.2.2/tests/utils/resize_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-17 18:18:31.000000 deep_utils-1.2.2/tests/utils/resize_utils/resize_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.630346 deep_utils-1.2.2/tests/utils/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/tests/utils/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.630346 deep_utils-1.2.2/tests/vision/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/tests/vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.630346 deep_utils-1.2.2/tests/vision/face_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/tests/vision/face_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.630346 deep_utils-1.2.2/tests/vision/face_detection/mtcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/tests/vision/face_detection/mtcnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.630346 deep_utils-1.2.2/tests/vision/face_detection/mtcnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/tests/vision/face_detection/mtcnn/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-17 18:18:31.000000 deep_utils-1.2.2/tests/vision/face_detection/mtcnn/torch/mtcnn_torch_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.630346 deep_utils-1.2.2/tests/vision/face_detection/ultralight/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/tests/vision/face_detection/ultralight/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.630346 deep_utils-1.2.2/tests/vision/face_detection/ultralight/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/tests/vision/face_detection/ultralight/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-17 18:18:31.000000 deep_utils-1.2.2/tests/vision/face_detection/ultralight/torch/ultralight_torch_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.630346 deep_utils-1.2.2/tests/vision/object_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/tests/vision/object_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.630346 deep_utils-1.2.2/tests/vision/object_detection/yolo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/tests/vision/object_detection/yolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.630346 deep_utils-1.2.2/tests/vision/object_detection/yolo/v5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/tests/vision/object_detection/yolo/v5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.630346 deep_utils-1.2.2/tests/vision/object_detection/yolo/v5/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/tests/vision/object_detection/yolo/v5/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-17 18:18:31.000000 deep_utils-1.2.2/tests/vision/object_detection/yolo/v5/torch/yolov5_detection_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.630346 deep_utils-1.2.2/tests/vision/vision_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/tests/vision/vision_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:42.630346 deep_utils-1.2.2/tests/vision/vision_utils/torch_vision_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:18:31.000000 deep_utils-1.2.2/tests/vision/vision_utils/torch_vision_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-17 18:18:31.000000 deep_utils-1.2.2/tests/vision/vision_utils/torch_vision_utils/torch_vision_utils_test.py
```

### Comparing `deep_utils-1.2.1/LICENSE` & `deep_utils-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/PKG-INFO` & `deep_utils-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: deep_utils
-Version: 1.2.1
+Version: 1.2.2
 Summary: Deep Utils
 Home-page: https://github.com/pooya-mohammadi/deep_utils
 Author: Pooya Mohammadi Kazaj
 Author-email: pooyamohammadikazaj@gmial.com
 License: UNKNOWN
-Download-URL: https://github.com/pooya-mohammadi/deep_utils/archive/refs/tags/1.2.1.tar.gz
+Download-URL: https://github.com/pooya-mohammadi/deep_utils/archive/refs/tags/1.2.2.tar.gz
 Description: [![Downloads](https://static.pepy.tech/badge/deep_utils)](https://pepy.tech/project/deep_utils) [![PyPI](https://img.shields.io/pypi/v/deep_utils.svg)](https://pypi.python.org/pypi/deep_utils)
         
         <div id="top"></div>
         <!-- PROJECT LOGO -->
         <br />
         <div align="center">
           <a href="https://github.com/pooya-mohammadi/deep_utils">
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: deep_utils Version: 1.2.1 Summary: Deep Utils Home-
+Metadata-Version: 2.1 Name: deep_utils Version: 1.2.2 Summary: Deep Utils Home-
 page: https://github.com/pooya-mohammadi/deep_utils Author: Pooya Mohammadi
 Kazaj Author-email: pooyamohammadikazaj@gmial.com License: UNKNOWN Download-
 URL: https://github.com/pooya-mohammadi/deep_utils/archive/refs/tags/
-1.2.1.tar.gz Description: [![Downloads](https://static.pepy.tech/badge/
+1.2.2.tar.gz Description: [![Downloads](https://static.pepy.tech/badge/
 deep_utils)](https://pepy.tech/project/deep_utils) [![PyPI](https://
 img.shields.io/pypi/v/deep_utils.svg)](https://pypi.python.org/pypi/deep_utils)
 
                                     [Logo]
                              **** Deep Utils ****
                   A toolkit for deep-learning practitioners!
 This repository contains the most frequently used deep learning models and
```

### Comparing `deep_utils-1.2.1/deep_utils/__init__.py` & `deep_utils-1.2.2/deep_utils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     is_timm_available,
     is_glide_text2im_available,
     is_pillow_available,
     is_requests_available,
 )
 
 # Deep Utils version number
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 
 # no third-party python libraries are required for the following classes
 _import_structure = {
     "utils.box_utils.boxes": ["Box", "Point"],
     "utils.box_utils.box_dataclasses": ["BoxDataClass", "PointDataClass"],
     "utils.os_utils.os_path": ["validate_file_extension", "is_img", "split_extension", "split_all", "get_file_name"],
     "utils.dir_utils.dir_utils": ["transfer_directory_items",
@@ -32,15 +32,15 @@
                                   "file_incremental",
                                   "cp_mv_all",
                                   "split_segmentation_dirs",
                                   "find_file",
                                   "combine_directory_of_directories"],
     "utils.pickle_utils.pickle_utils": ["dump_pickle", "load_pickle"],
     "utils.logging_utils.logging_utils": ["get_logger"],
-
+    "utils.lr_scheduler_utils.warmup": ["cosine_reduce", "warmup_cosine"],
 }
 
 if is_requests_available():
     _import_structure["utils.download_utils.download_utils"] = ["DownloadUtils"]
 else:
     from ._dummy_objects import requests_dummy
 
@@ -54,15 +54,16 @@
 else:
     from ._dummy_objects import groundingdino_torch_dummy
 
     _import_structure["_dummy_objects.groundingdino_torch_dummy"] = [
         name for name in dir(groundingdino_torch_dummy) if not name.startswith("_")
     ]
 if is_glide_text2im_available() and is_torch_available():
-    _import_structure["vision.image_editing.glide.glide_image_editing"] = ["ImageEditingGLIDE", "ImageEditingGLIDETypes"]
+    _import_structure["vision.image_editing.glide.glide_image_editing"] = ["ImageEditingGLIDE",
+                                                                           "ImageEditingGLIDETypes"]
 else:
     from ._dummy_objects import glide_text2im_dummy
 
     _import_structure["_dummy_objects.glide_text2im_dummy"] = [
         name for name in dir(glide_text2im_dummy) if not name.startswith("_")
     ]
 if is_timm_available() and is_transformers_available() and is_torchvision_available() and is_torch_available():
@@ -168,14 +169,15 @@
     from .vision.color_recognition.cnn_color.torch.color_cnn_torch_pred import ColorRecognitionCNNTorchPrediction
     from .vision.ocr.crnn.torch.crnn_inference import CRNNInferenceTorch
     from .vision.ocr.crnn.torch.crnn_model import CRNNModelTorch
     from .utils.logging_utils.logging_utils import get_logger
     from .vision.image_editing.glide.glide_image_editing import ImageEditingGLIDE, ImageEditingGLIDETypes
     from .vision.text2box_visual_grounding.dino.visual_grounding_dino_torch import Text2BoxVisualGroundingDino
     from .utils.download_utils.download_utils import DownloadUtils
+    from .utils.lr_scheduler_utils.warmup import cosine_reduce, warmup_cosine
 else:
     import sys
 
     sys.modules[__name__] = _LazyModule(
         __name__,
         globals()["__file__"],
         _import_structure,
```

### Comparing `deep_utils-1.2.1/deep_utils/_dummy_objects/cv2_dummy.py` & `deep_utils-1.2.2/deep_utils/_dummy_objects/cv2_dummy.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/_dummy_objects/dummy_framework/dummy_framework.py` & `deep_utils-1.2.2/deep_utils/_dummy_objects/dummy_framework/dummy_framework.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/_dummy_objects/glide_text2im_dummy.py` & `deep_utils-1.2.2/deep_utils/_dummy_objects/glide_text2im_dummy.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/_dummy_objects/groundingdino_torch_dummy.py` & `deep_utils-1.2.2/deep_utils/_dummy_objects/groundingdino_torch_dummy.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/_dummy_objects/torch_cv2_dummy.py` & `deep_utils-1.2.2/deep_utils/_dummy_objects/torch_cv2_dummy.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/_dummy_objects/torch_dummy.py` & `deep_utils-1.2.2/deep_utils/_dummy_objects/torch_dummy.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/_dummy_objects/torchvision_torch_timm_transformers_fairscale_dummy.py` & `deep_utils-1.2.2/deep_utils/_dummy_objects/torchvision_torch_timm_transformers_fairscale_dummy.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/_dummy_objects/utils/sqlalchemy_utils/__init__.py` & `deep_utils-1.2.2/deep_utils/_dummy_objects/utils/sqlalchemy_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/_dummy_objects/vision/face_detection/__init__.py` & `deep_utils-1.2.2/deep_utils/_dummy_objects/vision/face_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/_dummy_objects/vision/object_detection/__init__.py` & `deep_utils-1.2.2/deep_utils/_dummy_objects/vision/object_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/_dummy_objects/vision/object_tracker/__init__.py` & `deep_utils-1.2.2/deep_utils/_dummy_objects/vision/object_tracker/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/audio/asr/wav2vec2/torch/main.py` & `deep_utils-1.2.2/deep_utils/audio/asr/wav2vec2/torch/main.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/audio/audio_utils/librosa_utils.py` & `deep_utils-1.2.2/deep_utils/audio/audio_utils/librosa_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/audio/audio_utils/torchaudio_utils.py` & `deep_utils-1.2.2/deep_utils/audio/audio_utils/torchaudio_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/audio/audio_utils/vox_utils.py` & `deep_utils-1.2.2/deep_utils/audio/audio_utils/vox_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/audio/classification/wav2vec2/torch/audio_classification_wav2vec2.py` & `deep_utils-1.2.2/deep_utils/audio/classification/wav2vec2/torch/audio_classification_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/audio/diarization/pyannote/pyannote_audio_diarization.py` & `deep_utils-1.2.2/deep_utils/audio/diarization/pyannote/pyannote_audio_diarization.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/audio/vad/pyannote/pyannote_audio_vad.py` & `deep_utils-1.2.2/deep_utils/audio/vad/pyannote/pyannote_audio_vad.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/augmentation/cutmix/cutmix_tf.py` & `deep_utils-1.2.2/deep_utils/augmentation/cutmix/cutmix_tf.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/augmentation/cutmix/cutmix_torch.py` & `deep_utils-1.2.2/deep_utils/augmentation/cutmix/cutmix_torch.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/augmentation/torch/augmentation_torch.py` & `deep_utils-1.2.2/deep_utils/augmentation/torch/augmentation_torch.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/blocks/tf/blocks_tf.py` & `deep_utils-1.2.2/deep_utils/blocks/tf/blocks_tf.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/blocks/torch/blocks_torch.py` & `deep_utils-1.2.2/deep_utils/blocks/torch/blocks_torch.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/callbacks/tf_keras/lr.py` & `deep_utils-1.2.2/deep_utils/callbacks/tf_keras/lr.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/callbacks/torch/torch_csv_logger.py` & `deep_utils-1.2.2/deep_utils/callbacks/torch/torch_csv_logger.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/callbacks/torch/torch_model_checkpoint.py` & `deep_utils-1.2.2/deep_utils/callbacks/torch/torch_model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/callbacks/torch/torch_tensorboard.py` & `deep_utils-1.2.2/deep_utils/callbacks/torch/torch_tensorboard.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/design_patterns/chain_of_responsibility/chain_of_responsibilities_handlers.py` & `deep_utils-1.2.2/deep_utils/design_patterns/chain_of_responsibility/chain_of_responsibilities_handlers.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/elasticsearch/search_engine/elasticsearch_search_engine.py` & `deep_utils-1.2.2/deep_utils/elasticsearch/search_engine/elasticsearch_search_engine.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/gis/projection/main.py` & `deep_utils-1.2.2/deep_utils/gis/projection/main.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/main_abs/cv2/cv2_caffe.py` & `deep_utils-1.2.2/deep_utils/main_abs/cv2/cv2_caffe.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/main_abs/cv2/cv2_main.py` & `deep_utils-1.2.2/deep_utils/main_abs/cv2/cv2_main.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/main_abs/main.py` & `deep_utils-1.2.2/deep_utils/main_abs/main.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/main_abs/main_config.py` & `deep_utils-1.2.2/deep_utils/main_abs/main_config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/multi_modals/_models/blip/torch/models/blip.py` & `deep_utils-1.2.2/deep_utils/multi_modals/_models/blip/torch/models/blip.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/multi_modals/_models/blip/torch/models/med.py` & `deep_utils-1.2.2/deep_utils/multi_modals/_models/blip/torch/models/med.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/multi_modals/_models/blip/torch/models/med_configs.py` & `deep_utils-1.2.2/deep_utils/multi_modals/_models/blip/torch/models/med_configs.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/multi_modals/_models/blip/torch/models/vit.py` & `deep_utils-1.2.2/deep_utils/multi_modals/_models/blip/torch/models/vit.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/nlp/ner/augmentation.py` & `deep_utils-1.2.2/deep_utils/nlp/ner/augmentation.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/nlp/ner/base_operations.py` & `deep_utils-1.2.2/deep_utils/nlp/ner/base_operations.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/nlp/ner/preprocessing.py` & `deep_utils-1.2.2/deep_utils/nlp/ner/preprocessing.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/nlp/ner/utils_.py` & `deep_utils-1.2.2/deep_utils/nlp/ner/utils_.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/nlp/utils/persian/utils.py` & `deep_utils-1.2.2/deep_utils/nlp/utils/persian/utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/preprocessing/monai/monai_segmentation.py` & `deep_utils-1.2.2/deep_utils/preprocessing/monai/monai_segmentation.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/__init__.py` & `deep_utils-1.2.2/deep_utils/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/algorithm_utils/main.py` & `deep_utils-1.2.2/deep_utils/utils/algorithm_utils/main.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/box_utils/boxes.py` & `deep_utils-1.2.2/deep_utils/utils/box_utils/boxes.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/coco_utils/main.py` & `deep_utils-1.2.2/deep_utils/utils/coco_utils/main.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/color_utils/color_utils.py` & `deep_utils-1.2.2/deep_utils/utils/color_utils/color_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/compress_utils/zip_utils.py` & `deep_utils-1.2.2/deep_utils/utils/compress_utils/zip_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/ctc_decoder/ctc_decoder.py` & `deep_utils-1.2.2/deep_utils/utils/ctc_decoder/ctc_decoder.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/decorators/main.py` & `deep_utils-1.2.2/deep_utils/utils/decorators/main.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/dict_named_tuple_utils/dictnamedtuple_37.py` & `deep_utils-1.2.2/deep_utils/utils/dict_named_tuple_utils/dictnamedtuple_37.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/dict_named_tuple_utils/dictnamedtuple_38.py` & `deep_utils-1.2.2/deep_utils/utils/dict_named_tuple_utils/dictnamedtuple_38.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/dict_utils/dict_utils.py` & `deep_utils-1.2.2/deep_utils/utils/dict_utils/dict_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/dir_utils/dir_utils.py` & `deep_utils-1.2.2/deep_utils/utils/dir_utils/dir_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/download_utils/download_utils.py` & `deep_utils-1.2.2/deep_utils/utils/download_utils/download_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,15 +69,16 @@
                     total = int(total)
                     for data in response.iter_content(
                             chunk_size=max(int(total / 1000), 1024 * 1024)
                     ):
                         downloaded += len(data)
                         f.write(data)
                         done = int(50 * downloaded / total)
-                        sys.stdout.write("\rDownloading: [{}{}]".format("█" * done, "." * (50 - done)))
+                        sys.stdout.write("\rDownloading {}: {}% [{}{}]"
+                                         .format(file_name, round((downloaded*100/total), 2), "█" * done, "." * (50 - done)))
                         sys.stdout.flush()
             sys.stdout.write("\n")
             shutil.move(temp_download_des, download_des)
         except (Exception, KeyboardInterrupt):
             if (
                     temp_download_des is not None
                     and os.path.isfile(temp_download_des)
```

### Comparing `deep_utils-1.2.1/deep_utils/utils/encodes/b64.py` & `deep_utils-1.2.2/deep_utils/utils/encodes/b64.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/gif_utils/gif_utils.py` & `deep_utils-1.2.2/deep_utils/utils/gif_utils/gif_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/hash_utils/hash_utils.py` & `deep_utils-1.2.2/deep_utils/utils/hash_utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/image_utils/image_utils.py` & `deep_utils-1.2.2/deep_utils/utils/image_utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/json_utils/json_utils.py` & `deep_utils-1.2.2/deep_utils/utils/json_utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/kafka_utils/kafka_utils.py` & `deep_utils-1.2.2/deep_utils/utils/kafka_utils/kafka_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/lib_utils/download_utils.py` & `deep_utils-1.2.2/deep_utils/utils/lib_utils/download_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/lib_utils/lib_decorators.py` & `deep_utils-1.2.2/deep_utils/utils/lib_utils/lib_decorators.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/lib_utils/main_utils.py` & `deep_utils-1.2.2/deep_utils/utils/lib_utils/main_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/logging_utils/logging_utils.py` & `deep_utils-1.2.2/deep_utils/utils/logging_utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/lr_scheduler_utils/warmup.py` & `deep_utils-1.2.2/deep_utils/utils/lr_scheduler_utils/warmup.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/matplotlib_utils/bar_plots.py` & `deep_utils-1.2.2/deep_utils/utils/matplotlib_utils/bar_plots.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/matplotlib_utils/main.py` & `deep_utils-1.2.2/deep_utils/utils/matplotlib_utils/main.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/memory_utils/torch_memory_utils.py` & `deep_utils-1.2.2/deep_utils/utils/memory_utils/torch_memory_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/minio_lib/main.py` & `deep_utils-1.2.2/deep_utils/utils/minio_lib/main.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/multi_label_utils/stratify/stratify_train_test_split.py` & `deep_utils-1.2.2/deep_utils/utils/multi_label_utils/stratify/stratify_train_test_split.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/np_utils/main_np.py` & `deep_utils-1.2.2/deep_utils/utils/np_utils/main_np.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/object_utils/object_utils.py` & `deep_utils-1.2.2/deep_utils/utils/object_utils/object_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/opencv_utils/opencv_utils.py` & `deep_utils-1.2.2/deep_utils/utils/opencv_utils/opencv_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/optimizers/tf.py` & `deep_utils-1.2.2/deep_utils/utils/optimizers/tf.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/os_utils/os_path.py` & `deep_utils-1.2.2/deep_utils/utils/os_utils/os_path.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/postgresql_utils/postgresql_utils.py` & `deep_utils-1.2.2/deep_utils/utils/postgresql_utils/postgresql_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/re_utils/re_utils.py` & `deep_utils-1.2.2/deep_utils/utils/re_utils/re_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/requests_utils/requests_utils.py` & `deep_utils-1.2.2/deep_utils/utils/requests_utils/requests_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/resize_utils/main_resize.py` & `deep_utils-1.2.2/deep_utils/utils/resize_utils/main_resize.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/shutil_utils/shutil_utils.py` & `deep_utils-1.2.2/deep_utils/utils/shutil_utils/shutil_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/sqlalchemy/__init__.py` & `deep_utils-1.2.2/deep_utils/utils/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/sqlalchemy/checks.py` & `deep_utils-1.2.2/deep_utils/utils/sqlalchemy/checks.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/sqlalchemy/sqlalchemy_utils.py` & `deep_utils-1.2.2/deep_utils/utils/sqlalchemy/sqlalchemy_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/tensorboard_utils/tesnsorboard_utils.py` & `deep_utils-1.2.2/deep_utils/utils/tensorboard_utils/tesnsorboard_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/tf_utils/logging.py` & `deep_utils-1.2.2/deep_utils/utils/tf_utils/logging.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/tf_utils/main.py` & `deep_utils-1.2.2/deep_utils/utils/tf_utils/main.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/torch_utils/torch_utils.py` & `deep_utils-1.2.2/deep_utils/utils/torch_utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/utils/hyper_parameters.py` & `deep_utils-1.2.2/deep_utils/utils/utils/hyper_parameters.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/utils/shuffle_utils.py` & `deep_utils-1.2.2/deep_utils/utils/utils/shuffle_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/utils/str_utils.py` & `deep_utils-1.2.2/deep_utils/utils/utils/str_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/utils/utils/yaml_utils.py` & `deep_utils-1.2.2/deep_utils/utils/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/color_recognition/cnn_color/torch/color_cnn_torch.py` & `deep_utils-1.2.2/deep_utils/vision/color_recognition/cnn_color/torch/color_cnn_torch.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/color_recognition/cnn_color/torch/color_cnn_torch_pred.py` & `deep_utils-1.2.2/deep_utils/vision/color_recognition/cnn_color/torch/color_cnn_torch_pred.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/__init__.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/haarcascade/cv2_/config.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/haarcascade/cv2_/config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/haarcascade/cv2_/haarcascade_cv2_face_detection.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/haarcascade/cv2_/haarcascade_cv2_face_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/main/main_face_detection.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/main/main_face_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/tf/config.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/tf/config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/tf/mtcnn_tf_face_detection.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/tf/mtcnn_tf_face_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/tf/src/box_utils.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/tf/src/box_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/tf/src/first_stage.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/tf/src/first_stage.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/tf/src/get_nets.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/tf/src/get_nets.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/torch/config.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/torch/config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/torch/mtcnn_torch_face_detection.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/torch/mtcnn_torch_face_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/torch/src/box_utils.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/torch/src/box_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/torch/src/first_stage.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/torch/src/first_stage.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/mtcnn/torch/src/get_nets.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/mtcnn/torch/src/get_nets.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/config.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/retinaface_torch_face_detection.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/retinaface_torch_face_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/src/layers/functions/prior_box.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/src/layers/functions/prior_box.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/src/layers/modules/multibox_loss.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/src/layers/modules/multibox_loss.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/src/load_model.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/src/load_model.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/src/net.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/src/net.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/src/retinaface.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/src/retinaface.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/src/utils/box_utils.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/src/utils/box_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/src/utils/nms/py_cpu_nms.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/src/utils/nms/py_cpu_nms.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/retinaface/torch/src/utils/timer.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/retinaface/torch/src/utils/timer.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/ssd/cv2/caffe/config.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/ssd/cv2/caffe/config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/ssd/cv2/caffe/ssd_cv2_caffe_face_detection.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/ssd/cv2/caffe/ssd_cv2_caffe_face_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/tf/ultralight_tf_face_detection.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/tf/ultralight_tf_face_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/tf/utils/op.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/tf/utils/op.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/tf/utils/rfb_320.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/tf/utils/rfb_320.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/tf/utils/slim_320.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/tf/utils/slim_320.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/tf/utils/utils.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/tf/utils/utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/config.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/ultralight_torch_face_detection.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/ultralight_torch_face_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/utils/box_utils.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/utils/box_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/utils/data_preprocessing.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/utils/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/utils/fd_config.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/utils/fd_config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_RFB.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_RFB.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_RFB_fd.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_RFB_fd.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_fd.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_fd.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/utils/misc.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/utils/misc.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/utils/predictor.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/utils/predictor.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/utils/ssd.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/utils/ssd.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_detection/ultralight/torch/utils/transforms.py` & `deep_utils-1.2.2/deep_utils/vision/face_detection/ultralight/torch/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_recognition/main/main_face_recognition.py` & `deep_utils-1.2.2/deep_utils/vision/face_recognition/main/main_face_recognition.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_recognition/vggface2/torch/config.py` & `deep_utils-1.2.2/deep_utils/vision/face_recognition/vggface2/torch/config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_recognition/vggface2/torch/src/senet_model.py` & `deep_utils-1.2.2/deep_utils/vision/face_recognition/vggface2/torch/src/senet_model.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/face_recognition/vggface2/torch/vggface2_torch.py` & `deep_utils-1.2.2/deep_utils/vision/face_recognition/vggface2/torch/vggface2_torch.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/image_caption/blip/torch/blip_torch_image_caption.py` & `deep_utils-1.2.2/deep_utils/vision/image_caption/blip/torch/blip_torch_image_caption.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/image_caption/image_caption.py` & `deep_utils-1.2.2/deep_utils/vision/image_caption/image_caption.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/image_editing/glide/glide_image_editing.py` & `deep_utils-1.2.2/deep_utils/vision/image_editing/glide/glide_image_editing.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/__init__.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/main/main_object_detection.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/main/main_object_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/config.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/models/common.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/models/common.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/models/experimental.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/models/experimental.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/models/tf.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/models/tf.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/models/yolo.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/models/yolo.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolo_v5_torch_object_detection.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolo_v5_torch_object_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/__init__.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/activations.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/activations.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/augmentations.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/augmentations.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/autoanchor.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/autoanchor.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/autobatch.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/callbacks.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/dataloaders.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/dataloaders.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/datasets.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/datasets.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/downloads.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/downloads.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/general.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/general.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/google_utils.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/google_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/loss.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/loss.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/metrics.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/plots.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/plots.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/augmentations.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/augmentations.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/dataloaders.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/dataloaders.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/general.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/general.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/loss.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/loss.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/metrics.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/metrics.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/plots.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/plots.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/torch_utils.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/triton.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/triton.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/config.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/models/common.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/models/common.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/models/experimental.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/models/experimental.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/models/yolo.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/models/yolo.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/yolo_v7_torch_object_detection.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/yolo_v7_torch_object_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/activations.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/activations.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/add_nms.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/add_nms.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/autoanchor.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/autoanchor.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/datasets.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/datasets.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/general.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/general.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/google_utils.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/google_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/loss.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/loss.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/metrics.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/plots.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/plots.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/torch_utils.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_detection/yolo/yolo_detector.py` & `deep_utils-1.2.2/deep_utils/vision/object_detection/yolo/yolo_detector.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_tracker/__init__.py` & `deep_utils-1.2.2/deep_utils/vision/object_tracker/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/__init__.py` & `deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/deep_sort.py` & `deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/deep_sort.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/sort/detection.py` & `deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/sort/iou_matching.py` & `deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/iou_matching.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/sort/kalman_filter.py` & `deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/sort/linear_assignment.py` & `deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/linear_assignment.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/sort/nn_matching.py` & `deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/nn_matching.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/sort/preprocessing.py` & `deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/preprocessing.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/sort/track.py` & `deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/track.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/sort/tracker.py` & `deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/tracker.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/utils/draw.py` & `deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/draw.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/utils/evaluation.py` & `deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/utils/io.py` & `deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/io.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/utils/json_logger.py` & `deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/json_logger.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/utils/parser.py` & `deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/parser.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/object_tracker/deep_sort/torch/utils/tools.py` & `deep_utils-1.2.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/tools.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/ocr/crnn/torch/crnn_inference.py` & `deep_utils-1.2.2/deep_utils/vision/ocr/crnn/torch/crnn_inference.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/ocr/crnn/torch/crnn_model.py` & `deep_utils-1.2.2/deep_utils/vision/ocr/crnn/torch/crnn_model.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/text2box_visual_grounding/dino/visual_grounding_dino_torch.py` & `deep_utils-1.2.2/deep_utils/vision/text2box_visual_grounding/dino/visual_grounding_dino_torch.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/torch_vision/torch_vision_inference/torch_vision_inference.py` & `deep_utils-1.2.2/deep_utils/vision/torch_vision/torch_vision_inference/torch_vision_inference.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/torch_vision/torch_vision_models/torch_vision_models.py` & `deep_utils-1.2.2/deep_utils/vision/torch_vision/torch_vision_models/torch_vision_models.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils/vision/vision_utils/torch_vision_utils/torch_vision_utils.py` & `deep_utils-1.2.2/deep_utils/vision/vision_utils/torch_vision_utils/torch_vision_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/deep_utils.egg-info/PKG-INFO` & `deep_utils-1.2.2/deep_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: deep-utils
-Version: 1.2.1
+Version: 1.2.2
 Summary: Deep Utils
 Home-page: https://github.com/pooya-mohammadi/deep_utils
 Author: Pooya Mohammadi Kazaj
 Author-email: pooyamohammadikazaj@gmial.com
 License: UNKNOWN
-Download-URL: https://github.com/pooya-mohammadi/deep_utils/archive/refs/tags/1.2.1.tar.gz
+Download-URL: https://github.com/pooya-mohammadi/deep_utils/archive/refs/tags/1.2.2.tar.gz
 Description: [![Downloads](https://static.pepy.tech/badge/deep_utils)](https://pepy.tech/project/deep_utils) [![PyPI](https://img.shields.io/pypi/v/deep_utils.svg)](https://pypi.python.org/pypi/deep_utils)
         
         <div id="top"></div>
         <!-- PROJECT LOGO -->
         <br />
         <div align="center">
           <a href="https://github.com/pooya-mohammadi/deep_utils">
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: deep-utils Version: 1.2.1 Summary: Deep Utils Home-
+Metadata-Version: 2.1 Name: deep-utils Version: 1.2.2 Summary: Deep Utils Home-
 page: https://github.com/pooya-mohammadi/deep_utils Author: Pooya Mohammadi
 Kazaj Author-email: pooyamohammadikazaj@gmial.com License: UNKNOWN Download-
 URL: https://github.com/pooya-mohammadi/deep_utils/archive/refs/tags/
-1.2.1.tar.gz Description: [![Downloads](https://static.pepy.tech/badge/
+1.2.2.tar.gz Description: [![Downloads](https://static.pepy.tech/badge/
 deep_utils)](https://pepy.tech/project/deep_utils) [![PyPI](https://
 img.shields.io/pypi/v/deep_utils.svg)](https://pypi.python.org/pypi/deep_utils)
 
                                     [Logo]
                              **** Deep Utils ****
                   A toolkit for deep-learning practitioners!
 This repository contains the most frequently used deep learning models and
```

### Comparing `deep_utils-1.2.1/deep_utils.egg-info/SOURCES.txt` & `deep_utils-1.2.2/deep_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/setup.py` & `deep_utils-1.2.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 import setuptools
 
-VERSION = "1.2.1"
+VERSION = "1.2.2"
 
-try:
-    import pypandoc
-
-    long_description = pypandoc.convert("Readme.md", "rst")
-except (IOError, ImportError):
-    long_description = open("Readme.md", mode="r", encoding="utf-8").read()
+long_description = open("Readme.md", mode="r", encoding="utf-8").read()
 
 # Module dependencies
 dependency_links = []
 
 requirements = [
     "numpy>=1.21.0",
     "requests>=2.27.1",
```

### Comparing `deep_utils-1.2.1/tests/utils/encoding_utils/encoding_utils_test.py` & `deep_utils-1.2.2/tests/utils/encoding_utils/encoding_utils_test.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/tests/utils/np_utils/np_utils_test.py` & `deep_utils-1.2.2/tests/utils/np_utils/np_utils_test.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/tests/utils/resize_utils/resize_utils_test.py` & `deep_utils-1.2.2/tests/utils/resize_utils/resize_utils_test.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/tests/vision/face_detection/mtcnn/torch/mtcnn_torch_test.py` & `deep_utils-1.2.2/tests/vision/face_detection/mtcnn/torch/mtcnn_torch_test.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/tests/vision/face_detection/ultralight/torch/ultralight_torch_test.py` & `deep_utils-1.2.2/tests/vision/face_detection/ultralight/torch/ultralight_torch_test.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/tests/vision/object_detection/yolo/v5/torch/yolov5_detection_test.py` & `deep_utils-1.2.2/tests/vision/object_detection/yolo/v5/torch/yolov5_detection_test.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.2.1/tests/vision/vision_utils/torch_vision_utils/torch_vision_utils_test.py` & `deep_utils-1.2.2/tests/vision/vision_utils/torch_vision_utils/torch_vision_utils_test.py`

 * *Files identical despite different names*

