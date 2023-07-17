# Comparing `tmp/iman-0.0.85.tar.gz` & `tmp/iman-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\iman-0.0.85.tar", last modified: Mon Jul 17 06:14:07 2023, max compression
+gzip compressed data, was "dist\iman-0.0.9.tar", last modified: Wed Oct 26 09:01:02 2022, max compression
```

## Comparing `iman-0.0.85.tar` & `iman-0.0.9.tar`

### file list

```diff
@@ -1,72 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 06:14:07.000000 iman-0.0.85/
--rw-rw-rw-   0        0        0     6595 2023-07-17 06:14:07.000000 iman-0.0.85/PKG-INFO
--rw-rw-rw-   0        0        0     6221 2023-07-17 06:13:47.000000 iman-0.0.85/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-17 06:14:07.000000 iman-0.0.85/iman/
--rw-rw-rw-   0        0        0     2070 2022-12-25 10:45:05.000000 iman-0.0.85/iman/AUG.py
--rw-rw-rw-   0        0        0    17314 2023-07-16 08:57:47.000000 iman-0.0.85/iman/Audio.py
--rw-rw-rw-   0        0        0      124 2023-01-29 08:15:58.000000 iman-0.0.85/iman/Boors.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:14:07.000000 iman-0.0.85/iman/Features/
--rw-rw-rw-   0        0        0       42 2022-11-13 07:01:23.000000 iman-0.0.85/iman/Features/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:14:07.000000 iman-0.0.85/iman/Features/mfcc/
--rw-rw-rw-   0        0        0     2836 2022-11-13 07:05:02.000000 iman-0.0.85/iman/Features/mfcc/LS.py
--rw-rw-rw-   0        0        0      604 2022-12-12 11:32:38.000000 iman-0.0.85/iman/Features/mfcc/SB.py
--rw-rw-rw-   0        0        0        0 2022-11-13 06:42:54.000000 iman-0.0.85/iman/Features/mfcc/__init__.py
--rw-rw-rw-   0        0        0    11080 2021-12-01 10:31:39.000000 iman-0.0.85/iman/Features/mfcc/getmfcc_from_librosa.py
--rw-rw-rw-   0        0        0    41655 2022-12-12 11:33:13.000000 iman-0.0.85/iman/Features/mfcc/sb_mfcc_class.py
--rw-rw-rw-   0        0        0     1057 2022-12-25 10:05:56.000000 iman-0.0.85/iman/Image.py
--rw-rw-rw-   0        0        0      815 2022-12-20 06:25:42.000000 iman-0.0.85/iman/Report.py
--rw-rw-rw-   0        0        0     2640 2023-02-20 05:13:55.000000 iman-0.0.85/iman/Text.py
--rw-rw-rw-   0        0        0     4391 2023-01-31 04:41:51.000000 iman-0.0.85/iman/__init__.py
--rw-rw-rw-   0        0        0      686 2022-12-17 11:18:42.000000 iman-0.0.85/iman/examples.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:14:07.000000 iman-0.0.85/iman/examples_folder/
--rw-rw-rw-   0        0        0        0 2022-12-17 11:24:05.000000 iman-0.0.85/iman/examples_folder/__init__.py
--rw-rw-rw-   0        0        0      539 2023-01-01 11:18:41.000000 iman-0.0.85/iman/examples_folder/age.py
--rw-rw-rw-   0        0        0      100 2023-01-01 05:01:21.000000 iman-0.0.85/iman/examples_folder/ffmpeg.py
--rw-rw-rw-   0        0        0      490 2022-12-17 09:55:52.000000 iman-0.0.85/iman/examples_folder/flask.py
--rw-rw-rw-   0        0        0      262 2021-01-05 11:07:03.000000 iman-0.0.85/iman/examples_folder/gpu_allocate_tf.py
--rw-rw-rw-   0        0        0      299 2022-12-31 09:42:30.000000 iman-0.0.85/iman/examples_folder/graphviz_chart.py
--rw-rw-rw-   0        0        0      345 2022-12-17 11:09:10.000000 iman-0.0.85/iman/examples_folder/parallel.py
--rw-rw-rw-   0        0        0      217 2022-12-17 11:12:20.000000 iman-0.0.85/iman/examples_folder/post_by_python.py
--rw-rw-rw-   0        0        0      775 2019-12-03 03:31:26.000000 iman-0.0.85/iman/examples_folder/pyworldd.py
--rw-rw-rw-   0        0        0      406 2022-12-05 05:24:04.000000 iman-0.0.85/iman/examples_folder/queue_worker.py
--rw-rw-rw-   0        0        0     1607 2021-11-28 10:10:27.000000 iman-0.0.85/iman/examples_folder/save_docx.py
--rw-rw-rw-   0        0        0      478 2019-05-05 06:27:38.000000 iman-0.0.85/iman/examples_folder/stft_test.py
--rw-rw-rw-   0        0        0      276 2019-11-19 00:37:16.000000 iman-0.0.85/iman/examples_folder/threading_example.py
--rw-rw-rw-   0        0        0      454 2021-05-25 08:55:10.000000 iman-0.0.85/iman/examples_folder/wikipedia.py
--rw-rw-rw-   0        0        0    15323 2022-11-06 10:39:16.000000 iman-0.0.85/iman/gpu_info.py
--rw-rw-rw-   0        0        0     1862 2022-11-12 05:34:50.000000 iman-0.0.85/iman/info.py
--rw-rw-rw-   0        0        0      318 2022-11-08 10:24:41.000000 iman-0.0.85/iman/matlab.py
--rw-rw-rw-   0        0        0     3422 2022-12-26 10:35:15.000000 iman-0.0.85/iman/metrics.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:14:07.000000 iman-0.0.85/iman/num2fa/
--rw-rw-rw-   0        0        0     8938 2023-01-28 05:46:54.000000 iman-0.0.85/iman/num2fa/__init__.py
--rw-rw-rw-   0        0        0      506 2023-01-28 05:46:54.000000 iman-0.0.85/iman/num2fa/__main__.py
--rw-rw-rw-   0        0        0      237 2022-12-19 06:23:20.000000 iman-0.0.85/iman/par.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:14:07.000000 iman-0.0.85/iman/sad_tf/
--rw-rw-rw-   0        0        0       92 2022-12-19 05:24:00.000000 iman-0.0.85/iman/sad_tf/__init__.py
--rw-rw-rw-   0        0        0     5614 2023-07-17 06:10:42.000000 iman-0.0.85/iman/sad_tf/export_funcs.py
--rw-rw-rw-   0        0        0     2221 2023-07-05 11:06:11.000000 iman-0.0.85/iman/sad_tf/features.py
--rw-rw-rw-   0        0        0    18763 2023-07-12 07:14:24.000000 iman-0.0.85/iman/sad_tf/segmenter.py
--rw-rw-rw-   0        0        0    13783 2022-11-30 10:00:38.000000 iman-0.0.85/iman/sad_tf/sidekit_mfcc.py
--rw-rw-rw-   0        0        0      553 2022-01-12 05:39:10.000000 iman-0.0.85/iman/sad_tf/thread_returning.py
--rw-rw-rw-   0        0        0     7808 2022-01-12 05:39:09.000000 iman-0.0.85/iman/sad_tf/viterbi.py
--rw-rw-rw-   0        0        0     1755 2022-01-12 05:39:10.000000 iman-0.0.85/iman/sad_tf/viterbi_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:14:07.000000 iman-0.0.85/iman/sad_torch_mfcc/
--rw-rw-rw-   0        0        0      107 2022-12-26 10:21:43.000000 iman-0.0.85/iman/sad_torch_mfcc/__init__.py
--rw-rw-rw-   0        0        0     4645 2022-12-11 08:33:44.000000 iman-0.0.85/iman/sad_torch_mfcc/export_funcs.py
--rw-rw-rw-   0        0        0     2002 2023-07-05 11:08:54.000000 iman-0.0.85/iman/sad_torch_mfcc/features.py
--rw-rw-rw-   0        0        0     3098 2022-12-11 08:39:59.000000 iman-0.0.85/iman/sad_torch_mfcc/sad_model.py
--rw-rw-rw-   0        0        0    19230 2023-07-05 11:15:27.000000 iman-0.0.85/iman/sad_torch_mfcc/segmenter.py
--rw-rw-rw-   0        0        0      553 2022-01-12 05:39:10.000000 iman-0.0.85/iman/sad_torch_mfcc/thread_returning.py
--rw-rw-rw-   0        0        0     7808 2022-01-12 05:39:09.000000 iman-0.0.85/iman/sad_torch_mfcc/viterbi.py
--rw-rw-rw-   0        0        0     1755 2022-01-12 05:39:10.000000 iman-0.0.85/iman/sad_torch_mfcc/viterbi_utils.py
--rw-rw-rw-   0        0        0      422 2022-11-22 05:36:39.000000 iman-0.0.85/iman/tsne.py
--rw-rw-rw-   0        0        0     2234 2023-06-10 12:42:19.000000 iman-0.0.85/iman/web.py
--rw-rw-rw-   0        0        0     7159 2022-10-26 09:16:54.000000 iman-0.0.85/iman/xvector.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:14:07.000000 iman-0.0.85/iman.egg-info/
--rw-rw-rw-   0        0        0     6595 2023-07-17 06:14:06.000000 iman-0.0.85/iman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1596 2023-07-17 06:14:06.000000 iman-0.0.85/iman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 06:14:06.000000 iman-0.0.85/iman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-07-17 06:14:06.000000 iman-0.0.85/iman.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-17 06:14:06.000000 iman-0.0.85/iman.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 06:14:07.000000 iman-0.0.85/setup.cfg
--rw-rw-rw-   0        0        0      903 2023-07-17 06:13:56.000000 iman-0.0.85/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-26 09:01:02.000000 iman-0.0.9/
+-rw-rw-rw-   0        0        0     1801 2022-10-26 09:01:02.000000 iman-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-10-26 09:01:02.000000 iman-0.0.9/iman/
+-rw-rw-rw-   0        0        0    11046 2022-10-25 11:17:35.000000 iman-0.0.9/iman/Audio.py
+-rw-rw-rw-   0        0        0     3963 2022-10-26 08:59:53.000000 iman-0.0.9/iman/__init__.py
+-rw-rw-rw-   0        0        0      843 2022-10-25 11:17:47.000000 iman-0.0.9/iman/info.py
+-rw-rw-rw-   0        0        0     2440 2022-10-26 08:38:23.000000 iman-0.0.9/iman/metrics.py
+-rw-rw-rw-   0        0        0      329 2022-10-25 11:18:01.000000 iman-0.0.9/iman/tsne.py
+-rw-rw-rw-   0        0        0     7143 2022-10-26 08:59:26.000000 iman-0.0.9/iman/xvector.py
+drwxrwxrwx   0        0        0        0 2022-10-26 09:01:02.000000 iman-0.0.9/iman.egg-info/
+-rw-rw-rw-   0        0        0     1801 2022-10-26 09:01:02.000000 iman-0.0.9/iman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2022-10-26 09:01:02.000000 iman-0.0.9/iman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-26 09:01:02.000000 iman-0.0.9/iman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2022-10-26 09:01:02.000000 iman-0.0.9/iman.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2022-10-26 09:01:02.000000 iman-0.0.9/iman.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-10-26 09:01:02.000000 iman-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2204 2022-10-26 09:00:03.000000 iman-0.0.9/setup.py
```

### Comparing `iman-0.0.85/iman/Audio.py` & `iman-0.0.9/iman/Audio.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 import numpy as np
 from scipy import signal
 import os
 import scipy.io.wavfile as wave
 from numpy.lib.stride_tricks import as_strided
 import six
-import subprocess
-import platform
-from iman import *
-
-_system = platform.system().lower()
 
 
 ALawDecompressTable =[
 
      -5504, -5248, -6016, -5760, -4480, -4224, -4992, -4736,
 
      -7552, -7296, -8064, -7808, -6528, -6272, -7040, -6784,
@@ -73,40 +68,19 @@
 
       1888,  1824,  2016,  1952,  1632,  1568,  1760,  1696,
 
       688,   656,   752,   720,   560,   528,   624,   592,
 
       944,   912,  1008,   976,   816,   784,   880,   848]
 
-def Read_Alaw_1(filename):
+def Read_Alaw(filename):
     with open(filename, "rb") as binaryfile :
        myArr = bytearray(binaryfile.read())
     g=[ALawDecompressTable[x]/32768 for x in myArr]
     return np.array(g , dtype=np.float32)
-    
-    
-def Read_Alaw(filename,sr=8000,ffmpeg_path='c:\\ffmpeg.exe'):
-
-           ffmpeg_command = [ffmpeg_path, "-ar","8000", "-f" ,"alaw" ,'-i', filename, '-ac', "1", '-ar', str(sr), '-f', 'wav', 'pipe:1']
-
-           
-           pipe = subprocess.run(ffmpeg_command, stdout=subprocess.PIPE,   stderr=subprocess.PIPE,  bufsize=10**8)
-           
-           audio_np = np.frombuffer(buffer=pipe.stdout, dtype=np.uint16, offset=8*44)
-             
-           x =np.where(audio_np>32768)    [0]    
-           y =np.where(audio_np<=32768)    [0]  
-           
-           out_wav = np.zeros(len(audio_np) , dtype=np.float32)
-           out_wav[x] = (audio_np[x] - 32768)/32768-1
-           out_wav[y] = audio_np[y] /32768
-           
-          
-           return(out_wav) 
-       
 
 def Resample(data , fs, sr):
     """Return Resampled Data.
 
     Parameters
     ----------
     data : input audio data
@@ -121,25 +95,77 @@
     if (fs!=sr):
         nesbat = sr/fs
         m = np.max(np.abs(data))
         data = 0.5*(data/(m+1e-6))
         data = signal.resample(data, int(len(data)*nesbat))
     return (np.array(data , dtype=np.float32))    
 
-def ReadMp3_miniaudio(filename,sr,mono=True):
+def Read(filename,sr):   # output sampling rate is sr
+   """Return Audio Data. (Just Mono Files)
+
+    Parameters
+    ----------
+    filename : input file path (PCM or alaw or [alaw_raw with .l or .r ext])
+    sr : desired sampling rate
+    
+    Output
+    ----------
+    data with sampling rate --> sr
+
+   """   
+   ext = os.path.basename(filename).split('.')[-1] 
+   if (ext.lower() == 'l' or ext.lower() == 'r' ):
+       return( Resample( Read_Alaw(filename) , 8000, sr) )
+   
+   File_Type_Header= np.fromfile(filename, dtype=np.byte, count=4, offset=8)
+   File_Type_Header = "".join(map(chr, File_Type_Header))   # Must be WAVE
+   if (File_Type_Header!="WAVE"):
+       return("no_wav")
+   Type_of_format = np.fromfile(filename, dtype=np.int8, count=1, offset=20)[0]  # 1 is PCM   6 is alaw
+
+   ch = np.fromfile(filename, dtype=np.int8, count=1, offset=22)[0]  
+   
+   if (ch!=1):
+       return("sterio file")
+   
+   fs = np.fromfile(filename, dtype=np.int32, count=1, offset=24)[0] # Hz
+   
+   if (Type_of_format!=1 and Type_of_format!=6 ):
+       return ("no_pcm_alaw")
+   
+   if (Type_of_format==6):   # if file is alaw
+        byte_length = np.fromfile(filename, dtype=np.int32, count=1, offset=40)[0]
+        data = np.fromfile(filename, dtype=np.byte, count=byte_length*4, offset=44)
+        data=np.array([ALawDecompressTable[x]/32768 for x in data], dtype=np.float32)
+        return (Resample(data,fs,sr))
+   
+   chunk_header = np.fromfile(filename, dtype=np.byte, count=4, offset=36)
+   chunk_header = "".join(map(chr, chunk_header))
+   if (chunk_header=="LIST"):
+     import librosa
+     data,_ = librosa.load(filename,sr)
+   elif(chunk_header=="data"):
+      byte_length = np.fromfile(filename, dtype=np.int32, count=1, offset=40)[0]
+      data = np.fromfile(filename, dtype=np.int16, count=byte_length // 2, offset=44)/32768
+      data = Resample(data,fs,sr)
+   else:
+       return ("Unknown chunk_header-->" + chunk_header)
+   return (data)
+
+def ReadMp3(filename,sr,mono=True):
     import miniaudio
     mp3file = miniaudio.read_file(filename,True)
     sample_rate = mp3file.sample_rate
     data =  np.array(mp3file.samples , dtype=np.float32)/32768
     if (mp3file.nchannels==1):
        if (sample_rate!=sr):
             data = Resample(data ,sample_rate ,sr )
     else:
-         ch1=np.array( data[::2] , dtype=np.float32)
-         ch2=np.array(data[1::2], dtype=np.float32)
+         ch1=np.array( [ data[i] for i in range(0,len(data),2)  ] , dtype=np.float32)
+         ch2=np.array([ data[i] for i in range(1,len(data),2)  ], dtype=np.float32)
          if (mono):
            cha = ch1+ch2
          if (sample_rate!=sr):
                 if (mono):
                   cha = Resample(cha ,sample_rate ,sr )
                 else:  
                    ch1 = Resample(ch1 ,sample_rate ,sr )
@@ -147,104 +173,14 @@
          if (mono):          
            data = cha
          else:
            data=  [ch1,ch2]       
     return(data)
 
 
-def ReadMp3(filename,sr=16000,mono=True,ffmpeg_path='c:\\ffmpeg.exe'):
-     chnum=2
-     if (mono):
-        chnum=1
-     
-     if (True):      
-           
-           ffmpeg_command = [ffmpeg_path, '-i', filename, '-ac', str(chnum), '-ar', str(sr), '-f', 'wav', 'pipe:1']
-           
-           pipe = subprocess.run(ffmpeg_command, stdout=subprocess.PIPE,   stderr=subprocess.PIPE,  bufsize=10**8)
-           
-           audio_np = np.frombuffer(buffer=pipe.stdout, dtype=np.uint16, offset=8*44)
-             
-           x =np.where(audio_np>32768)    [0]    
-           y =np.where(audio_np<=32768)    [0]  
-           
-           out_wav = np.zeros(len(audio_np) , dtype=np.float32)
-           out_wav[x] = (audio_np[x] - 32768)/32768-1
-           out_wav[y] = audio_np[y] /32768
-           
-           if (mono):
-              return(out_wav) 
-           else:
-              ch1 = out_wav[::2]
-              ch2=out_wav[1::2]
-              return(ch1,ch2)
-      
-
-def Read(filename,sr=8000,ffmpeg_path='c:\\ffmpeg.exe'):   # output sampling rate is sr
-   """Return Audio Data. (Just Mono Files)
-
-    Parameters
-    ----------
-    filename : input file path (PCM or alaw or [alaw_raw with .l or .r ext] or mp3)
-    sr : desired sampling rate
-    
-    Output
-    ----------
-    data with sampling rate --> sr
-
-   """   
-   ext = os.path.basename(filename).split('.')[-1] 
-   if (ext.lower() == 'l' or ext.lower() == 'r' or os.path.basename(filename).lower().endswith('.r.wav') or os.path.basename(filename).lower().endswith('.l.wav') or os.path.basename(filename).lower().endswith('.rtemp.wav') or os.path.basename(filename).lower().endswith('.ltemp.wav')):
-         return( Read_Alaw(filename,sr=sr ,ffmpeg_path=ffmpeg_path ))
-       
-  
-   return(ReadMp3(filename,sr=sr, mono=True,ffmpeg_path=ffmpeg_path))
-    
-   
-   
-   # if (ext.lower() == 'mp3'):
-         # return(ReadMp3(filename,sr=sr, mono=True,ffmpeg_path=ffmpeg_path))
-   
-   # File_Type_Header= np.fromfile(filename, dtype=np.byte, count=4, offset=8)
-   # File_Type_Header = "".join(map(chr, File_Type_Header))   # Must be WAVE
-   # if (File_Type_Header!="WAVE"):
-       # return(ReadMp3(filename,sr=sr, mono=True,ffmpeg_path=ffmpeg_path))
-       
-   # Type_of_format = np.fromfile(filename, dtype=np.int8, count=1, offset=20)[0]  # 1 is PCM   6 is alaw
-
-   # ch = np.fromfile(filename, dtype=np.int8, count=1, offset=22)[0]  
-   
-   # if (ch!=1):
-       # return(ReadMp3(filename,sr=sr, mono=True,ffmpeg_path=ffmpeg_path))
-   
-   # fs = np.fromfile(filename, dtype=np.int32, count=1, offset=24)[0] # Hz
-   
-   # if (Type_of_format!=1 and Type_of_format!=6 ):
-       # return(ReadMp3(filename,sr=sr, mono=True,ffmpeg_path=ffmpeg_path))
-   
-   # if (Type_of_format==6):   # if file is alaw
-        # byte_length = np.fromfile(filename, dtype=np.int32, count=1, offset=40)[0]
-        # data = np.fromfile(filename, dtype=np.byte, count=byte_length*4, offset=44)
-        # data=np.array([ALawDecompressTable[x]/32768 for x in data], dtype=np.float32)
-        # return (Resample(data,fs,sr))
-   
-   # chunk_header = np.fromfile(filename, dtype=np.byte, count=4, offset=36)
-   # chunk_header = "".join(map(chr, chunk_header))
-   # if (chunk_header!="data"):
-     # if (_system == 'windows'):
-      # data=ReadMp3(filename,sr=sr, mono=True,ffmpeg_path=ffmpeg_path)
-     # else:
-      # import librosa
-      # data,_ = librosa.load(filename , sr)      
-   # elif(chunk_header=="data"):
-      # byte_length = np.fromfile(filename, dtype=np.int32, count=1, offset=40)[0]
-      # data = np.fromfile(filename, dtype=np.int16, count=byte_length // 2, offset=44)/32768
-      # data = Resample(data,fs,sr)
-   # return (data)
-
 def Write(filename, data ,fs):
 
    """Write Audio Data.
 
     Parameters
     ----------
     filename : Output file path (.wav)
@@ -253,33 +189,15 @@
     
     Output
     ----------
     Nothing
 
    """
    wave.write(filename, fs, np.int16(data*32768))
-   
-def WriteS(filename, data ,fs):
-
-   """Write Audio Data Sterio.
-
-    Parameters
-    ----------
-    filename : Output file path (.wav)
-    data : Audio data
-    fs : sampling rate
-    
-    Output
-    ----------
-    Nothing
-
-   """
-   xx = np.asarray( [np.int16(data*32768) , np.int16(data*32768)]).transpose()
 
-   wave.write(filename, fs, xx)
 def rmse(y=None, S=None, frame_length=2048, hop_length=512,
          center=True, pad_mode='reflect'):
     
     if y is not None and S is not None:
         raise ValueError('Either `y` or `S` should be input.')
     if y is not None:
         y = (y)
@@ -373,14 +291,17 @@
 
     non_silent = _signal_to_frame_nonsilent(y,
                                             frame_length=frame_length,
                                             hop_length=hop_length,
                                             ref=ref,
                                             top_db=top_db)
 
+    # Interval slicing, adapted from
+    # https://stackoverflow.com/questions/2619413/efficiently-finding-the-interval-with-non-zeros-in-scipy-numpy-in-python
+    # Find points where the sign flips
     edges = np.flatnonzero(np.diff(non_silent.astype(int)))
 
     # Pad back the sample lost in the diff
     edges = [edges + 1]
 
     # If the first frame had high energy, count it
     if non_silent[0]:
@@ -395,146 +316,16 @@
                                    hop_length=hop_length)
 
     # Clip to the signal duration
     edges = np.minimum(edges, y.shape[-1])
 
     # Stack the results back as an ndarray
     return edges.reshape((-1, 2))
-    
 def frames_to_samples(frames, hop_length=512, n_fft=None):
- 
+  
+
     offset = 0
     if n_fft is not None:
         offset = int(n_fft // 2)
 
     return (np.asanyarray(frames) * hop_length + offset).astype(int)
-    
-def ReadT(filename, sr=8000 , mono=True): 
-    import torchaudio
-    
-    wavs, fs = torchaudio.load(filename)
-    
-    if (fs!=sr):
-       import torchaudio.transforms as T  
-       resampler = T.Resample(fs, sr, dtype=wavs.dtype)
-       wavs  = resampler(wavs)
-    
-    if (len(wavs)==2 and mono==True):
-        return ( (wavs[0] +wavs[1]).unsqueeze(0))
-        
-    return wavs
-    
-def VAD(wav,top_db=40, frame_length=200, hop_length=80):
-    a = split(wav,top_db=top_db, frame_length=frame_length, hop_length=hop_length)
-    v_wav=[]
-    for x in a:
-        v_wav.append(wav[x[0]:x[1]])
-    v = np.concatenate(v_wav)
-    return(v)       
-    
-def change_format(fname , sr=16000 , ext='mp3' , mono=True ,ffmpeg_path='c:\\ffmpeg.exe' ,oname=None ):
-    chnum=2
-    if (mono):
-      chnum=1
-      
-    forext = []
-    if (PE(fname).lower()=='.l' or PE(fname).lower()=='.r') :
-         forext = ['-ar', '8000', '-f' ,'alaw']    
-      
-      
-    if (not ext.startswith('.')):
-       ext = '.' + ext    
-
-    if (oname==None):
-       outfile =  PJ(PD(fname) , PN(fname)+ ext)
-    else:
-      if ('.' in oname):
-        outfile =  oname
-      else:
-        outfile =  oname + ext
-    
-    if (PX(outfile)):
-       print('File Exists--> ' + PB(outfile))
-       return 0
-       
-    try:
-    
-      if (forext==[]):
-         ffmpeg_command = [ffmpeg_path, '-i', fname, '-ac', str(chnum), '-ar', str(sr), 'outfile']
-      else:
-          ffmpeg_command = [ffmpeg_path]
-          ffmpeg_command.extend(forext)
-          ffmpeg_command.extend(['-i', fname, '-ac', str(chnum), '-ar', str(sr), 'outfile'])
-
-      x = cmd(ffmpeg_command )
-      if (PX(outfile) and PS(outfile)>1):
-         return 1
-      else:
-          try:
-             os.remove(outfile)
-          except:
-             pass 
-          return 0             
-          
-    except:
-      print('ffmpeg has Problem with --> ' + PB(outfile)) 
-      try:
-         os.remove(outfile)
-      except:
-         pass
-      
-      return 0
- 
-
-def fun(fname , b):
-   change_format(fname , sr=b[0] , ext=b[1] , mono=b[2] , ffmpeg_path=b[3] , oname=PJ(b[4] , PN(fname) + b[1] ) )
- 
-def compress (fname_pattern , sr=16000 , ext='mp3' , mono=True ,ffmpeg_path='c:\\ffmpeg.exe' , ofolder=None , worker=4): 
-    
-    if (not ext.startswith('.')):
-       ext = '.' + ext    
-       
-    files = gf(fname_pattern) 
-    
-    
-    if (len(files)==0):
-        print('no File!!!')
-        return
-    
-   
-    if (ofolder==None):
-        pp = input('It is better to set ofolder\n press y to continue compression: ')
-        if (pp.lower()=='y'):
-          ofolder=""
-        else:
-           return        
-    else:
-       PM(ofolder)
-    
-    worker=min(len(files) , worker)     
-
-    from multiprocessing import Pool
-    from functools import partial  
-    with Pool(processes=worker) as pool:
-         pool.map(partial(fun, b=[sr , ext,mono , ffmpeg_path,ofolder]), files)     
-
-
-
-def clip_value(wav):
 
-    # wav must be output of sad
-    wav = abs( wav / abs(wav).max())
-
-    cli= np.where(wav>=0.99)[0]
-    cli1 = np.insert(np.delete(cli-1 ,0) , len(cli)-1,0)
-    cli2=np.delete(np.insert(cli+1,0,0) , len(cli))   
-    
-    a=(cli == cli1 ) 
-    b=(cli == cli2)
-    c = np.logical_or(a, b)
-    
-    x = len(np.where(c==True)[0])
-        
-    clip_percentage = 100*x / len(wav)
-    return (clip_percentage)         
-    
-
```

### Comparing `iman-0.0.85/iman/__init__.py` & `iman-0.0.9/iman/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,16 @@
 import matplotlib.pyplot as plt
 import time
 from glob import glob as gf
 import os
 import numpy as np
-from joblib import load,dump
 
 def help():
-    from iman import web
-    x=web.dl(r'https://pypi.org/project/iman/')
-    idx = x.index('class="project-description"')
-    idy = x.index('</div>' , idx+1)
-    y= (x[idx+29:idy].strip().replace('<span class="docutils literal">','<').replace('</span>','>').replace('</section>','').replace('<h2>','').replace('</h2>','').replace('<p>','').replace('</p>','').replace('<section id=from-iman-import>',''))
-    
+   print('from iman import Audio:\n1-Read(filename,sr)\n2-Resample(data , fs, sr)\n3-Read_Alaw(filename)\n4-ReadMp3(filename,sr,mono=True)\n5-Write(filename, data ,fs)\n6-frame(y)\n7-split(y)\n\nfrom iman import *:\n1-plt\n2-now() (get time)\n3-F (format floating point)\n4-D (format int number)\n5-Write_List(MyList,Filename)\n6-Write_Dic(MyDic,Filename)\n7-Read(Filename) (read txt file)\n8-Read_Lines(Filename) (read txt file line by line and return list)\n9-Write(_str,Filename)\n10-gf(pattern) (Get files in a directory)\n11-gfa(directory , ext="*.*") (Get Files in a Directory and SubDirectories)\n12-ReadE(Filename) (Read Excel files)\n13-PM(dir)(creat directory)\n14-PB(fname)(get basename)\n15-PN(fname) (get file name)\n16-PE(fname)(get ext)\n17-PD(fname)(get directory)\n18-PS(fname)(get size)\n19-PJ(segments) (Join Path)\n20-clear() (clear cmd)\n21-os\n22-np\n23-RI(start_int , end_int , count=1) (random int)\n24-RF(start_float , end_float , count=1) (random float)\n25-RS(Arr) (shuffle)\n\nfrom iman import info:\n1-get() info about cpu and gpu (need torch)\n\n\nfrom iman import metrics:\n1-EER(lab,score)\n2-cosine_distance(v1,v2)\n3-roc(lab,score)\n4-wer(ref, hyp)\n5-cer(ref, hyp)\n6-wer_list(ref_list , hyp_list)\n7-cer_list(ref_list , hyp_list)\n\nfrom iman import tsne:\n1-plot(fea , label)\n\nfrom iman import xvector:\n1-xvec,lda_xvec,gender = get(filename , model(model_path , model_name , model_speaker_num))\n\n')
 
-    while(True):
-       try:
-        idx=0
-        idx = y.index('<section',idx+1)
-
-        idy = y.index('>' , idx+1)
-
-        y = y.replace(y[idx:idy+1] , '')
-       except:
-         break       
-    print(y)
    
 def clear():
     if os.name == 'nt':
         _ = os.system('cls')  
     else:
         _ = os.system('clear')
         
@@ -61,23 +44,20 @@
          return(fid.read())
 
 def Read_Lines(Filename):
     with open(Filename , 'r' , encoding='utf-8') as fid:
          return([x.strip() for x in fid if (x.strip()!="")])    
 
 def gfa(directory , ext="*.*"):
- fols = gf(directory)
- a=[]
- for _fol in fols: 
-   [a.append(x) for x in gf(os.path.join(_fol , ext))]
-   for root, dirs, files in os.walk(_fol):
+   a=[]
+   for root, dirs, files in os.walk(directory):
       for dirname in dirs:
-         _dir =os.path.join(root, dirname)         
-         [a.append(x) for x in gf(os.path.join(_dir , ext))]           
- return a         
+         _dir =os.path.join(root, dirname)  
+         [a.append(x) for x in gf(os.path.join(_dir , ext))]   
+   return a         
 
 def ReadE(Filename):
     import pandas as pd
     pp = pd.read_excel(Filename , engine='openpyxl')
     return pp
     
 def PB(filename):
@@ -89,18 +69,15 @@
 def PM(folname):
    return os.makedirs(folname , exist_ok=True)
        
 def PN(filename):
    return os.path.basename(os.path.splitext(filename)[0])  
 
 def PE(filename):
-   return os.path.splitext(filename)[1]   
-
-def PX(filename):
-   return os.path.exists(filename)    
+   return os.path.splitext(filename)[1]    
    
 def PJ(*_segments):
    x=""
    for p in _segments:
       x = os.path.join(x,p)
    return x   
    
@@ -111,49 +88,8 @@
    return np.random.randint(low=int(start_int), high=int(end_int), size=(count,))
    
 def RF(start_float , end_float , count=1):
   return np.random.uniform(start_float, end_float , count)
   
 def RS(Arr):
   np.random.shuffle(Arr)
-  return Arr
-  
-def RC(Arr , _size=1):
-   return np.random.choice(Arr , _size)
-
-
-def LJ(job_file_name):
-   return load(job_file_name)
-   
-def SJ(value , job_file_name):
-   dump(value , job_file_name)   
-   
-def LN(np_file_name):
-   return np.load(np_file_name) 
-   
-def SN(arr , np_file_name):
-   return np.save(np_file_name , arr)   
-   
-def cmd(command , redirect=True):
-  if (redirect):
-   return os.popen(command).read()   
-  else:
-    os.system(command)  
-    
-    
-def onehot(data, nb_classes):
-    """Convert an iterable of indices to one-hot encoded labels."""
-    targets = np.array(data).reshape(-1)
-    return np.eye(nb_classes)[targets]
-    
-    
-def exe(fname):
-    cmd('pyinstaller --onefile ' + fname , False)    
-    
-def FWL(wavfolder , sr): #Get Audio Lenth Exist in this folder    
-    files=gfa(wavfolder , '*.wav')
-    n=0
-    for filename in files:
-         n=n+PS(filename)
-    header=len(files)*44       
-    print((n-header)/(sr*2*60*60))
-    return  ((n-header)/(sr*2*60*60))       
+  return Arr
```

### Comparing `iman-0.0.85/iman/metrics.py` & `iman-0.0.9/iman/metrics.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import numpy as np
 from sklearn.metrics import roc_curve as rc
 from iman import *
 import Levenshtein as Lev
-import scipy.spatial as sp
 
 
 def help():
    print('\nneed <Levenshtein> and <sklearn>\n')
 
 
 def cosine_distance(v1,v2):
-  return sp.distance.cdist(v1, v2, 'cosine')
-  
+  dot_product = np.dot(v1, v2)
+  norm_a = np.linalg.norm(v1)
+  norm_b = np.linalg.norm(v2)
+  return dot_product / (norm_a * norm_b)
 
 def compute_eer(fpr,tpr,thresholds):
     fnr = 1-tpr
     abs_diffs = np.abs(fpr - fnr)
     min_index = np.argmin(abs_diffs)
     eer = np.mean((fpr[min_index], fnr[min_index]))
     return eer, thresholds[min_index]  ,min_index
@@ -69,51 +70,8 @@
        x.append(wer(ref_list[i] , hyp_list[i]))
     return np.mean(x)   
     
 def cer_list(ref_list , hyp_list):
     x=[]
     for i in range(len(ref_list)):
        x.append(cer(ref_list[i] , hyp_list[i]))
-    return np.mean(x)    
-    
-    
-def DER(ref_list , res_list , file_dur=-1 , sr=8000):
-    """ input--> [ [st1,en1] , [st2 , en2] , ....   ]
-        just for speech parts
-        Output--> Miss , FA , DER , miss_points, fa_points
-    """        
-    
-    if (file_dur==-1):
-        file_dur = max(ref_list[-1][1] , res_list[-1][1])
-    
-    ref = np.zeros((int(file_dur*sr)))
-    
-    for a,b in ref_list:
-        ref[int(sr * a) : int(sr*b)]=1
-              
-    res = np.zeros((int(file_dur*sr)))
-    
-    for a,b in res_list:
-        res[int(sr * a) : int(sr*b)]=1
-     
-    
-    _miss_points=[]
-    _y=np.where(ref==1)[0] 
-    for i in _y:
-        if (res[i]==0):
-            _miss_points.append(i)
-    x = len(_miss_points)
-    miss = x / file_dur 
-    
-
-    _fa_points=[]
-    _y=np.where(res==1)[0] 
-    for i in _y:
-        if (ref[i]==0):
-            _fa_points.append(i)
-    x1 = len(_fa_points)
-    fa = x1 / file_dur 
-    
-    _der =(x+x1)/file_dur
-    
-
-    return (miss , fa ,_der ,_miss_points,_fa_points)
+    return np.mean(x)
```

### Comparing `iman-0.0.85/iman/xvector.py` & `iman-0.0.9/iman/xvector.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,21 +193,21 @@
 def get_xvec(feat, modelxvec ,batch_size):
  
   xvec,gender = modelxvec.predict(feat, batch_size = batch_size,verbose=1,use_multiprocessing=True)
   return xvec,gender
 
 
 def model(model_path , model_name , model_speaker_num):
-    return [get_model(model_path , model_name , model_speaker_num) , model_path]
+    return get_model(model_path , model_name , model_speaker_num)
 
 def get(filename , _model):
    sample_rate=8000
    data =Audio.Read(filename , sample_rate)
    fea = get_fea_file(data , sample_rate)
-   xvec, a = get_xvec(np.reshape(fea , (1 , np.shape(fea)[0], np.shape(fea)[1])), _model[0], batch_size=1)
-   xvec_lda = apply_lda(xvec, PJ(_model[1], 'meanvec.npy'), PJ(_model[1], 'lda.job'))
+   xvec, a = get_xvec(np.reshape(fea , (1 , np.shape(fea)[0], np.shape(fea)[1])), _model, batch_size=1)
+   xvec_lda = apply_lda(xvec, PJ(model_path, 'meanvec.npy'), PJ(model_path, 'lda.job'))
    gender='male'
    if (a[0][0]>=a[0][1]):
        gender='female'
    return(np.squeeze(xvec),np.squeeze(xvec_lda),gender)
```

