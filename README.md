# Short-Text-Summarization

## 基础方法

### 提取关键词法计算文本摘要

#### tfidf提取关键词计算文本摘要 [论文地址](http://www.di.ubi.pt/~jpaulo/competence/general/(1958)Luhn.pdf)

#### 结果
![](https://github.com/yangzhiye/ImageCache/blob/master/LCSTS/LCSTS_tfidf_keyword.png)

## 评价指标

1.ROUGE(ROUGE.py) [论文地址](http://www.aclweb.org/anthology/W04-1013)

## 文本摘要调研

### 论文调研

#### LCSTS: A Large-Scale Chinese Short Text Summarization Dataset [论文地址](http://www.aclweb.org/website/anthology/D/D15/D15-1229.pdf)

1. 爬取并过滤了240W+条注明微博蓝V发布的[摘要,短文本],这是本系统所采用的语料(特别感谢哈尔滨工业大学深圳研究院智能计算研究中心的辛勤付出)。
2. 本文提出了word-based和character-based(为了改善UNK问题)两种数据处理的方法,并给出了RNN和RNN+context两种模型做baseline。
3. RNN+Context+Char组合表现最好，ROUGE-1:0.299 ROUGE-2:0.174 ROUGE-L:0.272

#### The Automatic Creation of Lierature Abstracts [论文地址](http://courses.ischool.berkeley.edu/i256/f06/papers/luhn58.pdf)

1. TFIDF计算关键词->通过关键词的密集程度计算关键句->通过关键句形成摘要