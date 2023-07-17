# Comparing `tmp/pegasusX-0.2.1.tar.gz` & `tmp/pegasusX-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pegasusX-0.2.1.tar", last modified: Mon Jul 17 14:08:55 2023, max compression
+gzip compressed data, was "pegasusX-0.2.2.tar", last modified: Mon Jul 17 14:21:44 2023, max compression
```

## Comparing `pegasusX-0.2.1.tar` & `pegasusX-0.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:08:55.578324 pegasusX-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 14:08:43.000000 pegasusX-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 14:08:55.578324 pegasusX-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-17 14:08:43.000000 pegasusX-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:08:55.574324 pegasusX-0.2.1/pegasus/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 14:08:43.000000 pegasusX-0.2.1/pegasus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-17 14:08:43.000000 pegasusX-0.2.1/pegasus/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:08:55.574324 pegasusX-0.2.1/pegasus/oceandb/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-17 14:08:43.000000 pegasusX-0.2.1/pegasus/oceandb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:08:55.574324 pegasusX-0.2.1/pegasus/oceandb/api/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 14:08:43.000000 pegasusX-0.2.1/pegasus/oceandb/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-07-17 14:08:43.000000 pegasusX-0.2.1/pegasus/oceandb/api/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-17 14:08:43.000000 pegasusX-0.2.1/pegasus/oceandb/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 14:08:43.000000 pegasusX-0.2.1/pegasus/oceandb/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:08:55.574324 pegasusX-0.2.1/pegasus/oceandb/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:08:43.000000 pegasusX-0.2.1/pegasus/oceandb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-17 14:08:43.000000 pegasusX-0.2.1/pegasus/oceandb/utils/embedding_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:08:55.578324 pegasusX-0.2.1/pegasusX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 14:08:55.000000 pegasusX-0.2.1/pegasusX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-17 14:08:55.000000 pegasusX-0.2.1/pegasusX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:08:55.000000 pegasusX-0.2.1/pegasusX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 14:08:55.000000 pegasusX-0.2.1/pegasusX.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 14:08:55.000000 pegasusX-0.2.1/pegasusX.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 14:08:55.578324 pegasusX-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-17 14:08:43.000000 pegasusX-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:21:44.259887 pegasusX-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 14:21:33.000000 pegasusX-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 14:21:44.259887 pegasusX-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-07-17 14:21:33.000000 pegasusX-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:21:44.259887 pegasusX-0.2.2/pegasus/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 14:21:33.000000 pegasusX-0.2.2/pegasus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-17 14:21:33.000000 pegasusX-0.2.2/pegasus/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:21:44.259887 pegasusX-0.2.2/pegasus/oceandb/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-17 14:21:33.000000 pegasusX-0.2.2/pegasus/oceandb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:21:44.259887 pegasusX-0.2.2/pegasus/oceandb/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 14:21:33.000000 pegasusX-0.2.2/pegasus/oceandb/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-07-17 14:21:33.000000 pegasusX-0.2.2/pegasus/oceandb/api/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-17 14:21:33.000000 pegasusX-0.2.2/pegasus/oceandb/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-17 14:21:33.000000 pegasusX-0.2.2/pegasus/oceandb/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:21:44.259887 pegasusX-0.2.2/pegasus/oceandb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:21:33.000000 pegasusX-0.2.2/pegasus/oceandb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-17 14:21:33.000000 pegasusX-0.2.2/pegasus/oceandb/utils/embedding_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:21:44.259887 pegasusX-0.2.2/pegasusX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 14:21:44.000000 pegasusX-0.2.2/pegasusX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-17 14:21:44.000000 pegasusX-0.2.2/pegasusX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:21:44.000000 pegasusX-0.2.2/pegasusX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 14:21:44.000000 pegasusX-0.2.2/pegasusX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 14:21:44.000000 pegasusX-0.2.2/pegasusX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 14:21:44.259887 pegasusX-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-17 14:21:33.000000 pegasusX-0.2.2/setup.py
```

### Comparing `pegasusX-0.2.1/LICENSE` & `pegasusX-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.1/PKG-INFO` & `pegasusX-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.2.1
+Version: 0.2.2
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.2.1/README.md` & `pegasusX-0.2.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,120 +1,108 @@
-# Pegasus: A State-of-the-Art Multimodal Embedding Model
+# PegasusX: The Future of Multimodal Embeddings 🦄 🦄 
 
 ![Pegasus Banner](./assets/banner.png)
 
-Welcome to Pegasus, the latest and most advanced model for creating high-quality embeddings from multimodal data. We're pushing the boundaries of what's possible with machine learning, enabling tasks and applications that were once mere visions of the future.
+Welcome to PegasusX, the latest and most advanced package for creating high-quality embeddings from multimodal data. We're pushing the boundaries of what's possible with machine learning, enabling tasks and applications that were once mere visions of the future.
 
-In essence, Pegasus is designed to transform the way we look at data. Our aim is to make it easier for anyone, regardless of their domain or discipline, to generate task-specific, high-quality embeddings from any type of data, be it text, image, video, audio, or even more complex data types.
+In essence, PegasusX is designed to transform the way we look at data. Our aim is to make it easier for anyone, regardless of their domain or discipline, to generate task-specific, high-quality embeddings from any type of data, be it text, image, video, audio, or even more complex data types.
 
-## The Vision
+## Installation
+```bash
+pip install pegasusx
+```
 
-When we began crafting Pegasus, we asked ourselves a fundamental question: What if an algorithm could see and understand all the modalities of data the same way we do, and even beyond?
+## Usage
 
-The answer lies in Pegasus. Powered by a unique blend of artificial intelligence and machine learning, Pegasus is capable of parsing and comprehending multi-modal data types, generating valuable insights in the process.
+```python
+from pegasus import Pegasus
 
-Much like the mythical creature it's named after, Pegasus is all about bridging worlds - in our case, the world of raw, multi-modal data and the world of actionable, contextualized information.
+# for video, audio do "Pegasus('vision'), Pegasus("audio") respectively then pass in the file path of the vision or audio data
+pegasus = Pegasus("text", multi_process=False, n_processes=4)
 
-## The Features
+text_data = ['This is a query about artificial intelligence',
+             'Another query about machine learning',
+             'Yet another query about deep learning',
+             'And one more about natural language processing']
 
-Pegasus is not just another run-of-the-mill machine learning model. We've painstakingly crafted this framework, ensuring it includes features that set it apart:
+embeddings = pegasus.embed_data(text_data)
 
-1. **Multimodal Data Understanding:** From text to images, audio, and more, Pegasus is designed to handle and understand a wide array of data types.
+print(embeddings)
+```
 
-2. **Personalized for Any Task:** Pegasus adapts to your specific task, generating high-quality, task-specific embeddings for a wide variety of applications.
+## Features
 
-3. **Scalability & Performance:** Pegasus has been optimized for efficiency and can scale according to the demands of your tasks, ensuring seamless operation even with large amounts of data.
+PegasusX is not just another run-of-the-mill machine learning package. We've painstakingly crafted this package, ensuring it includes features that set it apart:
 
-4. **Open Source:** We believe in the power of community and collaboration. Pegasus is an open-source project, welcoming contributions and improvements from the global developer community.
+1. **Multimodal Data Understanding:** From text to images, audio, and more, PegasusX is designed to handle and understand a wide array of data types.
 
-## Get Involved
+2. **Personalized for Any Task:** PegasusX adapts to your specific task, generating high-quality, task-specific embeddings for a wide variety of applications.
 
-We're just at the beginning of our journey. As we continue to develop and refine Pegasus, we invite you to join us. Whether you're a developer, researcher, or simply an enthusiast, your insights and contributions can help shape the future of Pegasus.
+3. **Scalability & Performance:** PegasusX has been optimized for efficiency and can scale according to the demands of your tasks, ensuring seamless operation even with large amounts of data.
 
-# Contributing to Pegasus
+4. **Open Source:** We believe in the power of community and collaboration. PegasusX is an open-source project, welcoming contributions and improvements from the global developer community.
 
-We are thrilled to invite you to be a part of the Pegasus project. This is not just an open source project but a community initiative, and we value your expertise and creativity. To show our appreciation, we have instituted a unique rewards system that directly compensates contributors from the revenue generated by the Pegasus API.
+## Contributing to PegasusX
 
-## Why Contribute
+We are thrilled to invite you to be a part of the PegasusX project. This is not just an open source project but a community initiative, and we value your expertise and creativity. To show our appreciation, we have instituted a unique rewards system that directly compensates contributors from the revenue generated by the PegasusX API.
 
-Contributing to Pegasus not only enhances your skills and profile but also comes with financial rewards. When you contribute code, documentation, or any form of improvement to the Pegasus project, you are adding value. As such, we believe it's only fair that you share in the rewards.
+### Why Contribute
 
-## Rewards Program
+Contributing to PegasusX not only enhances your skills and profile but also comes with financial rewards. When you contribute code, documentation, or any form of improvement to the PegasusX project, you are adding value. As such, we believe it's only fair that you share in the rewards.
 
-Here's how the Pegasus Rewards Program works:
+### Rewards Program
+
+Here's how the PegasusX Rewards Program works:
 
 1. **Submit a Pull Request:** This can be a code enhancement, bug fix, documentation update, new feature, or any improvement to the project.
 
 2. **Review and Approval:** Our team will review your contribution. If it gets approved and merged, you become eligible for the rewards program.
 
-3. **Revenue Share:** Once your pull request is merged, you will receive a percentage of the revenue generated by the Pegasus API. The percentage will be determined based on the significance and impact of your contribution. 
-
-This means you're not just contributing to an open source project; you're becoming a part of the Pegasus ecosystem. Your efforts can yield ongoing benefits as the Pegasus API grows and evolves.
+3. **Revenue Share:** Once your pull request is merged, you will receive a percentage of the revenue generated by the PegasusX API. The percentage will be determined based on the significance and impact of your contribution. 
 
 ## Becoming a Paid API
 
-As part of our growth strategy, we will be deploying Pegasus as a Paid API. The revenue generated from this API will not only sustain and further the project, but also fund the rewards program.
+As part of our growth strategy, we will be deploying PegasusX as a Paid API. The revenue generated from this API will not only sustain and further the project, but also fund the rewards program.
 
-## How to Start Contributing
+### How to Start Contributing
 
-If you're ready to become a part of Pegasus and contribute to the future of multimodal embeddings, here's what you need to do:
+If you're ready to become a part of PegasusX and contribute to the future of multimodal embeddings, here's what you need to do:
 
 1. Fork the repository.
 
 2. Make your improvements or additions in your forked repository.
 
 3. Submit a pull request detailing the changes you've made.
 
-4. Our team will review your submission. If it's approved, it will be merged into the main repository, and you will become part of the Pegasus Rewards Program.
-
-Thank you for considering contributing to Pegasus. Your expertise and commitment to this project are what make it thrive. Let's build the future of multimodal embeddings together.
-
-# Pegasus: The Future of Multimodal Embeddings
-
-Welcome to Pegasus, a state-of-the-art embedding model designed for a new era of multi-modality data understanding. We are at the forefront of AI research, and our mission is to provide high-quality, task-specific embeddings for any data type you're working with.
+4. Our team will review your submission. If it's approved, it will be merged into the main repository, and you will become part of the PegasusX Rewards Program.
 
 ## Roadmap
 
-Pegasus is a constant work in progress, and we're always striving for better. Our roadmap provides a snapshot of where we're heading. This iterative, continuous improvement process is fundamental to achieving our goal of creating the most effective SOTA omni-modality embeddings model. 
-
-### Phase 1: Reconfiguring the ImageBind Model
-
-To improve our handling of diverse data, we are reconfiguring the ImageBind model to utilize Flash Attention. This shift will allow us to manage longer context lengths and handle more complex inputs effectively.
-
-### Phase 2: Pretraining with Diverse Datasets
-
-Quality embeddings require quality training. To ensure our model is versatile and robust, we're pretraining Pegasus using the same datasets that ImageBind has been trained on. This step ensures our model inherits the benefits of proven training methodologies while also incorporating our enhancements.
-
-### Phase 3: Benchmarking
-
-It's important to know where we stand. After we've reconfigured and pretrained our model, we will conduct comprehensive benchmarking tests. This process will highlight any areas of strength or potential improvement, allowing us to further refine our model.
-
-### Phase 4: Finetuning on Long Samples
-
-We believe that Pegasus can handle more than short snippets of data. To prove this, we'll finetune our model using long data samples, pushing the boundaries of what's possible with embedding models.
-
-### Phase 5: Continued Innovation
+PegasusX is a constant work in progress, and we're always striving for better. Our roadmap provides a snapshot of where we're heading. 
 
-Our roadmap doesn't stop with finetuning. As we move forward, we're excited to explore new methodologies and techniques to enhance Pegasus. Potential areas of exploration include:
+* **Reconfiguring the ImageBind Model:** To improve our handling of diverse data, we are reconfiguring the ImageBind model to utilize Flash Attention. This shift will allow us to manage longer context lengths and handle more complex inputs effectively.
 
-1. **Advanced Training Techniques:** We'll look into more sophisticated methods to make the training process faster and more efficient. 
+* **Pretraining with Diverse Datasets:** Quality embeddings require quality training. To ensure our model is versatile and robust, we're pretraining PegasusX using the same datasets that ImageBind has been trained on. This step ensures our model inherits the benefits of proven training methodologies while also incorporating our enhancements.
 
-2. **Expanding Modality Types:** We aim to support more types of modalities, ensuring that Pegasus is truly a universal tool for multi-modal data.
+* **Benchmarking:** It's important to know where we stand. After we've reconfigured and pretrained our model, we will conduct comprehensive benchmarking tests. This process will highlight any areas of strength or potential improvement, allowing us to further refine our model.
 
+* **Finetuning on Long Samples:** We believe that PegasusX can handle more than short snippets of data. To prove this, we'll finetune our model using long data samples, pushing the boundaries of what's possible with embedding models.
 
-3. **Integration with More Frameworks:** We want Pegasus to be accessible and easy to use with popular machine learning and data processing frameworks.
+* **Continued Innovation:** Our roadmap doesn't stop with finetuning. As we move forward, we're excited to explore new methodologies and techniques to enhance PegasusX. 
 
-4. **Optimizing for Real-Time Processing:** We're focused on making Pegasus capable of generating embeddings in real-time, a critical feature for many applications.
+* **Advanced Training Techniques:** We'll look into more sophisticated methods to make the training process faster and more efficient.
 
-5. **Community Driven Enhancements:** We're excited to see what the community suggests and contributes - the possibilities are endless!
+* **Expanding Modality Types:** We aim to support more types of modalities, ensuring that PegasusX is truly a universal tool for multi-modal data.
 
-6. **Production-Level API Deployment:** Pegasus will enter Agora's paid API line up so you can effortlessly make API requests and recieve your embeddings no complicated setup necessary
+* **Integration with More Frameworks:** We want PegasusX to be accessible and easy to use with popular machine learning and data processing frameworks.
 
-As we continue our journey, we invite you to join us. Let's create the best SOTA omni-modality embeddings model together. Welcome to the future with Pegasus.
+* **Optimizing for Real-Time Processing:** We're focused on making PegasusX capable of generating embeddings in real-time, a critical feature for many applications.
 
+* **Community Driven Enhancements:** We're excited to see what the community suggests and contributes - the possibilities are endless!
 
+* **Production-Level API Deployment:** PegasusX will enter Agora's paid API line up so you can effortlessly make API requests and receive your embeddings no complicated setup necessary
 
-# Roadmap
+* **Making it Extremely Fast Through Quantization:** By utilizing quantization techniques, we aim to significantly increase the speed and efficiency of the PegasusX model.
 
-* Make it extremely fast through quantization
+* **Parallelization, Asynchrony, and Other Optimizations:** To ensure seamless operation even with large amounts of data, we're planning to implement parallelization, asynchronous operations, and other optimizations in the model.
 
-* Parrelization, ASYNCHORNNY + other optimizations
+Thank you for considering contributing to PegasusX. Your expertise and commitment to this project are what make it thrive. Let's build the future of multimodal embeddings together.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pegasusX-0.2.1/pegasus/main.py` & `pegasusX-0.2.2/pegasus/main.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.1/pegasus/oceandb/api/types.py` & `pegasusX-0.2.2/pegasus/oceandb/api/types.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.1/pegasus/oceandb/config.py` & `pegasusX-0.2.2/pegasus/oceandb/config.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.1/pegasus/oceandb/errors.py` & `pegasusX-0.2.2/pegasus/oceandb/errors.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.1/pegasus/oceandb/utils/embedding_functions.py` & `pegasusX-0.2.2/pegasus/oceandb/utils/embedding_functions.py`

 * *Files identical despite different names*

### Comparing `pegasusX-0.2.1/pegasusX.egg-info/PKG-INFO` & `pegasusX-0.2.2/pegasusX.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusX
-Version: 0.2.1
+Version: 0.2.2
 Summary: pegasus - Pytorch
 Home-page: https://github.com/kyegomez/pegasus
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pegasusX-0.2.1/setup.py` & `pegasusX-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'pegasusX',
   packages = find_packages(exclude=[]),
-  version = '0.2.1',
+  version = '0.2.2',
   license='MIT',
   description = 'pegasus - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/pegasus',
   keywords = [
```

