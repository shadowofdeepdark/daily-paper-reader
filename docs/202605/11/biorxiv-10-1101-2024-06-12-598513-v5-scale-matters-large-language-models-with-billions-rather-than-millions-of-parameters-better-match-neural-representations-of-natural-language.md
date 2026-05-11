---
title: "Scale matters: Large language models with billions (rather than millions) of parameters better match neural representations of natural language"
title_zh: 尺度的重要性：拥有数十亿（而非数百万）参数的大型语言模型更好地匹配自然语言的神经表征
authors: "Hong, Z., Wang, H., Zada, Z., Gazula, H., Turner, D., Aubrey, B., Niekerken, L., Doyle, W., Devore, S., Dugan, P., Friedman, D., Devinsky, O., Flinker, A., Hasson, U., Nastase, S., Goldstein, A."
date: 2026-05-10
pdf: "https://www.biorxiv.org/content/10.1101/2024.06.12.598513v5.full.pdf"
tags: ["query:q7"]
score: 8.5
evidence: 利用电皮质图研究大模型与自然语言神经表示的匹配
tldr: 该研究通过比较不同规模的Transformer语言模型与人脑ECoG数据，发现模型参数越大越能准确预测语言相关的神经活动，并揭示了模型层次与脑区功能的对应关系，为理解大脑语言处理提供了新证据。
source: biorxiv
selection_source: fresh_fetch
motivation: 研究旨在探究大规模语言模型能否更准确地反映人脑自然语言处理的神经机制。
method: 研究使用多种基于Transformer的LLM，并通过ECoG测量癫痫患者听自然语言故事时的大脑活动，分析模型各层输出与神经信号的对应关系。
result: 结果显示，参数规模更大的模型更能预测神经活动，并表现出模型层与脑区间有序对应的层级关系。
conclusion: 研究表明，LLM规模的扩大能更好地模拟人类大脑中语言处理的层级结构。
---

## 摘要
近期的研究利用大型语言模型（Large Language Models, LLMs）来探讨人类大脑处理自然语言的神经基础。随着LLMs复杂度的迅速提升，其语言处理能力也显著提高。然而，神经科学研究者尚未跟上LLM发展的快速步伐。本研究采用多个基于Transformer架构的LLM家族，探讨模型规模与其捕捉人脑中语言信息能力之间的关系。关键的是，我们使用了一部分在相同训练集上训练的LLMs，从而能够将模型规模与架构和训练集规模区分开来。研究中，我们利用皮层脑电图（ECoG）测量癫痫患者在聆听一个30分钟自然语音故事时的大脑神经活动。我们基于LLM各隐藏层提取的上下文嵌入，拟合逐电极的编码模型，以预测词级别的神经信号。与先前研究一致，我们发现规模更大的LLMs更好地捕捉自然语言结构，并更准确地预测神经活动。此外，我们发现一个对数线性关系：随着模型规模的增大，编码性能峰值出现在相对更早的层中。我们还观察到不同脑区中表现最佳层的差异，这与有序的语言处理层级相对应。

## Abstract
Recent research has used large language models (LLMs) to study the neural basis of naturalistic language processing in the human brain. LLMs have rapidly grown in complexity, leading to improved language processing capabilities. However, neuroscience researchers haven't kept up with the quick progress in LLM development. Here, we utilized several families of transformer-based LLMs to investigate the relationship between model size and their ability to capture linguistic information in the human brain. Crucially, a subset of LLMs were trained on a fixed training set, enabling us to dissociate model size from architecture and training set size. We used electrocorticography (ECoG) to measure neural activity in epilepsy patients while they listened to a 30-minute naturalistic audio story. We fit electrode-wise encoding models using contextual embeddings extracted from each hidden layer of the LLMs to predict word-level neural signals. In line with prior work, we found that larger LLMs better capture the structure of natural language and better predict neural activity. We also found a log-linear relationship where the encoding performance peaks in relatively earlier layers as model size increases. We also observed variations in the best-performing layer across different brain regions, corresponding to an organized language processing hierarchy.