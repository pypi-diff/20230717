# Comparing `tmp/text2vec-1.2.1.tar.gz` & `tmp/text2vec-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2vec-1.2.1.tar", last modified: Wed Jun 21 03:03:37 2023, max compression
+gzip compressed data, was "text2vec-1.2.2.tar", last modified: Mon Jul 17 08:29:15 2023, max compression
```

## Comparing `text2vec-1.2.1.tar` & `text2vec-1.2.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-21 03:03:37.425662 text2vec-1.2.1/
--rw-r--r--   0 xuming     (501) staff       (20)    49036 2023-06-21 03:03:37.425133 text2vec-1.2.1/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)    42020 2023-06-21 02:19:56.000000 text2vec-1.2.1/README.md
--rw-r--r--   0 xuming     (501) staff       (20)       38 2023-06-21 03:03:37.425895 text2vec-1.2.1/setup.cfg
--rw-r--r--   0 xuming     (501) staff       (20)     1606 2023-06-14 08:11:02.000000 text2vec-1.2.1/setup.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-21 03:03:37.386479 text2vec-1.2.1/text2vec/
--rw-r--r--   0 xuming     (501) staff       (20)     1221 2023-06-14 14:22:28.000000 text2vec-1.2.1/text2vec/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     3715 2023-06-14 14:12:57.000000 text2vec-1.2.1/text2vec/bertmatching_dataset.py
--rw-r--r--   0 xuming     (501) staff       (20)    18322 2023-06-15 02:51:06.000000 text2vec-1.2.1/text2vec/bertmatching_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     1803 2023-06-14 08:11:02.000000 text2vec-1.2.1/text2vec/bm25.py
--rw-r--r--   0 xuming     (501) staff       (20)     3377 2023-06-18 04:55:14.000000 text2vec-1.2.1/text2vec/cosent_dataset.py
--rw-r--r--   0 xuming     (501) staff       (20)    13840 2023-06-15 02:51:06.000000 text2vec-1.2.1/text2vec/cosent_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     3252 2023-06-14 12:45:18.000000 text2vec-1.2.1/text2vec/ngram.py
--rw-r--r--   0 xuming     (501) staff       (20)    12378 2023-06-20 03:07:55.000000 text2vec-1.2.1/text2vec/sentence_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    14566 2023-06-15 02:51:06.000000 text2vec-1.2.1/text2vec/sentencebert_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     9813 2023-06-20 03:12:38.000000 text2vec-1.2.1/text2vec/similarity.py
--rw-r--r--   0 xuming     (501) staff       (20)     9136 2021-09-11 10:12:24.000000 text2vec-1.2.1/text2vec/stopwords.txt
--rw-r--r--   0 xuming     (501) staff       (20)     6358 2023-06-18 04:53:18.000000 text2vec-1.2.1/text2vec/text_matching_dataset.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-21 03:03:37.421648 text2vec-1.2.1/text2vec/utils/
--rw-r--r--   0 xuming     (501) staff       (20)        0 2021-09-11 10:12:24.000000 text2vec-1.2.1/text2vec/utils/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     6413 2022-01-21 13:50:54.000000 text2vec-1.2.1/text2vec/utils/distance.py
--rw-r--r--   0 xuming     (501) staff       (20)    15066 2022-03-11 08:18:40.000000 text2vec-1.2.1/text2vec/utils/get_file.py
--rw-r--r--   0 xuming     (501) staff       (20)     1595 2023-06-14 13:27:05.000000 text2vec-1.2.1/text2vec/utils/io_util.py
--rw-r--r--   0 xuming     (501) staff       (20)     5630 2022-02-13 15:54:49.000000 text2vec-1.2.1/text2vec/utils/rank_bm25.py
--rw-r--r--   0 xuming     (501) staff       (20)      859 2022-02-25 17:04:46.000000 text2vec-1.2.1/text2vec/utils/stats_util.py
--rw-r--r--   0 xuming     (501) staff       (20)     1916 2022-01-23 04:13:14.000000 text2vec-1.2.1/text2vec/utils/tokenizer.py
--rw-r--r--   0 xuming     (501) staff       (20)       84 2023-06-21 03:03:19.000000 text2vec-1.2.1/text2vec/version.py
--rw-r--r--   0 xuming     (501) staff       (20)     6180 2023-06-14 12:45:19.000000 text2vec-1.2.1/text2vec/word2vec.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-21 03:03:37.413588 text2vec-1.2.1/text2vec.egg-info/
--rw-r--r--   0 xuming     (501) staff       (20)    49036 2023-06-21 03:03:37.000000 text2vec-1.2.1/text2vec.egg-info/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)      751 2023-06-21 03:03:37.000000 text2vec-1.2.1/text2vec.egg-info/SOURCES.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2023-06-21 03:03:37.000000 text2vec-1.2.1/text2vec.egg-info/dependency_links.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2022-05-17 02:41:49.000000 text2vec-1.2.1/text2vec.egg-info/not-zip-safe
--rw-r--r--   0 xuming     (501) staff       (20)       74 2023-06-21 03:03:37.000000 text2vec-1.2.1/text2vec.egg-info/requires.txt
--rw-r--r--   0 xuming     (501) staff       (20)        9 2023-06-21 03:03:37.000000 text2vec-1.2.1/text2vec.egg-info/top_level.txt
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-17 08:29:15.290018 text2vec-1.2.2/
+-rw-r--r--   0 xuming     (501) staff       (20)    51655 2023-07-17 08:29:15.289376 text2vec-1.2.2/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)    44575 2023-07-16 07:50:04.000000 text2vec-1.2.2/README.md
+-rw-r--r--   0 xuming     (501) staff       (20)       38 2023-07-17 08:29:15.290386 text2vec-1.2.2/setup.cfg
+-rw-r--r--   0 xuming     (501) staff       (20)     1606 2023-06-14 08:11:02.000000 text2vec-1.2.2/setup.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-17 08:29:15.273036 text2vec-1.2.2/text2vec/
+-rw-r--r--   0 xuming     (501) staff       (20)     1221 2023-06-14 14:22:28.000000 text2vec-1.2.2/text2vec/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3715 2023-06-14 14:12:57.000000 text2vec-1.2.2/text2vec/bertmatching_dataset.py
+-rw-r--r--   0 xuming     (501) staff       (20)    19099 2023-07-16 04:07:08.000000 text2vec-1.2.2/text2vec/bertmatching_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1803 2023-06-14 08:11:02.000000 text2vec-1.2.2/text2vec/bm25.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3377 2023-06-18 04:55:14.000000 text2vec-1.2.2/text2vec/cosent_dataset.py
+-rw-r--r--   0 xuming     (501) staff       (20)    14698 2023-07-16 04:07:08.000000 text2vec-1.2.2/text2vec/cosent_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3252 2023-06-14 12:45:18.000000 text2vec-1.2.2/text2vec/ngram.py
+-rw-r--r--   0 xuming     (501) staff       (20)    12614 2023-07-16 04:07:08.000000 text2vec-1.2.2/text2vec/sentence_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    15952 2023-07-16 04:07:08.000000 text2vec-1.2.2/text2vec/sentencebert_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     9813 2023-06-20 03:12:38.000000 text2vec-1.2.2/text2vec/similarity.py
+-rw-r--r--   0 xuming     (501) staff       (20)     9136 2021-09-11 10:12:24.000000 text2vec-1.2.2/text2vec/stopwords.txt
+-rw-r--r--   0 xuming     (501) staff       (20)     6358 2023-06-18 04:53:18.000000 text2vec-1.2.2/text2vec/text_matching_dataset.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-17 08:29:15.287690 text2vec-1.2.2/text2vec/utils/
+-rw-r--r--   0 xuming     (501) staff       (20)        0 2021-09-11 10:12:24.000000 text2vec-1.2.2/text2vec/utils/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6506 2023-07-17 08:26:35.000000 text2vec-1.2.2/text2vec/utils/distance.py
+-rw-r--r--   0 xuming     (501) staff       (20)    15066 2022-03-11 08:18:40.000000 text2vec-1.2.2/text2vec/utils/get_file.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1595 2023-06-14 13:27:05.000000 text2vec-1.2.2/text2vec/utils/io_util.py
+-rw-r--r--   0 xuming     (501) staff       (20)     5630 2022-02-13 15:54:49.000000 text2vec-1.2.2/text2vec/utils/rank_bm25.py
+-rw-r--r--   0 xuming     (501) staff       (20)      859 2022-02-25 17:04:46.000000 text2vec-1.2.2/text2vec/utils/stats_util.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1916 2022-01-23 04:13:14.000000 text2vec-1.2.2/text2vec/utils/tokenizer.py
+-rw-r--r--   0 xuming     (501) staff       (20)       84 2023-07-17 08:28:26.000000 text2vec-1.2.2/text2vec/version.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6180 2023-06-14 12:45:19.000000 text2vec-1.2.2/text2vec/word2vec.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-17 08:29:15.279471 text2vec-1.2.2/text2vec.egg-info/
+-rw-r--r--   0 xuming     (501) staff       (20)    51655 2023-07-17 08:29:14.000000 text2vec-1.2.2/text2vec.egg-info/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)      751 2023-07-17 08:29:14.000000 text2vec-1.2.2/text2vec.egg-info/SOURCES.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2023-07-17 08:29:14.000000 text2vec-1.2.2/text2vec.egg-info/dependency_links.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2022-05-17 02:41:49.000000 text2vec-1.2.2/text2vec.egg-info/not-zip-safe
+-rw-r--r--   0 xuming     (501) staff       (20)       74 2023-07-17 08:29:14.000000 text2vec-1.2.2/text2vec.egg-info/requires.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        9 2023-07-17 08:29:14.000000 text2vec-1.2.2/text2vec.egg-info/top_level.txt
```

### Comparing `text2vec-1.2.1/PKG-INFO` & `text2vec-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2vec
-Version: 1.2.1
+Version: 1.2.2
 Summary: Text to vector Tool, encode text
 Home-page: https://github.com/shibing624/text2vec
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache License 2.0
 Description: [**🇨🇳中文**](https://github.com/shibing624/text2vec/blob/master/README.md) | [**🌐English**](https://github.com/shibing624/text2vec/blob/master/README_EN.md) | [**📖文档/Docs**](https://github.com/shibing624/text2vec/wiki) | [**🤖模型/Models**](https://huggingface.co/shibing624) 
         
@@ -27,54 +27,57 @@
         
         
         **Text2vec**: Text to Vector, Get Sentence Embeddings. 文本向量化，把文本(包括词、句子、段落)表征为向量矩阵。
         
         **text2vec**实现了Word2Vec、RankBM25、BERT、Sentence-BERT、CoSENT等多种文本表征、文本相似度计算模型，并在文本语义匹配（相似度计算）任务上比较了各模型的效果。
         
         ### News
+        [2023/06/22] v1.2.2版本: 发布了多语言匹配模型[shibing624/text2vec-base-multilingual](https://huggingface.co/shibing624/text2vec-base-multilingual)，用CoSENT方法训练，基于`sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`用人工挑选后的多语言STS数据集[shibing624/nli-zh-all/text2vec-base-multilingual-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-multilingual-dataset)训练得到，并在中英文测试集评估相对于原模型效果有提升，详见[Release-v1.2.2](https://github.com/shibing624/text2vec/releases/tag/1.2.2)
+        
         [2023/06/19] v1.2.1版本: 更新了中文匹配模型`shibing624/text2vec-base-chinese-nli`为新版[shibing624/text2vec-base-chinese-sentence](https://huggingface.co/shibing624/text2vec-base-chinese-sentence)，针对CoSENT的loss计算对排序敏感特点，人工挑选并整理出高质量的有相关性排序的STS数据集[shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-sentence-dataset)，在各评估集表现相对之前有提升；发布了适用于s2p的中文匹配模型[shibing624/text2vec-base-chinese-paraphrase](https://huggingface.co/shibing624/text2vec-base-chinese-paraphrase)，详见[Release-v1.2.1](https://github.com/shibing624/text2vec/releases/tag/1.2.1)
         
         [2023/06/15] v1.2.0版本: 发布了中文匹配模型[shibing624/text2vec-base-chinese-nli](https://huggingface.co/shibing624/text2vec-base-chinese-nli)，基于`nghuyong/ernie-3.0-base-zh`模型，使用了中文NLI数据集[shibing624/nli_zh](https://huggingface.co/datasets/shibing624/nli_zh)全部语料训练的CoSENT文本匹配模型，在各评估集表现提升明显，详见[Release-v1.2.0](https://github.com/shibing624/text2vec/releases/tag/1.2.0)
         
         [2022/03/12] v1.1.4版本: 发布了中文匹配模型[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)，基于中文STS训练集训练的CoSENT匹配模型。详见[Release-v1.1.4](https://github.com/shibing624/text2vec/releases/tag/1.1.4)
         
         
         **Guide**
-        - [Feature](#Feature)
+        - [Features](#Features)
         - [Evaluation](#Evaluation)
         - [Install](#install)
         - [Usage](#usage)
         - [Contact](#Contact)
-        - [Reference](#reference)
+        - [References](#references)
         
         
-        # Feature
+        ## Features
         ### 文本向量表示模型
         - [Word2Vec](https://github.com/shibing624/text2vec/blob/master/text2vec/word2vec.py)：通过腾讯AI Lab开源的大规模高质量中文[词向量数据（800万中文词轻量版）](https://pan.baidu.com/s/1La4U4XNFe8s5BJqxPQpeiQ) (文件名：light_Tencent_AILab_ChineseEmbedding.bin 密码: tawe）实现词向量检索，本项目实现了句子（词向量求平均）的word2vec向量表示
         - [SBERT(Sentence-BERT)](https://github.com/shibing624/text2vec/blob/master/text2vec/sentencebert_model.py)：权衡性能和效率的句向量表示模型，训练时通过有监督训练上层分类函数，文本匹配预测时直接句子向量做余弦，本项目基于PyTorch复现了Sentence-BERT模型的训练和预测
         - [CoSENT(Cosine Sentence)](https://github.com/shibing624/text2vec/blob/master/text2vec/cosent_model.py)：CoSENT模型提出了一种排序的损失函数，使训练过程更贴近预测，模型收敛速度和效果比Sentence-BERT更好，本项目基于PyTorch实现了CoSENT模型的训练和预测
         
         详细文本向量表示方法见wiki: [文本向量表示方法](https://github.com/shibing624/text2vec/wiki/%E6%96%87%E6%9C%AC%E5%90%91%E9%87%8F%E8%A1%A8%E7%A4%BA%E6%96%B9%E6%B3%95)
-        # Evaluation
+        ## Evaluation
         
         文本匹配
         
         #### 英文匹配数据集的评测结果：
         
         
-        | Arch   | BaseModel                                        | Model                            | English-STS-B | 
-        |:-------|:------------------------------------------------|:-------------------------------------|:-------------:|
-        | GloVe  | glove                                           | Avg_word_embeddings_glove_6B_300d    |     61.77     |
-        | BERT   | bert-base-uncased                               | BERT-base-cls                        |     20.29     |
-        | BERT   | bert-base-uncased                               | BERT-base-first_last_avg             |     59.04     |
-        | BERT   | bert-base-uncased                               | BERT-base-first_last_avg-whiten(NLI) |     63.65     |
-        | SBERT  | sentence-transformers/bert-base-nli-mean-tokens | SBERT-base-nli-cls                   |     73.65     |
-        | SBERT  | sentence-transformers/bert-base-nli-mean-tokens | SBERT-base-nli-first_last_avg        |     77.96     |
-        | CoSENT | bert-base-uncased                               | CoSENT-base-first_last_avg           |     69.93     |
-        | CoSENT | sentence-transformers/bert-base-nli-mean-tokens | CoSENT-base-nli-first_last_avg       |     79.68     |
+        | Arch   | BaseModel                                        | Model                                                                                                                | English-STS-B | 
+        |:-------|:------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------|:-------------:|
+        | GloVe  | glove                                           | Avg_word_embeddings_glove_6B_300d                                                                                    |     61.77     |
+        | BERT   | bert-base-uncased                               | BERT-base-cls                                                                                                        |     20.29     |
+        | BERT   | bert-base-uncased                               | BERT-base-first_last_avg                                                                                             |     59.04     |
+        | BERT   | bert-base-uncased                               | BERT-base-first_last_avg-whiten(NLI)                                                                                 |     63.65     |
+        | SBERT  | sentence-transformers/bert-base-nli-mean-tokens | SBERT-base-nli-cls                                                                                                   |     73.65     |
+        | SBERT  | sentence-transformers/bert-base-nli-mean-tokens | SBERT-base-nli-first_last_avg                                                                                        |     77.96     |
+        | CoSENT | bert-base-uncased                               | CoSENT-base-first_last_avg                                                                                           |     69.93     |
+        | CoSENT | sentence-transformers/bert-base-nli-mean-tokens | CoSENT-base-nli-first_last_avg                                                                                       |     79.68     |
+        | CoSENT | sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2 | [shibing624/text2vec-base-multilingual](https://huggingface.co/shibing624/text2vec-base-multilingual)                |     80.12     |
         
         #### 中文匹配数据集的评测结果：
         
         
         | Arch   | BaseModel                    | Model           | ATEC  |  BQ   | LCQMC | PAWSX | STS-B |  Avg  | 
         |:-------|:----------------------------|:--------------------|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|
         | SBERT  | bert-base-chinese           | SBERT-bert-base     | 46.36 | 70.36 | 78.72 | 46.86 | 66.41 | 61.74 |
@@ -83,59 +86,60 @@
         | CoSENT | bert-base-chinese           | CoSENT-bert-base    | 49.74 | 72.38 | 78.69 | 60.00 | 79.27 | 68.01 |
         | CoSENT | hfl/chinese-macbert-base    | CoSENT-macbert-base | 50.39 | 72.93 | 79.17 | 60.86 | 79.30 | 68.53 |
         | CoSENT | hfl/chinese-roberta-wwm-ext | CoSENT-roberta-ext  | 50.81 | 71.45 | 79.31 | 61.56 | 79.96 | 68.61 |
         
         说明：
         - 结果评测指标：spearman系数
         - 为评测模型能力，结果均只用该数据集的train训练，在test上评估得到的表现，没用外部数据
+        - `SBERT-macbert-base`模型，是用SBert方法训练，运行[examples/training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model.py)代码可训练模型
+        - `sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`模型是用SBert训练，是`paraphrase-MiniLM-L12-v2`模型的多语言版本，支持中文、英文等
         
         
         ### Release Models
         - 本项目release模型的中文匹配评测结果：
         
-        | Arch       | BaseModel                         | Model                                                                                                                                             | ATEC  |  BQ   | LCQMC | PAWSX | STS-B | SOHU-dd | SOHU-dc |    Avg    |  QPS  |
-        |:-----------|:----------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------|:-----:|:-----:|:-----:|:-----:|:-----:|:-------:|:-------:|:---------:|:-----:|
-        | Word2Vec   | word2vec                          | [w2v-light-tencent-chinese](https://ai.tencent.com/ailab/nlp/en/download.html)                                                                    | 20.00 | 31.49 | 59.46 | 2.57  | 55.78 |  55.04  |  20.70  |   35.03   | 23769 |
-        | SBERT      | xlm-roberta-base                  | [sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2](https://huggingface.co/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2) | 18.42 | 38.52 | 63.96 | 10.14 | 78.90 |  63.01  |  52.28  |   46.46   | 3138  |
-        | Instructor | hfl/chinese-roberta-wwm-ext       | [moka-ai/m3e-base](https://huggingface.co/moka-ai/m3e-base)                                                                                       | 41.27 | 63.81 | 74.87 | 12.20 | 76.96 |  75.83  |  60.55  |   57.93   | 2980  |
-        | CoSENT     | hfl/chinese-macbert-base          | [shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)                                                       | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 |  70.27  |  50.42  |   51.61   | 3008  |
-        | CoSENT     | hfl/chinese-lert-large            | [GanymedeNil/text2vec-large-chinese](https://huggingface.co/GanymedeNil/text2vec-large-chinese)                                                   | 32.61 | 44.59 | 69.30 | 14.51 | 79.44 |  73.01  |  59.04  |   53.12   | 2092  |
-        | CoSENT     | nghuyong/ernie-3.0-base-zh        | [shibing624/text2vec-base-chinese-sentence](https://huggingface.co/shibing624/text2vec-base-chinese-sentence)                                     | 43.37 | 61.43 | 73.48 | 38.90 | 78.25 |  70.60  |  53.08  |   59.87   | 3089  |
-        | CoSENT     | nghuyong/ernie-3.0-base-zh        | [shibing624/text2vec-base-chinese-paraphrase](https://huggingface.co/shibing624/text2vec-base-chinese-paraphrase)                                 | 44.89 | 63.58 | 74.24 | 40.90 | 78.93 |  76.70  |  63.30  | **63.08** | 3066  |
+        | Arch       | BaseModel                                                    | Model                                                                                                                                             | ATEC  |  BQ   | LCQMC | PAWSX | STS-B | SOHU-dd | SOHU-dc |    Avg    |  QPS  |
+        |:-----------|:-------------------------------------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------|:-----:|:-----:|:-----:|:-----:|:-----:|:-------:|:-------:|:---------:|:-----:|
+        | Word2Vec   | word2vec                                                     | [w2v-light-tencent-chinese](https://ai.tencent.com/ailab/nlp/en/download.html)                                                                    | 20.00 | 31.49 | 59.46 | 2.57  | 55.78 |  55.04  |  20.70  |   35.03   | 23769 |
+        | SBERT      | xlm-roberta-base                                             | [sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2](https://huggingface.co/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2) | 18.42 | 38.52 | 63.96 | 10.14 | 78.90 |  63.01  |  52.28  |   46.46   | 3138  |
+        | CoSENT     | hfl/chinese-macbert-base                                     | [shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)                                                       | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 |  70.27  |  50.42  |   51.61   | 3008  |
+        | CoSENT     | hfl/chinese-lert-large                                       | [GanymedeNil/text2vec-large-chinese](https://huggingface.co/GanymedeNil/text2vec-large-chinese)                                                   | 32.61 | 44.59 | 69.30 | 14.51 | 79.44 |  73.01  |  59.04  |   53.12   | 2092  |
+        | CoSENT     | nghuyong/ernie-3.0-base-zh                                   | [shibing624/text2vec-base-chinese-sentence](https://huggingface.co/shibing624/text2vec-base-chinese-sentence)                                     | 43.37 | 61.43 | 73.48 | 38.90 | 78.25 |  70.60  |  53.08  |   59.87   | 3089  |
+        | CoSENT     | nghuyong/ernie-3.0-base-zh                                   | [shibing624/text2vec-base-chinese-paraphrase](https://huggingface.co/shibing624/text2vec-base-chinese-paraphrase)                                 | 44.89 | 63.58 | 74.24 | 40.90 | 78.93 |  76.70  |  63.30  | **63.08** | 3066  |
+        | CoSENT     | sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2  | [shibing624/text2vec-base-multilingual](https://huggingface.co/shibing624/text2vec-base-multilingual)                                             | 32.39 | 50.33 | 65.64 | 32.56 | 74.45 |  68.88  |  51.17  |   53.67   | 3138  |
         
         
         说明：
         - 结果评测指标：spearman系数
-        - 模型训练实验报告：[实验报告](https://github.com/shibing624/text2vec/blob/master/docs/model_report.md)
         - `shibing624/text2vec-base-chinese`模型，是用CoSENT方法训练，基于`hfl/chinese-macbert-base`在中文STS-B数据训练得到，并在中文STS-B测试集评估达到较好效果，运行[examples/training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model.py)代码可训练模型，模型文件已经上传HF model hub，中文通用语义匹配任务推荐使用
         - `shibing624/text2vec-base-chinese-sentence`模型，是用CoSENT方法训练，基于`nghuyong/ernie-3.0-base-zh`用人工挑选后的中文STS数据集[shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-sentence-dataset)训练得到，并在中文各NLI测试集评估达到较好效果，运行[examples/training_sup_text_matching_model_jsonl_data.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model_jsonl_data.py)代码可训练模型，模型文件已经上传HF model hub，中文s2s(句子vs句子)语义匹配任务推荐使用
         - `shibing624/text2vec-base-chinese-paraphrase`模型，是用CoSENT方法训练，基于`nghuyong/ernie-3.0-base-zh`用人工挑选后的中文STS数据集[shibing624/nli-zh-all/text2vec-base-chinese-paraphrase-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-paraphrase-dataset)，数据集相对于[shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-sentence-dataset)加入了s2p(sentence to paraphrase)数据，强化了其长文本的表征能力，并在中文各NLI测试集评估达到SOTA，运行[examples/training_sup_text_matching_model_jsonl_data.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model_jsonl_data.py)代码可训练模型，模型文件已经上传HF model hub，中文s2p(句子vs段落)语义匹配任务推荐使用
-        - `SBERT-macbert-base`模型，是用SBERT方法训练，运行[examples/training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model.py)代码可训练模型
-        - `sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`模型是用SBERT训练，是`paraphrase-MiniLM-L12-v2`模型的多语言版本，支持中文、英文等
+        - `shibing624/text2vec-base-multilingual`模型，是用CoSENT方法训练，基于`sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`用人工挑选后的多语言STS数据集[shibing624/nli-zh-all/text2vec-base-multilingual-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-multilingual-dataset)训练得到，并在中英文测试集评估相对于原模型效果有提升，运行[examples/training_sup_text_matching_model_jsonl_data.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model_jsonl_data.py)代码可训练模型，模型文件已经上传HF model hub，多语言语义匹配任务推荐使用
         - `w2v-light-tencent-chinese`是腾讯词向量的Word2Vec模型，CPU加载使用，适用于中文字面匹配任务和缺少数据的冷启动情况
         - 各预训练模型均可以通过transformers调用，如MacBERT模型：`--model_name hfl/chinese-macbert-base` 或者roberta模型：`--model_name uer/roberta-medium-wwm-chinese-cluecorpussmall`
         - 为测评模型的鲁棒性，加入了未训练过的SOHU测试集，用于测试模型的泛化能力；为达到开箱即用的实用效果，使用了搜集到的各中文匹配数据集，数据集也上传到HF datasets[链接见下方](#数据集)
         - 中文匹配任务实验表明，pooling最优是`EncoderType.FIRST_LAST_AVG`和`EncoderType.MEAN`，两者预测效果差异很小
         - 中文匹配评测结果复现，可以下载中文匹配数据集到`examples/data`，运行[tests/test_model_spearman.py](https://github.com/shibing624/text2vec/blob/master/tests/test_model_spearman.py)代码复现评测结果
         - QPS的GPU测试环境是Tesla V100，显存32GB
         
-        # Demo
+        模型训练实验报告：[实验报告](https://github.com/shibing624/text2vec/blob/master/docs/model_report.md)
+        ## Demo
         
         Official Demo: https://www.mulanai.com/product/short_text_sim/
         
         HuggingFace Demo: https://huggingface.co/spaces/shibing624/text2vec
         
         ![](docs/hf.png)
         
         run example: [examples/gradio_demo.py](https://github.com/shibing624/text2vec/blob/master/examples/gradio_demo.py) to see the demo:
         ```shell
         python examples/gradio_demo.py
         ```
         
-        # Install
+        ## Install
         ```shell
         pip install torch # conda install pytorch
         pip install -U text2vec
         ```
         
         or
         
@@ -144,17 +148,17 @@
         pip install -r requirements.txt
         
         git clone https://github.com/shibing624/text2vec.git
         cd text2vec
         pip install --no-deps .
         ```
         
-        # Usage
+        ## Usage
         
-        ## 文本向量表征
+        ### 文本向量表征
         
         基于`pretrained model`计算文本向量：
         
         ```zsh
         >>> from text2vec import SentenceModel
         >>> m = SentenceModel()
         >>> m.encode("如何更换花呗绑定银行卡")
@@ -194,16 +198,16 @@
         
         
         if __name__ == "__main__":
             # 中文句向量模型(CoSENT)，中文语义匹配任务推荐，支持fine-tune继续训练
             t2v_model = SentenceModel("shibing624/text2vec-base-chinese")
             compute_emb(t2v_model)
         
-            # 支持多语言的句向量模型（Sentence-BERT），英文语义匹配任务推荐，支持fine-tune继续训练
-            sbert_model = SentenceModel("sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2")
+            # 支持多语言的句向量模型（CoSENT），多语言（包括中英文）语义匹配任务推荐，支持fine-tune继续训练
+            sbert_model = SentenceModel("shibing624/text2vec-base-multilingual")
             compute_emb(sbert_model)
         
             # 中文词向量模型(word2vec)，中文字面匹配任务和冷启动适用
             w2v_model = Word2Vec("w2v-light-tencent-chinese")
             compute_emb(w2v_model)
         
         ```
@@ -220,16 +224,14 @@
         ```
         
         - 返回值`embeddings`是`numpy.ndarray`类型，shape为`(sentences_size, model_embedding_size)`，三个模型任选一种即可，推荐用第一个。
         - `shibing624/text2vec-base-chinese`模型是CoSENT方法在中文STS-B数据集训练得到的，模型已经上传到huggingface的
         模型库[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)，
         是`text2vec.SentenceModel`指定的默认模型，可以通过上面示例调用，或者如下所示用[transformers库](https://github.com/huggingface/transformers)调用，
         模型自动下载到本机路径：`~/.cache/huggingface/transformers`
-        - `sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`模型是Sentence-BERT的多语言句向量模型，
-        适用于释义（paraphrase）识别，文本匹配，通过`text2vec.SentenceModel`和[sentence-transformers库]((https://github.com/UKPLab/sentence-transformers))都可以调用该模型
         - `w2v-light-tencent-chinese`是通过gensim加载的Word2Vec模型，使用腾讯词向量`Tencent_AILab_ChineseEmbedding.tar.gz`计算各字词的词向量，句子向量通过单词词
         向量取平均值得到，模型自动下载到本机路径：`~/.text2vec/datasets/light_Tencent_AILab_ChineseEmbedding.bin`
         
         #### Usage (HuggingFace Transformers)
         Without [text2vec](https://github.com/shibing624/text2vec), you can use the model like this: 
         
         First, you pass your input through the transformer model, then you have to apply the right pooling-operation on-top of the contextualized word embeddings.
@@ -447,17 +449,17 @@
         from similarities import Similarity
         
         m = Similarity()
         r = m.similarity('如何更换花呗绑定银行卡', '花呗更改绑定银行卡')
         print(f"similarity score: {float(r)}")  # similarity score: 0.855146050453186
         ```
         
-        # Models
+        ## Models
         
-        ## CoSENT model
+        ### CoSENT model
         
         CoSENT（Cosine Sentence）文本匹配模型，在Sentence-BERT上改进了CosineRankLoss的句向量方案
         
         
         Network structure:
         
         Training:
@@ -488,16 +490,22 @@
         python training_sup_text_matching_model.py --task_name ATEC --model_arch cosent --do_train --do_predict --num_epochs 10 --model_name hfl/chinese-macbert-base --output_dir ./outputs/ATEC-cosent
         ```
         
         - 在自有中文数据集上训练模型
         
         example: [examples/training_sup_text_matching_model_mydata.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model_mydata.py)
         
+        单卡训练：
+        ```shell
+        CUDA_VISIBLE_DEVICES=0 python training_sup_text_matching_model_mydata.py --do_train --do_predict
+        ```
+        
+        多卡训练：
         ```shell
-        python training_sup_text_matching_model_mydata.py --do_train --do_predict
+        CUDA_VISIBLE_DEVICES=0,1 torchrun --nproc_per_node 2  training_sup_text_matching_model_mydata.py --do_train --do_predict --output_dir outputs/STS-B-text2vec-macbert-v1 --batch_size 64 --fp16 --data_parallel 
         ```
         
         训练集格式参考[examples/data/STS-B/STS-B.valid.data](https://github.com/shibing624/text2vec/blob/master/examples/data/STS-B/STS-B.valid.data)
         
         ```shell
         sentence1   sentence2   label
         一个女孩在给她的头发做发型。	一个女孩在梳头。	2
@@ -524,15 +532,15 @@
         
         ```shell
         cd examples
         python training_unsup_text_matching_model_en.py --model_arch cosent --do_train --do_predict --num_epochs 10 --model_name bert-base-uncased --output_dir ./outputs/STS-B-en-unsup-cosent
         ```
         
         
-        ## Sentence-BERT model
+        ### Sentence-BERT model
         
         Sentence-BERT文本匹配模型，表征式句向量表示方案
         
         Network structure:
         
         Training:
         
@@ -567,38 +575,38 @@
         example: [examples/training_unsup_text_matching_model_en.py](https://github.com/shibing624/text2vec/blob/master/examples/training_unsup_text_matching_model_en.py)
         
         ```shell
         cd examples
         python training_unsup_text_matching_model_en.py --model_arch sentencebert --do_train --do_predict --num_epochs 10 --model_name bert-base-uncased --output_dir ./outputs/STS-B-en-unsup-sbert
         ```
         
-        ## BERT-Match model
+        ### BERT-Match model
         BERT文本匹配模型，原生BERT匹配网络结构，交互式句向量匹配模型
         
         Network structure:
         
         Training and inference:
         
         <img src="docs/bert-fc-train.png" width="300" />
         
         训练脚本同上[examples/training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model.py)。
         
         
-        ## 模型蒸馏（Model Distillation）
+        ### 模型蒸馏（Model Distillation）
         
         由于text2vec训练的模型可以使用[sentence-transformers](https://github.com/UKPLab/sentence-transformers)库加载，此处复用其模型蒸馏方法[distillation](https://github.com/UKPLab/sentence-transformers/tree/master/examples/training/distillation)。
         
         1. 模型降维，参考[dimensionality_reduction.py](https://github.com/UKPLab/sentence-transformers/blob/master/examples/training/distillation/dimensionality_reduction.py)使用PCA对模型输出embedding降维，可减少milvus等向量检索数据库的存储压力，还能轻微提升模型效果。
         2. 模型蒸馏，参考[model_distillation.py](https://github.com/UKPLab/sentence-transformers/blob/master/examples/training/distillation/model_distillation.py)使用蒸馏方法，将Teacher大模型蒸馏到更少layers层数的student模型中，在权衡效果的情况下，可大幅提升模型预测速度。
         
-        ## 模型部署
+        ### 模型部署
         
         提供两种部署模型，搭建服务的方法： 1）基于Jina搭建gRPC服务【推荐】；2）基于FastAPI搭建原生Http服务。
         
-        ### Jina服务
+        #### Jina服务
         采用C/S模式搭建高性能服务，支持docker云原生，gRPC/HTTP/WebSocket，支持多个模型同时预测，GPU多卡处理。
         
         - 安装：
         ```pip install jina```
         
         - 启动服务：
         
@@ -637,15 +645,15 @@
         r = c.post('/', inputs=DocumentArray([Document(text='如何更换花呗绑定银行卡'), Document(text='花呗更改绑定银行卡')]))
         print(r.embeddings)
         ```
         
         批量调用方法见example: [examples/jina_client_demo.py](https://github.com/shibing624/text2vec/blob/master/examples/jina_client_demo.py)
         
         
-        ### FastAPI服务
+        #### FastAPI服务
         
         - 安装：
         ```pip install fastapi uvicorn```
         
         - 启动服务：
         
         example: [examples/fastapi_server_demo.py](https://github.com/shibing624/text2vec/blob/master/examples/fastapi_server_demo.py)
@@ -658,15 +666,15 @@
         ```shell
         curl -X 'GET' \
           'http://0.0.0.0:8001/emb?q=hello' \
           -H 'accept: application/json'
         ```
         
         
-        ## 数据集
+        ## Dataset
         
         - 本项目release的数据集：
         
         | Dataset                    | Introduce                                                                | Download Link                                                                                                                                                                                                                                                                                         |
         |:---------------------------|:-------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
         | shibing624/nli-zh-all      | 中文语义匹配数据合集，整合了文本推理，相似，摘要，问答，指令微调等任务的820万高质量数据，并转化为匹配格式数据集                | [https://huggingface.co/datasets/shibing624/nli-zh-all](https://huggingface.co/datasets/shibing624/nli-zh-all)                                                                                                                                                                                        |
         | shibing624/snli-zh         | 中文SNLI和MultiNLI数据集，翻译自英文SNLI和MultiNLI                                    | [https://huggingface.co/datasets/shibing624/snli-zh](https://huggingface.co/datasets/shibing624/snli-zh)                                                                                                                                                                                              |
@@ -677,16 +685,16 @@
         | LCQMC                      | 中文LCQMC(large-scale Chinese question matching corpus)数据集，Q-Qpair数据集      | [LCQMC](http://icrc.hitsz.edu.cn/Article/show/171.html)                                                                                                                                                                                                                                               |
         | PAWSX                      | 中文PAWS(Paraphrase Adversaries from Word Scrambling)数据集，Q-Qpair数据集        | [PAWSX](https://arxiv.org/abs/1908.11828)                                                                                                                                                                                                                                                             |
         | STS-B                      | 中文STS-B数据集，中文自然语言推理数据集，从英文STS-B翻译为中文的数据集                                 | [STS-B](https://github.com/pluto-junzeng/CNSD)                                                                                                                                                                                                                                                        |
         
         
         常用英文匹配数据集：
         
-        - 大名鼎鼎的multi_nli和snli: https://huggingface.co/datasets/multi_nli
-        - 大名鼎鼎的multi_nli和snli: https://huggingface.co/datasets/snli
+        - 英文匹配数据集：multi_nli: https://huggingface.co/datasets/multi_nli
+        - 英文匹配数据集：snli: https://huggingface.co/datasets/snli
         - https://huggingface.co/datasets/metaeval/cnli
         - https://huggingface.co/datasets/mteb/stsbenchmark-sts
         - https://huggingface.co/datasets/JeremiahZ/simcse_sup_nli
         - https://huggingface.co/datasets/MoritzLaurer/multilingual-NLI-26lang-2mil7
         
         
         数据集使用示例：
@@ -721,59 +729,59 @@
         {'sentence1': '一个女孩在给她的头发做发型。', 'sentence2': '一个女孩在梳头。', 'label': 2}
         ```
         
         
         
         
         
-        # Contact
+        ## Contact
         
         - Issue(建议)：[![GitHub issues](https://img.shields.io/github/issues/shibing624/text2vec.svg)](https://github.com/shibing624/text2vec/issues)
         - 邮件我：xuming: xuming624@qq.com
         - 微信我：加我*微信号：xuming624, 备注：姓名-公司-NLP* 进NLP交流群。
         
         <img src="docs/wechat.jpeg" width="200" />
         
         
-        # Citation
+        ## Citation
         
         如果你在研究中使用了text2vec，请按如下格式引用：
         
         APA:
         ```latex
         Xu, M. Text2vec: Text to vector toolkit (Version 1.1.2) [Computer software]. https://github.com/shibing624/text2vec
         ```
         
         BibTeX:
         ```latex
         @misc{Text2vec,
-          author = {Xu, Ming},
+          author = {Ming Xu},
           title = {Text2vec: Text to vector toolkit},
-          year = {2022},
+          year = {2023},
           publisher = {GitHub},
           journal = {GitHub repository},
           howpublished = {\url{https://github.com/shibing624/text2vec}},
         }
         ```
         
-        # License
+        ## License
         
         
         授权协议为 [The Apache License 2.0](LICENSE)，可免费用做商业用途。请在产品说明中附加text2vec的链接和授权协议。
         
         
-        # Contribute
+        ## Contribute
         项目代码还很粗糙，如果大家对代码有所改进，欢迎提交回本项目，在提交之前，注意以下两点：
         
          - 在`tests`添加相应的单元测试
          - 使用`python -m pytest -v`来运行所有单元测试，确保所有单测都是通过的
         
         之后即可提交PR。
         
-        # Reference
+        ## References
         - [将句子表示为向量（上）：无监督句子表示学习（sentence embedding）](https://www.cnblogs.com/llhthinker/p/10335164.html)
         - [将句子表示为向量（下）：无监督句子表示学习（sentence embedding）](https://www.cnblogs.com/llhthinker/p/10341841.html)
         - [A Simple but Tough-to-Beat Baseline for Sentence Embeddings[Sanjeev Arora and Yingyu Liang and Tengyu Ma, 2017]](https://openreview.net/forum?id=SyK00v5xx)
         - [四种计算文本相似度的方法对比[Yves Peirsman]](https://zhuanlan.zhihu.com/p/37104535)
         - [Improvements to BM25 and Language Models Examined](http://www.cs.otago.ac.nz/homepages/andrew/papers/2014-2.pdf)
         - [CoSENT：比Sentence-BERT更有效的句向量方案](https://kexue.fm/archives/8847)
         - [谈谈文本匹配和多轮检索](https://zhuanlan.zhihu.com/p/111769969)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: text2vec Version: 1.2.1 Summary: Text to vector
+Metadata-Version: 2.1 Name: text2vec Version: 1.2.2 Summary: Text to vector
 Tool, encode text Home-page: https://github.com/shibing624/text2vec Author:
 XuMing Author-email: xuming624@qq.com License: Apache License 2.0 Description:
 [**ð¨ð³ä¸­æ**](https://github.com/shibing624/text2vec/blob/master/
 README.md) | [**ðEnglish**](https://github.com/shibing624/text2vec/blob/
 master/README_EN.md) | [**ðææ¡£/Docs**](https://github.com/shibing624/
 text2vec/wiki) | [**ð¤æ¨¡å/Models**](https://huggingface.co/shibing624)
                                     [Logo]
@@ -17,17 +17,26 @@
 shibing624/text2vec.svg)](https://github.com/shibing624/text2vec/issues) [!
 [Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/
 wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact) **Text2vec**: Text to
 Vector, Get Sentence Embeddings. ææ¬åéåï¼æææ¬
 (åæ¬è¯ãå¥å­ãæ®µè½)è¡¨å¾ä¸ºåéç©éµã
 **text2vec**å®ç°äºWord2VecãRankBM25ãBERTãSentence-
 BERTãCoSENTç­å¤ç§ææ¬è¡¨å¾ãææ¬ç¸ä¼¼åº¦è®¡ç®æ¨¡åï¼å¹¶å¨ææ¬è¯­ä¹å¹éï¼ç¸ä¼¼åº¦è®¡ç®ï¼ä»»å¡ä¸æ¯è¾äºåæ¨¡åçææã
-### News [2023/06/19] v1.2.1çæ¬: æ´æ°äºä¸­æå¹éæ¨¡å`shibing624/
-text2vec-base-chinese-nli`ä¸ºæ°ç[shibing624/text2vec-base-chinese-sentence]
-(https://huggingface.co/shibing624/text2vec-base-chinese-
+### News [2023/06/22] v1.2.2çæ¬: åå¸äºå¤è¯­è¨å¹éæ¨¡å[shibing624/
+text2vec-base-multilingual](https://huggingface.co/shibing624/text2vec-base-
+multilingual)ï¼ç¨CoSENTæ¹æ³è®­ç»ï¼åºäº`sentence-transformers/
+paraphrase-multilingual-MiniLM-L12-
+v2`ç¨äººå·¥æéåçå¤è¯­è¨STSæ°æ®é[shibing624/nli-zh-all/text2vec-
+base-multilingual-dataset](https://huggingface.co/datasets/shibing624/nli-zh-
+all/tree/main/text2vec-base-multilingual-
+dataset)è®­ç»å¾å°ï¼å¹¶å¨ä¸­è±ææµè¯éè¯ä¼°ç¸å¯¹äºåæ¨¡åææææåï¼è¯¦è§
+[Release-v1.2.2](https://github.com/shibing624/text2vec/releases/tag/1.2.2)
+[2023/06/19] v1.2.1çæ¬: æ´æ°äºä¸­æå¹éæ¨¡å`shibing624/text2vec-
+base-chinese-nli`ä¸ºæ°ç[shibing624/text2vec-base-chinese-sentence](https://
+huggingface.co/shibing624/text2vec-base-chinese-
 sentence)ï¼éå¯¹CoSENTçlossè®¡ç®å¯¹æåºææç¹ç¹ï¼äººå·¥æéå¹¶æ´çåºé«è´¨éçæç¸å³æ§æåºçSTSæ°æ®é
 [shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://
 huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-
 sentence-
 dataset)ï¼å¨åè¯ä¼°éè¡¨ç°ç¸å¯¹ä¹åææåï¼åå¸äºéç¨äºs2pçä¸­æå¹éæ¨¡å
 [shibing624/text2vec-base-chinese-paraphrase](https://huggingface.co/
 shibing624/text2vec-base-chinese-paraphrase)ï¼è¯¦è§[Release-v1.2.1](https://
@@ -38,17 +47,17 @@
 huggingface.co/datasets/shibing624/
 nli_zh)å¨é¨è¯­æè®­ç»çCoSENTææ¬å¹éæ¨¡åï¼å¨åè¯ä¼°éè¡¨ç°æåææ¾ï¼è¯¦è§
 [Release-v1.2.0](https://github.com/shibing624/text2vec/releases/tag/1.2.0)
 [2022/03/12] v1.1.4çæ¬: åå¸äºä¸­æå¹éæ¨¡å[shibing624/text2vec-
 base-chinese](https://huggingface.co/shibing624/text2vec-base-
 chinese)ï¼åºäºä¸­æSTSè®­ç»éè®­ç»çCoSENTå¹éæ¨¡åãè¯¦è§
 [Release-v1.1.4](https://github.com/shibing624/text2vec/releases/tag/1.1.4)
-**Guide** - [Feature](#Feature) - [Evaluation](#Evaluation) - [Install]
-(#install) - [Usage](#usage) - [Contact](#Contact) - [Reference](#reference) #
-Feature ### ææ¬åéè¡¨ç¤ºæ¨¡å - [Word2Vec](https://github.com/
+**Guide** - [Features](#Features) - [Evaluation](#Evaluation) - [Install]
+(#install) - [Usage](#usage) - [Contact](#Contact) - [References](#references)
+## Features ### ææ¬åéè¡¨ç¤ºæ¨¡å - [Word2Vec](https://github.com/
 shibing624/text2vec/blob/master/text2vec/word2vec.py)ï¼éè¿è¾è®¯AI
 Labå¼æºçå¤§è§æ¨¡é«è´¨éä¸­æ
 [è¯åéæ°æ®ï¼800ä¸ä¸­æè¯è½»éçï¼](https://pan.baidu.com/s/
 1La4U4XNFe8s5BJqxPQpeiQ) (æä»¶åï¼light_Tencent_AILab_ChineseEmbedding.bin
 å¯ç :
 taweï¼å®ç°è¯åéæ£ç´¢ï¼æ¬é¡¹ç®å®ç°äºå¥å­ï¼è¯åéæ±å¹³åï¼çword2vecåéè¡¨ç¤º
 - [SBERT(Sentence-BERT)](https://github.com/shibing624/text2vec/blob/master/
@@ -56,67 +65,76 @@
 sentencebert_model.py)ï¼æè¡¡æ§è½åæççå¥åéè¡¨ç¤ºæ¨¡åï¼è®­ç»æ¶éè¿æçç£è®­ç»ä¸å±åç±»å½æ°ï¼ææ¬å¹éé¢æµæ¶ç´æ¥å¥å­åéåä½å¼¦ï¼æ¬é¡¹ç®åºäºPyTorchå¤ç°äºSentence-
 BERTæ¨¡åçè®­ç»åé¢æµ - [CoSENT(Cosine Sentence)](https://github.com/
 shibing624/text2vec/blob/master/text2vec/
 cosent_model.py)ï¼CoSENTæ¨¡åæåºäºä¸ç§æåºçæå¤±å½æ°ï¼ä½¿è®­ç»è¿ç¨æ´è´´è¿é¢æµï¼æ¨¡åæ¶æéåº¦åæææ¯Sentence-
 BERTæ´å¥½ï¼æ¬é¡¹ç®åºäºPyTorchå®ç°äºCoSENTæ¨¡åçè®­ç»åé¢æµ
 è¯¦ç»ææ¬åéè¡¨ç¤ºæ¹æ³è§wiki: [ææ¬åéè¡¨ç¤ºæ¹æ³](https://
 github.com/shibing624/text2vec/wiki/
-%E6%96%87%E6%9C%AC%E5%90%91%E9%87%8F%E8%A1%A8%E7%A4%BA%E6%96%B9%E6%B3%95) #
+%E6%96%87%E6%9C%AC%E5%90%91%E9%87%8F%E8%A1%A8%E7%A4%BA%E6%96%B9%E6%B3%95) ##
 Evaluation ææ¬å¹é #### è±æå¹éæ°æ®éçè¯æµç»æï¼ | Arch |
 BaseModel | Model | English-STS-B | |:-------|:--------------------------------
-----------------|:-------------------------------------|:-------------:| |
+----------------|:-------------------------------------------------------------
+--------------------------------------------------------|:-------------:| |
 GloVe | glove | Avg_word_embeddings_glove_6B_300d | 61.77 | | BERT | bert-base-
 uncased | BERT-base-cls | 20.29 | | BERT | bert-base-uncased | BERT-base-
 first_last_avg | 59.04 | | BERT | bert-base-uncased | BERT-base-first_last_avg-
 whiten(NLI) | 63.65 | | SBERT | sentence-transformers/bert-base-nli-mean-tokens
 | SBERT-base-nli-cls | 73.65 | | SBERT | sentence-transformers/bert-base-nli-
 mean-tokens | SBERT-base-nli-first_last_avg | 77.96 | | CoSENT | bert-base-
 uncased | CoSENT-base-first_last_avg | 69.93 | | CoSENT | sentence-
 transformers/bert-base-nli-mean-tokens | CoSENT-base-nli-first_last_avg | 79.68
-| #### ä¸­æå¹éæ°æ®éçè¯æµç»æï¼ | Arch | BaseModel | Model |
-ATEC | BQ | LCQMC | PAWSX | STS-B | Avg | |:-------|:--------------------------
---|:--------------------|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:| |
-SBERT | bert-base-chinese | SBERT-bert-base | 46.36 | 70.36 | 78.72 | 46.86 |
-66.41 | 61.74 | | SBERT | hfl/chinese-macbert-base | SBERT-macbert-base | 47.28
-| 68.63 | 79.42 | 55.59 | 64.82 | 63.15 | | SBERT | hfl/chinese-roberta-wwm-ext
-| SBERT-roberta-ext | 48.29 | 69.99 | 79.22 | 44.10 | 72.42 | 62.80 | | CoSENT
-| bert-base-chinese | CoSENT-bert-base | 49.74 | 72.38 | 78.69 | 60.00 | 79.27
-| 68.01 | | CoSENT | hfl/chinese-macbert-base | CoSENT-macbert-base | 50.39 |
-72.93 | 79.17 | 60.86 | 79.30 | 68.53 | | CoSENT | hfl/chinese-roberta-wwm-ext
-| CoSENT-roberta-ext | 50.81 | 71.45 | 79.31 | 61.56 | 79.96 | 68.61 |
-è¯´æï¼ - ç»æè¯æµææ ï¼spearmanç³»æ° -
+| | CoSENT | sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2 |
+[shibing624/text2vec-base-multilingual](https://huggingface.co/shibing624/
+text2vec-base-multilingual) | 80.12 | ####
+ä¸­æå¹éæ°æ®éçè¯æµç»æï¼ | Arch | BaseModel | Model | ATEC | BQ
+| LCQMC | PAWSX | STS-B | Avg | |:-------|:----------------------------|:------
+--------------|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:| | SBERT | bert-
+base-chinese | SBERT-bert-base | 46.36 | 70.36 | 78.72 | 46.86 | 66.41 | 61.74
+| | SBERT | hfl/chinese-macbert-base | SBERT-macbert-base | 47.28 | 68.63 |
+79.42 | 55.59 | 64.82 | 63.15 | | SBERT | hfl/chinese-roberta-wwm-ext | SBERT-
+roberta-ext | 48.29 | 69.99 | 79.22 | 44.10 | 72.42 | 62.80 | | CoSENT | bert-
+base-chinese | CoSENT-bert-base | 49.74 | 72.38 | 78.69 | 60.00 | 79.27 | 68.01
+| | CoSENT | hfl/chinese-macbert-base | CoSENT-macbert-base | 50.39 | 72.93 |
+79.17 | 60.86 | 79.30 | 68.53 | | CoSENT | hfl/chinese-roberta-wwm-ext |
+CoSENT-roberta-ext | 50.81 | 71.45 | 79.31 | 61.56 | 79.96 | 68.61 | è¯´æï¼
+- ç»æè¯æµææ ï¼spearmanç³»æ° -
 ä¸ºè¯æµæ¨¡åè½åï¼ç»æååªç¨è¯¥æ°æ®éçtrainè®­ç»ï¼å¨testä¸è¯ä¼°å¾å°çè¡¨ç°ï¼æ²¡ç¨å¤é¨æ°æ®
-### Release Models - æ¬é¡¹ç®releaseæ¨¡åçä¸­æå¹éè¯æµç»æï¼ |
-Arch | BaseModel | Model | ATEC | BQ | LCQMC | PAWSX | STS-B | SOHU-dd | SOHU-
-dc | Avg | QPS | |:-----------|:----------------------------------|:-----------
+- `SBERT-macbert-base`æ¨¡åï¼æ¯ç¨SBertæ¹æ³è®­ç»ï¼è¿è¡[examples/
+training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/
+blob/master/examples/training_sup_text_matching_model.py)ä»£ç å¯è®­ç»æ¨¡å
+- `sentence-transformers/paraphrase-multilingual-MiniLM-L12-
+v2`æ¨¡åæ¯ç¨SBertè®­ç»ï¼æ¯`paraphrase-MiniLM-L12-
+v2`æ¨¡åçå¤è¯­è¨çæ¬ï¼æ¯æä¸­æãè±æç­ ### Release Models -
+æ¬é¡¹ç®releaseæ¨¡åçä¸­æå¹éè¯æµç»æï¼ | Arch | BaseModel | Model
+| ATEC | BQ | LCQMC | PAWSX | STS-B | SOHU-dd | SOHU-dc | Avg | QPS | |:-------
+----|:-------------------------------------------------------------|:----------
 -------------------------------------------------------------------------------
---------------------------------------------------------|:-----:|:-----:|:----
+---------------------------------------------------------|:-----:|:-----:|:----
 -:|:-----:|:-----:|:-------:|:-------:|:---------:|:-----:| | Word2Vec |
 word2vec | [w2v-light-tencent-chinese](https://ai.tencent.com/ailab/nlp/en/
 download.html) | 20.00 | 31.49 | 59.46 | 2.57 | 55.78 | 55.04 | 20.70 | 35.03 |
 23769 | | SBERT | xlm-roberta-base | [sentence-transformers/paraphrase-
 multilingual-MiniLM-L12-v2](https://huggingface.co/sentence-transformers/
 paraphrase-multilingual-MiniLM-L12-v2) | 18.42 | 38.52 | 63.96 | 10.14 | 78.90
-| 63.01 | 52.28 | 46.46 | 3138 | | Instructor | hfl/chinese-roberta-wwm-ext |
-[moka-ai/m3e-base](https://huggingface.co/moka-ai/m3e-base) | 41.27 | 63.81 |
-74.87 | 12.20 | 76.96 | 75.83 | 60.55 | 57.93 | 2980 | | CoSENT | hfl/chinese-
-macbert-base | [shibing624/text2vec-base-chinese](https://huggingface.co/
-shibing624/text2vec-base-chinese) | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 |
-70.27 | 50.42 | 51.61 | 3008 | | CoSENT | hfl/chinese-lert-large |
-[GanymedeNil/text2vec-large-chinese](https://huggingface.co/GanymedeNil/
-text2vec-large-chinese) | 32.61 | 44.59 | 69.30 | 14.51 | 79.44 | 73.01 | 59.04
-| 53.12 | 2092 | | CoSENT | nghuyong/ernie-3.0-base-zh | [shibing624/text2vec-
-base-chinese-sentence](https://huggingface.co/shibing624/text2vec-base-chinese-
-sentence) | 43.37 | 61.43 | 73.48 | 38.90 | 78.25 | 70.60 | 53.08 | 59.87 |
-3089 | | CoSENT | nghuyong/ernie-3.0-base-zh | [shibing624/text2vec-base-
-chinese-paraphrase](https://huggingface.co/shibing624/text2vec-base-chinese-
-paraphrase) | 44.89 | 63.58 | 74.24 | 40.90 | 78.93 | 76.70 | 63.30 | **63.08**
-| 3066 | è¯´æï¼ - ç»æè¯æµææ ï¼spearmanç³»æ° -
-æ¨¡åè®­ç»å®éªæ¥åï¼[å®éªæ¥å](https://github.com/shibing624/
-text2vec/blob/master/docs/model_report.md) - `shibing624/text2vec-base-
+| 63.01 | 52.28 | 46.46 | 3138 | | CoSENT | hfl/chinese-macbert-base |
+[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-
+base-chinese) | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 | 70.27 | 50.42 | 51.61 |
+3008 | | CoSENT | hfl/chinese-lert-large | [GanymedeNil/text2vec-large-chinese]
+(https://huggingface.co/GanymedeNil/text2vec-large-chinese) | 32.61 | 44.59 |
+69.30 | 14.51 | 79.44 | 73.01 | 59.04 | 53.12 | 2092 | | CoSENT | nghuyong/
+ernie-3.0-base-zh | [shibing624/text2vec-base-chinese-sentence](https://
+huggingface.co/shibing624/text2vec-base-chinese-sentence) | 43.37 | 61.43 |
+73.48 | 38.90 | 78.25 | 70.60 | 53.08 | 59.87 | 3089 | | CoSENT | nghuyong/
+ernie-3.0-base-zh | [shibing624/text2vec-base-chinese-paraphrase](https://
+huggingface.co/shibing624/text2vec-base-chinese-paraphrase) | 44.89 | 63.58 |
+74.24 | 40.90 | 78.93 | 76.70 | 63.30 | **63.08** | 3066 | | CoSENT | sentence-
+transformers/paraphrase-multilingual-MiniLM-L12-v2 | [shibing624/text2vec-base-
+multilingual](https://huggingface.co/shibing624/text2vec-base-multilingual) |
+32.39 | 50.33 | 65.64 | 32.56 | 74.45 | 68.88 | 51.17 | 53.67 | 3138 |
+è¯´æï¼ - ç»æè¯æµææ ï¼spearmanç³»æ° - `shibing624/text2vec-base-
 chinese`æ¨¡åï¼æ¯ç¨CoSENTæ¹æ³è®­ç»ï¼åºäº`hfl/chinese-macbert-
 base`å¨ä¸­æSTS-Bæ°æ®è®­ç»å¾å°ï¼å¹¶å¨ä¸­æSTS-
 Bæµè¯éè¯ä¼°è¾¾å°è¾å¥½ææï¼è¿è¡[examples/
 training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/
 blob/master/examples/
 training_sup_text_matching_model.py)ä»£ç å¯è®­ç»æ¨¡åï¼æ¨¡åæä»¶å·²ç»ä¸ä¼ HF
 model hubï¼ä¸­æéç¨è¯­ä¹å¹éä»»å¡æ¨èä½¿ç¨ - `shibing624/text2vec-
@@ -137,81 +155,83 @@
 [shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://
 huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-
 sentence-dataset)å å¥äºs2p(sentence to
 paraphrase)æ°æ®ï¼å¼ºåäºå¶é¿ææ¬çè¡¨å¾è½åï¼å¹¶å¨ä¸­æåNLIæµè¯éè¯ä¼°è¾¾å°SOTAï¼è¿è¡
 [examples/training_sup_text_matching_model_jsonl_data.py](https://github.com/
 shibing624/text2vec/blob/master/examples/
 training_sup_text_matching_model_jsonl_data.py)ä»£ç å¯è®­ç»æ¨¡åï¼æ¨¡åæä»¶å·²ç»ä¸ä¼ HF
-model hubï¼ä¸­æs2p(å¥å­vsæ®µè½)è¯­ä¹å¹éä»»å¡æ¨èä½¿ç¨ - `SBERT-
-macbert-base`æ¨¡åï¼æ¯ç¨SBERTæ¹æ³è®­ç»ï¼è¿è¡[examples/
-training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/
-blob/master/examples/training_sup_text_matching_model.py)ä»£ç å¯è®­ç»æ¨¡å
-- `sentence-transformers/paraphrase-multilingual-MiniLM-L12-
-v2`æ¨¡åæ¯ç¨SBERTè®­ç»ï¼æ¯`paraphrase-MiniLM-L12-
-v2`æ¨¡åçå¤è¯­è¨çæ¬ï¼æ¯æä¸­æãè±æç­ - `w2v-light-tencent-
+model hubï¼ä¸­æs2p(å¥å­vsæ®µè½)è¯­ä¹å¹éä»»å¡æ¨èä½¿ç¨ -
+`shibing624/text2vec-base-
+multilingual`æ¨¡åï¼æ¯ç¨CoSENTæ¹æ³è®­ç»ï¼åºäº`sentence-transformers/
+paraphrase-multilingual-MiniLM-L12-
+v2`ç¨äººå·¥æéåçå¤è¯­è¨STSæ°æ®é[shibing624/nli-zh-all/text2vec-
+base-multilingual-dataset](https://huggingface.co/datasets/shibing624/nli-zh-
+all/tree/main/text2vec-base-multilingual-
+dataset)è®­ç»å¾å°ï¼å¹¶å¨ä¸­è±ææµè¯éè¯ä¼°ç¸å¯¹äºåæ¨¡åææææåï¼è¿è¡
+[examples/training_sup_text_matching_model_jsonl_data.py](https://github.com/
+shibing624/text2vec/blob/master/examples/
+training_sup_text_matching_model_jsonl_data.py)ä»£ç å¯è®­ç»æ¨¡åï¼æ¨¡åæä»¶å·²ç»ä¸ä¼ HF
+model hubï¼å¤è¯­è¨è¯­ä¹å¹éä»»å¡æ¨èä½¿ç¨ - `w2v-light-tencent-
 chinese`æ¯è¾è®¯è¯åéçWord2Vecæ¨¡åï¼CPUå è½½ä½¿ç¨ï¼éç¨äºä¸­æå­é¢å¹éä»»å¡åç¼ºå°æ°æ®çå·å¯å¨æåµ
 - åé¢è®­ç»æ¨¡ååå¯ä»¥éè¿transformersè°ç¨ï¼å¦MacBERTæ¨¡åï¼`--
 model_name hfl/chinese-macbert-base` æèrobertaæ¨¡åï¼`--model_name uer/
 roberta-medium-wwm-chinese-cluecorpussmall` -
 ä¸ºæµè¯æ¨¡åçé²æ£æ§ï¼å å¥äºæªè®­ç»è¿çSOHUæµè¯éï¼ç¨äºæµè¯æ¨¡åçæ³åè½åï¼ä¸ºè¾¾å°å¼ç®±å³ç¨çå®ç¨ææï¼ä½¿ç¨äºæéå°çåä¸­æå¹éæ°æ®éï¼æ°æ®éä¹ä¸ä¼ å°HF
 datasets[é¾æ¥è§ä¸æ¹](#æ°æ®é) -
 ä¸­æå¹éä»»å¡å®éªè¡¨æï¼poolingæä¼æ¯`EncoderType.FIRST_LAST_AVG`å`EncoderType.MEAN`ï¼ä¸¤èé¢æµææå·®å¼å¾å°
 -
 ä¸­æå¹éè¯æµç»æå¤ç°ï¼å¯ä»¥ä¸è½½ä¸­æå¹éæ°æ®éå°`examples/
 data`ï¼è¿è¡[tests/test_model_spearman.py](https://github.com/shibing624/
 text2vec/blob/master/tests/test_model_spearman.py)ä»£ç å¤ç°è¯æµç»æ -
-QPSçGPUæµè¯ç¯å¢æ¯Tesla V100ï¼æ¾å­32GB # Demo Official Demo: https://
-www.mulanai.com/product/short_text_sim/ HuggingFace Demo: https://
-huggingface.co/spaces/shibing624/text2vec ![](docs/hf.png) run example:
-[examples/gradio_demo.py](https://github.com/shibing624/text2vec/blob/master/
-examples/gradio_demo.py) to see the demo: ```shell python examples/
-gradio_demo.py ``` # Install ```shell pip install torch # conda install pytorch
-pip install -U text2vec ``` or ```shell pip install torch # conda install
-pytorch pip install -r requirements.txt git clone https://github.com/
-shibing624/text2vec.git cd text2vec pip install --no-deps . ``` # Usage ##
-ææ¬åéè¡¨å¾ åºäº`pretrained model`è®¡ç®ææ¬åéï¼ ```zsh >>>
-from text2vec import SentenceModel >>> m = SentenceModel() >>> m.encode
-("å¦ä½æ´æ¢è±åç»å®é¶è¡å¡") Embedding shape: (768,) ``` example:
-[examples/computing_embeddings_demo.py](https://github.com/shibing624/text2vec/
-blob/master/examples/computing_embeddings_demo.py) ```python import sys
-sys.path.append('..') from text2vec import SentenceModel from text2vec import
-Word2Vec def compute_emb(model): # Embed a list of sentences sentences =
-[ 'å¡', 'é¶è¡å¡', 'å¦ä½æ´æ¢è±åç»å®é¶è¡å¡',
-'è±åæ´æ¹ç»å®é¶è¡å¡', 'This framework generates embeddings for each
-input sentence', 'Sentences are passed as a list of string.', 'The quick brown
-fox jumps over the lazy dog.' ] sentence_embeddings = model.encode(sentences)
-print(type(sentence_embeddings), sentence_embeddings.shape) # The result is a
-list of sentence embeddings as numpy arrays for sentence, embedding in zip
-(sentences, sentence_embeddings): print("Sentence:", sentence) print("Embedding
-shape:", embedding.shape) print("Embedding head:", embedding[:10]) print() if
-__name__ == "__main__": # ä¸­æå¥åéæ¨¡å
-(CoSENT)ï¼ä¸­æè¯­ä¹å¹éä»»å¡æ¨èï¼æ¯æfine-tuneç»§ç»­è®­ç»
-t2v_model = SentenceModel("shibing624/text2vec-base-chinese") compute_emb
-(t2v_model) # æ¯æå¤è¯­è¨çå¥åéæ¨¡åï¼Sentence-
-BERTï¼ï¼è±æè¯­ä¹å¹éä»»å¡æ¨èï¼æ¯æfine-tuneç»§ç»­è®­ç»
-sbert_model = SentenceModel("sentence-transformers/paraphrase-multilingual-
-MiniLM-L12-v2") compute_emb(sbert_model) # ä¸­æè¯åéæ¨¡å
+QPSçGPUæµè¯ç¯å¢æ¯Tesla V100ï¼æ¾å­32GB æ¨¡åè®­ç»å®éªæ¥åï¼
+[å®éªæ¥å](https://github.com/shibing624/text2vec/blob/master/docs/
+model_report.md) ## Demo Official Demo: https://www.mulanai.com/product/
+short_text_sim/ HuggingFace Demo: https://huggingface.co/spaces/shibing624/
+text2vec ![](docs/hf.png) run example: [examples/gradio_demo.py](https://
+github.com/shibing624/text2vec/blob/master/examples/gradio_demo.py) to see the
+demo: ```shell python examples/gradio_demo.py ``` ## Install ```shell pip
+install torch # conda install pytorch pip install -U text2vec ``` or ```shell
+pip install torch # conda install pytorch pip install -r requirements.txt git
+clone https://github.com/shibing624/text2vec.git cd text2vec pip install --no-
+deps . ``` ## Usage ### ææ¬åéè¡¨å¾ åºäº`pretrained
+model`è®¡ç®ææ¬åéï¼ ```zsh >>> from text2vec import SentenceModel >>> m
+= SentenceModel() >>> m.encode("å¦ä½æ´æ¢è±åç»å®é¶è¡å¡") Embedding
+shape: (768,) ``` example: [examples/computing_embeddings_demo.py](https://
+github.com/shibing624/text2vec/blob/master/examples/
+computing_embeddings_demo.py) ```python import sys sys.path.append('..') from
+text2vec import SentenceModel from text2vec import Word2Vec def compute_emb
+(model): # Embed a list of sentences sentences = [ 'å¡', 'é¶è¡å¡',
+'å¦ä½æ´æ¢è±åç»å®é¶è¡å¡', 'è±åæ´æ¹ç»å®é¶è¡å¡', 'This
+framework generates embeddings for each input sentence', 'Sentences are passed
+as a list of string.', 'The quick brown fox jumps over the lazy dog.' ]
+sentence_embeddings = model.encode(sentences) print(type(sentence_embeddings),
+sentence_embeddings.shape) # The result is a list of sentence embeddings as
+numpy arrays for sentence, embedding in zip(sentences, sentence_embeddings):
+print("Sentence:", sentence) print("Embedding shape:", embedding.shape) print
+("Embedding head:", embedding[:10]) print() if __name__ == "__main__": #
+ä¸­æå¥åéæ¨¡å(CoSENT)ï¼ä¸­æè¯­ä¹å¹éä»»å¡æ¨èï¼æ¯æfine-
+tuneç»§ç»­è®­ç» t2v_model = SentenceModel("shibing624/text2vec-base-chinese")
+compute_emb(t2v_model) #
+æ¯æå¤è¯­è¨çå¥åéæ¨¡åï¼CoSENTï¼ï¼å¤è¯­è¨ï¼åæ¬ä¸­è±æï¼è¯­ä¹å¹éä»»å¡æ¨èï¼æ¯æfine-
+tuneç»§ç»­è®­ç» sbert_model = SentenceModel("shibing624/text2vec-base-
+multilingual") compute_emb(sbert_model) # ä¸­æè¯åéæ¨¡å
 (word2vec)ï¼ä¸­æå­é¢å¹éä»»å¡åå·å¯å¨éç¨ w2v_model = Word2Vec
 ("w2v-light-tencent-chinese") compute_emb(w2v_model) ``` output: ```
 numpy.ndarray'> (7, 768) Sentence: å¡ Embedding shape: (768,) Sentence:
 é¶è¡å¡ Embedding shape: (768,) ... ``` -
 è¿åå¼`embeddings`æ¯`numpy.ndarray`ç±»åï¼shapeä¸º`(sentences_size,
 model_embedding_size)`ï¼ä¸ä¸ªæ¨¡åä»»éä¸ç§å³å¯ï¼æ¨èç¨ç¬¬ä¸ä¸ªã
 - `shibing624/text2vec-base-chinese`æ¨¡åæ¯CoSENTæ¹æ³å¨ä¸­æSTS-
 Bæ°æ®éè®­ç»å¾å°çï¼æ¨¡åå·²ç»ä¸ä¼ å°huggingfaceç æ¨¡ååº
 [shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-
 base-chinese)ï¼
 æ¯`text2vec.SentenceModel`æå®çé»è®¤æ¨¡åï¼å¯ä»¥éè¿ä¸é¢ç¤ºä¾è°ç¨ï¼æèå¦ä¸æç¤ºç¨
 [transformersåº](https://github.com/huggingface/transformers)è°ç¨ï¼
-æ¨¡åèªå¨ä¸è½½å°æ¬æºè·¯å¾ï¼`~/.cache/huggingface/transformers` -
-`sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`æ¨¡åæ¯Sentence-
-BERTçå¤è¯­è¨å¥åéæ¨¡åï¼
-éç¨äºéä¹ï¼paraphraseï¼è¯å«ï¼ææ¬å¹éï¼éè¿`text2vec.SentenceModel`å
-[sentence-transformersåº]((https://github.com/UKPLab/sentence-
-transformers))é½å¯ä»¥è°ç¨è¯¥æ¨¡å - `w2v-light-tencent-
+æ¨¡åèªå¨ä¸è½½å°æ¬æºè·¯å¾ï¼`~/.cache/huggingface/transformers` - `w2v-
+light-tencent-
 chinese`æ¯éè¿gensimå è½½çWord2Vecæ¨¡åï¼ä½¿ç¨è¾è®¯è¯åé`Tencent_AILab_ChineseEmbedding.tar.gz`è®¡ç®åå­è¯çè¯åéï¼å¥å­åééè¿åè¯è¯
 åéåå¹³åå¼å¾å°ï¼æ¨¡åèªå¨ä¸è½½å°æ¬æºè·¯å¾ï¼`~/.text2vec/
 datasets/light_Tencent_AILab_ChineseEmbedding.bin` #### Usage (HuggingFace
 Transformers) Without [text2vec](https://github.com/shibing624/text2vec), you
 can use the model like this: First, you pass your input through the transformer
 model, then you have to apply the right pooling-operation on-top of the
 contextualized word embeddings. example: [examples/
@@ -322,16 +342,16 @@
 ææ¬ç¸ä¼¼åº¦è®¡ç®åææ¬å¹éæç´¢ä»»å¡ï¼æ¨èä½¿ç¨
 [similaritiesåº](https://github.com/shibing624/similarities)
 ï¼å¼å®¹æ¬é¡¹ç®releaseç
 Word2vecãSBERTãCosentç±»è¯­ä¹å¹éæ¨¡åï¼è¿æ¯æå­é¢ç»´åº¦ç¸ä¼¼åº¦è®¡ç®ãå¹éæç´¢ç®æ³ï¼æ¯æææ¬ãå¾åã
 å®è£ï¼ ```pip install -U similarities``` å¥å­ç¸ä¼¼åº¦è®¡ç®ï¼ ```python
 from similarities import Similarity m = Similarity() r = m.similarity
 ('å¦ä½æ´æ¢è±åç»å®é¶è¡å¡', 'è±åæ´æ¹ç»å®é¶è¡å¡') print
-(f"similarity score: {float(r)}") # similarity score: 0.855146050453186 ``` #
-Models ## CoSENT model CoSENTï¼Cosine
+(f"similarity score: {float(r)}") # similarity score: 0.855146050453186 ``` ##
+Models ### CoSENT model CoSENTï¼Cosine
 Sentenceï¼ææ¬å¹éæ¨¡åï¼å¨Sentence-
 BERTä¸æ¹è¿äºCosineRankLossçå¥åéæ¹æ¡ Network structure: Training:
 [docs/cosent_train.png] Inference: [docs/inference.png] #### CoSENT
 çç£æ¨¡å è®­ç»åé¢æµCoSENTæ¨¡åï¼ - å¨ä¸­æSTS-
 Bæ°æ®éè®­ç»åè¯ä¼°`CoSENT`æ¨¡å example: [examples/
 training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/
 blob/master/examples/training_sup_text_matching_model.py) ```shell cd examples
@@ -343,21 +363,24 @@
 'PAWSX'ï¼å·ä½åèHuggingFace datasets [https://huggingface.co/datasets/
 shibing624/nli_zh](https://huggingface.co/datasets/shibing624/nli_zh) ```shell
 python training_sup_text_matching_model.py --task_name ATEC --model_arch cosent
 --do_train --do_predict --num_epochs 10 --model_name hfl/chinese-macbert-base -
 -output_dir ./outputs/ATEC-cosent ``` - å¨èªæä¸­ææ°æ®éä¸è®­ç»æ¨¡å
 example: [examples/training_sup_text_matching_model_mydata.py](https://
 github.com/shibing624/text2vec/blob/master/examples/
-training_sup_text_matching_model_mydata.py) ```shell python
-training_sup_text_matching_model_mydata.py --do_train --do_predict ```
-è®­ç»éæ ¼å¼åè[examples/data/STS-B/STS-B.valid.data](https://github.com/
-shibing624/text2vec/blob/master/examples/data/STS-B/STS-B.valid.data) ```shell
-sentence1 sentence2 label ä¸ä¸ªå¥³å­©å¨ç»å¥¹çå¤´ååååã
-ä¸ä¸ªå¥³å­©å¨æ¢³å¤´ã 2 ä¸ç¾¤ç·äººå¨æµ·æ»©ä¸è¸¢è¶³çã
-ä¸ç¾¤ç·å­©å¨æµ·æ»©ä¸è¸¢è¶³çã 3
+training_sup_text_matching_model_mydata.py) åå¡è®­ç»ï¼ ```shell
+CUDA_VISIBLE_DEVICES=0 python training_sup_text_matching_model_mydata.py --
+do_train --do_predict ``` å¤å¡è®­ç»ï¼ ```shell CUDA_VISIBLE_DEVICES=0,1
+torchrun --nproc_per_node 2 training_sup_text_matching_model_mydata.py --
+do_train --do_predict --output_dir outputs/STS-B-text2vec-macbert-v1 --
+batch_size 64 --fp16 --data_parallel ``` è®­ç»éæ ¼å¼åè[examples/data/
+STS-B/STS-B.valid.data](https://github.com/shibing624/text2vec/blob/master/
+examples/data/STS-B/STS-B.valid.data) ```shell sentence1 sentence2 label
+ä¸ä¸ªå¥³å­©å¨ç»å¥¹çå¤´ååååã ä¸ä¸ªå¥³å­©å¨æ¢³å¤´ã 2
+ä¸ç¾¤ç·äººå¨æµ·æ»©ä¸è¸¢è¶³çã ä¸ç¾¤ç·å­©å¨æµ·æ»©ä¸è¸¢è¶³çã 3
 ä¸ä¸ªå¥³äººå¨æµéå¦ä¸ä¸ªå¥³äººçèè¸ã
 å¥³äººæµéå¦ä¸ä¸ªå¥³äººçèè¸ã 5 ```
 `label`å¯ä»¥æ¯0ï¼1æ ç­¾ï¼0ä»£è¡¨ä¸¤ä¸ªå¥å­ä¸ç¸ä¼¼ï¼1ä»£è¡¨ç¸ä¼¼ï¼ä¹å¯ä»¥æ¯0-
 5çè¯åï¼è¯åè¶é«ï¼è¡¨ç¤ºä¸¤ä¸ªå¥å­è¶ç¸ä¼¼ãæ¨¡åé½è½æ¯æã
 - å¨è±æSTS-Bæ°æ®éè®­ç»åè¯ä¼°`CoSENT`æ¨¡å example: [examples/
 training_sup_text_matching_model_en.py](https://github.com/shibing624/text2vec/
 blob/master/examples/training_sup_text_matching_model_en.py) ```shell cd
@@ -366,15 +389,15 @@
 output_dir ./outputs/STS-B-en-cosent ``` #### CoSENT æ çç£æ¨¡å -
 å¨è±æNLIæ°æ®éè®­ç»`CoSENT`æ¨¡åï¼å¨STS-Bæµè¯éè¯ä¼°ææ
 example: [examples/training_unsup_text_matching_model_en.py](https://
 github.com/shibing624/text2vec/blob/master/examples/
 training_unsup_text_matching_model_en.py) ```shell cd examples python
 training_unsup_text_matching_model_en.py --model_arch cosent --do_train --
 do_predict --num_epochs 10 --model_name bert-base-uncased --output_dir ./
-outputs/STS-B-en-unsup-cosent ``` ## Sentence-BERT model Sentence-
+outputs/STS-B-en-unsup-cosent ``` ### Sentence-BERT model Sentence-
 BERTææ¬å¹éæ¨¡åï¼è¡¨å¾å¼å¥åéè¡¨ç¤ºæ¹æ¡ Network structure:
 Training: [docs/sbert_train.png] Inference: [docs/sbert_inference.png] ####
 SentenceBERT çç£æ¨¡å - å¨ä¸­æSTS-Bæ°æ®éè®­ç»åè¯ä¼°`SBERT`æ¨¡å
 example: [examples/training_sup_text_matching_model.py](https://github.com/
 shibing624/text2vec/blob/master/examples/training_sup_text_matching_model.py)
 ```shell cd examples python training_sup_text_matching_model.py --model_arch
 sentencebert --do_train --do_predict --num_epochs 10 --model_name hfl/chinese-
@@ -387,35 +410,35 @@
 uncased --output_dir ./outputs/STS-B-en-sbert ``` #### SentenceBERT
 æ çç£æ¨¡å - å¨è±æNLIæ°æ®éè®­ç»`SBERT`æ¨¡åï¼å¨STS-
 Bæµè¯éè¯ä¼°ææ example: [examples/
 training_unsup_text_matching_model_en.py](https://github.com/shibing624/
 text2vec/blob/master/examples/training_unsup_text_matching_model_en.py)
 ```shell cd examples python training_unsup_text_matching_model_en.py --
 model_arch sentencebert --do_train --do_predict --num_epochs 10 --model_name
-bert-base-uncased --output_dir ./outputs/STS-B-en-unsup-sbert ``` ## BERT-Match
-model
+bert-base-uncased --output_dir ./outputs/STS-B-en-unsup-sbert ``` ### BERT-
+Match model
 BERTææ¬å¹éæ¨¡åï¼åçBERTå¹éç½ç»ç»æï¼äº¤äºå¼å¥åéå¹éæ¨¡å
 Network structure: Training and inference: [docs/bert-fc-train.png]
 è®­ç»èæ¬åä¸[examples/training_sup_text_matching_model.py](https://
 github.com/shibing624/text2vec/blob/master/examples/
-training_sup_text_matching_model.py)ã ## æ¨¡åè¸é¦ï¼Model Distillationï¼
-ç±äºtext2vecè®­ç»çæ¨¡åå¯ä»¥ä½¿ç¨[sentence-transformers](https://
-github.com/UKPLab/sentence-
+training_sup_text_matching_model.py)ã ### æ¨¡åè¸é¦ï¼Model
+Distillationï¼ ç±äºtext2vecè®­ç»çæ¨¡åå¯ä»¥ä½¿ç¨[sentence-
+transformers](https://github.com/UKPLab/sentence-
 transformers)åºå è½½ï¼æ­¤å¤å¤ç¨å¶æ¨¡åè¸é¦æ¹æ³[distillation](https:
 //github.com/UKPLab/sentence-transformers/tree/master/examples/training/
 distillation)ã 1. æ¨¡åéç»´ï¼åè[dimensionality_reduction.py](https://
 github.com/UKPLab/sentence-transformers/blob/master/examples/training/
 distillation/
 dimensionality_reduction.py)ä½¿ç¨PCAå¯¹æ¨¡åè¾åºembeddingéç»´ï¼å¯åå°milvusç­åéæ£ç´¢æ°æ®åºçå­å¨ååï¼è¿è½è½»å¾®æåæ¨¡åææã
 2. æ¨¡åè¸é¦ï¼åè[model_distillation.py](https://github.com/UKPLab/
 sentence-transformers/blob/master/examples/training/distillation/
 model_distillation.py)ä½¿ç¨è¸é¦æ¹æ³ï¼å°Teacherå¤§æ¨¡åè¸é¦å°æ´å°layerså±æ°çstudentæ¨¡åä¸­ï¼å¨æè¡¡ææçæåµä¸ï¼å¯å¤§å¹æåæ¨¡åé¢æµéåº¦ã
-## æ¨¡åé¨ç½² æä¾ä¸¤ç§é¨ç½²æ¨¡åï¼æ­å»ºæå¡çæ¹æ³ï¼
+### æ¨¡åé¨ç½² æä¾ä¸¤ç§é¨ç½²æ¨¡åï¼æ­å»ºæå¡çæ¹æ³ï¼
 1ï¼åºäºJinaæ­å»ºgRPCæå¡ãæ¨èãï¼2ï¼åºäºFastAPIæ­å»ºåçHttpæå¡ã
-### Jinaæå¡ éç¨C/
+#### Jinaæå¡ éç¨C/
 Sæ¨¡å¼æ­å»ºé«æ§è½æå¡ï¼æ¯ædockeräºåçï¼gRPC/HTTP/
 WebSocketï¼æ¯æå¤ä¸ªæ¨¡ååæ¶é¢æµï¼GPUå¤å¡å¤çã - å®è£ï¼
 ```pip install jina``` - å¯å¨æå¡ï¼ example: [examples/
 jina_server_demo.py](examples/jina_server_demo.py) ```python from jina import
 Flow port = 50001 f = Flow(port=port).add( uses='jinahub://Text2vecEncoder',
 uses_with={'model_name': 'shibing624/text2vec-base-chinese'} ) with f: #
 backend server forever f.block() ```
@@ -424,27 +447,27 @@
 è°ç¨æå¡ï¼ ```python from jina import Client from docarray import
 Document, DocumentArray port = 50001 c = Client(port=port) data =
 ['å¦ä½æ´æ¢è±åç»å®é¶è¡å¡', 'è±åæ´æ¹ç»å®é¶è¡å¡'] print
 ("data:", data) print('data embs:') r = c.post('/', inputs=DocumentArray(
 [Document(text='å¦ä½æ´æ¢è±åç»å®é¶è¡å¡'), Document
 (text='è±åæ´æ¹ç»å®é¶è¡å¡')])) print(r.embeddings) ```
 æ¹éè°ç¨æ¹æ³è§example: [examples/jina_client_demo.py](https://
-github.com/shibing624/text2vec/blob/master/examples/jina_client_demo.py) ###
+github.com/shibing624/text2vec/blob/master/examples/jina_client_demo.py) ####
 FastAPIæå¡ - å®è£ï¼ ```pip install fastapi uvicorn``` - å¯å¨æå¡ï¼
 example: [examples/fastapi_server_demo.py](https://github.com/shibing624/
 text2vec/blob/master/examples/fastapi_server_demo.py) ```shell cd examples
 python fastapi_server_demo.py ``` - è°ç¨æå¡ï¼ ```shell curl -X 'GET' \
 'http://0.0.0.0:8001/emb?q=hello' \ -H 'accept: application/json' ``` ##
-æ°æ®é - æ¬é¡¹ç®releaseçæ°æ®éï¼ | Dataset | Introduce | Download
-Link | |:---------------------------|:-----------------------------------------
---------------------------------|:---------------------------------------------
+Dataset - æ¬é¡¹ç®releaseçæ°æ®éï¼ | Dataset | Introduce | Download Link
+| |:---------------------------|:----------------------------------------------
+---------------------------|:--------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
-------------| | shibing624/nli-zh-all |
+-------| | shibing624/nli-zh-all |
 ä¸­æè¯­ä¹å¹éæ°æ®åéï¼æ´åäºææ¬æ¨çï¼ç¸ä¼¼ï¼æè¦ï¼é®ç­ï¼æä»¤å¾®è°ç­ä»»å¡ç820ä¸é«è´¨éæ°æ®ï¼å¹¶è½¬åä¸ºå¹éæ ¼å¼æ°æ®é
 | [https://huggingface.co/datasets/shibing624/nli-zh-all](https://
 huggingface.co/datasets/shibing624/nli-zh-all) | | shibing624/snli-zh |
 ä¸­æSNLIåMultiNLIæ°æ®éï¼ç¿»è¯èªè±æSNLIåMultiNLI | [https://
 huggingface.co/datasets/shibing624/snli-zh](https://huggingface.co/datasets/
 shibing624/snli-zh) | | shibing624/nli_zh |
 ä¸­æè¯­ä¹å¹éæ°æ®éï¼æ´åäºä¸­æATECãBQãLCQMCãPAWSXãSTS-
@@ -462,46 +485,46 @@
 info/1037/1162.htm) | | LCQMC | ä¸­æLCQMC(large-scale Chinese question
 matching corpus)æ°æ®éï¼Q-Qpairæ°æ®é | [LCQMC](http://
 icrc.hitsz.edu.cn/Article/show/171.html) | | PAWSX | ä¸­æPAWS(Paraphrase
 Adversaries from Word Scrambling)æ°æ®éï¼Q-Qpairæ°æ®é | [PAWSX](https:/
 /arxiv.org/abs/1908.11828) | | STS-B | ä¸­æSTS-
 Bæ°æ®éï¼ä¸­æèªç¶è¯­è¨æ¨çæ°æ®éï¼ä»è±æSTS-
 Bç¿»è¯ä¸ºä¸­æçæ°æ®é | [STS-B](https://github.com/pluto-junzeng/CNSD) |
-å¸¸ç¨è±æå¹éæ°æ®éï¼ - å¤§åé¼é¼çmulti_nliåsnli: https://
-huggingface.co/datasets/multi_nli - å¤§åé¼é¼çmulti_nliåsnli: https://
+å¸¸ç¨è±æå¹éæ°æ®éï¼ - è±æå¹éæ°æ®éï¼multi_nli: https://
+huggingface.co/datasets/multi_nli - è±æå¹éæ°æ®éï¼snli: https://
 huggingface.co/datasets/snli - https://huggingface.co/datasets/metaeval/cnli -
 https://huggingface.co/datasets/mteb/stsbenchmark-sts - https://huggingface.co/
 datasets/JeremiahZ/simcse_sup_nli - https://huggingface.co/datasets/
 MoritzLaurer/multilingual-NLI-26lang-2mil7 æ°æ®éä½¿ç¨ç¤ºä¾ï¼ ```shell
 pip install datasets ``` ```python from datasets import load_dataset dataset =
 load_dataset("shibing624/nli_zh", "STS-B") # ATEC or BQ or LCQMC or PAWSX or
 STS-B print(dataset) print(dataset['test'][0]) ``` output: ```shell DatasetDict
 ({ train: Dataset({ features: ['sentence1', 'sentence2', 'label'], num_rows:
 5231 }) validation: Dataset({ features: ['sentence1', 'sentence2', 'label'],
 num_rows: 1458 }) test: Dataset({ features: ['sentence1', 'sentence2',
 'label'], num_rows: 1361 }) }) {'sentence1':
 'ä¸ä¸ªå¥³å­©å¨ç»å¥¹çå¤´ååååã', 'sentence2':
-'ä¸ä¸ªå¥³å­©å¨æ¢³å¤´ã', 'label': 2} ``` # Contact - Issue(å»ºè®®)ï¼[!
+'ä¸ä¸ªå¥³å­©å¨æ¢³å¤´ã', 'label': 2} ``` ## Contact - Issue(å»ºè®®)ï¼[!
 [GitHub issues](https://img.shields.io/github/issues/shibing624/text2vec.svg)]
 (https://github.com/shibing624/text2vec/issues) - é®ä»¶æï¼xuming:
 xuming624@qq.com - å¾®ä¿¡æï¼å æ*å¾®ä¿¡å·ï¼xuming624, å¤æ³¨ï¼å§å-
-å¬å¸-NLP* è¿NLPäº¤æµç¾¤ã [docs/wechat.jpeg] # Citation
+å¬å¸-NLP* è¿NLPäº¤æµç¾¤ã [docs/wechat.jpeg] ## Citation
 å¦æä½ å¨ç ç©¶ä¸­ä½¿ç¨äºtext2vecï¼è¯·æå¦ä¸æ ¼å¼å¼ç¨ï¼ APA:
 ```latex Xu, M. Text2vec: Text to vector toolkit (Version 1.1.2) [Computer
 software]. https://github.com/shibing624/text2vec ``` BibTeX: ```latex @misc
-{Text2vec, author = {Xu, Ming}, title = {Text2vec: Text to vector toolkit},
-year = {2022}, publisher = {GitHub}, journal = {GitHub repository},
-howpublished = {\url{https://github.com/shibing624/text2vec}}, } ``` # License
+{Text2vec, author = {Ming Xu}, title = {Text2vec: Text to vector toolkit}, year
+= {2023}, publisher = {GitHub}, journal = {GitHub repository}, howpublished =
+{\url{https://github.com/shibing624/text2vec}}, } ``` ## License
 ææåè®®ä¸º [The Apache License 2.0]
 (LICENSE)ï¼å¯åè´¹ç¨ååä¸ç¨éãè¯·å¨äº§åè¯´æä¸­éå text2vecçé¾æ¥åææåè®®ã
-# Contribute
+## Contribute
 é¡¹ç®ä»£ç è¿å¾ç²ç³ï¼å¦æå¤§å®¶å¯¹ä»£ç æææ¹è¿ï¼æ¬¢è¿æäº¤åæ¬é¡¹ç®ï¼å¨æäº¤ä¹åï¼æ³¨æä»¥ä¸ä¸¤ç¹ï¼
 - å¨`tests`æ·»å ç¸åºçååæµè¯ - ä½¿ç¨`python -m pytest -
 v`æ¥è¿è¡ææååæµè¯ï¼ç¡®ä¿ææåæµé½æ¯éè¿ç
-ä¹åå³å¯æäº¤PRã # Reference -
+ä¹åå³å¯æäº¤PRã ## References -
 [å°å¥å­è¡¨ç¤ºä¸ºåéï¼ä¸ï¼ï¼æ çç£å¥å­è¡¨ç¤ºå­¦ä¹ ï¼sentence
 embeddingï¼](https://www.cnblogs.com/llhthinker/p/10335164.html) -
 [å°å¥å­è¡¨ç¤ºä¸ºåéï¼ä¸ï¼ï¼æ çç£å¥å­è¡¨ç¤ºå­¦ä¹ ï¼sentence
 embeddingï¼](https://www.cnblogs.com/llhthinker/p/10341841.html) - [A Simple
 but Tough-to-Beat Baseline for Sentence Embeddings[Sanjeev Arora and Yingyu
 Liang and Tengyu Ma, 2017]](https://openreview.net/forum?id=SyK00v5xx) -
 [åç§è®¡ç®ææ¬ç¸ä¼¼åº¦çæ¹æ³å¯¹æ¯[Yves Peirsman]](https://
```

### Comparing `text2vec-1.2.1/README.md` & `text2vec-1.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,54 +19,57 @@
 
 
 **Text2vec**: Text to Vector, Get Sentence Embeddings. 文本向量化，把文本(包括词、句子、段落)表征为向量矩阵。
 
 **text2vec**实现了Word2Vec、RankBM25、BERT、Sentence-BERT、CoSENT等多种文本表征、文本相似度计算模型，并在文本语义匹配（相似度计算）任务上比较了各模型的效果。
 
 ### News
+[2023/06/22] v1.2.2版本: 发布了多语言匹配模型[shibing624/text2vec-base-multilingual](https://huggingface.co/shibing624/text2vec-base-multilingual)，用CoSENT方法训练，基于`sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`用人工挑选后的多语言STS数据集[shibing624/nli-zh-all/text2vec-base-multilingual-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-multilingual-dataset)训练得到，并在中英文测试集评估相对于原模型效果有提升，详见[Release-v1.2.2](https://github.com/shibing624/text2vec/releases/tag/1.2.2)
+
 [2023/06/19] v1.2.1版本: 更新了中文匹配模型`shibing624/text2vec-base-chinese-nli`为新版[shibing624/text2vec-base-chinese-sentence](https://huggingface.co/shibing624/text2vec-base-chinese-sentence)，针对CoSENT的loss计算对排序敏感特点，人工挑选并整理出高质量的有相关性排序的STS数据集[shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-sentence-dataset)，在各评估集表现相对之前有提升；发布了适用于s2p的中文匹配模型[shibing624/text2vec-base-chinese-paraphrase](https://huggingface.co/shibing624/text2vec-base-chinese-paraphrase)，详见[Release-v1.2.1](https://github.com/shibing624/text2vec/releases/tag/1.2.1)
 
 [2023/06/15] v1.2.0版本: 发布了中文匹配模型[shibing624/text2vec-base-chinese-nli](https://huggingface.co/shibing624/text2vec-base-chinese-nli)，基于`nghuyong/ernie-3.0-base-zh`模型，使用了中文NLI数据集[shibing624/nli_zh](https://huggingface.co/datasets/shibing624/nli_zh)全部语料训练的CoSENT文本匹配模型，在各评估集表现提升明显，详见[Release-v1.2.0](https://github.com/shibing624/text2vec/releases/tag/1.2.0)
 
 [2022/03/12] v1.1.4版本: 发布了中文匹配模型[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)，基于中文STS训练集训练的CoSENT匹配模型。详见[Release-v1.1.4](https://github.com/shibing624/text2vec/releases/tag/1.1.4)
 
 
 **Guide**
-- [Feature](#Feature)
+- [Features](#Features)
 - [Evaluation](#Evaluation)
 - [Install](#install)
 - [Usage](#usage)
 - [Contact](#Contact)
-- [Reference](#reference)
+- [References](#references)
 
 
-# Feature
+## Features
 ### 文本向量表示模型
 - [Word2Vec](https://github.com/shibing624/text2vec/blob/master/text2vec/word2vec.py)：通过腾讯AI Lab开源的大规模高质量中文[词向量数据（800万中文词轻量版）](https://pan.baidu.com/s/1La4U4XNFe8s5BJqxPQpeiQ) (文件名：light_Tencent_AILab_ChineseEmbedding.bin 密码: tawe）实现词向量检索，本项目实现了句子（词向量求平均）的word2vec向量表示
 - [SBERT(Sentence-BERT)](https://github.com/shibing624/text2vec/blob/master/text2vec/sentencebert_model.py)：权衡性能和效率的句向量表示模型，训练时通过有监督训练上层分类函数，文本匹配预测时直接句子向量做余弦，本项目基于PyTorch复现了Sentence-BERT模型的训练和预测
 - [CoSENT(Cosine Sentence)](https://github.com/shibing624/text2vec/blob/master/text2vec/cosent_model.py)：CoSENT模型提出了一种排序的损失函数，使训练过程更贴近预测，模型收敛速度和效果比Sentence-BERT更好，本项目基于PyTorch实现了CoSENT模型的训练和预测
 
 详细文本向量表示方法见wiki: [文本向量表示方法](https://github.com/shibing624/text2vec/wiki/%E6%96%87%E6%9C%AC%E5%90%91%E9%87%8F%E8%A1%A8%E7%A4%BA%E6%96%B9%E6%B3%95)
-# Evaluation
+## Evaluation
 
 文本匹配
 
 #### 英文匹配数据集的评测结果：
 
 
-| Arch   | BaseModel                                        | Model                            | English-STS-B | 
-|:-------|:------------------------------------------------|:-------------------------------------|:-------------:|
-| GloVe  | glove                                           | Avg_word_embeddings_glove_6B_300d    |     61.77     |
-| BERT   | bert-base-uncased                               | BERT-base-cls                        |     20.29     |
-| BERT   | bert-base-uncased                               | BERT-base-first_last_avg             |     59.04     |
-| BERT   | bert-base-uncased                               | BERT-base-first_last_avg-whiten(NLI) |     63.65     |
-| SBERT  | sentence-transformers/bert-base-nli-mean-tokens | SBERT-base-nli-cls                   |     73.65     |
-| SBERT  | sentence-transformers/bert-base-nli-mean-tokens | SBERT-base-nli-first_last_avg        |     77.96     |
-| CoSENT | bert-base-uncased                               | CoSENT-base-first_last_avg           |     69.93     |
-| CoSENT | sentence-transformers/bert-base-nli-mean-tokens | CoSENT-base-nli-first_last_avg       |     79.68     |
+| Arch   | BaseModel                                        | Model                                                                                                                | English-STS-B | 
+|:-------|:------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------|:-------------:|
+| GloVe  | glove                                           | Avg_word_embeddings_glove_6B_300d                                                                                    |     61.77     |
+| BERT   | bert-base-uncased                               | BERT-base-cls                                                                                                        |     20.29     |
+| BERT   | bert-base-uncased                               | BERT-base-first_last_avg                                                                                             |     59.04     |
+| BERT   | bert-base-uncased                               | BERT-base-first_last_avg-whiten(NLI)                                                                                 |     63.65     |
+| SBERT  | sentence-transformers/bert-base-nli-mean-tokens | SBERT-base-nli-cls                                                                                                   |     73.65     |
+| SBERT  | sentence-transformers/bert-base-nli-mean-tokens | SBERT-base-nli-first_last_avg                                                                                        |     77.96     |
+| CoSENT | bert-base-uncased                               | CoSENT-base-first_last_avg                                                                                           |     69.93     |
+| CoSENT | sentence-transformers/bert-base-nli-mean-tokens | CoSENT-base-nli-first_last_avg                                                                                       |     79.68     |
+| CoSENT | sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2 | [shibing624/text2vec-base-multilingual](https://huggingface.co/shibing624/text2vec-base-multilingual)                |     80.12     |
 
 #### 中文匹配数据集的评测结果：
 
 
 | Arch   | BaseModel                    | Model           | ATEC  |  BQ   | LCQMC | PAWSX | STS-B |  Avg  | 
 |:-------|:----------------------------|:--------------------|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|
 | SBERT  | bert-base-chinese           | SBERT-bert-base     | 46.36 | 70.36 | 78.72 | 46.86 | 66.41 | 61.74 |
@@ -75,59 +78,60 @@
 | CoSENT | bert-base-chinese           | CoSENT-bert-base    | 49.74 | 72.38 | 78.69 | 60.00 | 79.27 | 68.01 |
 | CoSENT | hfl/chinese-macbert-base    | CoSENT-macbert-base | 50.39 | 72.93 | 79.17 | 60.86 | 79.30 | 68.53 |
 | CoSENT | hfl/chinese-roberta-wwm-ext | CoSENT-roberta-ext  | 50.81 | 71.45 | 79.31 | 61.56 | 79.96 | 68.61 |
 
 说明：
 - 结果评测指标：spearman系数
 - 为评测模型能力，结果均只用该数据集的train训练，在test上评估得到的表现，没用外部数据
+- `SBERT-macbert-base`模型，是用SBert方法训练，运行[examples/training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model.py)代码可训练模型
+- `sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`模型是用SBert训练，是`paraphrase-MiniLM-L12-v2`模型的多语言版本，支持中文、英文等
 
 
 ### Release Models
 - 本项目release模型的中文匹配评测结果：
 
-| Arch       | BaseModel                         | Model                                                                                                                                             | ATEC  |  BQ   | LCQMC | PAWSX | STS-B | SOHU-dd | SOHU-dc |    Avg    |  QPS  |
-|:-----------|:----------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------|:-----:|:-----:|:-----:|:-----:|:-----:|:-------:|:-------:|:---------:|:-----:|
-| Word2Vec   | word2vec                          | [w2v-light-tencent-chinese](https://ai.tencent.com/ailab/nlp/en/download.html)                                                                    | 20.00 | 31.49 | 59.46 | 2.57  | 55.78 |  55.04  |  20.70  |   35.03   | 23769 |
-| SBERT      | xlm-roberta-base                  | [sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2](https://huggingface.co/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2) | 18.42 | 38.52 | 63.96 | 10.14 | 78.90 |  63.01  |  52.28  |   46.46   | 3138  |
-| Instructor | hfl/chinese-roberta-wwm-ext       | [moka-ai/m3e-base](https://huggingface.co/moka-ai/m3e-base)                                                                                       | 41.27 | 63.81 | 74.87 | 12.20 | 76.96 |  75.83  |  60.55  |   57.93   | 2980  |
-| CoSENT     | hfl/chinese-macbert-base          | [shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)                                                       | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 |  70.27  |  50.42  |   51.61   | 3008  |
-| CoSENT     | hfl/chinese-lert-large            | [GanymedeNil/text2vec-large-chinese](https://huggingface.co/GanymedeNil/text2vec-large-chinese)                                                   | 32.61 | 44.59 | 69.30 | 14.51 | 79.44 |  73.01  |  59.04  |   53.12   | 2092  |
-| CoSENT     | nghuyong/ernie-3.0-base-zh        | [shibing624/text2vec-base-chinese-sentence](https://huggingface.co/shibing624/text2vec-base-chinese-sentence)                                     | 43.37 | 61.43 | 73.48 | 38.90 | 78.25 |  70.60  |  53.08  |   59.87   | 3089  |
-| CoSENT     | nghuyong/ernie-3.0-base-zh        | [shibing624/text2vec-base-chinese-paraphrase](https://huggingface.co/shibing624/text2vec-base-chinese-paraphrase)                                 | 44.89 | 63.58 | 74.24 | 40.90 | 78.93 |  76.70  |  63.30  | **63.08** | 3066  |
+| Arch       | BaseModel                                                    | Model                                                                                                                                             | ATEC  |  BQ   | LCQMC | PAWSX | STS-B | SOHU-dd | SOHU-dc |    Avg    |  QPS  |
+|:-----------|:-------------------------------------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------|:-----:|:-----:|:-----:|:-----:|:-----:|:-------:|:-------:|:---------:|:-----:|
+| Word2Vec   | word2vec                                                     | [w2v-light-tencent-chinese](https://ai.tencent.com/ailab/nlp/en/download.html)                                                                    | 20.00 | 31.49 | 59.46 | 2.57  | 55.78 |  55.04  |  20.70  |   35.03   | 23769 |
+| SBERT      | xlm-roberta-base                                             | [sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2](https://huggingface.co/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2) | 18.42 | 38.52 | 63.96 | 10.14 | 78.90 |  63.01  |  52.28  |   46.46   | 3138  |
+| CoSENT     | hfl/chinese-macbert-base                                     | [shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)                                                       | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 |  70.27  |  50.42  |   51.61   | 3008  |
+| CoSENT     | hfl/chinese-lert-large                                       | [GanymedeNil/text2vec-large-chinese](https://huggingface.co/GanymedeNil/text2vec-large-chinese)                                                   | 32.61 | 44.59 | 69.30 | 14.51 | 79.44 |  73.01  |  59.04  |   53.12   | 2092  |
+| CoSENT     | nghuyong/ernie-3.0-base-zh                                   | [shibing624/text2vec-base-chinese-sentence](https://huggingface.co/shibing624/text2vec-base-chinese-sentence)                                     | 43.37 | 61.43 | 73.48 | 38.90 | 78.25 |  70.60  |  53.08  |   59.87   | 3089  |
+| CoSENT     | nghuyong/ernie-3.0-base-zh                                   | [shibing624/text2vec-base-chinese-paraphrase](https://huggingface.co/shibing624/text2vec-base-chinese-paraphrase)                                 | 44.89 | 63.58 | 74.24 | 40.90 | 78.93 |  76.70  |  63.30  | **63.08** | 3066  |
+| CoSENT     | sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2  | [shibing624/text2vec-base-multilingual](https://huggingface.co/shibing624/text2vec-base-multilingual)                                             | 32.39 | 50.33 | 65.64 | 32.56 | 74.45 |  68.88  |  51.17  |   53.67   | 3138  |
 
 
 说明：
 - 结果评测指标：spearman系数
-- 模型训练实验报告：[实验报告](https://github.com/shibing624/text2vec/blob/master/docs/model_report.md)
 - `shibing624/text2vec-base-chinese`模型，是用CoSENT方法训练，基于`hfl/chinese-macbert-base`在中文STS-B数据训练得到，并在中文STS-B测试集评估达到较好效果，运行[examples/training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model.py)代码可训练模型，模型文件已经上传HF model hub，中文通用语义匹配任务推荐使用
 - `shibing624/text2vec-base-chinese-sentence`模型，是用CoSENT方法训练，基于`nghuyong/ernie-3.0-base-zh`用人工挑选后的中文STS数据集[shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-sentence-dataset)训练得到，并在中文各NLI测试集评估达到较好效果，运行[examples/training_sup_text_matching_model_jsonl_data.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model_jsonl_data.py)代码可训练模型，模型文件已经上传HF model hub，中文s2s(句子vs句子)语义匹配任务推荐使用
 - `shibing624/text2vec-base-chinese-paraphrase`模型，是用CoSENT方法训练，基于`nghuyong/ernie-3.0-base-zh`用人工挑选后的中文STS数据集[shibing624/nli-zh-all/text2vec-base-chinese-paraphrase-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-paraphrase-dataset)，数据集相对于[shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-sentence-dataset)加入了s2p(sentence to paraphrase)数据，强化了其长文本的表征能力，并在中文各NLI测试集评估达到SOTA，运行[examples/training_sup_text_matching_model_jsonl_data.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model_jsonl_data.py)代码可训练模型，模型文件已经上传HF model hub，中文s2p(句子vs段落)语义匹配任务推荐使用
-- `SBERT-macbert-base`模型，是用SBERT方法训练，运行[examples/training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model.py)代码可训练模型
-- `sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`模型是用SBERT训练，是`paraphrase-MiniLM-L12-v2`模型的多语言版本，支持中文、英文等
+- `shibing624/text2vec-base-multilingual`模型，是用CoSENT方法训练，基于`sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`用人工挑选后的多语言STS数据集[shibing624/nli-zh-all/text2vec-base-multilingual-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-multilingual-dataset)训练得到，并在中英文测试集评估相对于原模型效果有提升，运行[examples/training_sup_text_matching_model_jsonl_data.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model_jsonl_data.py)代码可训练模型，模型文件已经上传HF model hub，多语言语义匹配任务推荐使用
 - `w2v-light-tencent-chinese`是腾讯词向量的Word2Vec模型，CPU加载使用，适用于中文字面匹配任务和缺少数据的冷启动情况
 - 各预训练模型均可以通过transformers调用，如MacBERT模型：`--model_name hfl/chinese-macbert-base` 或者roberta模型：`--model_name uer/roberta-medium-wwm-chinese-cluecorpussmall`
 - 为测评模型的鲁棒性，加入了未训练过的SOHU测试集，用于测试模型的泛化能力；为达到开箱即用的实用效果，使用了搜集到的各中文匹配数据集，数据集也上传到HF datasets[链接见下方](#数据集)
 - 中文匹配任务实验表明，pooling最优是`EncoderType.FIRST_LAST_AVG`和`EncoderType.MEAN`，两者预测效果差异很小
 - 中文匹配评测结果复现，可以下载中文匹配数据集到`examples/data`，运行[tests/test_model_spearman.py](https://github.com/shibing624/text2vec/blob/master/tests/test_model_spearman.py)代码复现评测结果
 - QPS的GPU测试环境是Tesla V100，显存32GB
 
-# Demo
+模型训练实验报告：[实验报告](https://github.com/shibing624/text2vec/blob/master/docs/model_report.md)
+## Demo
 
 Official Demo: https://www.mulanai.com/product/short_text_sim/
 
 HuggingFace Demo: https://huggingface.co/spaces/shibing624/text2vec
 
 ![](docs/hf.png)
 
 run example: [examples/gradio_demo.py](https://github.com/shibing624/text2vec/blob/master/examples/gradio_demo.py) to see the demo:
 ```shell
 python examples/gradio_demo.py
 ```
 
-# Install
+## Install
 ```shell
 pip install torch # conda install pytorch
 pip install -U text2vec
 ```
 
 or
 
@@ -136,17 +140,17 @@
 pip install -r requirements.txt
 
 git clone https://github.com/shibing624/text2vec.git
 cd text2vec
 pip install --no-deps .
 ```
 
-# Usage
+## Usage
 
-## 文本向量表征
+### 文本向量表征
 
 基于`pretrained model`计算文本向量：
 
 ```zsh
 >>> from text2vec import SentenceModel
 >>> m = SentenceModel()
 >>> m.encode("如何更换花呗绑定银行卡")
@@ -186,16 +190,16 @@
 
 
 if __name__ == "__main__":
     # 中文句向量模型(CoSENT)，中文语义匹配任务推荐，支持fine-tune继续训练
     t2v_model = SentenceModel("shibing624/text2vec-base-chinese")
     compute_emb(t2v_model)
 
-    # 支持多语言的句向量模型（Sentence-BERT），英文语义匹配任务推荐，支持fine-tune继续训练
-    sbert_model = SentenceModel("sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2")
+    # 支持多语言的句向量模型（CoSENT），多语言（包括中英文）语义匹配任务推荐，支持fine-tune继续训练
+    sbert_model = SentenceModel("shibing624/text2vec-base-multilingual")
     compute_emb(sbert_model)
 
     # 中文词向量模型(word2vec)，中文字面匹配任务和冷启动适用
     w2v_model = Word2Vec("w2v-light-tencent-chinese")
     compute_emb(w2v_model)
 
 ```
@@ -212,16 +216,14 @@
 ```
 
 - 返回值`embeddings`是`numpy.ndarray`类型，shape为`(sentences_size, model_embedding_size)`，三个模型任选一种即可，推荐用第一个。
 - `shibing624/text2vec-base-chinese`模型是CoSENT方法在中文STS-B数据集训练得到的，模型已经上传到huggingface的
 模型库[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)，
 是`text2vec.SentenceModel`指定的默认模型，可以通过上面示例调用，或者如下所示用[transformers库](https://github.com/huggingface/transformers)调用，
 模型自动下载到本机路径：`~/.cache/huggingface/transformers`
-- `sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`模型是Sentence-BERT的多语言句向量模型，
-适用于释义（paraphrase）识别，文本匹配，通过`text2vec.SentenceModel`和[sentence-transformers库]((https://github.com/UKPLab/sentence-transformers))都可以调用该模型
 - `w2v-light-tencent-chinese`是通过gensim加载的Word2Vec模型，使用腾讯词向量`Tencent_AILab_ChineseEmbedding.tar.gz`计算各字词的词向量，句子向量通过单词词
 向量取平均值得到，模型自动下载到本机路径：`~/.text2vec/datasets/light_Tencent_AILab_ChineseEmbedding.bin`
 
 #### Usage (HuggingFace Transformers)
 Without [text2vec](https://github.com/shibing624/text2vec), you can use the model like this: 
 
 First, you pass your input through the transformer model, then you have to apply the right pooling-operation on-top of the contextualized word embeddings.
@@ -439,17 +441,17 @@
 from similarities import Similarity
 
 m = Similarity()
 r = m.similarity('如何更换花呗绑定银行卡', '花呗更改绑定银行卡')
 print(f"similarity score: {float(r)}")  # similarity score: 0.855146050453186
 ```
 
-# Models
+## Models
 
-## CoSENT model
+### CoSENT model
 
 CoSENT（Cosine Sentence）文本匹配模型，在Sentence-BERT上改进了CosineRankLoss的句向量方案
 
 
 Network structure:
 
 Training:
@@ -480,16 +482,22 @@
 python training_sup_text_matching_model.py --task_name ATEC --model_arch cosent --do_train --do_predict --num_epochs 10 --model_name hfl/chinese-macbert-base --output_dir ./outputs/ATEC-cosent
 ```
 
 - 在自有中文数据集上训练模型
 
 example: [examples/training_sup_text_matching_model_mydata.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model_mydata.py)
 
+单卡训练：
+```shell
+CUDA_VISIBLE_DEVICES=0 python training_sup_text_matching_model_mydata.py --do_train --do_predict
+```
+
+多卡训练：
 ```shell
-python training_sup_text_matching_model_mydata.py --do_train --do_predict
+CUDA_VISIBLE_DEVICES=0,1 torchrun --nproc_per_node 2  training_sup_text_matching_model_mydata.py --do_train --do_predict --output_dir outputs/STS-B-text2vec-macbert-v1 --batch_size 64 --fp16 --data_parallel 
 ```
 
 训练集格式参考[examples/data/STS-B/STS-B.valid.data](https://github.com/shibing624/text2vec/blob/master/examples/data/STS-B/STS-B.valid.data)
 
 ```shell
 sentence1   sentence2   label
 一个女孩在给她的头发做发型。	一个女孩在梳头。	2
@@ -516,15 +524,15 @@
 
 ```shell
 cd examples
 python training_unsup_text_matching_model_en.py --model_arch cosent --do_train --do_predict --num_epochs 10 --model_name bert-base-uncased --output_dir ./outputs/STS-B-en-unsup-cosent
 ```
 
 
-## Sentence-BERT model
+### Sentence-BERT model
 
 Sentence-BERT文本匹配模型，表征式句向量表示方案
 
 Network structure:
 
 Training:
 
@@ -559,38 +567,38 @@
 example: [examples/training_unsup_text_matching_model_en.py](https://github.com/shibing624/text2vec/blob/master/examples/training_unsup_text_matching_model_en.py)
 
 ```shell
 cd examples
 python training_unsup_text_matching_model_en.py --model_arch sentencebert --do_train --do_predict --num_epochs 10 --model_name bert-base-uncased --output_dir ./outputs/STS-B-en-unsup-sbert
 ```
 
-## BERT-Match model
+### BERT-Match model
 BERT文本匹配模型，原生BERT匹配网络结构，交互式句向量匹配模型
 
 Network structure:
 
 Training and inference:
 
 <img src="docs/bert-fc-train.png" width="300" />
 
 训练脚本同上[examples/training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model.py)。
 
 
-## 模型蒸馏（Model Distillation）
+### 模型蒸馏（Model Distillation）
 
 由于text2vec训练的模型可以使用[sentence-transformers](https://github.com/UKPLab/sentence-transformers)库加载，此处复用其模型蒸馏方法[distillation](https://github.com/UKPLab/sentence-transformers/tree/master/examples/training/distillation)。
 
 1. 模型降维，参考[dimensionality_reduction.py](https://github.com/UKPLab/sentence-transformers/blob/master/examples/training/distillation/dimensionality_reduction.py)使用PCA对模型输出embedding降维，可减少milvus等向量检索数据库的存储压力，还能轻微提升模型效果。
 2. 模型蒸馏，参考[model_distillation.py](https://github.com/UKPLab/sentence-transformers/blob/master/examples/training/distillation/model_distillation.py)使用蒸馏方法，将Teacher大模型蒸馏到更少layers层数的student模型中，在权衡效果的情况下，可大幅提升模型预测速度。
 
-## 模型部署
+### 模型部署
 
 提供两种部署模型，搭建服务的方法： 1）基于Jina搭建gRPC服务【推荐】；2）基于FastAPI搭建原生Http服务。
 
-### Jina服务
+#### Jina服务
 采用C/S模式搭建高性能服务，支持docker云原生，gRPC/HTTP/WebSocket，支持多个模型同时预测，GPU多卡处理。
 
 - 安装：
 ```pip install jina```
 
 - 启动服务：
 
@@ -629,15 +637,15 @@
 r = c.post('/', inputs=DocumentArray([Document(text='如何更换花呗绑定银行卡'), Document(text='花呗更改绑定银行卡')]))
 print(r.embeddings)
 ```
 
 批量调用方法见example: [examples/jina_client_demo.py](https://github.com/shibing624/text2vec/blob/master/examples/jina_client_demo.py)
 
 
-### FastAPI服务
+#### FastAPI服务
 
 - 安装：
 ```pip install fastapi uvicorn```
 
 - 启动服务：
 
 example: [examples/fastapi_server_demo.py](https://github.com/shibing624/text2vec/blob/master/examples/fastapi_server_demo.py)
@@ -650,15 +658,15 @@
 ```shell
 curl -X 'GET' \
   'http://0.0.0.0:8001/emb?q=hello' \
   -H 'accept: application/json'
 ```
 
 
-## 数据集
+## Dataset
 
 - 本项目release的数据集：
 
 | Dataset                    | Introduce                                                                | Download Link                                                                                                                                                                                                                                                                                         |
 |:---------------------------|:-------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | shibing624/nli-zh-all      | 中文语义匹配数据合集，整合了文本推理，相似，摘要，问答，指令微调等任务的820万高质量数据，并转化为匹配格式数据集                | [https://huggingface.co/datasets/shibing624/nli-zh-all](https://huggingface.co/datasets/shibing624/nli-zh-all)                                                                                                                                                                                        |
 | shibing624/snli-zh         | 中文SNLI和MultiNLI数据集，翻译自英文SNLI和MultiNLI                                    | [https://huggingface.co/datasets/shibing624/snli-zh](https://huggingface.co/datasets/shibing624/snli-zh)                                                                                                                                                                                              |
@@ -669,16 +677,16 @@
 | LCQMC                      | 中文LCQMC(large-scale Chinese question matching corpus)数据集，Q-Qpair数据集      | [LCQMC](http://icrc.hitsz.edu.cn/Article/show/171.html)                                                                                                                                                                                                                                               |
 | PAWSX                      | 中文PAWS(Paraphrase Adversaries from Word Scrambling)数据集，Q-Qpair数据集        | [PAWSX](https://arxiv.org/abs/1908.11828)                                                                                                                                                                                                                                                             |
 | STS-B                      | 中文STS-B数据集，中文自然语言推理数据集，从英文STS-B翻译为中文的数据集                                 | [STS-B](https://github.com/pluto-junzeng/CNSD)                                                                                                                                                                                                                                                        |
 
 
 常用英文匹配数据集：
 
-- 大名鼎鼎的multi_nli和snli: https://huggingface.co/datasets/multi_nli
-- 大名鼎鼎的multi_nli和snli: https://huggingface.co/datasets/snli
+- 英文匹配数据集：multi_nli: https://huggingface.co/datasets/multi_nli
+- 英文匹配数据集：snli: https://huggingface.co/datasets/snli
 - https://huggingface.co/datasets/metaeval/cnli
 - https://huggingface.co/datasets/mteb/stsbenchmark-sts
 - https://huggingface.co/datasets/JeremiahZ/simcse_sup_nli
 - https://huggingface.co/datasets/MoritzLaurer/multilingual-NLI-26lang-2mil7
 
 
 数据集使用示例：
@@ -713,59 +721,59 @@
 {'sentence1': '一个女孩在给她的头发做发型。', 'sentence2': '一个女孩在梳头。', 'label': 2}
 ```
 
 
 
 
 
-# Contact
+## Contact
 
 - Issue(建议)：[![GitHub issues](https://img.shields.io/github/issues/shibing624/text2vec.svg)](https://github.com/shibing624/text2vec/issues)
 - 邮件我：xuming: xuming624@qq.com
 - 微信我：加我*微信号：xuming624, 备注：姓名-公司-NLP* 进NLP交流群。
 
 <img src="docs/wechat.jpeg" width="200" />
 
 
-# Citation
+## Citation
 
 如果你在研究中使用了text2vec，请按如下格式引用：
 
 APA:
 ```latex
 Xu, M. Text2vec: Text to vector toolkit (Version 1.1.2) [Computer software]. https://github.com/shibing624/text2vec
 ```
 
 BibTeX:
 ```latex
 @misc{Text2vec,
-  author = {Xu, Ming},
+  author = {Ming Xu},
   title = {Text2vec: Text to vector toolkit},
-  year = {2022},
+  year = {2023},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/shibing624/text2vec}},
 }
 ```
 
-# License
+## License
 
 
 授权协议为 [The Apache License 2.0](LICENSE)，可免费用做商业用途。请在产品说明中附加text2vec的链接和授权协议。
 
 
-# Contribute
+## Contribute
 项目代码还很粗糙，如果大家对代码有所改进，欢迎提交回本项目，在提交之前，注意以下两点：
 
  - 在`tests`添加相应的单元测试
  - 使用`python -m pytest -v`来运行所有单元测试，确保所有单测都是通过的
 
 之后即可提交PR。
 
-# Reference
+## References
 - [将句子表示为向量（上）：无监督句子表示学习（sentence embedding）](https://www.cnblogs.com/llhthinker/p/10335164.html)
 - [将句子表示为向量（下）：无监督句子表示学习（sentence embedding）](https://www.cnblogs.com/llhthinker/p/10341841.html)
 - [A Simple but Tough-to-Beat Baseline for Sentence Embeddings[Sanjeev Arora and Yingyu Liang and Tengyu Ma, 2017]](https://openreview.net/forum?id=SyK00v5xx)
 - [四种计算文本相似度的方法对比[Yves Peirsman]](https://zhuanlan.zhihu.com/p/37104535)
 - [Improvements to BM25 and Language Models Examined](http://www.cs.otago.ac.nz/homepages/andrew/papers/2014-2.pdf)
 - [CoSENT：比Sentence-BERT更有效的句向量方案](https://kexue.fm/archives/8847)
 - [谈谈文本匹配和多轮检索](https://zhuanlan.zhihu.com/p/111769969)
```

#### html2text {}

```diff
@@ -14,17 +14,26 @@
 shibing624/text2vec.svg)](https://github.com/shibing624/text2vec/issues) [!
 [Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/
 wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact) **Text2vec**: Text to
 Vector, Get Sentence Embeddings. ææ¬åéåï¼æææ¬
 (åæ¬è¯ãå¥å­ãæ®µè½)è¡¨å¾ä¸ºåéç©éµã
 **text2vec**å®ç°äºWord2VecãRankBM25ãBERTãSentence-
 BERTãCoSENTç­å¤ç§ææ¬è¡¨å¾ãææ¬ç¸ä¼¼åº¦è®¡ç®æ¨¡åï¼å¹¶å¨ææ¬è¯­ä¹å¹éï¼ç¸ä¼¼åº¦è®¡ç®ï¼ä»»å¡ä¸æ¯è¾äºåæ¨¡åçææã
-### News [2023/06/19] v1.2.1çæ¬: æ´æ°äºä¸­æå¹éæ¨¡å`shibing624/
-text2vec-base-chinese-nli`ä¸ºæ°ç[shibing624/text2vec-base-chinese-sentence]
-(https://huggingface.co/shibing624/text2vec-base-chinese-
+### News [2023/06/22] v1.2.2çæ¬: åå¸äºå¤è¯­è¨å¹éæ¨¡å[shibing624/
+text2vec-base-multilingual](https://huggingface.co/shibing624/text2vec-base-
+multilingual)ï¼ç¨CoSENTæ¹æ³è®­ç»ï¼åºäº`sentence-transformers/
+paraphrase-multilingual-MiniLM-L12-
+v2`ç¨äººå·¥æéåçå¤è¯­è¨STSæ°æ®é[shibing624/nli-zh-all/text2vec-
+base-multilingual-dataset](https://huggingface.co/datasets/shibing624/nli-zh-
+all/tree/main/text2vec-base-multilingual-
+dataset)è®­ç»å¾å°ï¼å¹¶å¨ä¸­è±ææµè¯éè¯ä¼°ç¸å¯¹äºåæ¨¡åææææåï¼è¯¦è§
+[Release-v1.2.2](https://github.com/shibing624/text2vec/releases/tag/1.2.2)
+[2023/06/19] v1.2.1çæ¬: æ´æ°äºä¸­æå¹éæ¨¡å`shibing624/text2vec-
+base-chinese-nli`ä¸ºæ°ç[shibing624/text2vec-base-chinese-sentence](https://
+huggingface.co/shibing624/text2vec-base-chinese-
 sentence)ï¼éå¯¹CoSENTçlossè®¡ç®å¯¹æåºææç¹ç¹ï¼äººå·¥æéå¹¶æ´çåºé«è´¨éçæç¸å³æ§æåºçSTSæ°æ®é
 [shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://
 huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-
 sentence-
 dataset)ï¼å¨åè¯ä¼°éè¡¨ç°ç¸å¯¹ä¹åææåï¼åå¸äºéç¨äºs2pçä¸­æå¹éæ¨¡å
 [shibing624/text2vec-base-chinese-paraphrase](https://huggingface.co/
 shibing624/text2vec-base-chinese-paraphrase)ï¼è¯¦è§[Release-v1.2.1](https://
@@ -35,17 +44,17 @@
 huggingface.co/datasets/shibing624/
 nli_zh)å¨é¨è¯­æè®­ç»çCoSENTææ¬å¹éæ¨¡åï¼å¨åè¯ä¼°éè¡¨ç°æåææ¾ï¼è¯¦è§
 [Release-v1.2.0](https://github.com/shibing624/text2vec/releases/tag/1.2.0)
 [2022/03/12] v1.1.4çæ¬: åå¸äºä¸­æå¹éæ¨¡å[shibing624/text2vec-
 base-chinese](https://huggingface.co/shibing624/text2vec-base-
 chinese)ï¼åºäºä¸­æSTSè®­ç»éè®­ç»çCoSENTå¹éæ¨¡åãè¯¦è§
 [Release-v1.1.4](https://github.com/shibing624/text2vec/releases/tag/1.1.4)
-**Guide** - [Feature](#Feature) - [Evaluation](#Evaluation) - [Install]
-(#install) - [Usage](#usage) - [Contact](#Contact) - [Reference](#reference) #
-Feature ### ææ¬åéè¡¨ç¤ºæ¨¡å - [Word2Vec](https://github.com/
+**Guide** - [Features](#Features) - [Evaluation](#Evaluation) - [Install]
+(#install) - [Usage](#usage) - [Contact](#Contact) - [References](#references)
+## Features ### ææ¬åéè¡¨ç¤ºæ¨¡å - [Word2Vec](https://github.com/
 shibing624/text2vec/blob/master/text2vec/word2vec.py)ï¼éè¿è¾è®¯AI
 Labå¼æºçå¤§è§æ¨¡é«è´¨éä¸­æ
 [è¯åéæ°æ®ï¼800ä¸ä¸­æè¯è½»éçï¼](https://pan.baidu.com/s/
 1La4U4XNFe8s5BJqxPQpeiQ) (æä»¶åï¼light_Tencent_AILab_ChineseEmbedding.bin
 å¯ç :
 taweï¼å®ç°è¯åéæ£ç´¢ï¼æ¬é¡¹ç®å®ç°äºå¥å­ï¼è¯åéæ±å¹³åï¼çword2vecåéè¡¨ç¤º
 - [SBERT(Sentence-BERT)](https://github.com/shibing624/text2vec/blob/master/
@@ -53,67 +62,76 @@
 sentencebert_model.py)ï¼æè¡¡æ§è½åæççå¥åéè¡¨ç¤ºæ¨¡åï¼è®­ç»æ¶éè¿æçç£è®­ç»ä¸å±åç±»å½æ°ï¼ææ¬å¹éé¢æµæ¶ç´æ¥å¥å­åéåä½å¼¦ï¼æ¬é¡¹ç®åºäºPyTorchå¤ç°äºSentence-
 BERTæ¨¡åçè®­ç»åé¢æµ - [CoSENT(Cosine Sentence)](https://github.com/
 shibing624/text2vec/blob/master/text2vec/
 cosent_model.py)ï¼CoSENTæ¨¡åæåºäºä¸ç§æåºçæå¤±å½æ°ï¼ä½¿è®­ç»è¿ç¨æ´è´´è¿é¢æµï¼æ¨¡åæ¶æéåº¦åæææ¯Sentence-
 BERTæ´å¥½ï¼æ¬é¡¹ç®åºäºPyTorchå®ç°äºCoSENTæ¨¡åçè®­ç»åé¢æµ
 è¯¦ç»ææ¬åéè¡¨ç¤ºæ¹æ³è§wiki: [ææ¬åéè¡¨ç¤ºæ¹æ³](https://
 github.com/shibing624/text2vec/wiki/
-%E6%96%87%E6%9C%AC%E5%90%91%E9%87%8F%E8%A1%A8%E7%A4%BA%E6%96%B9%E6%B3%95) #
+%E6%96%87%E6%9C%AC%E5%90%91%E9%87%8F%E8%A1%A8%E7%A4%BA%E6%96%B9%E6%B3%95) ##
 Evaluation ææ¬å¹é #### è±æå¹éæ°æ®éçè¯æµç»æï¼ | Arch |
 BaseModel | Model | English-STS-B | |:-------|:--------------------------------
-----------------|:-------------------------------------|:-------------:| |
+----------------|:-------------------------------------------------------------
+--------------------------------------------------------|:-------------:| |
 GloVe | glove | Avg_word_embeddings_glove_6B_300d | 61.77 | | BERT | bert-base-
 uncased | BERT-base-cls | 20.29 | | BERT | bert-base-uncased | BERT-base-
 first_last_avg | 59.04 | | BERT | bert-base-uncased | BERT-base-first_last_avg-
 whiten(NLI) | 63.65 | | SBERT | sentence-transformers/bert-base-nli-mean-tokens
 | SBERT-base-nli-cls | 73.65 | | SBERT | sentence-transformers/bert-base-nli-
 mean-tokens | SBERT-base-nli-first_last_avg | 77.96 | | CoSENT | bert-base-
 uncased | CoSENT-base-first_last_avg | 69.93 | | CoSENT | sentence-
 transformers/bert-base-nli-mean-tokens | CoSENT-base-nli-first_last_avg | 79.68
-| #### ä¸­æå¹éæ°æ®éçè¯æµç»æï¼ | Arch | BaseModel | Model |
-ATEC | BQ | LCQMC | PAWSX | STS-B | Avg | |:-------|:--------------------------
---|:--------------------|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:| |
-SBERT | bert-base-chinese | SBERT-bert-base | 46.36 | 70.36 | 78.72 | 46.86 |
-66.41 | 61.74 | | SBERT | hfl/chinese-macbert-base | SBERT-macbert-base | 47.28
-| 68.63 | 79.42 | 55.59 | 64.82 | 63.15 | | SBERT | hfl/chinese-roberta-wwm-ext
-| SBERT-roberta-ext | 48.29 | 69.99 | 79.22 | 44.10 | 72.42 | 62.80 | | CoSENT
-| bert-base-chinese | CoSENT-bert-base | 49.74 | 72.38 | 78.69 | 60.00 | 79.27
-| 68.01 | | CoSENT | hfl/chinese-macbert-base | CoSENT-macbert-base | 50.39 |
-72.93 | 79.17 | 60.86 | 79.30 | 68.53 | | CoSENT | hfl/chinese-roberta-wwm-ext
-| CoSENT-roberta-ext | 50.81 | 71.45 | 79.31 | 61.56 | 79.96 | 68.61 |
-è¯´æï¼ - ç»æè¯æµææ ï¼spearmanç³»æ° -
+| | CoSENT | sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2 |
+[shibing624/text2vec-base-multilingual](https://huggingface.co/shibing624/
+text2vec-base-multilingual) | 80.12 | ####
+ä¸­æå¹éæ°æ®éçè¯æµç»æï¼ | Arch | BaseModel | Model | ATEC | BQ
+| LCQMC | PAWSX | STS-B | Avg | |:-------|:----------------------------|:------
+--------------|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:| | SBERT | bert-
+base-chinese | SBERT-bert-base | 46.36 | 70.36 | 78.72 | 46.86 | 66.41 | 61.74
+| | SBERT | hfl/chinese-macbert-base | SBERT-macbert-base | 47.28 | 68.63 |
+79.42 | 55.59 | 64.82 | 63.15 | | SBERT | hfl/chinese-roberta-wwm-ext | SBERT-
+roberta-ext | 48.29 | 69.99 | 79.22 | 44.10 | 72.42 | 62.80 | | CoSENT | bert-
+base-chinese | CoSENT-bert-base | 49.74 | 72.38 | 78.69 | 60.00 | 79.27 | 68.01
+| | CoSENT | hfl/chinese-macbert-base | CoSENT-macbert-base | 50.39 | 72.93 |
+79.17 | 60.86 | 79.30 | 68.53 | | CoSENT | hfl/chinese-roberta-wwm-ext |
+CoSENT-roberta-ext | 50.81 | 71.45 | 79.31 | 61.56 | 79.96 | 68.61 | è¯´æï¼
+- ç»æè¯æµææ ï¼spearmanç³»æ° -
 ä¸ºè¯æµæ¨¡åè½åï¼ç»æååªç¨è¯¥æ°æ®éçtrainè®­ç»ï¼å¨testä¸è¯ä¼°å¾å°çè¡¨ç°ï¼æ²¡ç¨å¤é¨æ°æ®
-### Release Models - æ¬é¡¹ç®releaseæ¨¡åçä¸­æå¹éè¯æµç»æï¼ |
-Arch | BaseModel | Model | ATEC | BQ | LCQMC | PAWSX | STS-B | SOHU-dd | SOHU-
-dc | Avg | QPS | |:-----------|:----------------------------------|:-----------
+- `SBERT-macbert-base`æ¨¡åï¼æ¯ç¨SBertæ¹æ³è®­ç»ï¼è¿è¡[examples/
+training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/
+blob/master/examples/training_sup_text_matching_model.py)ä»£ç å¯è®­ç»æ¨¡å
+- `sentence-transformers/paraphrase-multilingual-MiniLM-L12-
+v2`æ¨¡åæ¯ç¨SBertè®­ç»ï¼æ¯`paraphrase-MiniLM-L12-
+v2`æ¨¡åçå¤è¯­è¨çæ¬ï¼æ¯æä¸­æãè±æç­ ### Release Models -
+æ¬é¡¹ç®releaseæ¨¡åçä¸­æå¹éè¯æµç»æï¼ | Arch | BaseModel | Model
+| ATEC | BQ | LCQMC | PAWSX | STS-B | SOHU-dd | SOHU-dc | Avg | QPS | |:-------
+----|:-------------------------------------------------------------|:----------
 -------------------------------------------------------------------------------
---------------------------------------------------------|:-----:|:-----:|:----
+---------------------------------------------------------|:-----:|:-----:|:----
 -:|:-----:|:-----:|:-------:|:-------:|:---------:|:-----:| | Word2Vec |
 word2vec | [w2v-light-tencent-chinese](https://ai.tencent.com/ailab/nlp/en/
 download.html) | 20.00 | 31.49 | 59.46 | 2.57 | 55.78 | 55.04 | 20.70 | 35.03 |
 23769 | | SBERT | xlm-roberta-base | [sentence-transformers/paraphrase-
 multilingual-MiniLM-L12-v2](https://huggingface.co/sentence-transformers/
 paraphrase-multilingual-MiniLM-L12-v2) | 18.42 | 38.52 | 63.96 | 10.14 | 78.90
-| 63.01 | 52.28 | 46.46 | 3138 | | Instructor | hfl/chinese-roberta-wwm-ext |
-[moka-ai/m3e-base](https://huggingface.co/moka-ai/m3e-base) | 41.27 | 63.81 |
-74.87 | 12.20 | 76.96 | 75.83 | 60.55 | 57.93 | 2980 | | CoSENT | hfl/chinese-
-macbert-base | [shibing624/text2vec-base-chinese](https://huggingface.co/
-shibing624/text2vec-base-chinese) | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 |
-70.27 | 50.42 | 51.61 | 3008 | | CoSENT | hfl/chinese-lert-large |
-[GanymedeNil/text2vec-large-chinese](https://huggingface.co/GanymedeNil/
-text2vec-large-chinese) | 32.61 | 44.59 | 69.30 | 14.51 | 79.44 | 73.01 | 59.04
-| 53.12 | 2092 | | CoSENT | nghuyong/ernie-3.0-base-zh | [shibing624/text2vec-
-base-chinese-sentence](https://huggingface.co/shibing624/text2vec-base-chinese-
-sentence) | 43.37 | 61.43 | 73.48 | 38.90 | 78.25 | 70.60 | 53.08 | 59.87 |
-3089 | | CoSENT | nghuyong/ernie-3.0-base-zh | [shibing624/text2vec-base-
-chinese-paraphrase](https://huggingface.co/shibing624/text2vec-base-chinese-
-paraphrase) | 44.89 | 63.58 | 74.24 | 40.90 | 78.93 | 76.70 | 63.30 | **63.08**
-| 3066 | è¯´æï¼ - ç»æè¯æµææ ï¼spearmanç³»æ° -
-æ¨¡åè®­ç»å®éªæ¥åï¼[å®éªæ¥å](https://github.com/shibing624/
-text2vec/blob/master/docs/model_report.md) - `shibing624/text2vec-base-
+| 63.01 | 52.28 | 46.46 | 3138 | | CoSENT | hfl/chinese-macbert-base |
+[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-
+base-chinese) | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 | 70.27 | 50.42 | 51.61 |
+3008 | | CoSENT | hfl/chinese-lert-large | [GanymedeNil/text2vec-large-chinese]
+(https://huggingface.co/GanymedeNil/text2vec-large-chinese) | 32.61 | 44.59 |
+69.30 | 14.51 | 79.44 | 73.01 | 59.04 | 53.12 | 2092 | | CoSENT | nghuyong/
+ernie-3.0-base-zh | [shibing624/text2vec-base-chinese-sentence](https://
+huggingface.co/shibing624/text2vec-base-chinese-sentence) | 43.37 | 61.43 |
+73.48 | 38.90 | 78.25 | 70.60 | 53.08 | 59.87 | 3089 | | CoSENT | nghuyong/
+ernie-3.0-base-zh | [shibing624/text2vec-base-chinese-paraphrase](https://
+huggingface.co/shibing624/text2vec-base-chinese-paraphrase) | 44.89 | 63.58 |
+74.24 | 40.90 | 78.93 | 76.70 | 63.30 | **63.08** | 3066 | | CoSENT | sentence-
+transformers/paraphrase-multilingual-MiniLM-L12-v2 | [shibing624/text2vec-base-
+multilingual](https://huggingface.co/shibing624/text2vec-base-multilingual) |
+32.39 | 50.33 | 65.64 | 32.56 | 74.45 | 68.88 | 51.17 | 53.67 | 3138 |
+è¯´æï¼ - ç»æè¯æµææ ï¼spearmanç³»æ° - `shibing624/text2vec-base-
 chinese`æ¨¡åï¼æ¯ç¨CoSENTæ¹æ³è®­ç»ï¼åºäº`hfl/chinese-macbert-
 base`å¨ä¸­æSTS-Bæ°æ®è®­ç»å¾å°ï¼å¹¶å¨ä¸­æSTS-
 Bæµè¯éè¯ä¼°è¾¾å°è¾å¥½ææï¼è¿è¡[examples/
 training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/
 blob/master/examples/
 training_sup_text_matching_model.py)ä»£ç å¯è®­ç»æ¨¡åï¼æ¨¡åæä»¶å·²ç»ä¸ä¼ HF
 model hubï¼ä¸­æéç¨è¯­ä¹å¹éä»»å¡æ¨èä½¿ç¨ - `shibing624/text2vec-
@@ -134,81 +152,83 @@
 [shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://
 huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-
 sentence-dataset)å å¥äºs2p(sentence to
 paraphrase)æ°æ®ï¼å¼ºåäºå¶é¿ææ¬çè¡¨å¾è½åï¼å¹¶å¨ä¸­æåNLIæµè¯éè¯ä¼°è¾¾å°SOTAï¼è¿è¡
 [examples/training_sup_text_matching_model_jsonl_data.py](https://github.com/
 shibing624/text2vec/blob/master/examples/
 training_sup_text_matching_model_jsonl_data.py)ä»£ç å¯è®­ç»æ¨¡åï¼æ¨¡åæä»¶å·²ç»ä¸ä¼ HF
-model hubï¼ä¸­æs2p(å¥å­vsæ®µè½)è¯­ä¹å¹éä»»å¡æ¨èä½¿ç¨ - `SBERT-
-macbert-base`æ¨¡åï¼æ¯ç¨SBERTæ¹æ³è®­ç»ï¼è¿è¡[examples/
-training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/
-blob/master/examples/training_sup_text_matching_model.py)ä»£ç å¯è®­ç»æ¨¡å
-- `sentence-transformers/paraphrase-multilingual-MiniLM-L12-
-v2`æ¨¡åæ¯ç¨SBERTè®­ç»ï¼æ¯`paraphrase-MiniLM-L12-
-v2`æ¨¡åçå¤è¯­è¨çæ¬ï¼æ¯æä¸­æãè±æç­ - `w2v-light-tencent-
+model hubï¼ä¸­æs2p(å¥å­vsæ®µè½)è¯­ä¹å¹éä»»å¡æ¨èä½¿ç¨ -
+`shibing624/text2vec-base-
+multilingual`æ¨¡åï¼æ¯ç¨CoSENTæ¹æ³è®­ç»ï¼åºäº`sentence-transformers/
+paraphrase-multilingual-MiniLM-L12-
+v2`ç¨äººå·¥æéåçå¤è¯­è¨STSæ°æ®é[shibing624/nli-zh-all/text2vec-
+base-multilingual-dataset](https://huggingface.co/datasets/shibing624/nli-zh-
+all/tree/main/text2vec-base-multilingual-
+dataset)è®­ç»å¾å°ï¼å¹¶å¨ä¸­è±ææµè¯éè¯ä¼°ç¸å¯¹äºåæ¨¡åææææåï¼è¿è¡
+[examples/training_sup_text_matching_model_jsonl_data.py](https://github.com/
+shibing624/text2vec/blob/master/examples/
+training_sup_text_matching_model_jsonl_data.py)ä»£ç å¯è®­ç»æ¨¡åï¼æ¨¡åæä»¶å·²ç»ä¸ä¼ HF
+model hubï¼å¤è¯­è¨è¯­ä¹å¹éä»»å¡æ¨èä½¿ç¨ - `w2v-light-tencent-
 chinese`æ¯è¾è®¯è¯åéçWord2Vecæ¨¡åï¼CPUå è½½ä½¿ç¨ï¼éç¨äºä¸­æå­é¢å¹éä»»å¡åç¼ºå°æ°æ®çå·å¯å¨æåµ
 - åé¢è®­ç»æ¨¡ååå¯ä»¥éè¿transformersè°ç¨ï¼å¦MacBERTæ¨¡åï¼`--
 model_name hfl/chinese-macbert-base` æèrobertaæ¨¡åï¼`--model_name uer/
 roberta-medium-wwm-chinese-cluecorpussmall` -
 ä¸ºæµè¯æ¨¡åçé²æ£æ§ï¼å å¥äºæªè®­ç»è¿çSOHUæµè¯éï¼ç¨äºæµè¯æ¨¡åçæ³åè½åï¼ä¸ºè¾¾å°å¼ç®±å³ç¨çå®ç¨ææï¼ä½¿ç¨äºæéå°çåä¸­æå¹éæ°æ®éï¼æ°æ®éä¹ä¸ä¼ å°HF
 datasets[é¾æ¥è§ä¸æ¹](#æ°æ®é) -
 ä¸­æå¹éä»»å¡å®éªè¡¨æï¼poolingæä¼æ¯`EncoderType.FIRST_LAST_AVG`å`EncoderType.MEAN`ï¼ä¸¤èé¢æµææå·®å¼å¾å°
 -
 ä¸­æå¹éè¯æµç»æå¤ç°ï¼å¯ä»¥ä¸è½½ä¸­æå¹éæ°æ®éå°`examples/
 data`ï¼è¿è¡[tests/test_model_spearman.py](https://github.com/shibing624/
 text2vec/blob/master/tests/test_model_spearman.py)ä»£ç å¤ç°è¯æµç»æ -
-QPSçGPUæµè¯ç¯å¢æ¯Tesla V100ï¼æ¾å­32GB # Demo Official Demo: https://
-www.mulanai.com/product/short_text_sim/ HuggingFace Demo: https://
-huggingface.co/spaces/shibing624/text2vec ![](docs/hf.png) run example:
-[examples/gradio_demo.py](https://github.com/shibing624/text2vec/blob/master/
-examples/gradio_demo.py) to see the demo: ```shell python examples/
-gradio_demo.py ``` # Install ```shell pip install torch # conda install pytorch
-pip install -U text2vec ``` or ```shell pip install torch # conda install
-pytorch pip install -r requirements.txt git clone https://github.com/
-shibing624/text2vec.git cd text2vec pip install --no-deps . ``` # Usage ##
-ææ¬åéè¡¨å¾ åºäº`pretrained model`è®¡ç®ææ¬åéï¼ ```zsh >>>
-from text2vec import SentenceModel >>> m = SentenceModel() >>> m.encode
-("å¦ä½æ´æ¢è±åç»å®é¶è¡å¡") Embedding shape: (768,) ``` example:
-[examples/computing_embeddings_demo.py](https://github.com/shibing624/text2vec/
-blob/master/examples/computing_embeddings_demo.py) ```python import sys
-sys.path.append('..') from text2vec import SentenceModel from text2vec import
-Word2Vec def compute_emb(model): # Embed a list of sentences sentences =
-[ 'å¡', 'é¶è¡å¡', 'å¦ä½æ´æ¢è±åç»å®é¶è¡å¡',
-'è±åæ´æ¹ç»å®é¶è¡å¡', 'This framework generates embeddings for each
-input sentence', 'Sentences are passed as a list of string.', 'The quick brown
-fox jumps over the lazy dog.' ] sentence_embeddings = model.encode(sentences)
-print(type(sentence_embeddings), sentence_embeddings.shape) # The result is a
-list of sentence embeddings as numpy arrays for sentence, embedding in zip
-(sentences, sentence_embeddings): print("Sentence:", sentence) print("Embedding
-shape:", embedding.shape) print("Embedding head:", embedding[:10]) print() if
-__name__ == "__main__": # ä¸­æå¥åéæ¨¡å
-(CoSENT)ï¼ä¸­æè¯­ä¹å¹éä»»å¡æ¨èï¼æ¯æfine-tuneç»§ç»­è®­ç»
-t2v_model = SentenceModel("shibing624/text2vec-base-chinese") compute_emb
-(t2v_model) # æ¯æå¤è¯­è¨çå¥åéæ¨¡åï¼Sentence-
-BERTï¼ï¼è±æè¯­ä¹å¹éä»»å¡æ¨èï¼æ¯æfine-tuneç»§ç»­è®­ç»
-sbert_model = SentenceModel("sentence-transformers/paraphrase-multilingual-
-MiniLM-L12-v2") compute_emb(sbert_model) # ä¸­æè¯åéæ¨¡å
+QPSçGPUæµè¯ç¯å¢æ¯Tesla V100ï¼æ¾å­32GB æ¨¡åè®­ç»å®éªæ¥åï¼
+[å®éªæ¥å](https://github.com/shibing624/text2vec/blob/master/docs/
+model_report.md) ## Demo Official Demo: https://www.mulanai.com/product/
+short_text_sim/ HuggingFace Demo: https://huggingface.co/spaces/shibing624/
+text2vec ![](docs/hf.png) run example: [examples/gradio_demo.py](https://
+github.com/shibing624/text2vec/blob/master/examples/gradio_demo.py) to see the
+demo: ```shell python examples/gradio_demo.py ``` ## Install ```shell pip
+install torch # conda install pytorch pip install -U text2vec ``` or ```shell
+pip install torch # conda install pytorch pip install -r requirements.txt git
+clone https://github.com/shibing624/text2vec.git cd text2vec pip install --no-
+deps . ``` ## Usage ### ææ¬åéè¡¨å¾ åºäº`pretrained
+model`è®¡ç®ææ¬åéï¼ ```zsh >>> from text2vec import SentenceModel >>> m
+= SentenceModel() >>> m.encode("å¦ä½æ´æ¢è±åç»å®é¶è¡å¡") Embedding
+shape: (768,) ``` example: [examples/computing_embeddings_demo.py](https://
+github.com/shibing624/text2vec/blob/master/examples/
+computing_embeddings_demo.py) ```python import sys sys.path.append('..') from
+text2vec import SentenceModel from text2vec import Word2Vec def compute_emb
+(model): # Embed a list of sentences sentences = [ 'å¡', 'é¶è¡å¡',
+'å¦ä½æ´æ¢è±åç»å®é¶è¡å¡', 'è±åæ´æ¹ç»å®é¶è¡å¡', 'This
+framework generates embeddings for each input sentence', 'Sentences are passed
+as a list of string.', 'The quick brown fox jumps over the lazy dog.' ]
+sentence_embeddings = model.encode(sentences) print(type(sentence_embeddings),
+sentence_embeddings.shape) # The result is a list of sentence embeddings as
+numpy arrays for sentence, embedding in zip(sentences, sentence_embeddings):
+print("Sentence:", sentence) print("Embedding shape:", embedding.shape) print
+("Embedding head:", embedding[:10]) print() if __name__ == "__main__": #
+ä¸­æå¥åéæ¨¡å(CoSENT)ï¼ä¸­æè¯­ä¹å¹éä»»å¡æ¨èï¼æ¯æfine-
+tuneç»§ç»­è®­ç» t2v_model = SentenceModel("shibing624/text2vec-base-chinese")
+compute_emb(t2v_model) #
+æ¯æå¤è¯­è¨çå¥åéæ¨¡åï¼CoSENTï¼ï¼å¤è¯­è¨ï¼åæ¬ä¸­è±æï¼è¯­ä¹å¹éä»»å¡æ¨èï¼æ¯æfine-
+tuneç»§ç»­è®­ç» sbert_model = SentenceModel("shibing624/text2vec-base-
+multilingual") compute_emb(sbert_model) # ä¸­æè¯åéæ¨¡å
 (word2vec)ï¼ä¸­æå­é¢å¹éä»»å¡åå·å¯å¨éç¨ w2v_model = Word2Vec
 ("w2v-light-tencent-chinese") compute_emb(w2v_model) ``` output: ```
 numpy.ndarray'> (7, 768) Sentence: å¡ Embedding shape: (768,) Sentence:
 é¶è¡å¡ Embedding shape: (768,) ... ``` -
 è¿åå¼`embeddings`æ¯`numpy.ndarray`ç±»åï¼shapeä¸º`(sentences_size,
 model_embedding_size)`ï¼ä¸ä¸ªæ¨¡åä»»éä¸ç§å³å¯ï¼æ¨èç¨ç¬¬ä¸ä¸ªã
 - `shibing624/text2vec-base-chinese`æ¨¡åæ¯CoSENTæ¹æ³å¨ä¸­æSTS-
 Bæ°æ®éè®­ç»å¾å°çï¼æ¨¡åå·²ç»ä¸ä¼ å°huggingfaceç æ¨¡ååº
 [shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-
 base-chinese)ï¼
 æ¯`text2vec.SentenceModel`æå®çé»è®¤æ¨¡åï¼å¯ä»¥éè¿ä¸é¢ç¤ºä¾è°ç¨ï¼æèå¦ä¸æç¤ºç¨
 [transformersåº](https://github.com/huggingface/transformers)è°ç¨ï¼
-æ¨¡åèªå¨ä¸è½½å°æ¬æºè·¯å¾ï¼`~/.cache/huggingface/transformers` -
-`sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`æ¨¡åæ¯Sentence-
-BERTçå¤è¯­è¨å¥åéæ¨¡åï¼
-éç¨äºéä¹ï¼paraphraseï¼è¯å«ï¼ææ¬å¹éï¼éè¿`text2vec.SentenceModel`å
-[sentence-transformersåº]((https://github.com/UKPLab/sentence-
-transformers))é½å¯ä»¥è°ç¨è¯¥æ¨¡å - `w2v-light-tencent-
+æ¨¡åèªå¨ä¸è½½å°æ¬æºè·¯å¾ï¼`~/.cache/huggingface/transformers` - `w2v-
+light-tencent-
 chinese`æ¯éè¿gensimå è½½çWord2Vecæ¨¡åï¼ä½¿ç¨è¾è®¯è¯åé`Tencent_AILab_ChineseEmbedding.tar.gz`è®¡ç®åå­è¯çè¯åéï¼å¥å­åééè¿åè¯è¯
 åéåå¹³åå¼å¾å°ï¼æ¨¡åèªå¨ä¸è½½å°æ¬æºè·¯å¾ï¼`~/.text2vec/
 datasets/light_Tencent_AILab_ChineseEmbedding.bin` #### Usage (HuggingFace
 Transformers) Without [text2vec](https://github.com/shibing624/text2vec), you
 can use the model like this: First, you pass your input through the transformer
 model, then you have to apply the right pooling-operation on-top of the
 contextualized word embeddings. example: [examples/
@@ -319,16 +339,16 @@
 ææ¬ç¸ä¼¼åº¦è®¡ç®åææ¬å¹éæç´¢ä»»å¡ï¼æ¨èä½¿ç¨
 [similaritiesåº](https://github.com/shibing624/similarities)
 ï¼å¼å®¹æ¬é¡¹ç®releaseç
 Word2vecãSBERTãCosentç±»è¯­ä¹å¹éæ¨¡åï¼è¿æ¯æå­é¢ç»´åº¦ç¸ä¼¼åº¦è®¡ç®ãå¹éæç´¢ç®æ³ï¼æ¯æææ¬ãå¾åã
 å®è£ï¼ ```pip install -U similarities``` å¥å­ç¸ä¼¼åº¦è®¡ç®ï¼ ```python
 from similarities import Similarity m = Similarity() r = m.similarity
 ('å¦ä½æ´æ¢è±åç»å®é¶è¡å¡', 'è±åæ´æ¹ç»å®é¶è¡å¡') print
-(f"similarity score: {float(r)}") # similarity score: 0.855146050453186 ``` #
-Models ## CoSENT model CoSENTï¼Cosine
+(f"similarity score: {float(r)}") # similarity score: 0.855146050453186 ``` ##
+Models ### CoSENT model CoSENTï¼Cosine
 Sentenceï¼ææ¬å¹éæ¨¡åï¼å¨Sentence-
 BERTä¸æ¹è¿äºCosineRankLossçå¥åéæ¹æ¡ Network structure: Training:
 [docs/cosent_train.png] Inference: [docs/inference.png] #### CoSENT
 çç£æ¨¡å è®­ç»åé¢æµCoSENTæ¨¡åï¼ - å¨ä¸­æSTS-
 Bæ°æ®éè®­ç»åè¯ä¼°`CoSENT`æ¨¡å example: [examples/
 training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/
 blob/master/examples/training_sup_text_matching_model.py) ```shell cd examples
@@ -340,21 +360,24 @@
 'PAWSX'ï¼å·ä½åèHuggingFace datasets [https://huggingface.co/datasets/
 shibing624/nli_zh](https://huggingface.co/datasets/shibing624/nli_zh) ```shell
 python training_sup_text_matching_model.py --task_name ATEC --model_arch cosent
 --do_train --do_predict --num_epochs 10 --model_name hfl/chinese-macbert-base -
 -output_dir ./outputs/ATEC-cosent ``` - å¨èªæä¸­ææ°æ®éä¸è®­ç»æ¨¡å
 example: [examples/training_sup_text_matching_model_mydata.py](https://
 github.com/shibing624/text2vec/blob/master/examples/
-training_sup_text_matching_model_mydata.py) ```shell python
-training_sup_text_matching_model_mydata.py --do_train --do_predict ```
-è®­ç»éæ ¼å¼åè[examples/data/STS-B/STS-B.valid.data](https://github.com/
-shibing624/text2vec/blob/master/examples/data/STS-B/STS-B.valid.data) ```shell
-sentence1 sentence2 label ä¸ä¸ªå¥³å­©å¨ç»å¥¹çå¤´ååååã
-ä¸ä¸ªå¥³å­©å¨æ¢³å¤´ã 2 ä¸ç¾¤ç·äººå¨æµ·æ»©ä¸è¸¢è¶³çã
-ä¸ç¾¤ç·å­©å¨æµ·æ»©ä¸è¸¢è¶³çã 3
+training_sup_text_matching_model_mydata.py) åå¡è®­ç»ï¼ ```shell
+CUDA_VISIBLE_DEVICES=0 python training_sup_text_matching_model_mydata.py --
+do_train --do_predict ``` å¤å¡è®­ç»ï¼ ```shell CUDA_VISIBLE_DEVICES=0,1
+torchrun --nproc_per_node 2 training_sup_text_matching_model_mydata.py --
+do_train --do_predict --output_dir outputs/STS-B-text2vec-macbert-v1 --
+batch_size 64 --fp16 --data_parallel ``` è®­ç»éæ ¼å¼åè[examples/data/
+STS-B/STS-B.valid.data](https://github.com/shibing624/text2vec/blob/master/
+examples/data/STS-B/STS-B.valid.data) ```shell sentence1 sentence2 label
+ä¸ä¸ªå¥³å­©å¨ç»å¥¹çå¤´ååååã ä¸ä¸ªå¥³å­©å¨æ¢³å¤´ã 2
+ä¸ç¾¤ç·äººå¨æµ·æ»©ä¸è¸¢è¶³çã ä¸ç¾¤ç·å­©å¨æµ·æ»©ä¸è¸¢è¶³çã 3
 ä¸ä¸ªå¥³äººå¨æµéå¦ä¸ä¸ªå¥³äººçèè¸ã
 å¥³äººæµéå¦ä¸ä¸ªå¥³äººçèè¸ã 5 ```
 `label`å¯ä»¥æ¯0ï¼1æ ç­¾ï¼0ä»£è¡¨ä¸¤ä¸ªå¥å­ä¸ç¸ä¼¼ï¼1ä»£è¡¨ç¸ä¼¼ï¼ä¹å¯ä»¥æ¯0-
 5çè¯åï¼è¯åè¶é«ï¼è¡¨ç¤ºä¸¤ä¸ªå¥å­è¶ç¸ä¼¼ãæ¨¡åé½è½æ¯æã
 - å¨è±æSTS-Bæ°æ®éè®­ç»åè¯ä¼°`CoSENT`æ¨¡å example: [examples/
 training_sup_text_matching_model_en.py](https://github.com/shibing624/text2vec/
 blob/master/examples/training_sup_text_matching_model_en.py) ```shell cd
@@ -363,15 +386,15 @@
 output_dir ./outputs/STS-B-en-cosent ``` #### CoSENT æ çç£æ¨¡å -
 å¨è±æNLIæ°æ®éè®­ç»`CoSENT`æ¨¡åï¼å¨STS-Bæµè¯éè¯ä¼°ææ
 example: [examples/training_unsup_text_matching_model_en.py](https://
 github.com/shibing624/text2vec/blob/master/examples/
 training_unsup_text_matching_model_en.py) ```shell cd examples python
 training_unsup_text_matching_model_en.py --model_arch cosent --do_train --
 do_predict --num_epochs 10 --model_name bert-base-uncased --output_dir ./
-outputs/STS-B-en-unsup-cosent ``` ## Sentence-BERT model Sentence-
+outputs/STS-B-en-unsup-cosent ``` ### Sentence-BERT model Sentence-
 BERTææ¬å¹éæ¨¡åï¼è¡¨å¾å¼å¥åéè¡¨ç¤ºæ¹æ¡ Network structure:
 Training: [docs/sbert_train.png] Inference: [docs/sbert_inference.png] ####
 SentenceBERT çç£æ¨¡å - å¨ä¸­æSTS-Bæ°æ®éè®­ç»åè¯ä¼°`SBERT`æ¨¡å
 example: [examples/training_sup_text_matching_model.py](https://github.com/
 shibing624/text2vec/blob/master/examples/training_sup_text_matching_model.py)
 ```shell cd examples python training_sup_text_matching_model.py --model_arch
 sentencebert --do_train --do_predict --num_epochs 10 --model_name hfl/chinese-
@@ -384,35 +407,35 @@
 uncased --output_dir ./outputs/STS-B-en-sbert ``` #### SentenceBERT
 æ çç£æ¨¡å - å¨è±æNLIæ°æ®éè®­ç»`SBERT`æ¨¡åï¼å¨STS-
 Bæµè¯éè¯ä¼°ææ example: [examples/
 training_unsup_text_matching_model_en.py](https://github.com/shibing624/
 text2vec/blob/master/examples/training_unsup_text_matching_model_en.py)
 ```shell cd examples python training_unsup_text_matching_model_en.py --
 model_arch sentencebert --do_train --do_predict --num_epochs 10 --model_name
-bert-base-uncased --output_dir ./outputs/STS-B-en-unsup-sbert ``` ## BERT-Match
-model
+bert-base-uncased --output_dir ./outputs/STS-B-en-unsup-sbert ``` ### BERT-
+Match model
 BERTææ¬å¹éæ¨¡åï¼åçBERTå¹éç½ç»ç»æï¼äº¤äºå¼å¥åéå¹éæ¨¡å
 Network structure: Training and inference: [docs/bert-fc-train.png]
 è®­ç»èæ¬åä¸[examples/training_sup_text_matching_model.py](https://
 github.com/shibing624/text2vec/blob/master/examples/
-training_sup_text_matching_model.py)ã ## æ¨¡åè¸é¦ï¼Model Distillationï¼
-ç±äºtext2vecè®­ç»çæ¨¡åå¯ä»¥ä½¿ç¨[sentence-transformers](https://
-github.com/UKPLab/sentence-
+training_sup_text_matching_model.py)ã ### æ¨¡åè¸é¦ï¼Model
+Distillationï¼ ç±äºtext2vecè®­ç»çæ¨¡åå¯ä»¥ä½¿ç¨[sentence-
+transformers](https://github.com/UKPLab/sentence-
 transformers)åºå è½½ï¼æ­¤å¤å¤ç¨å¶æ¨¡åè¸é¦æ¹æ³[distillation](https:
 //github.com/UKPLab/sentence-transformers/tree/master/examples/training/
 distillation)ã 1. æ¨¡åéç»´ï¼åè[dimensionality_reduction.py](https://
 github.com/UKPLab/sentence-transformers/blob/master/examples/training/
 distillation/
 dimensionality_reduction.py)ä½¿ç¨PCAå¯¹æ¨¡åè¾åºembeddingéç»´ï¼å¯åå°milvusç­åéæ£ç´¢æ°æ®åºçå­å¨ååï¼è¿è½è½»å¾®æåæ¨¡åææã
 2. æ¨¡åè¸é¦ï¼åè[model_distillation.py](https://github.com/UKPLab/
 sentence-transformers/blob/master/examples/training/distillation/
 model_distillation.py)ä½¿ç¨è¸é¦æ¹æ³ï¼å°Teacherå¤§æ¨¡åè¸é¦å°æ´å°layerså±æ°çstudentæ¨¡åä¸­ï¼å¨æè¡¡ææçæåµä¸ï¼å¯å¤§å¹æåæ¨¡åé¢æµéåº¦ã
-## æ¨¡åé¨ç½² æä¾ä¸¤ç§é¨ç½²æ¨¡åï¼æ­å»ºæå¡çæ¹æ³ï¼
+### æ¨¡åé¨ç½² æä¾ä¸¤ç§é¨ç½²æ¨¡åï¼æ­å»ºæå¡çæ¹æ³ï¼
 1ï¼åºäºJinaæ­å»ºgRPCæå¡ãæ¨èãï¼2ï¼åºäºFastAPIæ­å»ºåçHttpæå¡ã
-### Jinaæå¡ éç¨C/
+#### Jinaæå¡ éç¨C/
 Sæ¨¡å¼æ­å»ºé«æ§è½æå¡ï¼æ¯ædockeräºåçï¼gRPC/HTTP/
 WebSocketï¼æ¯æå¤ä¸ªæ¨¡ååæ¶é¢æµï¼GPUå¤å¡å¤çã - å®è£ï¼
 ```pip install jina``` - å¯å¨æå¡ï¼ example: [examples/
 jina_server_demo.py](examples/jina_server_demo.py) ```python from jina import
 Flow port = 50001 f = Flow(port=port).add( uses='jinahub://Text2vecEncoder',
 uses_with={'model_name': 'shibing624/text2vec-base-chinese'} ) with f: #
 backend server forever f.block() ```
@@ -421,27 +444,27 @@
 è°ç¨æå¡ï¼ ```python from jina import Client from docarray import
 Document, DocumentArray port = 50001 c = Client(port=port) data =
 ['å¦ä½æ´æ¢è±åç»å®é¶è¡å¡', 'è±åæ´æ¹ç»å®é¶è¡å¡'] print
 ("data:", data) print('data embs:') r = c.post('/', inputs=DocumentArray(
 [Document(text='å¦ä½æ´æ¢è±åç»å®é¶è¡å¡'), Document
 (text='è±åæ´æ¹ç»å®é¶è¡å¡')])) print(r.embeddings) ```
 æ¹éè°ç¨æ¹æ³è§example: [examples/jina_client_demo.py](https://
-github.com/shibing624/text2vec/blob/master/examples/jina_client_demo.py) ###
+github.com/shibing624/text2vec/blob/master/examples/jina_client_demo.py) ####
 FastAPIæå¡ - å®è£ï¼ ```pip install fastapi uvicorn``` - å¯å¨æå¡ï¼
 example: [examples/fastapi_server_demo.py](https://github.com/shibing624/
 text2vec/blob/master/examples/fastapi_server_demo.py) ```shell cd examples
 python fastapi_server_demo.py ``` - è°ç¨æå¡ï¼ ```shell curl -X 'GET' \
 'http://0.0.0.0:8001/emb?q=hello' \ -H 'accept: application/json' ``` ##
-æ°æ®é - æ¬é¡¹ç®releaseçæ°æ®éï¼ | Dataset | Introduce | Download
-Link | |:---------------------------|:-----------------------------------------
---------------------------------|:---------------------------------------------
+Dataset - æ¬é¡¹ç®releaseçæ°æ®éï¼ | Dataset | Introduce | Download Link
+| |:---------------------------|:----------------------------------------------
+---------------------------|:--------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
-------------| | shibing624/nli-zh-all |
+-------| | shibing624/nli-zh-all |
 ä¸­æè¯­ä¹å¹éæ°æ®åéï¼æ´åäºææ¬æ¨çï¼ç¸ä¼¼ï¼æè¦ï¼é®ç­ï¼æä»¤å¾®è°ç­ä»»å¡ç820ä¸é«è´¨éæ°æ®ï¼å¹¶è½¬åä¸ºå¹éæ ¼å¼æ°æ®é
 | [https://huggingface.co/datasets/shibing624/nli-zh-all](https://
 huggingface.co/datasets/shibing624/nli-zh-all) | | shibing624/snli-zh |
 ä¸­æSNLIåMultiNLIæ°æ®éï¼ç¿»è¯èªè±æSNLIåMultiNLI | [https://
 huggingface.co/datasets/shibing624/snli-zh](https://huggingface.co/datasets/
 shibing624/snli-zh) | | shibing624/nli_zh |
 ä¸­æè¯­ä¹å¹éæ°æ®éï¼æ´åäºä¸­æATECãBQãLCQMCãPAWSXãSTS-
@@ -459,46 +482,46 @@
 info/1037/1162.htm) | | LCQMC | ä¸­æLCQMC(large-scale Chinese question
 matching corpus)æ°æ®éï¼Q-Qpairæ°æ®é | [LCQMC](http://
 icrc.hitsz.edu.cn/Article/show/171.html) | | PAWSX | ä¸­æPAWS(Paraphrase
 Adversaries from Word Scrambling)æ°æ®éï¼Q-Qpairæ°æ®é | [PAWSX](https:/
 /arxiv.org/abs/1908.11828) | | STS-B | ä¸­æSTS-
 Bæ°æ®éï¼ä¸­æèªç¶è¯­è¨æ¨çæ°æ®éï¼ä»è±æSTS-
 Bç¿»è¯ä¸ºä¸­æçæ°æ®é | [STS-B](https://github.com/pluto-junzeng/CNSD) |
-å¸¸ç¨è±æå¹éæ°æ®éï¼ - å¤§åé¼é¼çmulti_nliåsnli: https://
-huggingface.co/datasets/multi_nli - å¤§åé¼é¼çmulti_nliåsnli: https://
+å¸¸ç¨è±æå¹éæ°æ®éï¼ - è±æå¹éæ°æ®éï¼multi_nli: https://
+huggingface.co/datasets/multi_nli - è±æå¹éæ°æ®éï¼snli: https://
 huggingface.co/datasets/snli - https://huggingface.co/datasets/metaeval/cnli -
 https://huggingface.co/datasets/mteb/stsbenchmark-sts - https://huggingface.co/
 datasets/JeremiahZ/simcse_sup_nli - https://huggingface.co/datasets/
 MoritzLaurer/multilingual-NLI-26lang-2mil7 æ°æ®éä½¿ç¨ç¤ºä¾ï¼ ```shell
 pip install datasets ``` ```python from datasets import load_dataset dataset =
 load_dataset("shibing624/nli_zh", "STS-B") # ATEC or BQ or LCQMC or PAWSX or
 STS-B print(dataset) print(dataset['test'][0]) ``` output: ```shell DatasetDict
 ({ train: Dataset({ features: ['sentence1', 'sentence2', 'label'], num_rows:
 5231 }) validation: Dataset({ features: ['sentence1', 'sentence2', 'label'],
 num_rows: 1458 }) test: Dataset({ features: ['sentence1', 'sentence2',
 'label'], num_rows: 1361 }) }) {'sentence1':
 'ä¸ä¸ªå¥³å­©å¨ç»å¥¹çå¤´ååååã', 'sentence2':
-'ä¸ä¸ªå¥³å­©å¨æ¢³å¤´ã', 'label': 2} ``` # Contact - Issue(å»ºè®®)ï¼[!
+'ä¸ä¸ªå¥³å­©å¨æ¢³å¤´ã', 'label': 2} ``` ## Contact - Issue(å»ºè®®)ï¼[!
 [GitHub issues](https://img.shields.io/github/issues/shibing624/text2vec.svg)]
 (https://github.com/shibing624/text2vec/issues) - é®ä»¶æï¼xuming:
 xuming624@qq.com - å¾®ä¿¡æï¼å æ*å¾®ä¿¡å·ï¼xuming624, å¤æ³¨ï¼å§å-
-å¬å¸-NLP* è¿NLPäº¤æµç¾¤ã [docs/wechat.jpeg] # Citation
+å¬å¸-NLP* è¿NLPäº¤æµç¾¤ã [docs/wechat.jpeg] ## Citation
 å¦æä½ å¨ç ç©¶ä¸­ä½¿ç¨äºtext2vecï¼è¯·æå¦ä¸æ ¼å¼å¼ç¨ï¼ APA:
 ```latex Xu, M. Text2vec: Text to vector toolkit (Version 1.1.2) [Computer
 software]. https://github.com/shibing624/text2vec ``` BibTeX: ```latex @misc
-{Text2vec, author = {Xu, Ming}, title = {Text2vec: Text to vector toolkit},
-year = {2022}, publisher = {GitHub}, journal = {GitHub repository},
-howpublished = {\url{https://github.com/shibing624/text2vec}}, } ``` # License
+{Text2vec, author = {Ming Xu}, title = {Text2vec: Text to vector toolkit}, year
+= {2023}, publisher = {GitHub}, journal = {GitHub repository}, howpublished =
+{\url{https://github.com/shibing624/text2vec}}, } ``` ## License
 ææåè®®ä¸º [The Apache License 2.0]
 (LICENSE)ï¼å¯åè´¹ç¨ååä¸ç¨éãè¯·å¨äº§åè¯´æä¸­éå text2vecçé¾æ¥åææåè®®ã
-# Contribute
+## Contribute
 é¡¹ç®ä»£ç è¿å¾ç²ç³ï¼å¦æå¤§å®¶å¯¹ä»£ç æææ¹è¿ï¼æ¬¢è¿æäº¤åæ¬é¡¹ç®ï¼å¨æäº¤ä¹åï¼æ³¨æä»¥ä¸ä¸¤ç¹ï¼
 - å¨`tests`æ·»å ç¸åºçååæµè¯ - ä½¿ç¨`python -m pytest -
 v`æ¥è¿è¡ææååæµè¯ï¼ç¡®ä¿ææåæµé½æ¯éè¿ç
-ä¹åå³å¯æäº¤PRã # Reference -
+ä¹åå³å¯æäº¤PRã ## References -
 [å°å¥å­è¡¨ç¤ºä¸ºåéï¼ä¸ï¼ï¼æ çç£å¥å­è¡¨ç¤ºå­¦ä¹ ï¼sentence
 embeddingï¼](https://www.cnblogs.com/llhthinker/p/10335164.html) -
 [å°å¥å­è¡¨ç¤ºä¸ºåéï¼ä¸ï¼ï¼æ çç£å¥å­è¡¨ç¤ºå­¦ä¹ ï¼sentence
 embeddingï¼](https://www.cnblogs.com/llhthinker/p/10341841.html) - [A Simple
 but Tough-to-Beat Baseline for Sentence Embeddings[Sanjeev Arora and Yingyu
 Liang and Tengyu Ma, 2017]](https://openreview.net/forum?id=SyK00v5xx) -
 [åç§è®¡ç®ææ¬ç¸ä¼¼åº¦çæ¹æ³å¯¹æ¯[Yves Peirsman]](https://
```

### Comparing `text2vec-1.2.1/setup.py` & `text2vec-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.1/text2vec/__init__.py` & `text2vec-1.2.2/text2vec/__init__.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.1/text2vec/bertmatching_dataset.py` & `text2vec-1.2.2/text2vec/bertmatching_dataset.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.1/text2vec/bertmatching_model.py` & `text2vec-1.2.2/text2vec/bertmatching_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import math
 import pandas as pd
 import torch
 from loguru import logger
 from torch import nn
 from torch.utils.data import DataLoader, Dataset
-from tqdm.auto import tqdm, trange
+from tqdm import tqdm, trange
 from transformers import BertForSequenceClassification, BertTokenizer
 from transformers.optimization import AdamW, get_linear_schedule_with_warmup
 
 from text2vec.bertmatching_dataset import (
     BertMatchingTestDataset,
     BertMatchingTrainDataset,
     HFBertMatchingTrainDataset,
@@ -102,14 +102,16 @@
             eps: float = 1e-6,
             gradient_accumulation_steps: int = 1,
             max_grad_norm: float = 1.0,
             max_steps: int = -1,
             use_hf_dataset: bool = False,
             hf_dataset_name: str = "STS-B",
             save_model_every_epoch: bool = True,
+            bf16: bool = False,
+            data_parallel: bool = False,
     ):
         """
         Trains the model on 'train_file'
 
         Args:
             train_file: Path to text file containing the text to _train the language model on.
             output_dir: The directory where model files will be saved. If not given, self.args.output_dir will be used.
@@ -124,14 +126,16 @@
             eps (optional): Adam epsilon.
             gradient_accumulation_steps (optional): Number of updates steps to accumulate before performing a backward/update pass.
             max_grad_norm (optional): Max gradient norm.
             max_steps (optional): If > 0: set total number of training steps to perform. Override num_epochs.
             use_hf_dataset (optional): Whether to use the HuggingFace datasets for training.
             hf_dataset_name (optional): Name of the dataset to use for the HuggingFace datasets.
             save_model_every_epoch (optional): Save model checkpoint every epoch.
+            bf16 (optional): Use bfloat16 amp training.
+            data_parallel (optional): Use multi-gpu data parallel training.
         Returns:
             global_step: Number of global steps trained
             training_details: Full training progress scores
         """
         if use_hf_dataset and hf_dataset_name:
             logger.info(
                 f"Train_file will be ignored when use_hf_dataset is True, load HF dataset: {hf_dataset_name}")
@@ -159,14 +163,16 @@
             warmup_ratio=warmup_ratio,
             lr=lr,
             eps=eps,
             gradient_accumulation_steps=gradient_accumulation_steps,
             max_grad_norm=max_grad_norm,
             max_steps=max_steps,
             save_model_every_epoch=save_model_every_epoch,
+            bf16=bf16,
+            data_parallel=data_parallel,
         )
         logger.info(f" Training model done. Saved to {output_dir}.")
 
         return global_step, training_details
 
     def train(
             self,
@@ -181,25 +187,30 @@
             warmup_ratio: float = 0.05,
             lr: float = 2e-5,
             eps: float = 1e-6,
             gradient_accumulation_steps: int = 1,
             max_grad_norm: float = 1.0,
             max_steps: int = -1,
             save_model_every_epoch: bool = True,
+            bf16: bool = False,
+            data_parallel: bool = False,
     ):
         """
         Trains the model on train_dataset.
 
         Utility function to be used by the train_model() method. Not intended to be used directly.
         """
         os.makedirs(output_dir, exist_ok=True)
         logger.debug("Use pytorch device: {}".format(device))
         self.model.bert.to(device)
         set_seed(seed)
 
+        if data_parallel:
+            self.bert = nn.DataParallel(self.bert)
+
         train_dataloader = DataLoader(train_dataset, batch_size=batch_size)  # keep the order of the data, not shuffle
         total_steps = len(train_dataloader) * num_epochs
         param_optimizer = list(self.model.bert.named_parameters())
         no_decay = ['bias', 'LayerNorm.bias', 'LayerNorm.weight']
         optimizer_grouped_parameters = [
             {'params': [p for n, p in param_optimizer if not any(nd in n for nd in no_decay)],
              'weight_decay': weight_decay},
@@ -263,16 +274,24 @@
                     steps_trained_in_current_epoch -= 1
                     continue
                 inputs, labels = batch
                 labels = labels.to(device)
                 # inputs        [batch, 1, seq_len] -> [batch, seq_len]
                 input_ids = inputs.get('input_ids').squeeze(1).to(device)
                 attention_mask = inputs.get('attention_mask').squeeze(1).to(device)
-                token_type_ids = inputs.get('token_type_ids').squeeze(1).to(device)
-                loss, logits, probs = self.model(input_ids, attention_mask, token_type_ids, labels)
+                token_type_ids = inputs.get('token_type_ids', None)
+                if token_type_ids is not None:
+                    token_type_ids = token_type_ids.squeeze(1).to(self.device)
+
+                if bf16:
+                    with torch.autocast('cuda', dtype=torch.bfloat16):
+                        loss, logits, probs = self.model(input_ids, attention_mask, token_type_ids, labels)
+                else:
+                    loss, logits, probs = self.model(input_ids, attention_mask, token_type_ids, labels)
+                    
                 current_loss = loss.item()
 
                 if verbose:
                     batch_iterator.set_description(
                         f"Epoch: {epoch_number + 1}/{num_epochs}, Batch:{step}/{len(train_dataloader)}, Loss: {current_loss:9.4f}")
 
                 if gradient_accumulation_steps > 1:
```

### Comparing `text2vec-1.2.1/text2vec/bm25.py` & `text2vec-1.2.2/text2vec/bm25.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.1/text2vec/cosent_dataset.py` & `text2vec-1.2.2/text2vec/cosent_dataset.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.1/text2vec/cosent_model.py` & `text2vec-1.2.2/text2vec/cosent_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
 @description: Create CoSENT model for text matching task
 """
 
+import math
 import os
 
-import math
 import pandas as pd
 import torch
 from loguru import logger
+from torch import nn
 from torch.utils.data import DataLoader, Dataset
-from tqdm.auto import tqdm, trange
+from tqdm import tqdm, trange
 from transformers.optimization import AdamW, get_linear_schedule_with_warmup
 
 from text2vec.cosent_dataset import CosentTrainDataset, load_cosent_train_data, HFCosentTrainDataset
 from text2vec.sentence_model import SentenceModel
 from text2vec.text_matching_dataset import TextMatchingTestDataset, load_text_matching_test_data, \
     HFTextMatchingTestDataset
 from text2vec.utils.stats_util import set_seed
@@ -59,14 +60,16 @@
             eps: float = 1e-6,
             gradient_accumulation_steps: int = 1,
             max_grad_norm: float = 1.0,
             max_steps: int = -1,
             use_hf_dataset: bool = False,
             hf_dataset_name: str = "STS-B",
             save_model_every_epoch: bool = True,
+            bf16: bool = False,
+            data_parallel: bool = False,
     ):
         """
         Trains the model on 'train_file'
 
         Args:
             train_file: Path to text file containing the text to _train the language model on.
             output_dir: The directory where model files will be saved. If not given, self.args.output_dir will be used.
@@ -81,14 +84,16 @@
             eps (optional): Adam epsilon.
             gradient_accumulation_steps (optional): Number of updates steps to accumulate before performing a backward/update pass.
             max_grad_norm (optional): Max gradient norm.
             max_steps (optional): If > 0: set total number of training steps to perform. Override num_epochs.
             use_hf_dataset (optional): Whether to use the HF dataset.
             hf_dataset_name (optional): Name of the dataset to use for the HuggingFace datasets.
             save_model_every_epoch (optional): Save model checkpoint every epoch.
+            bf16 (optional): Use bfloat16 amp training.
+            data_parallel (optional): Use multi-gpu data parallel training.
         Returns:
             global_step: Number of global steps trained
             training_details: full training progress scores
         """
         if use_hf_dataset and hf_dataset_name:
             logger.info(
                 f"Train_file will be ignored when use_hf_dataset is True, load HF dataset: {hf_dataset_name}")
@@ -115,14 +120,16 @@
             warmup_ratio=warmup_ratio,
             lr=lr,
             eps=eps,
             gradient_accumulation_steps=gradient_accumulation_steps,
             max_grad_norm=max_grad_norm,
             max_steps=max_steps,
             save_model_every_epoch=save_model_every_epoch,
+            bf16=bf16,
+            data_parallel=data_parallel,
         )
         logger.info(f" Training model done. Saved to {output_dir}.")
 
         return global_step, training_details
 
     def calc_loss(self, y_true, y_pred):
         """
@@ -159,25 +166,30 @@
             warmup_ratio: float = 0.05,
             lr: float = 2e-5,
             eps: float = 1e-6,
             gradient_accumulation_steps: int = 1,
             max_grad_norm: float = 1.0,
             max_steps: int = -1,
             save_model_every_epoch: bool = True,
+            bf16: bool = False,
+            data_parallel: bool = False,
     ):
         """
         Trains the model on train_dataset.
 
         Utility function to be used by the train_model() method. Not intended to be used directly.
         """
         os.makedirs(output_dir, exist_ok=True)
         logger.debug("Use device: {}".format(self.device))
         self.bert.to(self.device)
         set_seed(seed)
 
+        if data_parallel:
+            self.bert = nn.DataParallel(self.bert)
+
         train_dataloader = DataLoader(train_dataset, batch_size=batch_size)  # keep the order of the data, not shuffle
         total_steps = len(train_dataloader) * num_epochs
         param_optimizer = list(self.bert.named_parameters())
         no_decay = ['bias', 'LayerNorm.bias', 'LayerNorm.weight']
         optimizer_grouped_parameters = [
             {'params': [p for n, p in param_optimizer if not any(nd in n for nd in no_decay)],
              'weight_decay': weight_decay},
@@ -241,17 +253,26 @@
                     steps_trained_in_current_epoch -= 1
                     continue
                 inputs, labels = batch
                 labels = labels.to(self.device)
                 # inputs        [batch, 1, seq_len] -> [batch, seq_len]
                 input_ids = inputs.get('input_ids').squeeze(1).to(self.device)
                 attention_mask = inputs.get('attention_mask').squeeze(1).to(self.device)
-                token_type_ids = inputs.get('token_type_ids').squeeze(1).to(self.device)
-                output_embeddings = self.get_sentence_embeddings(input_ids, attention_mask, token_type_ids)
-                loss = self.calc_loss(labels, output_embeddings)
+                token_type_ids = inputs.get('token_type_ids', None)
+                if token_type_ids is not None:
+                    token_type_ids = token_type_ids.squeeze(1).to(self.device)
+
+                if bf16:
+                    with torch.autocast('cuda', dtype=torch.bfloat16):
+                        output_embeddings = self.get_sentence_embeddings(input_ids, attention_mask, token_type_ids)
+                        loss = self.calc_loss(labels, output_embeddings)
+                else:
+                    output_embeddings = self.get_sentence_embeddings(input_ids, attention_mask, token_type_ids)
+                    loss = self.calc_loss(labels, output_embeddings)
+
                 current_loss = loss.item()
                 if verbose:
                     batch_iterator.set_description(
                         f"Epoch: {epoch_number + 1}/{num_epochs}, Batch:{step}/{len(train_dataloader)}, Loss: {current_loss:9.4f}")
 
                 if gradient_accumulation_steps > 1:
                     loss = loss / gradient_accumulation_steps
```

### Comparing `text2vec-1.2.1/text2vec/ngram.py` & `text2vec-1.2.2/text2vec/ngram.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.1/text2vec/sentence_model.py` & `text2vec-1.2.2/text2vec/sentence_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from enum import Enum
 from typing import List, Union, Optional
 
 import numpy as np
 import torch
 from loguru import logger
 from torch.utils.data import DataLoader, Dataset
-from tqdm.auto import tqdm, trange
+from tqdm import tqdm, trange
 from tqdm.autonotebook import trange
 from transformers import AutoTokenizer, AutoModel
 
 from text2vec.utils.stats_util import compute_spearmanr, compute_pearsonr
 
 os.environ["KMP_DUPLICATE_LIB_OK"] = "TRUE"
 os.environ["TOKENIZERS_PARALLELISM"] = "TRUE"
@@ -89,15 +89,15 @@
         -------
         int or None
             The dimension of the sentence embeddings, or None if it cannot be determined.
         """
         # Use getattr to safely access the out_features attribute of the pooler's dense layer
         return getattr(self.bert.pooler.dense, "out_features", None)
 
-    def get_sentence_embeddings(self, input_ids, attention_mask, token_type_ids):
+    def get_sentence_embeddings(self, input_ids, attention_mask, token_type_ids=None):
         """
         Returns the model output by encoder_type as embeddings.
 
         Utility function for self.bert() method.
         """
         model_output = self.bert(input_ids, attention_mask, token_type_ids, output_hidden_states=True)
 
@@ -223,20 +223,24 @@
         for batch in tqdm(eval_dataloader, disable=False, desc="Running Evaluation"):
             source, target, labels = batch
             labels = labels.to(self.device)
             batch_labels.extend(labels.cpu().numpy())
             # source        [batch, 1, seq_len] -> [batch, seq_len]
             source_input_ids = source.get('input_ids').squeeze(1).to(self.device)
             source_attention_mask = source.get('attention_mask').squeeze(1).to(self.device)
-            source_token_type_ids = source.get('token_type_ids').squeeze(1).to(self.device)
+            source_token_type_ids = source.get('token_type_ids', None)
+            if source_token_type_ids is not None:
+                source_token_type_ids = source_token_type_ids.squeeze(1).to(self.device)
 
             # target        [batch, 1, seq_len] -> [batch, seq_len]
             target_input_ids = target.get('input_ids').squeeze(1).to(self.device)
             target_attention_mask = target.get('attention_mask').squeeze(1).to(self.device)
-            target_token_type_ids = target.get('token_type_ids').squeeze(1).to(self.device)
+            target_token_type_ids = target.get('token_type_ids', None)
+            if target_token_type_ids is not None:
+                target_token_type_ids = target_token_type_ids.squeeze(1).to(self.device)
 
             with torch.no_grad():
                 source_embeddings = self.get_sentence_embeddings(source_input_ids, source_attention_mask,
                                                                  source_token_type_ids)
                 target_embeddings = self.get_sentence_embeddings(target_input_ids, target_attention_mask,
                                                                  target_token_type_ids)
                 preds = torch.cosine_similarity(source_embeddings, target_embeddings)
```

### Comparing `text2vec-1.2.1/text2vec/sentencebert_model.py` & `text2vec-1.2.2/text2vec/sentencebert_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
 @description: Create Sentence-BERT model for text matching task
 """
 
+import math
 import os
 
-import math
 import pandas as pd
 import torch
 from loguru import logger
 from torch import nn
 from torch.utils.data import DataLoader, Dataset
-from tqdm.auto import tqdm, trange
+from tqdm import tqdm, trange
 from transformers.optimization import AdamW, get_linear_schedule_with_warmup
 
 from text2vec.sentence_model import SentenceModel
 from text2vec.text_matching_dataset import (
     TextMatchingTrainDataset,
     TextMatchingTestDataset,
     load_text_matching_test_data,
@@ -68,14 +68,16 @@
             eps: float = 1e-6,
             gradient_accumulation_steps: int = 1,
             max_grad_norm: float = 1.0,
             max_steps: int = -1,
             use_hf_dataset: bool = False,
             hf_dataset_name: str = "STS-B",
             save_model_every_epoch: bool = True,
+            bf16: bool = False,
+            data_parallel: bool = False,
     ):
         """
         Trains the model on 'train_file'
 
         Args:
             train_file: Path to text file containing the text to _train the language model on.
             output_dir: The directory where model files will be saved. If not given, self.args.output_dir will be used.
@@ -90,14 +92,16 @@
             eps (optional): Adam epsilon.
             gradient_accumulation_steps (optional): Number of updates steps to accumulate before performing a backward/update pass.
             max_grad_norm (optional): Max gradient norm.
             max_steps (optional): If > 0: set total number of training steps to perform. Override num_epochs.
             use_hf_dataset (optional): Whether to use the HuggingFace datasets for training.
             hf_dataset_name (optional): Name of the dataset to use for the HuggingFace datasets.
             save_model_every_epoch (optional): Save model checkpoint every epoch.
+            bf16 (optional): Use bfloat16 amp training.
+            data_parallel (optional): Use multi-gpu data parallel training.
         Returns:
             global_step: Number of global steps trained
             training_details: Full training progress scores
         """
         if use_hf_dataset and hf_dataset_name:
             logger.info(
                 f"Train_file will be ignored when use_hf_dataset is True, load HF dataset: {hf_dataset_name}")
@@ -125,14 +129,16 @@
             warmup_ratio=warmup_ratio,
             lr=lr,
             eps=eps,
             gradient_accumulation_steps=gradient_accumulation_steps,
             max_grad_norm=max_grad_norm,
             max_steps=max_steps,
             save_model_every_epoch=save_model_every_epoch,
+            bf16=bf16,
+            data_parallel=data_parallel,
         )
         logger.info(f" Training model done. Saved to {output_dir}.")
 
         return global_step, training_details
 
     def concat_embeddings(self, source_embeddings, target_embeddings):
         """
@@ -169,25 +175,30 @@
             warmup_ratio: float = 0.05,
             lr: float = 2e-5,
             eps: float = 1e-6,
             gradient_accumulation_steps: int = 1,
             max_grad_norm: float = 1.0,
             max_steps: int = -1,
             save_model_every_epoch: bool = True,
+            bf16: bool = False,
+            data_parallel: bool = False,
     ):
         """
         Trains the model on train_dataset.
 
         Utility function to be used by the train_model() method. Not intended to be used directly.
         """
         os.makedirs(output_dir, exist_ok=True)
         logger.debug("Use pytorch device: {}".format(self.device))
         self.bert.to(self.device)
         set_seed(seed)
 
+        if data_parallel:
+            self.bert = nn.DataParallel(self.bert)
+
         train_dataloader = DataLoader(train_dataset, batch_size=batch_size)  # keep the order of the data, not shuffle
         total_steps = len(train_dataloader) * num_epochs
         param_optimizer = list(self.bert.named_parameters())
         no_decay = ['bias', 'LayerNorm.bias', 'LayerNorm.weight']
         optimizer_grouped_parameters = [
             {'params': [p for n, p in param_optimizer if not any(nd in n for nd in no_decay)],
              'weight_decay': weight_decay},
@@ -250,28 +261,42 @@
                 if steps_trained_in_current_epoch > 0:
                     steps_trained_in_current_epoch -= 1
                     continue
                 source, target, labels = batch
                 # source        [batch, 1, seq_len] -> [batch, seq_len]
                 source_input_ids = source.get('input_ids').squeeze(1).to(self.device)
                 source_attention_mask = source.get('attention_mask').squeeze(1).to(self.device)
-                source_token_type_ids = source.get('token_type_ids').squeeze(1).to(self.device)
+                source_token_type_ids = source.get('token_type_ids', None)
+                if source_token_type_ids is not None:
+                    source_token_type_ids = source_token_type_ids.squeeze(1).to(self.device)
                 # target        [batch, 1, seq_len] -> [batch, seq_len]
                 target_input_ids = target.get('input_ids').squeeze(1).to(self.device)
                 target_attention_mask = target.get('attention_mask').squeeze(1).to(self.device)
-                target_token_type_ids = target.get('token_type_ids').squeeze(1).to(self.device)
+                target_token_type_ids = target.get('token_type_ids', None)
+                if target_token_type_ids is not None:
+                    target_token_type_ids = target_token_type_ids.squeeze(1).to(self.device)
                 labels = labels.to(self.device)
 
                 # get sentence embeddings of BERT encoder
-                source_embeddings = self.get_sentence_embeddings(source_input_ids, source_attention_mask,
-                                                                 source_token_type_ids)
-                target_embeddings = self.get_sentence_embeddings(target_input_ids, target_attention_mask,
-                                                                 target_token_type_ids)
-                logits = self.concat_embeddings(source_embeddings, target_embeddings)
-                loss = self.calc_loss(labels, logits)
+                if bf16:
+                    with torch.autocast('cuda', dtype=torch.bfloat16):
+                        source_embeddings = self.get_sentence_embeddings(source_input_ids, source_attention_mask,
+                                                                         source_token_type_ids)
+                        target_embeddings = self.get_sentence_embeddings(target_input_ids, target_attention_mask,
+                                                                         target_token_type_ids)
+                        logits = self.concat_embeddings(source_embeddings, target_embeddings)
+                        loss = self.calc_loss(labels, logits)
+                else:
+                    source_embeddings = self.get_sentence_embeddings(source_input_ids, source_attention_mask,
+                                                                     source_token_type_ids)
+                    target_embeddings = self.get_sentence_embeddings(target_input_ids, target_attention_mask,
+                                                                     target_token_type_ids)
+                    logits = self.concat_embeddings(source_embeddings, target_embeddings)
+                    loss = self.calc_loss(labels, logits)
+
                 current_loss = loss.item()
                 if verbose:
                     batch_iterator.set_description(
                         f"Epoch: {epoch_number + 1}/{num_epochs}, Batch:{step}/{len(train_dataloader)}, Loss: {current_loss:9.4f}")
 
                 if gradient_accumulation_steps > 1:
                     loss = loss / gradient_accumulation_steps
```

### Comparing `text2vec-1.2.1/text2vec/similarity.py` & `text2vec-1.2.2/text2vec/similarity.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.1/text2vec/stopwords.txt` & `text2vec-1.2.2/text2vec/stopwords.txt`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.1/text2vec/text_matching_dataset.py` & `text2vec-1.2.2/text2vec/text_matching_dataset.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.1/text2vec/utils/distance.py` & `text2vec-1.2.2/text2vec/utils/distance.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     余弦距离
     return cos score
     """
     up = float(np.sum(v1 * v2))
     down = np.linalg.norm(v1) * np.linalg.norm(v2)
     return try_divide(up, down)
 
+
 def hamming_distance(v1, v2):
     n = int(v1, 2) ^ int(v2, 2)
     return bin(n & 0xffffffff).count('1')
 
 
 def euclidean_distance(v1, v2):  # 欧氏距离
     return np.sqrt(np.sum(np.square(v1 - v2)))
@@ -41,16 +42,21 @@
     return np.sum(np.abs(v1 - v2))
 
 
 def chebyshev_distance(v1, v2):  # 切比雪夫距离
     return np.max(np.abs(v1 - v2))
 
 
-def minkowski_distance(v1, v2):  # 闵可夫斯基距离
-    return np.sqrt(np.sum(np.square(v1 - v2)))
+def minkowski_distance(v1, v2, p=2):
+    """
+    闵可夫斯基距离
+        p=1 曼哈顿距离
+        p=2 欧氏距离
+    """
+    return np.power(np.sum(np.power(np.abs(v1 - v2), p)), 1 / p)
 
 
 def euclidean_distance_standardized(v1, v2):  # 标准化欧氏距离
     v1_v2 = np.vstack([v1, v2])
     sk_v1_v2 = np.var(v1_v2, axis=0, ddof=1)
     return np.sqrt(((v1 - v2) ** 2 / (sk_v1_v2 + zero_bit * np.ones_like(sk_v1_v2))).sum())
 
@@ -206,15 +212,14 @@
     x = np.array(x).astype(float)
     xr = np.rollaxis(x, axis=axis)
     xr -= np.mean(x, axis=axis)
     xr /= np.std(x, axis=axis)
     return x
 
 
-
 if __name__ == '__main__':
     vec1_test = np.array([1, 38, 17, 32])
     vec2_test = np.array([5, 6, 8, 9])
 
     str1_test = "你到底是谁?"
     str2_test = "没想到我是谁，是真样子"
```

### Comparing `text2vec-1.2.1/text2vec/utils/get_file.py` & `text2vec-1.2.2/text2vec/utils/get_file.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.1/text2vec/utils/io_util.py` & `text2vec-1.2.2/text2vec/utils/io_util.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.1/text2vec/utils/rank_bm25.py` & `text2vec-1.2.2/text2vec/utils/rank_bm25.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.1/text2vec/utils/stats_util.py` & `text2vec-1.2.2/text2vec/utils/stats_util.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.1/text2vec/utils/tokenizer.py` & `text2vec-1.2.2/text2vec/utils/tokenizer.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.1/text2vec/word2vec.py` & `text2vec-1.2.2/text2vec/word2vec.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.1/text2vec.egg-info/PKG-INFO` & `text2vec-1.2.2/text2vec.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2vec
-Version: 1.2.1
+Version: 1.2.2
 Summary: Text to vector Tool, encode text
 Home-page: https://github.com/shibing624/text2vec
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache License 2.0
 Description: [**🇨🇳中文**](https://github.com/shibing624/text2vec/blob/master/README.md) | [**🌐English**](https://github.com/shibing624/text2vec/blob/master/README_EN.md) | [**📖文档/Docs**](https://github.com/shibing624/text2vec/wiki) | [**🤖模型/Models**](https://huggingface.co/shibing624) 
         
@@ -27,54 +27,57 @@
         
         
         **Text2vec**: Text to Vector, Get Sentence Embeddings. 文本向量化，把文本(包括词、句子、段落)表征为向量矩阵。
         
         **text2vec**实现了Word2Vec、RankBM25、BERT、Sentence-BERT、CoSENT等多种文本表征、文本相似度计算模型，并在文本语义匹配（相似度计算）任务上比较了各模型的效果。
         
         ### News
+        [2023/06/22] v1.2.2版本: 发布了多语言匹配模型[shibing624/text2vec-base-multilingual](https://huggingface.co/shibing624/text2vec-base-multilingual)，用CoSENT方法训练，基于`sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`用人工挑选后的多语言STS数据集[shibing624/nli-zh-all/text2vec-base-multilingual-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-multilingual-dataset)训练得到，并在中英文测试集评估相对于原模型效果有提升，详见[Release-v1.2.2](https://github.com/shibing624/text2vec/releases/tag/1.2.2)
+        
         [2023/06/19] v1.2.1版本: 更新了中文匹配模型`shibing624/text2vec-base-chinese-nli`为新版[shibing624/text2vec-base-chinese-sentence](https://huggingface.co/shibing624/text2vec-base-chinese-sentence)，针对CoSENT的loss计算对排序敏感特点，人工挑选并整理出高质量的有相关性排序的STS数据集[shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-sentence-dataset)，在各评估集表现相对之前有提升；发布了适用于s2p的中文匹配模型[shibing624/text2vec-base-chinese-paraphrase](https://huggingface.co/shibing624/text2vec-base-chinese-paraphrase)，详见[Release-v1.2.1](https://github.com/shibing624/text2vec/releases/tag/1.2.1)
         
         [2023/06/15] v1.2.0版本: 发布了中文匹配模型[shibing624/text2vec-base-chinese-nli](https://huggingface.co/shibing624/text2vec-base-chinese-nli)，基于`nghuyong/ernie-3.0-base-zh`模型，使用了中文NLI数据集[shibing624/nli_zh](https://huggingface.co/datasets/shibing624/nli_zh)全部语料训练的CoSENT文本匹配模型，在各评估集表现提升明显，详见[Release-v1.2.0](https://github.com/shibing624/text2vec/releases/tag/1.2.0)
         
         [2022/03/12] v1.1.4版本: 发布了中文匹配模型[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)，基于中文STS训练集训练的CoSENT匹配模型。详见[Release-v1.1.4](https://github.com/shibing624/text2vec/releases/tag/1.1.4)
         
         
         **Guide**
-        - [Feature](#Feature)
+        - [Features](#Features)
         - [Evaluation](#Evaluation)
         - [Install](#install)
         - [Usage](#usage)
         - [Contact](#Contact)
-        - [Reference](#reference)
+        - [References](#references)
         
         
-        # Feature
+        ## Features
         ### 文本向量表示模型
         - [Word2Vec](https://github.com/shibing624/text2vec/blob/master/text2vec/word2vec.py)：通过腾讯AI Lab开源的大规模高质量中文[词向量数据（800万中文词轻量版）](https://pan.baidu.com/s/1La4U4XNFe8s5BJqxPQpeiQ) (文件名：light_Tencent_AILab_ChineseEmbedding.bin 密码: tawe）实现词向量检索，本项目实现了句子（词向量求平均）的word2vec向量表示
         - [SBERT(Sentence-BERT)](https://github.com/shibing624/text2vec/blob/master/text2vec/sentencebert_model.py)：权衡性能和效率的句向量表示模型，训练时通过有监督训练上层分类函数，文本匹配预测时直接句子向量做余弦，本项目基于PyTorch复现了Sentence-BERT模型的训练和预测
         - [CoSENT(Cosine Sentence)](https://github.com/shibing624/text2vec/blob/master/text2vec/cosent_model.py)：CoSENT模型提出了一种排序的损失函数，使训练过程更贴近预测，模型收敛速度和效果比Sentence-BERT更好，本项目基于PyTorch实现了CoSENT模型的训练和预测
         
         详细文本向量表示方法见wiki: [文本向量表示方法](https://github.com/shibing624/text2vec/wiki/%E6%96%87%E6%9C%AC%E5%90%91%E9%87%8F%E8%A1%A8%E7%A4%BA%E6%96%B9%E6%B3%95)
-        # Evaluation
+        ## Evaluation
         
         文本匹配
         
         #### 英文匹配数据集的评测结果：
         
         
-        | Arch   | BaseModel                                        | Model                            | English-STS-B | 
-        |:-------|:------------------------------------------------|:-------------------------------------|:-------------:|
-        | GloVe  | glove                                           | Avg_word_embeddings_glove_6B_300d    |     61.77     |
-        | BERT   | bert-base-uncased                               | BERT-base-cls                        |     20.29     |
-        | BERT   | bert-base-uncased                               | BERT-base-first_last_avg             |     59.04     |
-        | BERT   | bert-base-uncased                               | BERT-base-first_last_avg-whiten(NLI) |     63.65     |
-        | SBERT  | sentence-transformers/bert-base-nli-mean-tokens | SBERT-base-nli-cls                   |     73.65     |
-        | SBERT  | sentence-transformers/bert-base-nli-mean-tokens | SBERT-base-nli-first_last_avg        |     77.96     |
-        | CoSENT | bert-base-uncased                               | CoSENT-base-first_last_avg           |     69.93     |
-        | CoSENT | sentence-transformers/bert-base-nli-mean-tokens | CoSENT-base-nli-first_last_avg       |     79.68     |
+        | Arch   | BaseModel                                        | Model                                                                                                                | English-STS-B | 
+        |:-------|:------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------|:-------------:|
+        | GloVe  | glove                                           | Avg_word_embeddings_glove_6B_300d                                                                                    |     61.77     |
+        | BERT   | bert-base-uncased                               | BERT-base-cls                                                                                                        |     20.29     |
+        | BERT   | bert-base-uncased                               | BERT-base-first_last_avg                                                                                             |     59.04     |
+        | BERT   | bert-base-uncased                               | BERT-base-first_last_avg-whiten(NLI)                                                                                 |     63.65     |
+        | SBERT  | sentence-transformers/bert-base-nli-mean-tokens | SBERT-base-nli-cls                                                                                                   |     73.65     |
+        | SBERT  | sentence-transformers/bert-base-nli-mean-tokens | SBERT-base-nli-first_last_avg                                                                                        |     77.96     |
+        | CoSENT | bert-base-uncased                               | CoSENT-base-first_last_avg                                                                                           |     69.93     |
+        | CoSENT | sentence-transformers/bert-base-nli-mean-tokens | CoSENT-base-nli-first_last_avg                                                                                       |     79.68     |
+        | CoSENT | sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2 | [shibing624/text2vec-base-multilingual](https://huggingface.co/shibing624/text2vec-base-multilingual)                |     80.12     |
         
         #### 中文匹配数据集的评测结果：
         
         
         | Arch   | BaseModel                    | Model           | ATEC  |  BQ   | LCQMC | PAWSX | STS-B |  Avg  | 
         |:-------|:----------------------------|:--------------------|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|
         | SBERT  | bert-base-chinese           | SBERT-bert-base     | 46.36 | 70.36 | 78.72 | 46.86 | 66.41 | 61.74 |
@@ -83,59 +86,60 @@
         | CoSENT | bert-base-chinese           | CoSENT-bert-base    | 49.74 | 72.38 | 78.69 | 60.00 | 79.27 | 68.01 |
         | CoSENT | hfl/chinese-macbert-base    | CoSENT-macbert-base | 50.39 | 72.93 | 79.17 | 60.86 | 79.30 | 68.53 |
         | CoSENT | hfl/chinese-roberta-wwm-ext | CoSENT-roberta-ext  | 50.81 | 71.45 | 79.31 | 61.56 | 79.96 | 68.61 |
         
         说明：
         - 结果评测指标：spearman系数
         - 为评测模型能力，结果均只用该数据集的train训练，在test上评估得到的表现，没用外部数据
+        - `SBERT-macbert-base`模型，是用SBert方法训练，运行[examples/training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model.py)代码可训练模型
+        - `sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`模型是用SBert训练，是`paraphrase-MiniLM-L12-v2`模型的多语言版本，支持中文、英文等
         
         
         ### Release Models
         - 本项目release模型的中文匹配评测结果：
         
-        | Arch       | BaseModel                         | Model                                                                                                                                             | ATEC  |  BQ   | LCQMC | PAWSX | STS-B | SOHU-dd | SOHU-dc |    Avg    |  QPS  |
-        |:-----------|:----------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------|:-----:|:-----:|:-----:|:-----:|:-----:|:-------:|:-------:|:---------:|:-----:|
-        | Word2Vec   | word2vec                          | [w2v-light-tencent-chinese](https://ai.tencent.com/ailab/nlp/en/download.html)                                                                    | 20.00 | 31.49 | 59.46 | 2.57  | 55.78 |  55.04  |  20.70  |   35.03   | 23769 |
-        | SBERT      | xlm-roberta-base                  | [sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2](https://huggingface.co/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2) | 18.42 | 38.52 | 63.96 | 10.14 | 78.90 |  63.01  |  52.28  |   46.46   | 3138  |
-        | Instructor | hfl/chinese-roberta-wwm-ext       | [moka-ai/m3e-base](https://huggingface.co/moka-ai/m3e-base)                                                                                       | 41.27 | 63.81 | 74.87 | 12.20 | 76.96 |  75.83  |  60.55  |   57.93   | 2980  |
-        | CoSENT     | hfl/chinese-macbert-base          | [shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)                                                       | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 |  70.27  |  50.42  |   51.61   | 3008  |
-        | CoSENT     | hfl/chinese-lert-large            | [GanymedeNil/text2vec-large-chinese](https://huggingface.co/GanymedeNil/text2vec-large-chinese)                                                   | 32.61 | 44.59 | 69.30 | 14.51 | 79.44 |  73.01  |  59.04  |   53.12   | 2092  |
-        | CoSENT     | nghuyong/ernie-3.0-base-zh        | [shibing624/text2vec-base-chinese-sentence](https://huggingface.co/shibing624/text2vec-base-chinese-sentence)                                     | 43.37 | 61.43 | 73.48 | 38.90 | 78.25 |  70.60  |  53.08  |   59.87   | 3089  |
-        | CoSENT     | nghuyong/ernie-3.0-base-zh        | [shibing624/text2vec-base-chinese-paraphrase](https://huggingface.co/shibing624/text2vec-base-chinese-paraphrase)                                 | 44.89 | 63.58 | 74.24 | 40.90 | 78.93 |  76.70  |  63.30  | **63.08** | 3066  |
+        | Arch       | BaseModel                                                    | Model                                                                                                                                             | ATEC  |  BQ   | LCQMC | PAWSX | STS-B | SOHU-dd | SOHU-dc |    Avg    |  QPS  |
+        |:-----------|:-------------------------------------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------|:-----:|:-----:|:-----:|:-----:|:-----:|:-------:|:-------:|:---------:|:-----:|
+        | Word2Vec   | word2vec                                                     | [w2v-light-tencent-chinese](https://ai.tencent.com/ailab/nlp/en/download.html)                                                                    | 20.00 | 31.49 | 59.46 | 2.57  | 55.78 |  55.04  |  20.70  |   35.03   | 23769 |
+        | SBERT      | xlm-roberta-base                                             | [sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2](https://huggingface.co/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2) | 18.42 | 38.52 | 63.96 | 10.14 | 78.90 |  63.01  |  52.28  |   46.46   | 3138  |
+        | CoSENT     | hfl/chinese-macbert-base                                     | [shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)                                                       | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 |  70.27  |  50.42  |   51.61   | 3008  |
+        | CoSENT     | hfl/chinese-lert-large                                       | [GanymedeNil/text2vec-large-chinese](https://huggingface.co/GanymedeNil/text2vec-large-chinese)                                                   | 32.61 | 44.59 | 69.30 | 14.51 | 79.44 |  73.01  |  59.04  |   53.12   | 2092  |
+        | CoSENT     | nghuyong/ernie-3.0-base-zh                                   | [shibing624/text2vec-base-chinese-sentence](https://huggingface.co/shibing624/text2vec-base-chinese-sentence)                                     | 43.37 | 61.43 | 73.48 | 38.90 | 78.25 |  70.60  |  53.08  |   59.87   | 3089  |
+        | CoSENT     | nghuyong/ernie-3.0-base-zh                                   | [shibing624/text2vec-base-chinese-paraphrase](https://huggingface.co/shibing624/text2vec-base-chinese-paraphrase)                                 | 44.89 | 63.58 | 74.24 | 40.90 | 78.93 |  76.70  |  63.30  | **63.08** | 3066  |
+        | CoSENT     | sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2  | [shibing624/text2vec-base-multilingual](https://huggingface.co/shibing624/text2vec-base-multilingual)                                             | 32.39 | 50.33 | 65.64 | 32.56 | 74.45 |  68.88  |  51.17  |   53.67   | 3138  |
         
         
         说明：
         - 结果评测指标：spearman系数
-        - 模型训练实验报告：[实验报告](https://github.com/shibing624/text2vec/blob/master/docs/model_report.md)
         - `shibing624/text2vec-base-chinese`模型，是用CoSENT方法训练，基于`hfl/chinese-macbert-base`在中文STS-B数据训练得到，并在中文STS-B测试集评估达到较好效果，运行[examples/training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model.py)代码可训练模型，模型文件已经上传HF model hub，中文通用语义匹配任务推荐使用
         - `shibing624/text2vec-base-chinese-sentence`模型，是用CoSENT方法训练，基于`nghuyong/ernie-3.0-base-zh`用人工挑选后的中文STS数据集[shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-sentence-dataset)训练得到，并在中文各NLI测试集评估达到较好效果，运行[examples/training_sup_text_matching_model_jsonl_data.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model_jsonl_data.py)代码可训练模型，模型文件已经上传HF model hub，中文s2s(句子vs句子)语义匹配任务推荐使用
         - `shibing624/text2vec-base-chinese-paraphrase`模型，是用CoSENT方法训练，基于`nghuyong/ernie-3.0-base-zh`用人工挑选后的中文STS数据集[shibing624/nli-zh-all/text2vec-base-chinese-paraphrase-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-paraphrase-dataset)，数据集相对于[shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-sentence-dataset)加入了s2p(sentence to paraphrase)数据，强化了其长文本的表征能力，并在中文各NLI测试集评估达到SOTA，运行[examples/training_sup_text_matching_model_jsonl_data.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model_jsonl_data.py)代码可训练模型，模型文件已经上传HF model hub，中文s2p(句子vs段落)语义匹配任务推荐使用
-        - `SBERT-macbert-base`模型，是用SBERT方法训练，运行[examples/training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model.py)代码可训练模型
-        - `sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`模型是用SBERT训练，是`paraphrase-MiniLM-L12-v2`模型的多语言版本，支持中文、英文等
+        - `shibing624/text2vec-base-multilingual`模型，是用CoSENT方法训练，基于`sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`用人工挑选后的多语言STS数据集[shibing624/nli-zh-all/text2vec-base-multilingual-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-multilingual-dataset)训练得到，并在中英文测试集评估相对于原模型效果有提升，运行[examples/training_sup_text_matching_model_jsonl_data.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model_jsonl_data.py)代码可训练模型，模型文件已经上传HF model hub，多语言语义匹配任务推荐使用
         - `w2v-light-tencent-chinese`是腾讯词向量的Word2Vec模型，CPU加载使用，适用于中文字面匹配任务和缺少数据的冷启动情况
         - 各预训练模型均可以通过transformers调用，如MacBERT模型：`--model_name hfl/chinese-macbert-base` 或者roberta模型：`--model_name uer/roberta-medium-wwm-chinese-cluecorpussmall`
         - 为测评模型的鲁棒性，加入了未训练过的SOHU测试集，用于测试模型的泛化能力；为达到开箱即用的实用效果，使用了搜集到的各中文匹配数据集，数据集也上传到HF datasets[链接见下方](#数据集)
         - 中文匹配任务实验表明，pooling最优是`EncoderType.FIRST_LAST_AVG`和`EncoderType.MEAN`，两者预测效果差异很小
         - 中文匹配评测结果复现，可以下载中文匹配数据集到`examples/data`，运行[tests/test_model_spearman.py](https://github.com/shibing624/text2vec/blob/master/tests/test_model_spearman.py)代码复现评测结果
         - QPS的GPU测试环境是Tesla V100，显存32GB
         
-        # Demo
+        模型训练实验报告：[实验报告](https://github.com/shibing624/text2vec/blob/master/docs/model_report.md)
+        ## Demo
         
         Official Demo: https://www.mulanai.com/product/short_text_sim/
         
         HuggingFace Demo: https://huggingface.co/spaces/shibing624/text2vec
         
         ![](docs/hf.png)
         
         run example: [examples/gradio_demo.py](https://github.com/shibing624/text2vec/blob/master/examples/gradio_demo.py) to see the demo:
         ```shell
         python examples/gradio_demo.py
         ```
         
-        # Install
+        ## Install
         ```shell
         pip install torch # conda install pytorch
         pip install -U text2vec
         ```
         
         or
         
@@ -144,17 +148,17 @@
         pip install -r requirements.txt
         
         git clone https://github.com/shibing624/text2vec.git
         cd text2vec
         pip install --no-deps .
         ```
         
-        # Usage
+        ## Usage
         
-        ## 文本向量表征
+        ### 文本向量表征
         
         基于`pretrained model`计算文本向量：
         
         ```zsh
         >>> from text2vec import SentenceModel
         >>> m = SentenceModel()
         >>> m.encode("如何更换花呗绑定银行卡")
@@ -194,16 +198,16 @@
         
         
         if __name__ == "__main__":
             # 中文句向量模型(CoSENT)，中文语义匹配任务推荐，支持fine-tune继续训练
             t2v_model = SentenceModel("shibing624/text2vec-base-chinese")
             compute_emb(t2v_model)
         
-            # 支持多语言的句向量模型（Sentence-BERT），英文语义匹配任务推荐，支持fine-tune继续训练
-            sbert_model = SentenceModel("sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2")
+            # 支持多语言的句向量模型（CoSENT），多语言（包括中英文）语义匹配任务推荐，支持fine-tune继续训练
+            sbert_model = SentenceModel("shibing624/text2vec-base-multilingual")
             compute_emb(sbert_model)
         
             # 中文词向量模型(word2vec)，中文字面匹配任务和冷启动适用
             w2v_model = Word2Vec("w2v-light-tencent-chinese")
             compute_emb(w2v_model)
         
         ```
@@ -220,16 +224,14 @@
         ```
         
         - 返回值`embeddings`是`numpy.ndarray`类型，shape为`(sentences_size, model_embedding_size)`，三个模型任选一种即可，推荐用第一个。
         - `shibing624/text2vec-base-chinese`模型是CoSENT方法在中文STS-B数据集训练得到的，模型已经上传到huggingface的
         模型库[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)，
         是`text2vec.SentenceModel`指定的默认模型，可以通过上面示例调用，或者如下所示用[transformers库](https://github.com/huggingface/transformers)调用，
         模型自动下载到本机路径：`~/.cache/huggingface/transformers`
-        - `sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`模型是Sentence-BERT的多语言句向量模型，
-        适用于释义（paraphrase）识别，文本匹配，通过`text2vec.SentenceModel`和[sentence-transformers库]((https://github.com/UKPLab/sentence-transformers))都可以调用该模型
         - `w2v-light-tencent-chinese`是通过gensim加载的Word2Vec模型，使用腾讯词向量`Tencent_AILab_ChineseEmbedding.tar.gz`计算各字词的词向量，句子向量通过单词词
         向量取平均值得到，模型自动下载到本机路径：`~/.text2vec/datasets/light_Tencent_AILab_ChineseEmbedding.bin`
         
         #### Usage (HuggingFace Transformers)
         Without [text2vec](https://github.com/shibing624/text2vec), you can use the model like this: 
         
         First, you pass your input through the transformer model, then you have to apply the right pooling-operation on-top of the contextualized word embeddings.
@@ -447,17 +449,17 @@
         from similarities import Similarity
         
         m = Similarity()
         r = m.similarity('如何更换花呗绑定银行卡', '花呗更改绑定银行卡')
         print(f"similarity score: {float(r)}")  # similarity score: 0.855146050453186
         ```
         
-        # Models
+        ## Models
         
-        ## CoSENT model
+        ### CoSENT model
         
         CoSENT（Cosine Sentence）文本匹配模型，在Sentence-BERT上改进了CosineRankLoss的句向量方案
         
         
         Network structure:
         
         Training:
@@ -488,16 +490,22 @@
         python training_sup_text_matching_model.py --task_name ATEC --model_arch cosent --do_train --do_predict --num_epochs 10 --model_name hfl/chinese-macbert-base --output_dir ./outputs/ATEC-cosent
         ```
         
         - 在自有中文数据集上训练模型
         
         example: [examples/training_sup_text_matching_model_mydata.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model_mydata.py)
         
+        单卡训练：
+        ```shell
+        CUDA_VISIBLE_DEVICES=0 python training_sup_text_matching_model_mydata.py --do_train --do_predict
+        ```
+        
+        多卡训练：
         ```shell
-        python training_sup_text_matching_model_mydata.py --do_train --do_predict
+        CUDA_VISIBLE_DEVICES=0,1 torchrun --nproc_per_node 2  training_sup_text_matching_model_mydata.py --do_train --do_predict --output_dir outputs/STS-B-text2vec-macbert-v1 --batch_size 64 --fp16 --data_parallel 
         ```
         
         训练集格式参考[examples/data/STS-B/STS-B.valid.data](https://github.com/shibing624/text2vec/blob/master/examples/data/STS-B/STS-B.valid.data)
         
         ```shell
         sentence1   sentence2   label
         一个女孩在给她的头发做发型。	一个女孩在梳头。	2
@@ -524,15 +532,15 @@
         
         ```shell
         cd examples
         python training_unsup_text_matching_model_en.py --model_arch cosent --do_train --do_predict --num_epochs 10 --model_name bert-base-uncased --output_dir ./outputs/STS-B-en-unsup-cosent
         ```
         
         
-        ## Sentence-BERT model
+        ### Sentence-BERT model
         
         Sentence-BERT文本匹配模型，表征式句向量表示方案
         
         Network structure:
         
         Training:
         
@@ -567,38 +575,38 @@
         example: [examples/training_unsup_text_matching_model_en.py](https://github.com/shibing624/text2vec/blob/master/examples/training_unsup_text_matching_model_en.py)
         
         ```shell
         cd examples
         python training_unsup_text_matching_model_en.py --model_arch sentencebert --do_train --do_predict --num_epochs 10 --model_name bert-base-uncased --output_dir ./outputs/STS-B-en-unsup-sbert
         ```
         
-        ## BERT-Match model
+        ### BERT-Match model
         BERT文本匹配模型，原生BERT匹配网络结构，交互式句向量匹配模型
         
         Network structure:
         
         Training and inference:
         
         <img src="docs/bert-fc-train.png" width="300" />
         
         训练脚本同上[examples/training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model.py)。
         
         
-        ## 模型蒸馏（Model Distillation）
+        ### 模型蒸馏（Model Distillation）
         
         由于text2vec训练的模型可以使用[sentence-transformers](https://github.com/UKPLab/sentence-transformers)库加载，此处复用其模型蒸馏方法[distillation](https://github.com/UKPLab/sentence-transformers/tree/master/examples/training/distillation)。
         
         1. 模型降维，参考[dimensionality_reduction.py](https://github.com/UKPLab/sentence-transformers/blob/master/examples/training/distillation/dimensionality_reduction.py)使用PCA对模型输出embedding降维，可减少milvus等向量检索数据库的存储压力，还能轻微提升模型效果。
         2. 模型蒸馏，参考[model_distillation.py](https://github.com/UKPLab/sentence-transformers/blob/master/examples/training/distillation/model_distillation.py)使用蒸馏方法，将Teacher大模型蒸馏到更少layers层数的student模型中，在权衡效果的情况下，可大幅提升模型预测速度。
         
-        ## 模型部署
+        ### 模型部署
         
         提供两种部署模型，搭建服务的方法： 1）基于Jina搭建gRPC服务【推荐】；2）基于FastAPI搭建原生Http服务。
         
-        ### Jina服务
+        #### Jina服务
         采用C/S模式搭建高性能服务，支持docker云原生，gRPC/HTTP/WebSocket，支持多个模型同时预测，GPU多卡处理。
         
         - 安装：
         ```pip install jina```
         
         - 启动服务：
         
@@ -637,15 +645,15 @@
         r = c.post('/', inputs=DocumentArray([Document(text='如何更换花呗绑定银行卡'), Document(text='花呗更改绑定银行卡')]))
         print(r.embeddings)
         ```
         
         批量调用方法见example: [examples/jina_client_demo.py](https://github.com/shibing624/text2vec/blob/master/examples/jina_client_demo.py)
         
         
-        ### FastAPI服务
+        #### FastAPI服务
         
         - 安装：
         ```pip install fastapi uvicorn```
         
         - 启动服务：
         
         example: [examples/fastapi_server_demo.py](https://github.com/shibing624/text2vec/blob/master/examples/fastapi_server_demo.py)
@@ -658,15 +666,15 @@
         ```shell
         curl -X 'GET' \
           'http://0.0.0.0:8001/emb?q=hello' \
           -H 'accept: application/json'
         ```
         
         
-        ## 数据集
+        ## Dataset
         
         - 本项目release的数据集：
         
         | Dataset                    | Introduce                                                                | Download Link                                                                                                                                                                                                                                                                                         |
         |:---------------------------|:-------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
         | shibing624/nli-zh-all      | 中文语义匹配数据合集，整合了文本推理，相似，摘要，问答，指令微调等任务的820万高质量数据，并转化为匹配格式数据集                | [https://huggingface.co/datasets/shibing624/nli-zh-all](https://huggingface.co/datasets/shibing624/nli-zh-all)                                                                                                                                                                                        |
         | shibing624/snli-zh         | 中文SNLI和MultiNLI数据集，翻译自英文SNLI和MultiNLI                                    | [https://huggingface.co/datasets/shibing624/snli-zh](https://huggingface.co/datasets/shibing624/snli-zh)                                                                                                                                                                                              |
@@ -677,16 +685,16 @@
         | LCQMC                      | 中文LCQMC(large-scale Chinese question matching corpus)数据集，Q-Qpair数据集      | [LCQMC](http://icrc.hitsz.edu.cn/Article/show/171.html)                                                                                                                                                                                                                                               |
         | PAWSX                      | 中文PAWS(Paraphrase Adversaries from Word Scrambling)数据集，Q-Qpair数据集        | [PAWSX](https://arxiv.org/abs/1908.11828)                                                                                                                                                                                                                                                             |
         | STS-B                      | 中文STS-B数据集，中文自然语言推理数据集，从英文STS-B翻译为中文的数据集                                 | [STS-B](https://github.com/pluto-junzeng/CNSD)                                                                                                                                                                                                                                                        |
         
         
         常用英文匹配数据集：
         
-        - 大名鼎鼎的multi_nli和snli: https://huggingface.co/datasets/multi_nli
-        - 大名鼎鼎的multi_nli和snli: https://huggingface.co/datasets/snli
+        - 英文匹配数据集：multi_nli: https://huggingface.co/datasets/multi_nli
+        - 英文匹配数据集：snli: https://huggingface.co/datasets/snli
         - https://huggingface.co/datasets/metaeval/cnli
         - https://huggingface.co/datasets/mteb/stsbenchmark-sts
         - https://huggingface.co/datasets/JeremiahZ/simcse_sup_nli
         - https://huggingface.co/datasets/MoritzLaurer/multilingual-NLI-26lang-2mil7
         
         
         数据集使用示例：
@@ -721,59 +729,59 @@
         {'sentence1': '一个女孩在给她的头发做发型。', 'sentence2': '一个女孩在梳头。', 'label': 2}
         ```
         
         
         
         
         
-        # Contact
+        ## Contact
         
         - Issue(建议)：[![GitHub issues](https://img.shields.io/github/issues/shibing624/text2vec.svg)](https://github.com/shibing624/text2vec/issues)
         - 邮件我：xuming: xuming624@qq.com
         - 微信我：加我*微信号：xuming624, 备注：姓名-公司-NLP* 进NLP交流群。
         
         <img src="docs/wechat.jpeg" width="200" />
         
         
-        # Citation
+        ## Citation
         
         如果你在研究中使用了text2vec，请按如下格式引用：
         
         APA:
         ```latex
         Xu, M. Text2vec: Text to vector toolkit (Version 1.1.2) [Computer software]. https://github.com/shibing624/text2vec
         ```
         
         BibTeX:
         ```latex
         @misc{Text2vec,
-          author = {Xu, Ming},
+          author = {Ming Xu},
           title = {Text2vec: Text to vector toolkit},
-          year = {2022},
+          year = {2023},
           publisher = {GitHub},
           journal = {GitHub repository},
           howpublished = {\url{https://github.com/shibing624/text2vec}},
         }
         ```
         
-        # License
+        ## License
         
         
         授权协议为 [The Apache License 2.0](LICENSE)，可免费用做商业用途。请在产品说明中附加text2vec的链接和授权协议。
         
         
-        # Contribute
+        ## Contribute
         项目代码还很粗糙，如果大家对代码有所改进，欢迎提交回本项目，在提交之前，注意以下两点：
         
          - 在`tests`添加相应的单元测试
          - 使用`python -m pytest -v`来运行所有单元测试，确保所有单测都是通过的
         
         之后即可提交PR。
         
-        # Reference
+        ## References
         - [将句子表示为向量（上）：无监督句子表示学习（sentence embedding）](https://www.cnblogs.com/llhthinker/p/10335164.html)
         - [将句子表示为向量（下）：无监督句子表示学习（sentence embedding）](https://www.cnblogs.com/llhthinker/p/10341841.html)
         - [A Simple but Tough-to-Beat Baseline for Sentence Embeddings[Sanjeev Arora and Yingyu Liang and Tengyu Ma, 2017]](https://openreview.net/forum?id=SyK00v5xx)
         - [四种计算文本相似度的方法对比[Yves Peirsman]](https://zhuanlan.zhihu.com/p/37104535)
         - [Improvements to BM25 and Language Models Examined](http://www.cs.otago.ac.nz/homepages/andrew/papers/2014-2.pdf)
         - [CoSENT：比Sentence-BERT更有效的句向量方案](https://kexue.fm/archives/8847)
         - [谈谈文本匹配和多轮检索](https://zhuanlan.zhihu.com/p/111769969)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: text2vec Version: 1.2.1 Summary: Text to vector
+Metadata-Version: 2.1 Name: text2vec Version: 1.2.2 Summary: Text to vector
 Tool, encode text Home-page: https://github.com/shibing624/text2vec Author:
 XuMing Author-email: xuming624@qq.com License: Apache License 2.0 Description:
 [**ð¨ð³ä¸­æ**](https://github.com/shibing624/text2vec/blob/master/
 README.md) | [**ðEnglish**](https://github.com/shibing624/text2vec/blob/
 master/README_EN.md) | [**ðææ¡£/Docs**](https://github.com/shibing624/
 text2vec/wiki) | [**ð¤æ¨¡å/Models**](https://huggingface.co/shibing624)
                                     [Logo]
@@ -17,17 +17,26 @@
 shibing624/text2vec.svg)](https://github.com/shibing624/text2vec/issues) [!
 [Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/
 wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact) **Text2vec**: Text to
 Vector, Get Sentence Embeddings. ææ¬åéåï¼æææ¬
 (åæ¬è¯ãå¥å­ãæ®µè½)è¡¨å¾ä¸ºåéç©éµã
 **text2vec**å®ç°äºWord2VecãRankBM25ãBERTãSentence-
 BERTãCoSENTç­å¤ç§ææ¬è¡¨å¾ãææ¬ç¸ä¼¼åº¦è®¡ç®æ¨¡åï¼å¹¶å¨ææ¬è¯­ä¹å¹éï¼ç¸ä¼¼åº¦è®¡ç®ï¼ä»»å¡ä¸æ¯è¾äºåæ¨¡åçææã
-### News [2023/06/19] v1.2.1çæ¬: æ´æ°äºä¸­æå¹éæ¨¡å`shibing624/
-text2vec-base-chinese-nli`ä¸ºæ°ç[shibing624/text2vec-base-chinese-sentence]
-(https://huggingface.co/shibing624/text2vec-base-chinese-
+### News [2023/06/22] v1.2.2çæ¬: åå¸äºå¤è¯­è¨å¹éæ¨¡å[shibing624/
+text2vec-base-multilingual](https://huggingface.co/shibing624/text2vec-base-
+multilingual)ï¼ç¨CoSENTæ¹æ³è®­ç»ï¼åºäº`sentence-transformers/
+paraphrase-multilingual-MiniLM-L12-
+v2`ç¨äººå·¥æéåçå¤è¯­è¨STSæ°æ®é[shibing624/nli-zh-all/text2vec-
+base-multilingual-dataset](https://huggingface.co/datasets/shibing624/nli-zh-
+all/tree/main/text2vec-base-multilingual-
+dataset)è®­ç»å¾å°ï¼å¹¶å¨ä¸­è±ææµè¯éè¯ä¼°ç¸å¯¹äºåæ¨¡åææææåï¼è¯¦è§
+[Release-v1.2.2](https://github.com/shibing624/text2vec/releases/tag/1.2.2)
+[2023/06/19] v1.2.1çæ¬: æ´æ°äºä¸­æå¹éæ¨¡å`shibing624/text2vec-
+base-chinese-nli`ä¸ºæ°ç[shibing624/text2vec-base-chinese-sentence](https://
+huggingface.co/shibing624/text2vec-base-chinese-
 sentence)ï¼éå¯¹CoSENTçlossè®¡ç®å¯¹æåºææç¹ç¹ï¼äººå·¥æéå¹¶æ´çåºé«è´¨éçæç¸å³æ§æåºçSTSæ°æ®é
 [shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://
 huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-
 sentence-
 dataset)ï¼å¨åè¯ä¼°éè¡¨ç°ç¸å¯¹ä¹åææåï¼åå¸äºéç¨äºs2pçä¸­æå¹éæ¨¡å
 [shibing624/text2vec-base-chinese-paraphrase](https://huggingface.co/
 shibing624/text2vec-base-chinese-paraphrase)ï¼è¯¦è§[Release-v1.2.1](https://
@@ -38,17 +47,17 @@
 huggingface.co/datasets/shibing624/
 nli_zh)å¨é¨è¯­æè®­ç»çCoSENTææ¬å¹éæ¨¡åï¼å¨åè¯ä¼°éè¡¨ç°æåææ¾ï¼è¯¦è§
 [Release-v1.2.0](https://github.com/shibing624/text2vec/releases/tag/1.2.0)
 [2022/03/12] v1.1.4çæ¬: åå¸äºä¸­æå¹éæ¨¡å[shibing624/text2vec-
 base-chinese](https://huggingface.co/shibing624/text2vec-base-
 chinese)ï¼åºäºä¸­æSTSè®­ç»éè®­ç»çCoSENTå¹éæ¨¡åãè¯¦è§
 [Release-v1.1.4](https://github.com/shibing624/text2vec/releases/tag/1.1.4)
-**Guide** - [Feature](#Feature) - [Evaluation](#Evaluation) - [Install]
-(#install) - [Usage](#usage) - [Contact](#Contact) - [Reference](#reference) #
-Feature ### ææ¬åéè¡¨ç¤ºæ¨¡å - [Word2Vec](https://github.com/
+**Guide** - [Features](#Features) - [Evaluation](#Evaluation) - [Install]
+(#install) - [Usage](#usage) - [Contact](#Contact) - [References](#references)
+## Features ### ææ¬åéè¡¨ç¤ºæ¨¡å - [Word2Vec](https://github.com/
 shibing624/text2vec/blob/master/text2vec/word2vec.py)ï¼éè¿è¾è®¯AI
 Labå¼æºçå¤§è§æ¨¡é«è´¨éä¸­æ
 [è¯åéæ°æ®ï¼800ä¸ä¸­æè¯è½»éçï¼](https://pan.baidu.com/s/
 1La4U4XNFe8s5BJqxPQpeiQ) (æä»¶åï¼light_Tencent_AILab_ChineseEmbedding.bin
 å¯ç :
 taweï¼å®ç°è¯åéæ£ç´¢ï¼æ¬é¡¹ç®å®ç°äºå¥å­ï¼è¯åéæ±å¹³åï¼çword2vecåéè¡¨ç¤º
 - [SBERT(Sentence-BERT)](https://github.com/shibing624/text2vec/blob/master/
@@ -56,67 +65,76 @@
 sentencebert_model.py)ï¼æè¡¡æ§è½åæççå¥åéè¡¨ç¤ºæ¨¡åï¼è®­ç»æ¶éè¿æçç£è®­ç»ä¸å±åç±»å½æ°ï¼ææ¬å¹éé¢æµæ¶ç´æ¥å¥å­åéåä½å¼¦ï¼æ¬é¡¹ç®åºäºPyTorchå¤ç°äºSentence-
 BERTæ¨¡åçè®­ç»åé¢æµ - [CoSENT(Cosine Sentence)](https://github.com/
 shibing624/text2vec/blob/master/text2vec/
 cosent_model.py)ï¼CoSENTæ¨¡åæåºäºä¸ç§æåºçæå¤±å½æ°ï¼ä½¿è®­ç»è¿ç¨æ´è´´è¿é¢æµï¼æ¨¡åæ¶æéåº¦åæææ¯Sentence-
 BERTæ´å¥½ï¼æ¬é¡¹ç®åºäºPyTorchå®ç°äºCoSENTæ¨¡åçè®­ç»åé¢æµ
 è¯¦ç»ææ¬åéè¡¨ç¤ºæ¹æ³è§wiki: [ææ¬åéè¡¨ç¤ºæ¹æ³](https://
 github.com/shibing624/text2vec/wiki/
-%E6%96%87%E6%9C%AC%E5%90%91%E9%87%8F%E8%A1%A8%E7%A4%BA%E6%96%B9%E6%B3%95) #
+%E6%96%87%E6%9C%AC%E5%90%91%E9%87%8F%E8%A1%A8%E7%A4%BA%E6%96%B9%E6%B3%95) ##
 Evaluation ææ¬å¹é #### è±æå¹éæ°æ®éçè¯æµç»æï¼ | Arch |
 BaseModel | Model | English-STS-B | |:-------|:--------------------------------
-----------------|:-------------------------------------|:-------------:| |
+----------------|:-------------------------------------------------------------
+--------------------------------------------------------|:-------------:| |
 GloVe | glove | Avg_word_embeddings_glove_6B_300d | 61.77 | | BERT | bert-base-
 uncased | BERT-base-cls | 20.29 | | BERT | bert-base-uncased | BERT-base-
 first_last_avg | 59.04 | | BERT | bert-base-uncased | BERT-base-first_last_avg-
 whiten(NLI) | 63.65 | | SBERT | sentence-transformers/bert-base-nli-mean-tokens
 | SBERT-base-nli-cls | 73.65 | | SBERT | sentence-transformers/bert-base-nli-
 mean-tokens | SBERT-base-nli-first_last_avg | 77.96 | | CoSENT | bert-base-
 uncased | CoSENT-base-first_last_avg | 69.93 | | CoSENT | sentence-
 transformers/bert-base-nli-mean-tokens | CoSENT-base-nli-first_last_avg | 79.68
-| #### ä¸­æå¹éæ°æ®éçè¯æµç»æï¼ | Arch | BaseModel | Model |
-ATEC | BQ | LCQMC | PAWSX | STS-B | Avg | |:-------|:--------------------------
---|:--------------------|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:| |
-SBERT | bert-base-chinese | SBERT-bert-base | 46.36 | 70.36 | 78.72 | 46.86 |
-66.41 | 61.74 | | SBERT | hfl/chinese-macbert-base | SBERT-macbert-base | 47.28
-| 68.63 | 79.42 | 55.59 | 64.82 | 63.15 | | SBERT | hfl/chinese-roberta-wwm-ext
-| SBERT-roberta-ext | 48.29 | 69.99 | 79.22 | 44.10 | 72.42 | 62.80 | | CoSENT
-| bert-base-chinese | CoSENT-bert-base | 49.74 | 72.38 | 78.69 | 60.00 | 79.27
-| 68.01 | | CoSENT | hfl/chinese-macbert-base | CoSENT-macbert-base | 50.39 |
-72.93 | 79.17 | 60.86 | 79.30 | 68.53 | | CoSENT | hfl/chinese-roberta-wwm-ext
-| CoSENT-roberta-ext | 50.81 | 71.45 | 79.31 | 61.56 | 79.96 | 68.61 |
-è¯´æï¼ - ç»æè¯æµææ ï¼spearmanç³»æ° -
+| | CoSENT | sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2 |
+[shibing624/text2vec-base-multilingual](https://huggingface.co/shibing624/
+text2vec-base-multilingual) | 80.12 | ####
+ä¸­æå¹éæ°æ®éçè¯æµç»æï¼ | Arch | BaseModel | Model | ATEC | BQ
+| LCQMC | PAWSX | STS-B | Avg | |:-------|:----------------------------|:------
+--------------|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:| | SBERT | bert-
+base-chinese | SBERT-bert-base | 46.36 | 70.36 | 78.72 | 46.86 | 66.41 | 61.74
+| | SBERT | hfl/chinese-macbert-base | SBERT-macbert-base | 47.28 | 68.63 |
+79.42 | 55.59 | 64.82 | 63.15 | | SBERT | hfl/chinese-roberta-wwm-ext | SBERT-
+roberta-ext | 48.29 | 69.99 | 79.22 | 44.10 | 72.42 | 62.80 | | CoSENT | bert-
+base-chinese | CoSENT-bert-base | 49.74 | 72.38 | 78.69 | 60.00 | 79.27 | 68.01
+| | CoSENT | hfl/chinese-macbert-base | CoSENT-macbert-base | 50.39 | 72.93 |
+79.17 | 60.86 | 79.30 | 68.53 | | CoSENT | hfl/chinese-roberta-wwm-ext |
+CoSENT-roberta-ext | 50.81 | 71.45 | 79.31 | 61.56 | 79.96 | 68.61 | è¯´æï¼
+- ç»æè¯æµææ ï¼spearmanç³»æ° -
 ä¸ºè¯æµæ¨¡åè½åï¼ç»æååªç¨è¯¥æ°æ®éçtrainè®­ç»ï¼å¨testä¸è¯ä¼°å¾å°çè¡¨ç°ï¼æ²¡ç¨å¤é¨æ°æ®
-### Release Models - æ¬é¡¹ç®releaseæ¨¡åçä¸­æå¹éè¯æµç»æï¼ |
-Arch | BaseModel | Model | ATEC | BQ | LCQMC | PAWSX | STS-B | SOHU-dd | SOHU-
-dc | Avg | QPS | |:-----------|:----------------------------------|:-----------
+- `SBERT-macbert-base`æ¨¡åï¼æ¯ç¨SBertæ¹æ³è®­ç»ï¼è¿è¡[examples/
+training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/
+blob/master/examples/training_sup_text_matching_model.py)ä»£ç å¯è®­ç»æ¨¡å
+- `sentence-transformers/paraphrase-multilingual-MiniLM-L12-
+v2`æ¨¡åæ¯ç¨SBertè®­ç»ï¼æ¯`paraphrase-MiniLM-L12-
+v2`æ¨¡åçå¤è¯­è¨çæ¬ï¼æ¯æä¸­æãè±æç­ ### Release Models -
+æ¬é¡¹ç®releaseæ¨¡åçä¸­æå¹éè¯æµç»æï¼ | Arch | BaseModel | Model
+| ATEC | BQ | LCQMC | PAWSX | STS-B | SOHU-dd | SOHU-dc | Avg | QPS | |:-------
+----|:-------------------------------------------------------------|:----------
 -------------------------------------------------------------------------------
---------------------------------------------------------|:-----:|:-----:|:----
+---------------------------------------------------------|:-----:|:-----:|:----
 -:|:-----:|:-----:|:-------:|:-------:|:---------:|:-----:| | Word2Vec |
 word2vec | [w2v-light-tencent-chinese](https://ai.tencent.com/ailab/nlp/en/
 download.html) | 20.00 | 31.49 | 59.46 | 2.57 | 55.78 | 55.04 | 20.70 | 35.03 |
 23769 | | SBERT | xlm-roberta-base | [sentence-transformers/paraphrase-
 multilingual-MiniLM-L12-v2](https://huggingface.co/sentence-transformers/
 paraphrase-multilingual-MiniLM-L12-v2) | 18.42 | 38.52 | 63.96 | 10.14 | 78.90
-| 63.01 | 52.28 | 46.46 | 3138 | | Instructor | hfl/chinese-roberta-wwm-ext |
-[moka-ai/m3e-base](https://huggingface.co/moka-ai/m3e-base) | 41.27 | 63.81 |
-74.87 | 12.20 | 76.96 | 75.83 | 60.55 | 57.93 | 2980 | | CoSENT | hfl/chinese-
-macbert-base | [shibing624/text2vec-base-chinese](https://huggingface.co/
-shibing624/text2vec-base-chinese) | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 |
-70.27 | 50.42 | 51.61 | 3008 | | CoSENT | hfl/chinese-lert-large |
-[GanymedeNil/text2vec-large-chinese](https://huggingface.co/GanymedeNil/
-text2vec-large-chinese) | 32.61 | 44.59 | 69.30 | 14.51 | 79.44 | 73.01 | 59.04
-| 53.12 | 2092 | | CoSENT | nghuyong/ernie-3.0-base-zh | [shibing624/text2vec-
-base-chinese-sentence](https://huggingface.co/shibing624/text2vec-base-chinese-
-sentence) | 43.37 | 61.43 | 73.48 | 38.90 | 78.25 | 70.60 | 53.08 | 59.87 |
-3089 | | CoSENT | nghuyong/ernie-3.0-base-zh | [shibing624/text2vec-base-
-chinese-paraphrase](https://huggingface.co/shibing624/text2vec-base-chinese-
-paraphrase) | 44.89 | 63.58 | 74.24 | 40.90 | 78.93 | 76.70 | 63.30 | **63.08**
-| 3066 | è¯´æï¼ - ç»æè¯æµææ ï¼spearmanç³»æ° -
-æ¨¡åè®­ç»å®éªæ¥åï¼[å®éªæ¥å](https://github.com/shibing624/
-text2vec/blob/master/docs/model_report.md) - `shibing624/text2vec-base-
+| 63.01 | 52.28 | 46.46 | 3138 | | CoSENT | hfl/chinese-macbert-base |
+[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-
+base-chinese) | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 | 70.27 | 50.42 | 51.61 |
+3008 | | CoSENT | hfl/chinese-lert-large | [GanymedeNil/text2vec-large-chinese]
+(https://huggingface.co/GanymedeNil/text2vec-large-chinese) | 32.61 | 44.59 |
+69.30 | 14.51 | 79.44 | 73.01 | 59.04 | 53.12 | 2092 | | CoSENT | nghuyong/
+ernie-3.0-base-zh | [shibing624/text2vec-base-chinese-sentence](https://
+huggingface.co/shibing624/text2vec-base-chinese-sentence) | 43.37 | 61.43 |
+73.48 | 38.90 | 78.25 | 70.60 | 53.08 | 59.87 | 3089 | | CoSENT | nghuyong/
+ernie-3.0-base-zh | [shibing624/text2vec-base-chinese-paraphrase](https://
+huggingface.co/shibing624/text2vec-base-chinese-paraphrase) | 44.89 | 63.58 |
+74.24 | 40.90 | 78.93 | 76.70 | 63.30 | **63.08** | 3066 | | CoSENT | sentence-
+transformers/paraphrase-multilingual-MiniLM-L12-v2 | [shibing624/text2vec-base-
+multilingual](https://huggingface.co/shibing624/text2vec-base-multilingual) |
+32.39 | 50.33 | 65.64 | 32.56 | 74.45 | 68.88 | 51.17 | 53.67 | 3138 |
+è¯´æï¼ - ç»æè¯æµææ ï¼spearmanç³»æ° - `shibing624/text2vec-base-
 chinese`æ¨¡åï¼æ¯ç¨CoSENTæ¹æ³è®­ç»ï¼åºäº`hfl/chinese-macbert-
 base`å¨ä¸­æSTS-Bæ°æ®è®­ç»å¾å°ï¼å¹¶å¨ä¸­æSTS-
 Bæµè¯éè¯ä¼°è¾¾å°è¾å¥½ææï¼è¿è¡[examples/
 training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/
 blob/master/examples/
 training_sup_text_matching_model.py)ä»£ç å¯è®­ç»æ¨¡åï¼æ¨¡åæä»¶å·²ç»ä¸ä¼ HF
 model hubï¼ä¸­æéç¨è¯­ä¹å¹éä»»å¡æ¨èä½¿ç¨ - `shibing624/text2vec-
@@ -137,81 +155,83 @@
 [shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://
 huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-
 sentence-dataset)å å¥äºs2p(sentence to
 paraphrase)æ°æ®ï¼å¼ºåäºå¶é¿ææ¬çè¡¨å¾è½åï¼å¹¶å¨ä¸­æåNLIæµè¯éè¯ä¼°è¾¾å°SOTAï¼è¿è¡
 [examples/training_sup_text_matching_model_jsonl_data.py](https://github.com/
 shibing624/text2vec/blob/master/examples/
 training_sup_text_matching_model_jsonl_data.py)ä»£ç å¯è®­ç»æ¨¡åï¼æ¨¡åæä»¶å·²ç»ä¸ä¼ HF
-model hubï¼ä¸­æs2p(å¥å­vsæ®µè½)è¯­ä¹å¹éä»»å¡æ¨èä½¿ç¨ - `SBERT-
-macbert-base`æ¨¡åï¼æ¯ç¨SBERTæ¹æ³è®­ç»ï¼è¿è¡[examples/
-training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/
-blob/master/examples/training_sup_text_matching_model.py)ä»£ç å¯è®­ç»æ¨¡å
-- `sentence-transformers/paraphrase-multilingual-MiniLM-L12-
-v2`æ¨¡åæ¯ç¨SBERTè®­ç»ï¼æ¯`paraphrase-MiniLM-L12-
-v2`æ¨¡åçå¤è¯­è¨çæ¬ï¼æ¯æä¸­æãè±æç­ - `w2v-light-tencent-
+model hubï¼ä¸­æs2p(å¥å­vsæ®µè½)è¯­ä¹å¹éä»»å¡æ¨èä½¿ç¨ -
+`shibing624/text2vec-base-
+multilingual`æ¨¡åï¼æ¯ç¨CoSENTæ¹æ³è®­ç»ï¼åºäº`sentence-transformers/
+paraphrase-multilingual-MiniLM-L12-
+v2`ç¨äººå·¥æéåçå¤è¯­è¨STSæ°æ®é[shibing624/nli-zh-all/text2vec-
+base-multilingual-dataset](https://huggingface.co/datasets/shibing624/nli-zh-
+all/tree/main/text2vec-base-multilingual-
+dataset)è®­ç»å¾å°ï¼å¹¶å¨ä¸­è±ææµè¯éè¯ä¼°ç¸å¯¹äºåæ¨¡åææææåï¼è¿è¡
+[examples/training_sup_text_matching_model_jsonl_data.py](https://github.com/
+shibing624/text2vec/blob/master/examples/
+training_sup_text_matching_model_jsonl_data.py)ä»£ç å¯è®­ç»æ¨¡åï¼æ¨¡åæä»¶å·²ç»ä¸ä¼ HF
+model hubï¼å¤è¯­è¨è¯­ä¹å¹éä»»å¡æ¨èä½¿ç¨ - `w2v-light-tencent-
 chinese`æ¯è¾è®¯è¯åéçWord2Vecæ¨¡åï¼CPUå è½½ä½¿ç¨ï¼éç¨äºä¸­æå­é¢å¹éä»»å¡åç¼ºå°æ°æ®çå·å¯å¨æåµ
 - åé¢è®­ç»æ¨¡ååå¯ä»¥éè¿transformersè°ç¨ï¼å¦MacBERTæ¨¡åï¼`--
 model_name hfl/chinese-macbert-base` æèrobertaæ¨¡åï¼`--model_name uer/
 roberta-medium-wwm-chinese-cluecorpussmall` -
 ä¸ºæµè¯æ¨¡åçé²æ£æ§ï¼å å¥äºæªè®­ç»è¿çSOHUæµè¯éï¼ç¨äºæµè¯æ¨¡åçæ³åè½åï¼ä¸ºè¾¾å°å¼ç®±å³ç¨çå®ç¨ææï¼ä½¿ç¨äºæéå°çåä¸­æå¹éæ°æ®éï¼æ°æ®éä¹ä¸ä¼ å°HF
 datasets[é¾æ¥è§ä¸æ¹](#æ°æ®é) -
 ä¸­æå¹éä»»å¡å®éªè¡¨æï¼poolingæä¼æ¯`EncoderType.FIRST_LAST_AVG`å`EncoderType.MEAN`ï¼ä¸¤èé¢æµææå·®å¼å¾å°
 -
 ä¸­æå¹éè¯æµç»æå¤ç°ï¼å¯ä»¥ä¸è½½ä¸­æå¹éæ°æ®éå°`examples/
 data`ï¼è¿è¡[tests/test_model_spearman.py](https://github.com/shibing624/
 text2vec/blob/master/tests/test_model_spearman.py)ä»£ç å¤ç°è¯æµç»æ -
-QPSçGPUæµè¯ç¯å¢æ¯Tesla V100ï¼æ¾å­32GB # Demo Official Demo: https://
-www.mulanai.com/product/short_text_sim/ HuggingFace Demo: https://
-huggingface.co/spaces/shibing624/text2vec ![](docs/hf.png) run example:
-[examples/gradio_demo.py](https://github.com/shibing624/text2vec/blob/master/
-examples/gradio_demo.py) to see the demo: ```shell python examples/
-gradio_demo.py ``` # Install ```shell pip install torch # conda install pytorch
-pip install -U text2vec ``` or ```shell pip install torch # conda install
-pytorch pip install -r requirements.txt git clone https://github.com/
-shibing624/text2vec.git cd text2vec pip install --no-deps . ``` # Usage ##
-ææ¬åéè¡¨å¾ åºäº`pretrained model`è®¡ç®ææ¬åéï¼ ```zsh >>>
-from text2vec import SentenceModel >>> m = SentenceModel() >>> m.encode
-("å¦ä½æ´æ¢è±åç»å®é¶è¡å¡") Embedding shape: (768,) ``` example:
-[examples/computing_embeddings_demo.py](https://github.com/shibing624/text2vec/
-blob/master/examples/computing_embeddings_demo.py) ```python import sys
-sys.path.append('..') from text2vec import SentenceModel from text2vec import
-Word2Vec def compute_emb(model): # Embed a list of sentences sentences =
-[ 'å¡', 'é¶è¡å¡', 'å¦ä½æ´æ¢è±åç»å®é¶è¡å¡',
-'è±åæ´æ¹ç»å®é¶è¡å¡', 'This framework generates embeddings for each
-input sentence', 'Sentences are passed as a list of string.', 'The quick brown
-fox jumps over the lazy dog.' ] sentence_embeddings = model.encode(sentences)
-print(type(sentence_embeddings), sentence_embeddings.shape) # The result is a
-list of sentence embeddings as numpy arrays for sentence, embedding in zip
-(sentences, sentence_embeddings): print("Sentence:", sentence) print("Embedding
-shape:", embedding.shape) print("Embedding head:", embedding[:10]) print() if
-__name__ == "__main__": # ä¸­æå¥åéæ¨¡å
-(CoSENT)ï¼ä¸­æè¯­ä¹å¹éä»»å¡æ¨èï¼æ¯æfine-tuneç»§ç»­è®­ç»
-t2v_model = SentenceModel("shibing624/text2vec-base-chinese") compute_emb
-(t2v_model) # æ¯æå¤è¯­è¨çå¥åéæ¨¡åï¼Sentence-
-BERTï¼ï¼è±æè¯­ä¹å¹éä»»å¡æ¨èï¼æ¯æfine-tuneç»§ç»­è®­ç»
-sbert_model = SentenceModel("sentence-transformers/paraphrase-multilingual-
-MiniLM-L12-v2") compute_emb(sbert_model) # ä¸­æè¯åéæ¨¡å
+QPSçGPUæµè¯ç¯å¢æ¯Tesla V100ï¼æ¾å­32GB æ¨¡åè®­ç»å®éªæ¥åï¼
+[å®éªæ¥å](https://github.com/shibing624/text2vec/blob/master/docs/
+model_report.md) ## Demo Official Demo: https://www.mulanai.com/product/
+short_text_sim/ HuggingFace Demo: https://huggingface.co/spaces/shibing624/
+text2vec ![](docs/hf.png) run example: [examples/gradio_demo.py](https://
+github.com/shibing624/text2vec/blob/master/examples/gradio_demo.py) to see the
+demo: ```shell python examples/gradio_demo.py ``` ## Install ```shell pip
+install torch # conda install pytorch pip install -U text2vec ``` or ```shell
+pip install torch # conda install pytorch pip install -r requirements.txt git
+clone https://github.com/shibing624/text2vec.git cd text2vec pip install --no-
+deps . ``` ## Usage ### ææ¬åéè¡¨å¾ åºäº`pretrained
+model`è®¡ç®ææ¬åéï¼ ```zsh >>> from text2vec import SentenceModel >>> m
+= SentenceModel() >>> m.encode("å¦ä½æ´æ¢è±åç»å®é¶è¡å¡") Embedding
+shape: (768,) ``` example: [examples/computing_embeddings_demo.py](https://
+github.com/shibing624/text2vec/blob/master/examples/
+computing_embeddings_demo.py) ```python import sys sys.path.append('..') from
+text2vec import SentenceModel from text2vec import Word2Vec def compute_emb
+(model): # Embed a list of sentences sentences = [ 'å¡', 'é¶è¡å¡',
+'å¦ä½æ´æ¢è±åç»å®é¶è¡å¡', 'è±åæ´æ¹ç»å®é¶è¡å¡', 'This
+framework generates embeddings for each input sentence', 'Sentences are passed
+as a list of string.', 'The quick brown fox jumps over the lazy dog.' ]
+sentence_embeddings = model.encode(sentences) print(type(sentence_embeddings),
+sentence_embeddings.shape) # The result is a list of sentence embeddings as
+numpy arrays for sentence, embedding in zip(sentences, sentence_embeddings):
+print("Sentence:", sentence) print("Embedding shape:", embedding.shape) print
+("Embedding head:", embedding[:10]) print() if __name__ == "__main__": #
+ä¸­æå¥åéæ¨¡å(CoSENT)ï¼ä¸­æè¯­ä¹å¹éä»»å¡æ¨èï¼æ¯æfine-
+tuneç»§ç»­è®­ç» t2v_model = SentenceModel("shibing624/text2vec-base-chinese")
+compute_emb(t2v_model) #
+æ¯æå¤è¯­è¨çå¥åéæ¨¡åï¼CoSENTï¼ï¼å¤è¯­è¨ï¼åæ¬ä¸­è±æï¼è¯­ä¹å¹éä»»å¡æ¨èï¼æ¯æfine-
+tuneç»§ç»­è®­ç» sbert_model = SentenceModel("shibing624/text2vec-base-
+multilingual") compute_emb(sbert_model) # ä¸­æè¯åéæ¨¡å
 (word2vec)ï¼ä¸­æå­é¢å¹éä»»å¡åå·å¯å¨éç¨ w2v_model = Word2Vec
 ("w2v-light-tencent-chinese") compute_emb(w2v_model) ``` output: ```
 numpy.ndarray'> (7, 768) Sentence: å¡ Embedding shape: (768,) Sentence:
 é¶è¡å¡ Embedding shape: (768,) ... ``` -
 è¿åå¼`embeddings`æ¯`numpy.ndarray`ç±»åï¼shapeä¸º`(sentences_size,
 model_embedding_size)`ï¼ä¸ä¸ªæ¨¡åä»»éä¸ç§å³å¯ï¼æ¨èç¨ç¬¬ä¸ä¸ªã
 - `shibing624/text2vec-base-chinese`æ¨¡åæ¯CoSENTæ¹æ³å¨ä¸­æSTS-
 Bæ°æ®éè®­ç»å¾å°çï¼æ¨¡åå·²ç»ä¸ä¼ å°huggingfaceç æ¨¡ååº
 [shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-
 base-chinese)ï¼
 æ¯`text2vec.SentenceModel`æå®çé»è®¤æ¨¡åï¼å¯ä»¥éè¿ä¸é¢ç¤ºä¾è°ç¨ï¼æèå¦ä¸æç¤ºç¨
 [transformersåº](https://github.com/huggingface/transformers)è°ç¨ï¼
-æ¨¡åèªå¨ä¸è½½å°æ¬æºè·¯å¾ï¼`~/.cache/huggingface/transformers` -
-`sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`æ¨¡åæ¯Sentence-
-BERTçå¤è¯­è¨å¥åéæ¨¡åï¼
-éç¨äºéä¹ï¼paraphraseï¼è¯å«ï¼ææ¬å¹éï¼éè¿`text2vec.SentenceModel`å
-[sentence-transformersåº]((https://github.com/UKPLab/sentence-
-transformers))é½å¯ä»¥è°ç¨è¯¥æ¨¡å - `w2v-light-tencent-
+æ¨¡åèªå¨ä¸è½½å°æ¬æºè·¯å¾ï¼`~/.cache/huggingface/transformers` - `w2v-
+light-tencent-
 chinese`æ¯éè¿gensimå è½½çWord2Vecæ¨¡åï¼ä½¿ç¨è¾è®¯è¯åé`Tencent_AILab_ChineseEmbedding.tar.gz`è®¡ç®åå­è¯çè¯åéï¼å¥å­åééè¿åè¯è¯
 åéåå¹³åå¼å¾å°ï¼æ¨¡åèªå¨ä¸è½½å°æ¬æºè·¯å¾ï¼`~/.text2vec/
 datasets/light_Tencent_AILab_ChineseEmbedding.bin` #### Usage (HuggingFace
 Transformers) Without [text2vec](https://github.com/shibing624/text2vec), you
 can use the model like this: First, you pass your input through the transformer
 model, then you have to apply the right pooling-operation on-top of the
 contextualized word embeddings. example: [examples/
@@ -322,16 +342,16 @@
 ææ¬ç¸ä¼¼åº¦è®¡ç®åææ¬å¹éæç´¢ä»»å¡ï¼æ¨èä½¿ç¨
 [similaritiesåº](https://github.com/shibing624/similarities)
 ï¼å¼å®¹æ¬é¡¹ç®releaseç
 Word2vecãSBERTãCosentç±»è¯­ä¹å¹éæ¨¡åï¼è¿æ¯æå­é¢ç»´åº¦ç¸ä¼¼åº¦è®¡ç®ãå¹éæç´¢ç®æ³ï¼æ¯æææ¬ãå¾åã
 å®è£ï¼ ```pip install -U similarities``` å¥å­ç¸ä¼¼åº¦è®¡ç®ï¼ ```python
 from similarities import Similarity m = Similarity() r = m.similarity
 ('å¦ä½æ´æ¢è±åç»å®é¶è¡å¡', 'è±åæ´æ¹ç»å®é¶è¡å¡') print
-(f"similarity score: {float(r)}") # similarity score: 0.855146050453186 ``` #
-Models ## CoSENT model CoSENTï¼Cosine
+(f"similarity score: {float(r)}") # similarity score: 0.855146050453186 ``` ##
+Models ### CoSENT model CoSENTï¼Cosine
 Sentenceï¼ææ¬å¹éæ¨¡åï¼å¨Sentence-
 BERTä¸æ¹è¿äºCosineRankLossçå¥åéæ¹æ¡ Network structure: Training:
 [docs/cosent_train.png] Inference: [docs/inference.png] #### CoSENT
 çç£æ¨¡å è®­ç»åé¢æµCoSENTæ¨¡åï¼ - å¨ä¸­æSTS-
 Bæ°æ®éè®­ç»åè¯ä¼°`CoSENT`æ¨¡å example: [examples/
 training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/
 blob/master/examples/training_sup_text_matching_model.py) ```shell cd examples
@@ -343,21 +363,24 @@
 'PAWSX'ï¼å·ä½åèHuggingFace datasets [https://huggingface.co/datasets/
 shibing624/nli_zh](https://huggingface.co/datasets/shibing624/nli_zh) ```shell
 python training_sup_text_matching_model.py --task_name ATEC --model_arch cosent
 --do_train --do_predict --num_epochs 10 --model_name hfl/chinese-macbert-base -
 -output_dir ./outputs/ATEC-cosent ``` - å¨èªæä¸­ææ°æ®éä¸è®­ç»æ¨¡å
 example: [examples/training_sup_text_matching_model_mydata.py](https://
 github.com/shibing624/text2vec/blob/master/examples/
-training_sup_text_matching_model_mydata.py) ```shell python
-training_sup_text_matching_model_mydata.py --do_train --do_predict ```
-è®­ç»éæ ¼å¼åè[examples/data/STS-B/STS-B.valid.data](https://github.com/
-shibing624/text2vec/blob/master/examples/data/STS-B/STS-B.valid.data) ```shell
-sentence1 sentence2 label ä¸ä¸ªå¥³å­©å¨ç»å¥¹çå¤´ååååã
-ä¸ä¸ªå¥³å­©å¨æ¢³å¤´ã 2 ä¸ç¾¤ç·äººå¨æµ·æ»©ä¸è¸¢è¶³çã
-ä¸ç¾¤ç·å­©å¨æµ·æ»©ä¸è¸¢è¶³çã 3
+training_sup_text_matching_model_mydata.py) åå¡è®­ç»ï¼ ```shell
+CUDA_VISIBLE_DEVICES=0 python training_sup_text_matching_model_mydata.py --
+do_train --do_predict ``` å¤å¡è®­ç»ï¼ ```shell CUDA_VISIBLE_DEVICES=0,1
+torchrun --nproc_per_node 2 training_sup_text_matching_model_mydata.py --
+do_train --do_predict --output_dir outputs/STS-B-text2vec-macbert-v1 --
+batch_size 64 --fp16 --data_parallel ``` è®­ç»éæ ¼å¼åè[examples/data/
+STS-B/STS-B.valid.data](https://github.com/shibing624/text2vec/blob/master/
+examples/data/STS-B/STS-B.valid.data) ```shell sentence1 sentence2 label
+ä¸ä¸ªå¥³å­©å¨ç»å¥¹çå¤´ååååã ä¸ä¸ªå¥³å­©å¨æ¢³å¤´ã 2
+ä¸ç¾¤ç·äººå¨æµ·æ»©ä¸è¸¢è¶³çã ä¸ç¾¤ç·å­©å¨æµ·æ»©ä¸è¸¢è¶³çã 3
 ä¸ä¸ªå¥³äººå¨æµéå¦ä¸ä¸ªå¥³äººçèè¸ã
 å¥³äººæµéå¦ä¸ä¸ªå¥³äººçèè¸ã 5 ```
 `label`å¯ä»¥æ¯0ï¼1æ ç­¾ï¼0ä»£è¡¨ä¸¤ä¸ªå¥å­ä¸ç¸ä¼¼ï¼1ä»£è¡¨ç¸ä¼¼ï¼ä¹å¯ä»¥æ¯0-
 5çè¯åï¼è¯åè¶é«ï¼è¡¨ç¤ºä¸¤ä¸ªå¥å­è¶ç¸ä¼¼ãæ¨¡åé½è½æ¯æã
 - å¨è±æSTS-Bæ°æ®éè®­ç»åè¯ä¼°`CoSENT`æ¨¡å example: [examples/
 training_sup_text_matching_model_en.py](https://github.com/shibing624/text2vec/
 blob/master/examples/training_sup_text_matching_model_en.py) ```shell cd
@@ -366,15 +389,15 @@
 output_dir ./outputs/STS-B-en-cosent ``` #### CoSENT æ çç£æ¨¡å -
 å¨è±æNLIæ°æ®éè®­ç»`CoSENT`æ¨¡åï¼å¨STS-Bæµè¯éè¯ä¼°ææ
 example: [examples/training_unsup_text_matching_model_en.py](https://
 github.com/shibing624/text2vec/blob/master/examples/
 training_unsup_text_matching_model_en.py) ```shell cd examples python
 training_unsup_text_matching_model_en.py --model_arch cosent --do_train --
 do_predict --num_epochs 10 --model_name bert-base-uncased --output_dir ./
-outputs/STS-B-en-unsup-cosent ``` ## Sentence-BERT model Sentence-
+outputs/STS-B-en-unsup-cosent ``` ### Sentence-BERT model Sentence-
 BERTææ¬å¹éæ¨¡åï¼è¡¨å¾å¼å¥åéè¡¨ç¤ºæ¹æ¡ Network structure:
 Training: [docs/sbert_train.png] Inference: [docs/sbert_inference.png] ####
 SentenceBERT çç£æ¨¡å - å¨ä¸­æSTS-Bæ°æ®éè®­ç»åè¯ä¼°`SBERT`æ¨¡å
 example: [examples/training_sup_text_matching_model.py](https://github.com/
 shibing624/text2vec/blob/master/examples/training_sup_text_matching_model.py)
 ```shell cd examples python training_sup_text_matching_model.py --model_arch
 sentencebert --do_train --do_predict --num_epochs 10 --model_name hfl/chinese-
@@ -387,35 +410,35 @@
 uncased --output_dir ./outputs/STS-B-en-sbert ``` #### SentenceBERT
 æ çç£æ¨¡å - å¨è±æNLIæ°æ®éè®­ç»`SBERT`æ¨¡åï¼å¨STS-
 Bæµè¯éè¯ä¼°ææ example: [examples/
 training_unsup_text_matching_model_en.py](https://github.com/shibing624/
 text2vec/blob/master/examples/training_unsup_text_matching_model_en.py)
 ```shell cd examples python training_unsup_text_matching_model_en.py --
 model_arch sentencebert --do_train --do_predict --num_epochs 10 --model_name
-bert-base-uncased --output_dir ./outputs/STS-B-en-unsup-sbert ``` ## BERT-Match
-model
+bert-base-uncased --output_dir ./outputs/STS-B-en-unsup-sbert ``` ### BERT-
+Match model
 BERTææ¬å¹éæ¨¡åï¼åçBERTå¹éç½ç»ç»æï¼äº¤äºå¼å¥åéå¹éæ¨¡å
 Network structure: Training and inference: [docs/bert-fc-train.png]
 è®­ç»èæ¬åä¸[examples/training_sup_text_matching_model.py](https://
 github.com/shibing624/text2vec/blob/master/examples/
-training_sup_text_matching_model.py)ã ## æ¨¡åè¸é¦ï¼Model Distillationï¼
-ç±äºtext2vecè®­ç»çæ¨¡åå¯ä»¥ä½¿ç¨[sentence-transformers](https://
-github.com/UKPLab/sentence-
+training_sup_text_matching_model.py)ã ### æ¨¡åè¸é¦ï¼Model
+Distillationï¼ ç±äºtext2vecè®­ç»çæ¨¡åå¯ä»¥ä½¿ç¨[sentence-
+transformers](https://github.com/UKPLab/sentence-
 transformers)åºå è½½ï¼æ­¤å¤å¤ç¨å¶æ¨¡åè¸é¦æ¹æ³[distillation](https:
 //github.com/UKPLab/sentence-transformers/tree/master/examples/training/
 distillation)ã 1. æ¨¡åéç»´ï¼åè[dimensionality_reduction.py](https://
 github.com/UKPLab/sentence-transformers/blob/master/examples/training/
 distillation/
 dimensionality_reduction.py)ä½¿ç¨PCAå¯¹æ¨¡åè¾åºembeddingéç»´ï¼å¯åå°milvusç­åéæ£ç´¢æ°æ®åºçå­å¨ååï¼è¿è½è½»å¾®æåæ¨¡åææã
 2. æ¨¡åè¸é¦ï¼åè[model_distillation.py](https://github.com/UKPLab/
 sentence-transformers/blob/master/examples/training/distillation/
 model_distillation.py)ä½¿ç¨è¸é¦æ¹æ³ï¼å°Teacherå¤§æ¨¡åè¸é¦å°æ´å°layerså±æ°çstudentæ¨¡åä¸­ï¼å¨æè¡¡ææçæåµä¸ï¼å¯å¤§å¹æåæ¨¡åé¢æµéåº¦ã
-## æ¨¡åé¨ç½² æä¾ä¸¤ç§é¨ç½²æ¨¡åï¼æ­å»ºæå¡çæ¹æ³ï¼
+### æ¨¡åé¨ç½² æä¾ä¸¤ç§é¨ç½²æ¨¡åï¼æ­å»ºæå¡çæ¹æ³ï¼
 1ï¼åºäºJinaæ­å»ºgRPCæå¡ãæ¨èãï¼2ï¼åºäºFastAPIæ­å»ºåçHttpæå¡ã
-### Jinaæå¡ éç¨C/
+#### Jinaæå¡ éç¨C/
 Sæ¨¡å¼æ­å»ºé«æ§è½æå¡ï¼æ¯ædockeräºåçï¼gRPC/HTTP/
 WebSocketï¼æ¯æå¤ä¸ªæ¨¡ååæ¶é¢æµï¼GPUå¤å¡å¤çã - å®è£ï¼
 ```pip install jina``` - å¯å¨æå¡ï¼ example: [examples/
 jina_server_demo.py](examples/jina_server_demo.py) ```python from jina import
 Flow port = 50001 f = Flow(port=port).add( uses='jinahub://Text2vecEncoder',
 uses_with={'model_name': 'shibing624/text2vec-base-chinese'} ) with f: #
 backend server forever f.block() ```
@@ -424,27 +447,27 @@
 è°ç¨æå¡ï¼ ```python from jina import Client from docarray import
 Document, DocumentArray port = 50001 c = Client(port=port) data =
 ['å¦ä½æ´æ¢è±åç»å®é¶è¡å¡', 'è±åæ´æ¹ç»å®é¶è¡å¡'] print
 ("data:", data) print('data embs:') r = c.post('/', inputs=DocumentArray(
 [Document(text='å¦ä½æ´æ¢è±åç»å®é¶è¡å¡'), Document
 (text='è±åæ´æ¹ç»å®é¶è¡å¡')])) print(r.embeddings) ```
 æ¹éè°ç¨æ¹æ³è§example: [examples/jina_client_demo.py](https://
-github.com/shibing624/text2vec/blob/master/examples/jina_client_demo.py) ###
+github.com/shibing624/text2vec/blob/master/examples/jina_client_demo.py) ####
 FastAPIæå¡ - å®è£ï¼ ```pip install fastapi uvicorn``` - å¯å¨æå¡ï¼
 example: [examples/fastapi_server_demo.py](https://github.com/shibing624/
 text2vec/blob/master/examples/fastapi_server_demo.py) ```shell cd examples
 python fastapi_server_demo.py ``` - è°ç¨æå¡ï¼ ```shell curl -X 'GET' \
 'http://0.0.0.0:8001/emb?q=hello' \ -H 'accept: application/json' ``` ##
-æ°æ®é - æ¬é¡¹ç®releaseçæ°æ®éï¼ | Dataset | Introduce | Download
-Link | |:---------------------------|:-----------------------------------------
---------------------------------|:---------------------------------------------
+Dataset - æ¬é¡¹ç®releaseçæ°æ®éï¼ | Dataset | Introduce | Download Link
+| |:---------------------------|:----------------------------------------------
+---------------------------|:--------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
-------------| | shibing624/nli-zh-all |
+-------| | shibing624/nli-zh-all |
 ä¸­æè¯­ä¹å¹éæ°æ®åéï¼æ´åäºææ¬æ¨çï¼ç¸ä¼¼ï¼æè¦ï¼é®ç­ï¼æä»¤å¾®è°ç­ä»»å¡ç820ä¸é«è´¨éæ°æ®ï¼å¹¶è½¬åä¸ºå¹éæ ¼å¼æ°æ®é
 | [https://huggingface.co/datasets/shibing624/nli-zh-all](https://
 huggingface.co/datasets/shibing624/nli-zh-all) | | shibing624/snli-zh |
 ä¸­æSNLIåMultiNLIæ°æ®éï¼ç¿»è¯èªè±æSNLIåMultiNLI | [https://
 huggingface.co/datasets/shibing624/snli-zh](https://huggingface.co/datasets/
 shibing624/snli-zh) | | shibing624/nli_zh |
 ä¸­æè¯­ä¹å¹éæ°æ®éï¼æ´åäºä¸­æATECãBQãLCQMCãPAWSXãSTS-
@@ -462,46 +485,46 @@
 info/1037/1162.htm) | | LCQMC | ä¸­æLCQMC(large-scale Chinese question
 matching corpus)æ°æ®éï¼Q-Qpairæ°æ®é | [LCQMC](http://
 icrc.hitsz.edu.cn/Article/show/171.html) | | PAWSX | ä¸­æPAWS(Paraphrase
 Adversaries from Word Scrambling)æ°æ®éï¼Q-Qpairæ°æ®é | [PAWSX](https:/
 /arxiv.org/abs/1908.11828) | | STS-B | ä¸­æSTS-
 Bæ°æ®éï¼ä¸­æèªç¶è¯­è¨æ¨çæ°æ®éï¼ä»è±æSTS-
 Bç¿»è¯ä¸ºä¸­æçæ°æ®é | [STS-B](https://github.com/pluto-junzeng/CNSD) |
-å¸¸ç¨è±æå¹éæ°æ®éï¼ - å¤§åé¼é¼çmulti_nliåsnli: https://
-huggingface.co/datasets/multi_nli - å¤§åé¼é¼çmulti_nliåsnli: https://
+å¸¸ç¨è±æå¹éæ°æ®éï¼ - è±æå¹éæ°æ®éï¼multi_nli: https://
+huggingface.co/datasets/multi_nli - è±æå¹éæ°æ®éï¼snli: https://
 huggingface.co/datasets/snli - https://huggingface.co/datasets/metaeval/cnli -
 https://huggingface.co/datasets/mteb/stsbenchmark-sts - https://huggingface.co/
 datasets/JeremiahZ/simcse_sup_nli - https://huggingface.co/datasets/
 MoritzLaurer/multilingual-NLI-26lang-2mil7 æ°æ®éä½¿ç¨ç¤ºä¾ï¼ ```shell
 pip install datasets ``` ```python from datasets import load_dataset dataset =
 load_dataset("shibing624/nli_zh", "STS-B") # ATEC or BQ or LCQMC or PAWSX or
 STS-B print(dataset) print(dataset['test'][0]) ``` output: ```shell DatasetDict
 ({ train: Dataset({ features: ['sentence1', 'sentence2', 'label'], num_rows:
 5231 }) validation: Dataset({ features: ['sentence1', 'sentence2', 'label'],
 num_rows: 1458 }) test: Dataset({ features: ['sentence1', 'sentence2',
 'label'], num_rows: 1361 }) }) {'sentence1':
 'ä¸ä¸ªå¥³å­©å¨ç»å¥¹çå¤´ååååã', 'sentence2':
-'ä¸ä¸ªå¥³å­©å¨æ¢³å¤´ã', 'label': 2} ``` # Contact - Issue(å»ºè®®)ï¼[!
+'ä¸ä¸ªå¥³å­©å¨æ¢³å¤´ã', 'label': 2} ``` ## Contact - Issue(å»ºè®®)ï¼[!
 [GitHub issues](https://img.shields.io/github/issues/shibing624/text2vec.svg)]
 (https://github.com/shibing624/text2vec/issues) - é®ä»¶æï¼xuming:
 xuming624@qq.com - å¾®ä¿¡æï¼å æ*å¾®ä¿¡å·ï¼xuming624, å¤æ³¨ï¼å§å-
-å¬å¸-NLP* è¿NLPäº¤æµç¾¤ã [docs/wechat.jpeg] # Citation
+å¬å¸-NLP* è¿NLPäº¤æµç¾¤ã [docs/wechat.jpeg] ## Citation
 å¦æä½ å¨ç ç©¶ä¸­ä½¿ç¨äºtext2vecï¼è¯·æå¦ä¸æ ¼å¼å¼ç¨ï¼ APA:
 ```latex Xu, M. Text2vec: Text to vector toolkit (Version 1.1.2) [Computer
 software]. https://github.com/shibing624/text2vec ``` BibTeX: ```latex @misc
-{Text2vec, author = {Xu, Ming}, title = {Text2vec: Text to vector toolkit},
-year = {2022}, publisher = {GitHub}, journal = {GitHub repository},
-howpublished = {\url{https://github.com/shibing624/text2vec}}, } ``` # License
+{Text2vec, author = {Ming Xu}, title = {Text2vec: Text to vector toolkit}, year
+= {2023}, publisher = {GitHub}, journal = {GitHub repository}, howpublished =
+{\url{https://github.com/shibing624/text2vec}}, } ``` ## License
 ææåè®®ä¸º [The Apache License 2.0]
 (LICENSE)ï¼å¯åè´¹ç¨ååä¸ç¨éãè¯·å¨äº§åè¯´æä¸­éå text2vecçé¾æ¥åææåè®®ã
-# Contribute
+## Contribute
 é¡¹ç®ä»£ç è¿å¾ç²ç³ï¼å¦æå¤§å®¶å¯¹ä»£ç æææ¹è¿ï¼æ¬¢è¿æäº¤åæ¬é¡¹ç®ï¼å¨æäº¤ä¹åï¼æ³¨æä»¥ä¸ä¸¤ç¹ï¼
 - å¨`tests`æ·»å ç¸åºçååæµè¯ - ä½¿ç¨`python -m pytest -
 v`æ¥è¿è¡ææååæµè¯ï¼ç¡®ä¿ææåæµé½æ¯éè¿ç
-ä¹åå³å¯æäº¤PRã # Reference -
+ä¹åå³å¯æäº¤PRã ## References -
 [å°å¥å­è¡¨ç¤ºä¸ºåéï¼ä¸ï¼ï¼æ çç£å¥å­è¡¨ç¤ºå­¦ä¹ ï¼sentence
 embeddingï¼](https://www.cnblogs.com/llhthinker/p/10335164.html) -
 [å°å¥å­è¡¨ç¤ºä¸ºåéï¼ä¸ï¼ï¼æ çç£å¥å­è¡¨ç¤ºå­¦ä¹ ï¼sentence
 embeddingï¼](https://www.cnblogs.com/llhthinker/p/10341841.html) - [A Simple
 but Tough-to-Beat Baseline for Sentence Embeddings[Sanjeev Arora and Yingyu
 Liang and Tengyu Ma, 2017]](https://openreview.net/forum?id=SyK00v5xx) -
 [åç§è®¡ç®ææ¬ç¸ä¼¼åº¦çæ¹æ³å¯¹æ¯[Yves Peirsman]](https://
```

### Comparing `text2vec-1.2.1/text2vec.egg-info/SOURCES.txt` & `text2vec-1.2.2/text2vec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

