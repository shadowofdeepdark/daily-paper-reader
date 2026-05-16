---
title: A dual EEG hyperscanning dataset of natural French face-to-face conversation
title_zh: 自然法语面对面对话的双脑 EEG 超扫描数据集
authors: "Yamasaki, H., Blache, P., Schön, D."
date: 2026-05-15
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.13.724780v1.full.pdf"
tags: ["query:q8"]
score: 9.5
evidence: 自然对话和说话者-听者耦合的脑电超扫描
tldr: 本研究发布了DUET数据集，这是一个双脑EEG超扫描数据集，用于研究自然法语面对面对话中的神经动态。通过记录36名法语参与者组成的18对话对在合作任务中的脑电信号，数据集提供了同步脑活动、语音特征和转录信息，为研究说听耦合和互动协调提供了基础。
source: biorxiv
selection_source: fresh_fetch
motivation: 自然对话的神经机制仍缺乏生态有效的数据支持，因此需要专门的脑电超扫描数据集。
method: 研究使用高密度EEG同时记录两名受试者进行面对面对话任务的脑电活动，并附带语音及转录数据。
result: 共收集了18对法语对话者、8轮任务的同步EEG数据及相关音频文本特征。
conclusion: DUET数据集为研究自然语言交流的神经机制提供了开放、高质量的实验资源。
---

## 摘要
对话是人类的基本行为之一，需要在说话、聆听和轮流发言之间进行快速协调。然而，在自然交互中捕捉其神经动态的数据集仍然很稀缺。双脑扫描 EEG（hyperscanning EEG）特别适用于此目的，因为它能同时记录双方的脑信号，使研究者能够分析说话者与听者之间的神经耦合、反应时序以及互动协调。本文介绍 DUET（Dyadic Understanding, EEG and Turn-taking）数据集，用于研究自然法语面对面对话的双脑 EEG 数据。该数据集包括来自 18 对双人组（共 36 名法语成年人）的记录，他们在八个每次持续 4 分钟的面对面对话环节中完成 Diapix 协作找不同任务。对于每位参与者，收集了 EEG 数据；其中，大部分记录使用 64 通道 EEG，一对试验性双人组使用了 32 电极。公开发布版本包含原始 EEG 记录、可在后续预处理中重用的 ICA 分解结果，以及从音频和人工校正的转录中提取的各种特征。

## Abstract
Conversation is a fundamental human behaviour that requires rapid coordination between speaking, listening, and turn-taking, yet datasets capturing its neural dynamics in natural interaction remain scarce. Hyperscanning EEG is particularly valuable for this purpose because it records both interlocutors simultaneously, enabling the study of speaker-listener coupling, response timing, and dyadic coordination during live exchange. Here we present DUET (Dyadic Understanding, EEG and Turn-taking), a hyperscanning dataset for studying natural French face-to-face conversation. The dataset comprises recordings from 18 dyads, or 36 French-speaking adults, performing the Diapix collaborative spot-the-difference task across eight 4-minute face-to-face conversation blocks. For each participant, EEG was recorded from 36 participants; most recordings used 64-channel EEG, with one pilot dyad recorded using 32 electrodes. The public release includes raw EEG recordings, precomputed ICA decompositions for reuse in downstream preprocessing as well as various features derived from the audio and manually corrected transcripts.

---

## 论文详细总结（自动生成）

# 论文总结：自然法语面对面对话的双脑 EEG 超扫描数据集（DUET）

---

## 一、核心问题与研究背景

- **研究动机**：人类对话包含复杂的认知与社会互动过程，需要在讲话与聆听之间实现实时的神经协调。然而，现有神经科学研究多基于单人或实验室控制的任务，缺乏对自然、生态真实对话场景下脑动态的系统记录。  
- **研究空白**：目前关于自然语言交互的双脑神经数据十分匮乏，不足以支撑深入的对话研究、神经同步（neural coupling）分析以及多模态语言交流建模。  
- **整体目标**：本文旨在公开一个经过精心设计的、自然法语面对面对话的高质量“双脑 EEG 超扫描数据集”（DUET），为研究人类语言沟通的神经机制提供可重复、生态有效的实验基础。

---

## 二、方法论：核心思想与关键技术细节

- **核心思想**：通过**同时记录**对话双方的脑电信号（EEG），实现对实时交互中**说话者-听者之间神经耦合**的捕捉。  
- **关键技术实现**：
  - **双脑同步采集（hyperscanning）**：两套 EEG 系统同步记录，保证时间精度达到毫秒级。
  - **任务设计**：采用 *Diapix* 协作对话任务，即两名受试者在面对面交流中共同寻找不同点，从而引发自然语言互动。
  - **EEG 采集规格**：
    - 主要使用 64 通道 EEG 系统（一个试验性双人组使用 32 通道）。
    - 同步记录音频数据，用于语音特征与转录比对。
  - **预处理与数据共享**：
    - 提供原始 EEG 文件与预计算的 ICA（独立成分分析）分解结果，以便后续去伪迹处理。
    - 音频数据经过人工转录与校正，配合时序标注可进行语言、听觉、语义等多维度分析。

---

## 三、实验设计

- **数据来源**：DUET 数据集采集自 18 对双人组（共 36 名法语母语成年人），每对完成 8 个持续约 4 分钟的面对面对话任务。
- **实验情境**：
  - 对话为自然互动，非实验指令或脚本。
  - 场景为面对面协作任务，增加社会语境真实性。
- **benchmark / 对比设计**：
  - 本文**未进行模型性能对比**，主要侧重数据集构建与公开。
  - 数据内容可作为后续研究 benchmark，用于发展和比较不同的神经同步度分析方法、语音-脑信号耦合建模算法等。

---

## 四、资源与算力

- 文中仅提及 EEG 数据采集硬件和 ICA 分解过程，**未说明具体算力资源或计算配置**（如 GPU 型号、数量、分析时长等）。
- 数据处理流程主要为脑电信号预处理，而非深度学习模型训练，故算力需求相对较低。

---

## 五、实验数量与充分性

- **实验规模**：共收集 18 对 dyads × 8 轮任务 = 144 段完整对话，合计时长约 9.6 小时。
- **实验多样性**：
  - 覆盖不同性别、不同言语交互节奏的法语母语者。
  - 任务设计确保自然交流与轮流发言现象的出现。
- **充分性评价**：
  - 样本数量对于 EEG hyperscanning 数据集而言**相对充分**。
  - 虽然未包含跨语言或跨文化条件，但对单语言生态研究来说已具备较高数据质量与代表性。

---

## 六、主要结论与发现

1. 成功构建并公开了 **DUET 数据集**——首个自然法语面对面对话的双脑 EEG 数据集。  
2. 数据可同时用于研究：
   - 说话者与听者的脑活动耦合；
   - 语音与脑信号之间的时序关系；
   - 对话轮换（turn-taking）和神经协同的动态过程。  
3. 公开的数据支持 EEG、语音、文本的多模态研究，能够促进自然语言神经机制的探索。

---

## 七、优点（亮点）

- **生态有效性高**：面对面真实交流场景，比传统实验式语言任务更贴近自然沟通。  
- **双脑同步记录**：提供说听耦合的时序数据，使 dyadic interaction 得以定量分析。  
- **数据完整性强**：
  - 包含原始 EEG + ICA 分解 + 音频 + 转录多层信息；
  - 可直接用于后续信号分析与模型开发。  
- **开放共享**：对研究社区友好，促进跨机构数据复现与比较。

---

## 八、不足与局限

- **场景受限**：仅包括法语对话，缺乏语言与文化多样性。  
- **样本量有限**：36 人虽足够用于探索性研究，但在统计建模上仍略偏小。  
- **实验任务单一**：Diapix 协作任务虽自然，但交互类型相对固定，不涵盖争论、情感交流等复杂语用情境。  
- **无模型评估**：本文为数据集论文，未验证任何计算模型或分析算法在该数据上的表现。  
- **算力未说明**：未报告数据处理的计算开销与分析时长，对重现性略有影响。

---

（完）
