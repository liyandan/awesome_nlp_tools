# awesome_nlp_tools

整理常用的自然语言处理工具(包括Python接口)，如Stanford NLP、NLTK、Spacy、NLPIR、Pyltp、HanLP、Jieba。

Collates commonly used natural language processing tools (including Python interfaces) such as Stanford NLP, NLTK, Spacy, NLPIR, Pyltp, HanLP, Jieba.

---


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
<<<<<<< HEAD


### 7. [ChineseWordSegmentation](https://github.com/Moonshile/ChineseWordSegmentation)

- 描述：Chinese word segmentation algorithm without corpus

- 功能：中文分词

  ```python
  from wordseg import WordSegment
  doc = u'十四是十四四十是四十，十四不是四十，四十不是十四'
  ws = WordSegment(doc, max_word_len=2, min_aggregation=1, min_entropy=0.5)
  ws.segSentence(doc)
  ```

### 8. [Jiagu](<https://github.com/ownthink/Jiagu>)

- 描述：Jiagu深度学习自然语言处理工具--Tensorflow==1.14.0 < 2.0
- 功能：**知识图谱关系抽取 中文分词 词性标注 命名实体识别 情感分析 新词发现 关键词 文本摘要 文本聚类**
- [DOC](https://www.ownthink.com/docs/nlp/)

```shell
pip install jiagu
---
git clone https://github.com/ownthink/Jiagu
cd Jiagu
python setup.py install
```

### 9. [xmnlp](<https://github.com/SeanLee97/xmnlp>)

- 描述：小明NLP， 轻量级中文自然语言处理工具

- 功能：**中文分词, 词性标注, 拼写检查，文本转拼音，情感分析，文本摘要，偏旁部首**

- ```shell
  pip install xmnlp
  ---
  git clone https://github.com/SeanLee97/xmnlp.git
  cd /path/to/xmnlp
  pip install -r requirements.txt
  python setup.py install
  ```

### 10. [mynlp](<https://github.com/mayabot/mynlp>)

- 描述：一个高性能、模块化、可扩展的中文NLP工具包--**Java**
- 功能：中文分词 词性标注 命名实体识别 新词发现 文本分类 拼音简繁转换

### 11. [lightNLP](<https://github.com/ImportMe/lightNLP>)

- 描述：基于Pytorch和torchtext的自然语言处理深度学习框架

- 功能：**命名实体识别、中文分词、词性标注、语义角色标注、情感分析、关系抽取、语言模型、文本相似度、文本蕴含、依存句法分析、词向量训练、聊天机器人、机器翻译、文本摘要**等功能
