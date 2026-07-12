---
title: "BCCWJ-Brain: A Multi-Modal fMRI, MEG, and EEG Dataset of Naturalistic Japanese Reading"
title_zh: BCCWJ-Brain：自然日语阅读的多模态 fMRI、MEG 与 EEG 数据集
authors: "Sugimoto, Y., Asahara, M., Jeong, H., Kanno, A., Koizumi, M., Oseki, Y."
date: 2026-07-09
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.05.736621v1.full.pdf"
tags: ["query:profile-1"]
score: 9.0
evidence: 母语者自然阅读的多模态神经影像（fMRI、MEG、EEG）数据
tldr: 该研究发布了BCCWJ-Brain多模态脑成像数据集，记录112名日语母语者在阅读BCCWJ新闻文章时的fMRI、MEG和EEG信号。研究采用统一的RSVP自然阅读范式，在相同刺激条件下采集三种互补神经数据，为研究语言认知机制以及评估大语言模型等计算模型提供了公开且标准化的基准资源。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-05-736621-v1/fig-001.webp\", \"caption\": \"Figure 5: Average evoked response to all words across subjects (EEG).\", \"page\": 11, \"index\": 1, \"width\": 914, \"height\": 490}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-05-736621-v1/fig-002.webp\", \"caption\": \"Figure 4: Average evoked response to all words across subjects (MEG).\", \"page\": 10, \"index\": 2, \"width\": 914, \"height\": 489}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-05-736621-v1/fig-003.webp\", \"caption\": \"Table 5: Word length — FWE (p < 0.05, Bonferroni, k > 50 voxels, t > 6.53).\", \"page\": 10, \"index\": 3, \"width\": 936, \"height\": 190}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-05-736621-v1/fig-004.webp\", \"caption\": \"Table 1: Recent multimodal neuroimaging datasets for language processing research.\", \"page\": 3, \"index\": 4, \"width\": 936, \"height\": 761}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-05-736621-v1/fig-005.webp\", \"caption\": \"Figure 1: Directory structure of the BCCWJ-Brain datasets (BCCWJ-fMRI, BCCWJ-MEG, and BCCWJ-EEG, which use BIDS structures (v 1.9.0)). XX = subject ID; N = run number (1–4); * = sub-XX_task-BCCWJreading.\", \"page\": 8, \"index\": 5, \"width\": 1030, \"height\": 742}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-05-736621-v1/fig-006.webp\", \"caption\": \"Figure 2: Inter-subject correlation (ISC) results.\", \"page\": 9, \"index\": 6, \"width\": 952, \"height\": 206}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-05-736621-v1/fig-007.webp\", \"caption\": \"Figure 3: GLM analysis results. Top: word-rate contrast (FWE p < 0.05, Bonferroni, k > 50 voxels). Bottom: word-length contrast (FWE p < 0.05, Bonferroni, k > 50 voxels). Color bar indicates t-statistic values. L = left hemisphere; R = right hemisphere.\", \"page\": 9, \"index\": 7, \"width\": 922, \"height\": 306}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-05-736621-v1/fig-008.webp\", \"caption\": \"Table 2: Participants’ information\", \"page\": 5, \"index\": 8, \"width\": 921, \"height\": 998}]"
motivation: 现有自然语言脑成像数据缺乏统一刺激下的多模态记录，限制了对语言认知机制和计算模型的系统比较。
method: 研究在112名日语母语者中，采用RSVP范式阅读BCCWJ新闻文章，并同步采集fMRI、MEG和EEG三种脑成像数据。
result: 研究构建并公开了包含36名fMRI、35名MEG和41名EEG受试者的数据集，已发布于OpenNeuro平台供研究使用。
conclusion: BCCWJ-Brain为自然语言理解与脑活动建模提供了统一、多模态且公开的基准资源，可推动神经科学与大语言模型研究结合。
---

## 摘要
我们发布了 BCCWJ-Brain 数据集，这是一个多模态神经影像资源，包含来自日语母语者在阅读《现代日语书面语平衡语料库》（Balanced Corpus of Contemporary Written Japanese，BCCWJ）中的报纸文章时记录的功能性磁共振成像（fMRI）、脑磁图（MEG）和脑电图（EEG）数据。研究在 112 名参与者中采集了神经数据（其中 fMRI 36 人、MEG 35 人、EEG 41 人），参与者在快速序列视觉呈现（Rapid Serial Visual Presentation，RSVP）范式下阅读了二十篇报纸文章。通过提供在相同自然阅读刺激条件下采集的三种互补性神经影像模态，该数据集为大语言模型等计算模型提供了认知基准。该数据集已在 OpenNeuro 平台公开发布，为神经科学、自然语言处理及相关研究领域提供了宝贵资源。

## Abstract
We present the BCCWJ-Brain dataset, a multi-modal neuroimaging resource comprising functional magnetic resonance imaging (fMRI), magnetoencephalography (MEG), and electroencephalography (EEG) data recorded from native Japanese speakers reading newspaper articles from the Balanced Corpus of Contemporary Written Japanese (BCCWJ). Neural data were collected from 112 participants (36 fMRI, 35 MEG, and 41 EEG) as they read twenty newspaper articles presented in a Rapid Serial Visual Presentation (RSVP) paradigm. By providing three complementary neuroimaging modalities collected under identical naturalistic reading stimuli, this dataset provides a cognitive benchmark for computational models such as large language models. The dataset is publicly available on the OpenNeuro platform, offering a valuable resource for neuroscience, natural language processing, and related research fields.

---

## 论文详细总结（自动生成）

# BCCWJ-Brain：自然日语阅读的多模态 fMRI、MEG 与 EEG 数据集

## 1. 核心问题与整体含义（研究动机与背景）

### 研究背景
近年来，大语言模型（LLM）与人脑语言处理机制之间的对应关系，成为神经科学与 NLP 交叉领域的重要方向。已有大量研究尝试：

- 将 LLM 的内部表示与脑活动进行对齐；
- 用脑成像数据评估模型的“认知合理性”；
- 探索语言理解的神经计算机制。

这一方向高度依赖“自然语言条件下”的脑成像数据集。

### 现有数据集的不足
论文指出，现有自然语言脑数据资源存在几个关键问题：

- 多数数据集只有单一模态：
  - fMRI：空间分辨率高，但时间分辨率低；
  - EEG：时间分辨率高，但空间定位弱；
  - MEG：兼顾一定空间与高时间分辨率。
- 很少有“同一刺激下”的跨模态数据；
- 现有资源主要集中于：
  - 英语、
  - 中文、
  - 荷兰语等；
- 日语几乎缺失。

此外，大多数已有数据集研究的是“听觉语言理解（listening）”，而不是“阅读（reading）”。

### 本文的整体意义
该论文的核心贡献是构建并公开：

- 一个统一刺激条件下的
  - fMRI、
  - MEG、
  - EEG
  多模态日语阅读脑数据集。

其意义包括：

- 为脑-语言模型对齐研究提供 benchmark；
- 支持跨模态神经编码研究；
- 支持语言认知机制分析；
- 补足日语这一类型学重要语言的缺口；
- 为未来 LLM 与脑活动比较研究提供标准资源。

---

# 2. 方法论：核心思想与关键技术细节

## 核心思想

论文本质上是一项“数据集构建与验证工作”，而非新模型论文。

其核心方法思想是：

> 在完全一致的自然阅读刺激条件下，采集三种互补脑成像模态，从而建立统一的认知基准。

具体来说：

- 所有受试者阅读相同的 BCCWJ 新闻文本；
- 使用统一 RSVP（Rapid Serial Visual Presentation）呈现范式；
- 在不同受试者群体上分别采集：
  - fMRI
  - MEG
  - EEG

这样能够：

- 做跨模态对齐；
- 比较时间动态与空间激活；
- 支持神经编码与解码模型。

---

## 刺激材料与阅读范式

### 文本来源
使用：

- BCCWJ（Balanced Corpus of Contemporary Written Japanese）

这是日本语言学界标准的大规模语料库。

### 文本结构
共包含：

- 20 篇新闻文章
- 229 个句子
- 1642 个短语单位（bunsetsu）

### RSVP 呈现
每个 bunsetsu：

- 显示 500ms
- 空屏 500ms

因此：

- 每秒呈现一个语言单元。

整个阅读任务：

- 约 30 分钟。

---

## 三种脑成像模态

### fMRI
特点：

- 高空间分辨率；
- TR = 2000ms；
- voxel size = 3×3×4 mm。

预处理流程：

- realignment
- slice timing correction
- coregistration
- segmentation
- normalization
- smoothing (8mm FWHM)

使用：

- MATLAB
- SPM12

---

### MEG
设备：

- 200-channel whole-head MEG

采样率：

- 1000Hz

预处理：

- CALM filter
- ICA 去眼动
- 0.1–40Hz bandpass
- epoch:
  - -100ms ~ 1000ms
- baseline correction
- 自动坏道剔除
- downsample 到 200Hz

工具：

- MNE-python
- Eelbrain

---

### EEG

设备：

- BrainAmp
- 64 electrodes

采样率：

- 1000Hz

预处理：

- ICA
- average rereference
- 0.1–40Hz filter
- epoching
- baseline correction
- 阈值剔除（150 μV）

同样下采样至：

- 200Hz。

---

## 技术验证（Technical Validation）

### 1）fMRI：ISC（Inter-Subject Correlation）

采用 leave-one-out ISC：

- 将一个受试者的 voxel 时间序列
- 与其他受试者平均时间序列相关。

目的：

- 验证不同受试者是否存在一致语言加工活动。

结果发现：

- 语言网络、
- 视觉皮层、
- visual word form area

均具有显著 ISC。

说明：

- 数据具有稳定自然阅读信号。

---

### 2）fMRI：GLM 分析

构建两个回归变量：

#### word rate
每个 bunsetsu offset 记为 1。

目的：

- 捕获语言处理相关活动。

#### word length
短语长度。

目的：

- 捕获视觉词形加工。

之后：

- 与 canonical HRF 卷积；
- 使用 nilearn 做 GLM；
- group-level one-sample t-test；
- FWE correction。

结果：

- word rate 激活：
  - 双侧 superior temporal gyrus；
- word length 激活：
  - fusiform cortex
  - visual word form area。

符合已有语言神经科学结论。

---

### 3）MEG / EEG 验证

作者使用：

- grand average evoked response。

MEG 中：

- 170–200ms 出现典型 visual word recognition peak（类似 M170）。

说明：

- 数据质量合理。

---

# 3. 实验设计

## 数据集规模

最终数据：

| 模态 | 人数 |
|---|---|
| fMRI | 36 |
| MEG | 35 |
| EEG | 41 |
| 总计 | 112 |

---

## Benchmark 属性

该工作本身就是 benchmark / dataset paper。

目标 benchmark：

- 脑-LLM 对齐；
- 神经编码；
- 语言认知建模；
- 跨模态脑信号分析。

---

## 对比对象

论文没有做传统“模型性能对比”。

主要是：

### 与已有数据集比较
包括：

- MoUS
- SMN4Lang
- Alice Dataset
- Narratives
- Le Petit Prince 等。

强调：

- 本工作是首个：
  - 日语；
  - 阅读范式；
  - 同时包含 fMRI + MEG + EEG；
  - 同一刺激。

---

## 实验场景

主要包含：

- 跨受试者一致性分析；
- GLM 激活分析；
- ERP/ERF 可视化验证；
- 行为理解正确率统计。

---

# 4. 资源与算力

论文几乎没有讨论训练算力。

因为：

- 这不是深度学习训练论文；
- 核心是数据采集与整理。

文中未提供：

- GPU 型号；
- GPU 数量；
- 训练时长；
- FLOPs；
- 推理成本。

但提供了实验硬件：

### fMRI
- Philips Achieva 3.0T MRI scanner

### MEG
- 200-channel whole-head MEG system

### EEG
- BrainAmp amplifier
- 64-channel cap

---

# 5. 实验数量与充分性

## 实验内容

论文实验主要是“数据有效性验证”。

包括：

- 行为正确率；
- ISC；
- GLM；
- MEG 平均响应；
- EEG 平均响应。

总体约：

- 4~5 类验证实验。

---

## 是否充分

### 优点
对于 dataset paper 来说：

- 验证较标准；
- 包含空间与时间维度；
- 使用经典神经指标；
- 与文献一致。

因此：

- 能够证明数据质量可靠。

### 不足
但从 benchmark 角度：

缺少：

- LLM encoding benchmark；
- decoding baseline；
- cross-modal alignment baseline；
- RSA / representational similarity analysis；
- transformer 对齐实验。

因此：

- 数据潜力巨大，
- 但“基准任务生态”尚未建立。

---

# 6. 主要结论与发现

## 数据集成功构建
作者成功发布：

- 多模态日语自然阅读脑数据集。

---

## 数据具有可靠神经信号

### fMRI
观察到：

- superior temporal gyrus
- visual word form area

等经典语言区域激活。

### MEG
观察到：

- 170–200ms visual word peak。

### EEG
观察到：

- 稳定 ERP 响应。

---

## 多模态统一刺激具有重要价值

统一 RSVP 刺激使得：

- 跨模态比较成为可能；
- temporal-spatial integration 更容易；
- 更适合评估认知模型。

---

## 日语是重要补充

由于日语具有：

- 黏着语 morphology；
- 灵活语序；

因此：

- 能补充现有英语中心研究。

---

# 7. 优点与亮点

## 1）首个统一刺激下的日语三模态阅读数据集

这一点是最大贡献。

目前几乎没有：

- fMRI + MEG + EEG
- 同时共享刺激
- 自然阅读
- 日语

的数据资源。

---

## 2）自然语言材料质量高

使用：

- BCCWJ

意味着：

- 语言学标注成熟；
- 适合 NLP 与认知科学结合。

---

## 3）跨模态互补性强

三种模态分别提供：

- 空间定位（fMRI）
- 毫秒级动态（EEG/MEG）

适合：

- 多尺度语言建模。

---

## 4）BIDS 标准化

数据严格遵循：

- BIDS
- MEG-BIDS
- EEG-BIDS

因此：

- 易于复现；
- 易于共享；
- 易于工具链接入。

---

## 5）公开开放

OpenNeuro 发布：

- 可直接下载；
- 附 preprocessing；
- 附 reconstruction script。

降低使用门槛。

---

# 8. 不足与局限

## 1）文本版权限制

BCCWJ 并非完全开放。

因此：

- event 文件不包含完整文本；
- 研究者需额外申请语料许可。

会影响：

- 使用便利性；
- reproducibility。

---

## 2）不同模态不是同一批受试者

fMRI / MEG / EEG：

- 使用不同 participant groups。

因此：

- 无法做严格 individual-level cross-modal alignment。

---

## 3）阅读范式不完全自然

RSVP 固定速率呈现：

- 不允许自由眼动；
- 不是真实自然阅读。

可能影响：

- 句法整合；
- 预测加工；
- attention dynamics。

---

## 4）规模仍有限

虽然 112 人不小，但：

- 单模态人数仍偏中等；
- 对深度学习 encoding benchmark 可能不足。

尤其：

- fMRI 只有 36 人。

---

## 5）缺少 benchmark baseline

目前缺少：

- transformer encoding benchmark；
- GPT/BERT 对齐结果；
- decoding baseline。

因此：

- 生态尚需后续工作补全。

---

## 6）语言覆盖仍有限

虽然填补了日语空白，但：

- 仍主要是新闻阅读；
- 缺少对话、文学、社交媒体等语言风格。

泛化性有限。

---

# 总结

BCCWJ-Brain 是一项高价值的神经语言学基础设施工作。其核心贡献不在于提出新模型，而在于：

- 首次建立统一刺激条件下的日语 fMRI+MEG+EEG 阅读数据集；
- 为脑-LLM 对齐提供新的多模态 benchmark；
- 推动 NLP、认知科学与神经科学的融合研究。

该资源尤其适合：

- 神经编码模型；
- 表征相似性分析；
- 语言时间动态研究；
- 跨语言脑机制比较；
- LLM 认知合理性评估。

其主要局限在于：

- RSVP 阅读生态不够自然；
- 尚未建立完整 benchmark pipeline；
- 不同模态并非同一受试者。

但总体上，这是一个具有长期研究价值的重要公开数据资源。

（完）
