# awesome_nlp_tools

整理常用的自然语言处理工具(包括Python接口)，如Stanford NLP、NLTK、Spacy、NLPIR、Pyltp、HanLP、Jieba。

Collates commonly used natural language processing tools (including Python interfaces) such as Stanford NLP, NLTK, Spacy, NLPIR, Pyltp, HanLP, Jieba.

---

### 1. [Jieba](./jieba.ipynb)
- 描述：“结巴”中文分词：做最好的 Python 中文分词组件
- [Official](https://github.com/fxsjy/jieba)
- 功能：**分词**(支持自定义词典)，**词性标注**，**关键词提取**，模型可手动加载(默认延迟加载机制)


```shell
online: pip install jieba
offline: https://pypi.python.org/pypi/jieba/ # 解压运行 python setup.py install
```

### 2. [pyhanlp](./pyhanlp.ipynb)
- 描述：HanLP是由一系列模型与算法组成的工具包，目标是普及自然语言处理在生产环境中的应用。HanLP具备功能完善、性能高效、架构清晰、语料时新、可自定义的特点；HanLP的Python接口，支持自动下载与升级HanLP，兼容py2、py3，模型可延迟加载。
- 功能：**词法分析（中文分词（支持自定义词典）、词性标注、命名实体识别）、关键词提取，自动摘要，拼音转换，简繁转换，文本推荐，文本分类，句法分析、文本分类和情感分析**。
- [HanLP](https://github.com/hankcs/HanLP)
- [pyhanlp](https://github.com/hankcs/pyhanlp)


```shell
pip install pyhanlp
```
> Python接口下提供的功能有限：分词，关键词提取，自动摘要，依存句法分析；如果要使用java版本的全部功能，需要python调用java环境下的接口，方法如下：

```shell
from pyhanlp import *

PerceptronLexicalAnalyzer = JClass('com.hankcs.hanlp.model.perceptron.PerceptronLexicalAnalyzer')
analyzer = PerceptronLexicalAnalyzer()
print(analyzer.analyze("上海华安工业（集团）公司董事长谭旭光和秘书胡花蕊来到美国纽约现代艺术博物馆参观"))
```

### 3. [StanfordCoreNLP](。、stanford_corenlp.ipynb)

- 描述：Stanfordcorenlp is a Python wrapper for Stanford CoreNLP. It provides a simple API for text processing tasks.
- 功能：**Tokenization, Part of Speech Tagging, Named Entity Reconigtion, Constituency Parsing, Dependency Parsing, and more.**
- [Github](https://github.com/stanfordnlp/CoreNLP)
- [Official](https://stanfordnlp.github.io/CoreNLP/)
- [Python Wrapper](https://github.com/Good2NLP/stanford-corenlp)

```shell
pip install stanfordcorenlp # 需要下载对应语言版本的模型,或者all in one 
```

### 4. [NLTK](./nltk.ipynb)

- 描述：NLTK是构建Python程序以使用人类语言数据的领先平台。
- 功能：**分词，分句，实体识别，词干化，标记，解析和语义推理**的文本处理库
- [Doc](http://www.nltk.org/)
- [Online](http://www.nltk.org/book/)

```shell
pip install nltk

import nltk
nltk.download() # 下载需要的库
```

### 5. [Spacy](https://spacy.io/)

- 描述：一个工业级别的自然语言处理工具目前不支持中文
- 功能：**分词，词性标注，句法分析，命名实体识别，词向量，词干化，词形还原**
- [Official](https://spacy.io/)

```shell
1.pip install spacy
2.下载模型 en_core_web_sm
    2.1 在线安装 
        python -m spacy download en_core_web_sm
    2.2 离线安装 
        下载模型到本地，解压
        python setup.py install
        
3.使用模型 spacy.load("en_core_web_sm")

```

### 6. [PyLTP](https://github.com/HuangFJ/pyltp)

- 描述：pyltp 是 LTP 的 Python 封装，提供了分词，词性标注，命名实体识别，依存句法分析，语义角色标注的功能。
- 功能：**分词，词性标注，命名实体识别，依存句法分析，语义角色标注**
- [LTP Official](https://github.com/HIT-SCIR/ltp)
- [LTP Doc](https://ltp.readthedocs.io/zh_CN/latest/begin.html)
- [PyLTP Official](https://github.com/HuangFJ/pyltp)
- [PyLTP Doc](https://pyltp.readthedocs.io/zh_CN/develop/api.html)
- [DJH-pyltp(pyltp基本使用及关系三元组抽取的应用)](https://github.com/jasonhavenD/DJH-pyltp)
- [基于LTP的在线开放式关系三元组抽取平台](https://github.com/jasonhavenD/DJH-GraduationDesign)

```shell
pip install pyltp # 使用需要下载模型到本地
```
