---
title: "A multimodal dataset of EEG, eye-tracking, and physiological signals during naturalistic smartphone interactions"
title_zh: 自然化智能手机交互中的脑电图、眼动追踪与生理信号的多模态数据集
authors: "Mishra, P., Gandhi, T. K., Gandhi, S. R."
date: 2026-04-23
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.21.719334v1.full.pdf"
tags: ["query:profile-1"]
score: 9.0
evidence: 交互过程中的脑电与眼动多模态数据集
tldr: 本研究旨在弥补对自然化智能手机使用过程中神经和生理反应研究的空白，采集23名参与者在使用自己常用手机应用与观看自然视频时的EEG、眼动、PPG、GSR及问卷数据，构建公开的多模态数据集以支持相关行为和神经机制的研究。
source: biorxiv
selection_source: fresh_fetch
motivation: 当前对人们自然使用智能手机时的神经生理活动了解有限。
method: 研究让23名参与者在自然使用智能手机及观看视频时记录多模态生理数据并同步处理。
result: 数据集包含EEG、眼动、PPG和GSR等多模态同步记录，并附带智能手机使用相关问卷数据。
conclusion: 该数据集为研究智能手机使用的多维生理反应提供了开放且标准化的基础。
---

## 摘要
智能手机已成为用于通信、信息获取及数字交互的普遍工具，然而与自然化智能手机使用相关的神经生理动态仍未得到充分研究。本文提出了一个多模态生理数据集，该数据集采集于生态有效的智能手机交互任务及随后的标准化低参与度基线条件中。二十三名参与者各自使用他们最常使用的智能手机应用（主要为游戏或短视频）进行十分钟的交互，随后观看一个持续五分钟的标准化自然景观视频。同时记录包括脑电图（EEG，64通道）、可穿戴眼动追踪、光电容积脉搏波（PPG）以及皮肤电反应（GSR）传感器信号。通过问卷评估，包括智能手机成瘾量表（SAS）和移动电话问题使用量表（MPPUS），用于表征个体在智能手机相关行为特质上的差异。所有数据流均通过晶体管—晶体管逻辑（TTL）触发信号进行同步，以确保多模态之间的精确时间对齐。数据集按照脑成像数据结构（BIDS）规范进行组织，并已公开发布于 OpenNeuro（登录号：ds007537）。该数据集支持研究智能手机交互过程中的神经、眼部及自主反应，并为多模态分析多样化的智能手机行为提供生态有效的支持。

## Abstract
Smartphones have become pervasive tools for communication, information consumption, and digital interaction, yet the neurophysiological dynamics associated with naturalistic smartphone use remain insufficiently characterized. Here, we present a multimodal physiological dataset collected during ecologically valid smartphone interaction and a subsequent standardized low-engagement baseline condition. Twenty-three participants engaged with their most frequently used smartphone application (primarily gaming or short form video) for ten minutes, followed by a five-minute passive viewing of a standardized nature video. Simultaneous recordings were obtained from electroencephalography (EEG; 64 channels), wearable eye-tracking, photoplethysmography (PPG), and galvanic skin response (GSR) sensors. Questionnaire-based assessments, including the smartphone addiction scale (SAS) and the mobile phone problematic use scale (MPPUS), are also collected to characterize individual differences in smartphone-related behavioral traits. All data streams are synchronized using transistor-transistor logic (TTL) trigger signals to ensure precise temporal alignment across modalities. The dataset is organized according to the Brain Imaging Data Structure (BIDS) specification and is publicly available on OpenNeuro (Accession Number: ds007537). This dataset enables the investigation of neural, ocular, and autonomic responses during smartphone interaction and supports multimodal analysis of diverse smartphone behaviors while preserving ecological validity.

---

## 论文详细总结（自动生成）

# 自然化智能手机交互中的脑电图、眼动追踪与生理信号的多模态数据集 — 深度总结

---

## 一、研究核心问题与整体含义

- **研究动机**  
  当前智能手机已深度融入日常生活，对注意力、情绪调节与认知资源分配的影响受到越来越多关注。尽管已有大量行为学研究，但人们在**自然化使用智能手机（无任务约束、自由操作）**时的**神经与生理反应机制**尚未被系统刻画。  
- **核心问题**  
  过去研究大多使用实验控制下的单模态数据（如仅 EEG 或仅眼动），缺乏对多模态信号的同步记录。不同模态在时间尺度上难以对齐，限制了对真实交互状态的理解。  
- **研究目标**  
  本研究旨在**构建首个在自然手机使用情境下同步获取 EEG、眼动、心率（PPG）与皮肤电（GSR）信号的开放数据集**，为神经科学、心理学及人机交互领域提供生态有效的研究资源。

---

## 二、方法论与技术实现

- **核心思想**  
  - 通过生态有效的实验设计，让受试者在自然状态下使用自己的智能手机，从而保留真实的交互模式和心理动态。  
  - 同时采集脑电、眼动与自主神经信号，并通过 TTL（Transistor–Transistor Logic）触发信号实现**跨模态精确同步**。  
  - 按照 **BIDS（Brain Imaging Data Structure）标准**组织与发布，保证数据的互操作性与复现性。  

- **多模态采集系统架构**  
  1. **EEG**：Brain Products ActiCHamp 64 通道系统，采样率 1000 Hz；Cz 参照；可接收外部 TTL 触发。  
  2. **Eye-tracking**：Tobii Pro Glasses 2，可实时捕捉凝视点、瞳孔直径、头部加速度与角速度；独立同步接口接收 TTL。  
  3. **PPG/GSR**：通过 EEG 系统的辅助通道采集；通道 1 为 PPG，通道 2 为 GSR。  
  4. **同步机制**：实验开始与结束分别发送 5 个 1 Hz TTL 脉冲，每 20 秒发一次周期触发用于连续时间校准。  

- **数据结构组织与处理**  
  - 数据按 BIDS 层级（dataset → sub → modality）组织。  
  - EEG 储存采用 BrainVision 格式（.eeg, .vhdr, .vmrk）；眼动数据存为 TSV 压缩表格，附带 JSON 元数据。  
  - 使用 Python 工具链（MNE-BIDS、定制 parser）实现格式转换与元数据生成。  

---

## 三、实验设计

- **受试者信息**  
  - 共 23 名参与者（其中女性 8 名），年龄 20–32 岁（均正常视力）；无神经疾病史。  
- **实验流程**  
  - **阶段一：自然手机交互（10 分钟）**  
    - 受试者自由使用自己最常用的 App，不受内容或形式限制。  
    - 实际应用分布：短视频类（14 名，Instagram Reels/YouTube Shorts）、游戏类（7 名，Subway Surfers 等）、阅读类（2 名）。  
  - **阶段二：基线条件（5 分钟）**  
    - 观看标准化自然景观视频（Earth 4K Relaxation），建立低参与度参考状态。  
  - **问卷测评**  
    - 智能手机成瘾量表（SAS）  
    - 移动电话问题使用量表（MPPUS）  
- **对比基准**  
  - 研究未与其他方法性能进行比较，而是提供**数据质量验证基准**：EEG 信噪比（SNR）、眼动追踪精度、皮肤电与心率指标的生理合理性。  

---

## 四、资源与算力

- 文中未使用深度学习或大规模计算训练任务。  
- 数据处理与质量验证均在 **Python + MNE 1.7.0 环境** 下完成，未提及 GPU 或集群算力信息。  
- 可认定为轻量级信号处理与数据验证研究，无高性能算力需求。

---

## 五、实验数量与充分性

- **实验形式**：  
  1. EEG 信号质量验证（滤波、ICA、坏通道检测及插值）。  
  2. 频带信噪比计算（delta–gamma 各频段）。  
  3. 眼动数据质量检测（瞳孔值、视线分布、头部加速度）。  
  4. PPG 与 GSR 信号生理有效性验证（心率、HRV、SCR、EDA 均值）。  
- **充分性评价**  
  - 23 名被试虽非大规模样本，但对探索性生理数据研究而言具有可比代表性。  
  - 各模态均进行了系统内部一致性与外部生理合理性验证，整体客观充分。  

---

## 六、主要结论与发现

- 成功建立了一个**同步多模态自然化智能手机交互数据集**，覆盖 EEG、眼动、PPG、GSR 及行为问卷。  
- 数据集质量验证结果表明：  
  - EEG 各频段均具生理可信的功率分布，α 波在基线视频阶段显著增强、θ 波在任务期增强。  
  - 眼动与头部运动数据呈现自然姿态差异（手机使用时注视偏下，视频观看时偏上）。  
  - PPG 与 GSR 信号均在正常生理范围；任务条件下皮肤电反应频率略高，体现注意与情绪激活。  
- 研究验证 TTL 同步机制在多模态数据整合上的高稳定性（时间误差低于 0.1 s）。  
- 数据集已开放发布，可用于研究注意力机制、认知负荷、生理耦合及智能手机使用行为建模。

---

## 七、优点与贡献

- **生态有效性强**：采用个体自选常用 App，自然情境下采集；区别于人工任务实验。  
- **多模态同步记录**：首个实现 EEG–眼动–自主神经信号实时同步的开放数据集。  
- **BIDS 标准化存储**：便于直接兼容主流神经成像分析工具。  
- **内部质量验证严谨**：对各模态信号均提供系统性 QA 结果与统计指标。  
- **开放共享精神**：数据与代码均已公开，附详细元数据说明，确保复现性。  

---

## 八、不足与局限

- **样本量偏小**：仅 23 人，且偏向年轻人群，代表性有限。  
- **未涵盖多任务情境**：仅包含自由使用与观看视频两种状态，未区分任务复杂度、社会互动等变量。  
- **内容多样化受限**：虽然允许自选 App，但类型仍集中在短视频与游戏。  
- **未进行跨研究基准比较**：未评估与现有 EEG–眼动同步研究的相对性能。  
- **算力与实时分析缺失**：未探讨数据实时处理或在线情绪检测等应用潜力。  

---

**（完）**
