---
title: Human brains implicitly and rapidly distinguish AI from human voices before decoding prosodic meaning
title_zh: 在人类大脑中，在解码韵律意义之前，能够隐性且快速地区分 AI 与人类声音
authors: "Chen, W., Pell, M., Jiang, X."
date: 2026-04-09
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.08.716483v1.full.pdf"
tags: ["query:profile-1"]
score: 9.0
evidence: 脑电数据、韵律意义和神经时间进程
tldr: 本研究通过脑电实验发现，人脑在听到声音约134–176毫秒内即可区分AI和人声，远早于对语调意义的分析，表明快速的声学特征而非语调主导了这种识别，对理解人类如何检测AI语音具有重要意义。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-08-716483-v1/fig-001.webp\", \"caption\": \"Figure 2. Validation of training stimuli. (A) Mean F0 comparison between AI and human voices in two prosodies. Connecting lines link matched audio pairs (same prosody, statement, speaker). (B) Perceptual ratings of humanlikeness and vocal confidence (1-7 scale; error bars: SE). (C) Machine learning classification of confident vs. doubtful prosody at 5% intervals (5- 100% normalized duration). Filled markers indicate FDR-corrected significance (p < 0.05).\", \"page\": 15, \"index\": 1, \"width\": 892, \"height\": 627}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-08-716483-v1/fig-002.webp\", \"caption\": \"Figure 4. Partial RSA: Independent Acoustic Contributions to Neural Voice Source Structure. Partial Spearman correlations between neural and acoustic RDMs (N = 40, 2 ms resolution, 0–1500 ms). Each panel shows mean partial r (±1 SEM, shaded) after controlling for the specified features. Bottom colored bars: significant clusters vs. 0 (one-sided cluster permutation, p < .05); onset latencies annotated with downward arrows. Top bars: significant between-model differences (two-sided, p < .05); onset latencies annotated with upward arrows. Gray shading: MVPA source decoding onset (134–176 ms). Dashed line: mean stimulus duration (1559 ms). HFE = high-frequency energy (>4 kHz); MFCC = melfrequency cepstral coefficients.\", \"page\": 18, \"index\": 2, \"width\": 892, \"height\": 400}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-08-716483-v1/fig-003.webp\", \"caption\": \"Figure 1. Experimental Design and Analysis Pipeline. (A) Speaker identity learning task across 8 blocks (4 Human, 4 AI), each comprising a Training phase (24 trials; EEG recorded) and a Checking phase (12 trials). (B) MVPA was applied to EEG patterns (59 channels) from the Training phase to decode voice source (Human vs. AI) at each timepoint using linear discriminant analysis, yielding temporal decoding curves (AUC) and time generalization matrices. (C) Partial RSA compared neural RDMs (4×4, correlation distance; 2 ms resolution, 0–1500 ms) with acoustic feature RDMs (F0, HFE, MFCC). Four models assessed independent contributions of HFE and MFCC controlling for F0 and each other (M1: HFE|F0; M2: MFCC|F0; M3: HFE|F0+MFCC; M4: MFCC|F0+HFE). Schematic time courses illustrate the expected pattern of results.\", \"page\": 8, \"index\": 3, \"width\": 892, \"height\": 831}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-08-716483-v1/fig-004.webp\", \"caption\": \"Figure 3. Mel spectrograms and temporal decoding of voice source and prosody. (A-D) Spectrograms of an exemplar sentence across conditions. (E-H) Time-generalization matrices (TGM) showing decoding performance. (I-J) Temporal decoding curves. Shaded areas: SE. Colored bars: significant clusters (p < 0.05, cluster-based permutation). Dashed lines: mean (1559 ms) and maximum (2103 ms) stimulus duration.\", \"page\": 16, \"index\": 4, \"width\": 892, \"height\": 462}]"
motivation: 现有研究认为听众依靠语调线索识别AI声音，但尚不清楚这种差异在神经加工中何时出现。
method: 研究采用脑电图记录参与者听辨AI与人声的神经反应，并使用多变量模式分析和语音声学特征比较。
result: 结果显示神经层面对AI与人声的区分在约134–176毫秒即出现，而语调区分要到上千毫秒后才发生，且主要由声谱包络特征驱动。
conclusion: 研究表明人脑在处理声音时能在理解语调之前迅速区分AI与人声，说明这种识别依赖快速的声源特征而非语调。
---

## 摘要
人们每天都会接触到 AI 声音。现有的行为研究表明，听者依赖语调和表现力等韵律线索来检测音频深度伪造（deepfake），并报告称 AI 声音在韵律上比人类声音更缺乏丰富性。为了检验韵律加工是否在语音处理的神经时间进程中驱动深度伪造识别，我们记录了参与者在听取人类和 AI 生成说话者以自信与怀疑韵律（语音语调）发出的语句时的脑电图（EEG）数据，并要求他们注意记忆说话者姓名。我们使用语音克隆技术来控制人类与 AI 声音之间的说话者身份混淆。多变量模式分析（MVPA）结果显示，无论韵律类型如何，人类与 AI 声音的神经区分都迅速出现（自信韵律：176 毫秒；怀疑韵律：134 毫秒），显著早于韵律区分（在人体语音中自信 vs. 怀疑：2066 毫秒；在 AI 语音中：1366 毫秒）。声学分析证实，韵律差异仅在语句结束时（约归一化持续时间的 90%）才可分类，这与神经证据一致，表明韵律解码需要几乎完整的时间整合。这种快速的语音来源区分与迟发的韵律解码之间的时间分离表明，韵律在音频深度伪造检测中的作用比听者事后报告的更小。表征相似性分析进一步揭示，谱包络特征（梅尔频率倒谱系数，MFCC），而非视觉上显著的高频能量差异，驱动了神经层面对人类和 AI 声音的区分，其中 MFCC 的最早独立贡献（228 毫秒）与 MVPA 解码起始（134–176 毫秒）紧密对应。未来的研究可以操纵特定声学成分，以确定这种快速且持续的神经区分的因果来源。

## Abstract
People encounter AI voices daily. Existing behavioral studies suggest listeners rely on prosodic cues such as intonation and expressiveness to detect audio deepfakes, reporting that AI voices sound prosodically less rich than human voices. To test whether prosodic processing drives deepfake discrimination in the neural time course of voice processing, we recorded electroencephalographic (EEG) data while participants listened to human and AI-generated speakers producing utterances in confident vs. doubtful prosody (tone of voice), with attention directed toward memorizing speaker names. We used voice cloning to control for speaker identity confounds between human and AI voices. Multivariate pattern analysis revealed that neural discrimination of human vs. AI voices emerged rapidly regardless of prosody (confident: 176 ms; doubtful: 134 ms), substantially preceding prosody discrimination (confident vs. doubtful within human voices: 2066 ms; within AI voices: 1366 ms). Acoustic analysis confirmed that prosodic distinctions became classifiable only at utterance offset (90% normalized duration), converging with neural evidence that prosody requires near-complete temporal integration. This temporal dissociation between rapid voice source discrimination and late-emerging prosody decoding suggests that prosody plays a smaller role in audio deepfake detection than listeners retrospectively report. Representational similarity analysis further revealed that spectral envelope features (mel-frequency cepstral coefficients; MFCC), rather than the visually salient high-frequency energy differences, drove neural human-AI discrimination, with MFCC's earliest independent contribution (228 ms) closely following the MVPA decoding onset (134-176 ms). Future studies may manipulate specific acoustic components to establish the causal sources of this rapid and sustained neural discrimination.

---

## 论文详细总结（自动生成）

# 人脑在解码语调意义之前隐性且快速地区分 AI 与人类声音 — 深度总结

---

## 一、核心问题与研究动机

- **研究背景**：随着合成语音技术（voice cloning、deepfake）的广泛应用，人们日常生活中频繁接触 AI 合成声音（例如导航、语音助手、电话录音等）。
- **问题起点**：行为学研究表明，人类自觉地主要根据韵律特征（如语调的自然性或表现力）判断声音是否为 AI，但尚不清楚这种“韵律主导”的经验是否在神经加工层面真实存在。
- **理论意义**：理解人脑区分 AI 与人声的时间进程，可揭示潜在的自动检测机制，并为社会认知与深度伪造检测策略提供神经学依据。
- **研究目标**：探讨在人脑中，区分声音来源（人类 vs. AI）的神经过程是否依赖韵律处理，以及两者在时间上谁先发生。

---

## 二、方法论与技术路线

### 核心思想

通过**脑电 (EEG)** 与**多变量模式分析 (MVPA)** 技术，细致跟踪人脑在听到声音后的毫秒级反应；再结合**表征相似性分析 (RSA)**，将脑电模式与声学特征对齐，探寻导致区分 AI 与人类声音的主要声学信号。

### 关键技术步骤

1. **声音刺激准备**
   - 使用语音克隆技术（Huawei Celia 系统）为每位人类说话人生成对应的 AI 声音，确保人类与 AI 声源在说话者身份和句子内容上高度匹配，消除身份混淆。
2. **EEG 实验设计**
   - 参与者在听音过程中仅需**记忆说话者姓名**，不关注声音来源或语调，使研究可检测“隐性加工”而非显性判断。
3. **MVPA 时序解码**
   - 应用线性判别分析（LDA）分类器对 EEG 时序信号进行逐时间点解码，根据 **AUC 曲线** 识别在何时对“声音来源”与“韵律类别”实现显著区分。
4. **RSA 声学建模**
   - 构建音频特征向量（F0、HFE、MFCC）。
   - 计算 EEG 的 4×4 条件差异矩阵。
   - 使用**偏相关（Partial Spearman correlation）**在多个控制模型中分析各特征的独立贡献，从而筛选出驱动神经差异的关键声学线索。
5. **对比分析**
   - 对比“声音来源解码起始时间”与“韵律解码起始时间”，揭示两种加工的时间差。

*无复杂公式，主要依赖分类与相关分析的统计流程。*

---

## 三、实验设计与数据来源

- **被试群体**：40名健康的母语为普通话的大学生（男女各20名）。
- **语音数据集**：
  - 来自一个大型普通话语料库（共11,808条录音）。
  - 选取24名说话人录制“自信”和“怀疑”两种韵律语句。
  - 各自训练 AI 克隆版本，每种韵律独立建模。
  - 生成并录制匹配的 192 个句子（人声与 AI 各96句）。
- **EEG 数据采集条件**：64通道脑电帽（ActiCap）、采样率500 Hz，屏蔽室内记录。
- **实验过程**：
  1. 8个实验区块（前4区块为人声，后4区块为AI声）。
  2. 每区块包含训练与检测阶段；训练阶段记录EEG，检测阶段验证记忆效果。
  3. 任务：记忆名字，与声音源及韵律无关。
- **评测指标**：
  - 声学特征：F0、HFE、MFCC。
  - 神经指标：MVPA AUC时间曲线、RSA相关系数。
  - 行为指标：说话人识别准确率（均值94.2%）。

---

## 四、资源与算力

- **算力说明**：
  - 文中未报告具体 GPU、运算时间或算力配置。
  - 声音特征提取与分类使用 Python（librosa、scikit-learn）完成；脑电数据处理在 MATLAB/EEGLAB 环境中进行。
  - 由于任务以 EEG 数据分析为主，应该不涉及大规模模型训练，算力需求有限。

---

## 五、实验数量与充分性

- **主要实验组成**：
  1. **行为验证**（声源记忆任务准确率）；
  2. **声学分析**（F0对比、机器学习分类时间窗分析）；
  3. **神经解码**（MVPA时序分析与RSA多模型）；
  4. **声学与神经对应分析**（四个偏相关模型 M1–M4）。
- **实验丰富度**：
  - 共分析约7400+有效脑电试次。
  - 声学与神经数据相互验证。
  - 多重统计控制（FDR、Permutation Test）确保显著性。
- **公平性**：人类与AI声音均源自同一说话者与语句，实验设计避免声源偏差，控制良好。
- **充分性评价**：实验数量适中，分析多层次（声学、神经、感知），结论具有高可信度。

---

## 六、主要结论与发现

1. **AI 与人类声音的神经区分极早出现**：
   - 自信韵律下：176毫秒；
   - 怀疑韵律下：134毫秒；
   - 均早于韵律区分（AI：1366毫秒；人声：2066毫秒）。
2. **韵律信息解码出现较晚**：
   - 声学分类实验表明，语句90%持续时间后才可区分自信/怀疑韵律。
3. **神经区分主要由谱包络特征驱动**：
   - MFCC 特征在约 228 毫秒开始独立预测神经反应；
   - 高频能量（HFE）虽显著，但其效果被 MFCC 所涵盖。
4. **结论意义**：
   - 人脑能在理解语调意义之前“隐性且迅速”识别声音来源；
   - 听众所报告的“依赖语调识别AI”的主观看法可能是**事后归因**，并非真实的加工依据。

---

## 七、研究优点与亮点

- **创新性设计**：采用语音克隆匹配说话人身份，彻底消除声源差异的潜在混淆。
- **隐性任务范式**：让声音来源在任务中“无关”，揭示真正的自动化神经反应。
- **多层验证**：结合声学机器学习与脑电时序分析，确保跨模态一致性。
- **时间分辨率高**：毫秒级 MVPA 和 RSA 分析精准刻画大脑动态。
- **数据共享开放**：实验数据与代码全部在 OSF 平台公开。

---

## 八、不足与局限

- **语料与语言限制**：仅使用普通话语音，结论可能不直接适用于其他语言或多音节结构。
- **韵律类型局限**：仅比较自信 vs. 怀疑两种语调，未涵盖更丰富的情绪或表达性韵律。
- **区块顺序效应**：实验固定人声在前、AI在后，可能引入学习序列偏差。
- **群体样本**：数据来自年轻大学生，缺乏年龄与文化多样性验证。
- **算力与实时性**：研究偏神经认知，不涉及实时检测算法，实际应用的可迁移性尚待测试。
- **声学机制未完全解析**：MFCC 作为综合特征，无法指明具体哪一声谱组成是关键差异。

---

（完）
