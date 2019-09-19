# awesome_nlp_tools
Collates commonly used natural language processing tools (including Python interfaces) such as Stanford NLP, NLTK, Spacy, NLPIR, Pyltp, HanLP, Jieba
---

### 1. [Jieba](https://github.com/ImportMe/awesome_nlp_tools)
- “结巴”中文分词：做最好的 Python 中文分词组件
- [https://github.com/fxsjy/jieba](https://github.com/fxsjy/jieba)
- **分词**(支持自定义词典)，**词性标注**，**关键词提取**，模型可手动加载(默认延迟加载机制)


```shell
online: pip install jieba
offline: https://pypi.python.org/pypi/jieba/ ，解压运行 python setup.py install
```

### 2. [pyhanlp](https://github.com/ImportMe/awesome_nlp_tools)
- HanLP是由一系列模型与算法组成的工具包，目标是普及自然语言处理在生产环境中的应用。HanLP具备功能完善、性能高效、架构清晰、语料时新、可自定义的特点；**提供词法分析（中文分词（支持自定义词典）、词性标注、命名实体识别）、关键词提取，自动摘要，拼音转换，简繁转换，文本推荐，文本分类，句法分析、文本分类和情感分析**。
- HanLP的Python接口，支持自动下载与升级HanLP，兼容py2、py3，模型可延迟加载
- [https://github.com/hankcs/HanLP](https://github.com/hankcs/HanLP)
- [https://github.com/hankcs/pyhanlp](https://github.com/hankcs/pyhanlp)


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

### 3. [StanfordCoreNLP](https://github.com/ImportMe/awesome_nlp_tools)

- [Official](https://github.com/stanfordnlp/CoreNLP)
- [Official](https://stanfordnlp.github.io/CoreNLP/)
- [Python Wrapper](https://github.com/Good2NLP/stanford-corenlp)

```shell
pip install stanfordcorenlp # 需要下载对应语言版本的模型
```

### Todo

NLTK, Spacy, NLPIR, PyLTP