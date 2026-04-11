---
title: Human brains implicitly and rapidly distinguish AI from human voices before decoding prosodic meaning
title_zh: 在人类大脑解码韵律意义之前，能够隐性且快速区分AI与人类语音
authors: "Chen, W., Pell, M., Jiang, X."
date: 2026-04-09
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.08.716483v1.full.pdf"
tags: ["query:profile-1"]
score: 9.0
evidence: 关于人类与AI语音中语调及语用含义的脑电研究
tldr: 本研究探讨人类大脑识别AI声音的时间机制，通过EEG实验比较人类与AI语音在不同语调下的反应。结果显示，大脑能在约150毫秒内区分AI与人类声音，此过程独立于较晚出现的语调处理，说明语调在听觉深伪检测中的作用有限。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-08-716483-v1/fig-001.webp\", \"caption\": \"Figure 2. Validation of training stimuli. (A) Mean F0 comparison between AI and human voices in two prosodies. Connecting lines link matched audio pairs (same prosody, statement, speaker). (B) Perceptual ratings of humanlikeness and vocal confidence (1-7 scale; error bars: SE). (C) Machine learning classification of confident vs. doubtful prosody at 5% intervals (5- 100% normalized duration). Filled markers indicate FDR-corrected significance (p < 0.05).\", \"page\": 15, \"index\": 1, \"width\": 892, \"height\": 627}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-08-716483-v1/fig-002.webp\", \"caption\": \"Figure 4. Partial RSA: Independent Acoustic Contributions to Neural Voice Source Structure. Partial Spearman correlations between neural and acoustic RDMs (N = 40, 2 ms resolution, 0–1500 ms). Each panel shows mean partial r (±1 SEM, shaded) after controlling for the specified features. Bottom colored bars: significant clusters vs. 0 (one-sided cluster permutation, p < .05); onset latencies annotated with downward arrows. Top bars: significant between-model differences (two-sided, p < .05); onset latencies annotated with upward arrows. Gray shading: MVPA source decoding onset (134–176 ms). Dashed line: mean stimulus duration (1559 ms). HFE = high-frequency energy (>4 kHz); MFCC = melfrequency cepstral coefficients.\", \"page\": 18, \"index\": 2, \"width\": 892, \"height\": 400}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-08-716483-v1/fig-003.webp\", \"caption\": \"Figure 1. Experimental Design and Analysis Pipeline. (A) Speaker identity learning task across 8 blocks (4 Human, 4 AI), each comprising a Training phase (24 trials; EEG recorded) and a Checking phase (12 trials). (B) MVPA was applied to EEG patterns (59 channels) from the Training phase to decode voice source (Human vs. AI) at each timepoint using linear discriminant analysis, yielding temporal decoding curves (AUC) and time generalization matrices. (C) Partial RSA compared neural RDMs (4×4, correlation distance; 2 ms resolution, 0–1500 ms) with acoustic feature RDMs (F0, HFE, MFCC). Four models assessed independent contributions of HFE and MFCC controlling for F0 and each other (M1: HFE|F0; M2: MFCC|F0; M3: HFE|F0+MFCC; M4: MFCC|F0+HFE). Schematic time courses illustrate the expected pattern of results.\", \"page\": 8, \"index\": 3, \"width\": 892, \"height\": 831}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-08-716483-v1/fig-004.webp\", \"caption\": \"Figure 3. Mel spectrograms and temporal decoding of voice source and prosody. (A-D) Spectrograms of an exemplar sentence across conditions. (E-H) Time-generalization matrices (TGM) showing decoding performance. (I-J) Temporal decoding curves. Shaded areas: SE. Colored bars: significant clusters (p < 0.05, cluster-based permutation). Dashed lines: mean (1559 ms) and maximum (2103 ms) stimulus duration.\", \"page\": 16, \"index\": 4, \"width\": 892, \"height\": 462}]"
motivation: 研究旨在确定人类识别AI语音是否依赖语调处理及其在脑内的时间进程。
method: 利用EEG记录听众听人类与AI语音时的脑电反应，并进行多变量模式分析与声学特征分析。
result: 神经区分AI与人类声音在约134至176毫秒出现，而语调分析要等到超过1秒后才发生，且MFCC特征驱动区分过程。
conclusion: 研究表明人类大脑能在极短时间内区分AI与人类声音，这种区分独立于语调分析。
---

## 摘要
人们每天都会接触到人工智能（AI）生成的语音。现有的行为研究表明，听者依赖语调和表现力等韵律线索来检测音频深伪，认为AI语音在韵律上比人类语音更缺乏丰富性。为了检验韵律加工在语音处理的神经时间过程中是否驱动深伪识别，我们记录了参与者在听人类和AI生成的说话者以自信与怀疑两种语调（语气）发声时的脑电图（EEG）数据，并要求他们专注于记忆说话者的名字。我们使用语音克隆技术来控制人类与AI语音间与说话者身份相关的混杂因素。多变量模式分析显示，不论语调，自人类与AI语音的神经区分均迅速出现（自信语调：176毫秒；怀疑语调：134毫秒），这一过程显著早于语调区分的出现（在人类语音中自信 vs. 怀疑：2066毫秒；在AI语音中自信 vs. 怀疑：1366毫秒）。声学分析确认韵律差异仅在话语结束处（归一化时长的90%）变得可分类，这与神经证据一致，表明韵律加工需要几乎完整的时间整合。这种声音来源快速区分与韵律解码迟发之间的时间分离表明，韵律在音频深伪检测中所起的作用比听者事后报告的要小。表征相似性分析进一步揭示，谱包络特征（梅尔频率倒谱系数，MFCC），而非视觉上显著的高频能量差异，驱动了神经对人类与AI语音的区分；MFCC的最早独立贡献（228毫秒）紧随MVPA解码起点（134-176毫秒）。未来研究可操控具体声学成分，以确定这种快速而持续的神经区分的因果来源。

## Abstract
People encounter AI voices daily. Existing behavioral studies suggest listeners rely on prosodic cues such as intonation and expressiveness to detect audio deepfakes, reporting that AI voices sound prosodically less rich than human voices. To test whether prosodic processing drives deepfake discrimination in the neural time course of voice processing, we recorded electroencephalographic (EEG) data while participants listened to human and AI-generated speakers producing utterances in confident vs. doubtful prosody (tone of voice), with attention directed toward memorizing speaker names. We used voice cloning to control for speaker identity confounds between human and AI voices. Multivariate pattern analysis revealed that neural discrimination of human vs. AI voices emerged rapidly regardless of prosody (confident: 176 ms; doubtful: 134 ms), substantially preceding prosody discrimination (confident vs. doubtful within human voices: 2066 ms; within AI voices: 1366 ms). Acoustic analysis confirmed that prosodic distinctions became classifiable only at utterance offset (90% normalized duration), converging with neural evidence that prosody requires near-complete temporal integration. This temporal dissociation between rapid voice source discrimination and late-emerging prosody decoding suggests that prosody plays a smaller role in audio deepfake detection than listeners retrospectively report. Representational similarity analysis further revealed that spectral envelope features (mel-frequency cepstral coefficients; MFCC), rather than the visually salient high-frequency energy differences, drove neural human-AI discrimination, with MFCC's earliest independent contribution (228 ms) closely following the MVPA decoding onset (134-176 ms). Future studies may manipulate specific acoustic components to establish the causal sources of this rapid and sustained neural discrimination.

---

## 论文详细总结（自动生成）

# 论文总结：在人类大脑解码韵律意义之前，能够隐性且快速区分AI与人类语音  

---

## 一、核心问题与研究背景  

- **研究动机**：  
  人工智能语音（AI voice）在日常生活中频繁出现，如语音助手、导航、电话系统等。随着语音合成技术（尤其是语音克隆）的进步，AI生成语音越来越逼真，引发了公众对“人类是否还能分辨AI声音”的担忧。  
- **核心问题**：  
  行为学研究表明，听众通常声称是靠语调（intonation）和表现力（expressiveness）判断语音是否为AI生成。然而，尚不清楚大脑在时间上是如何实现这一识别的。**本研究的核心问题是：** 人类大脑区分AI和人类语音的神经过程是否依赖于语调加工，以及这种区分发生于何时。  
- **研究目标**：  
  以脑电（EEG）为工具，分析人类在无意识状态下听取AI与人类语音时的大脑反应，确定识别发生的具体时刻及对应的声学特征。

---

## 二、方法论  

### 1. 核心思想  
- 在**“语音来源判别”（human vs. AI）**与**“语调判别”（confident vs. doubtful）**之间建立时间相关的神经解码模型。  
- 通过比较两种判别时间的先后顺序，判断语调是否是区分AI语音的核心依据。  
- 使用**代表性相似性分析（Representational Similarity Analysis, RSA）**来揭示哪些声学特征驱动了大脑的神经模式分化。

### 2. 技术与分析流程  
- **多变量模式分析（MVPA）**：  
  对59通道EEG信号进行逐时点线性判别分析（LDA），计算在每毫秒级别上能否区分两类信号（AUC曲线）。  
- **代表性相似性分析（RSA）**：  
  - 构建神经RDM（不同条件下EEG时空分布差异）。  
  - 构建声学RDM（基于F0、高频能量HFE、谱包络MFCC）。  
  - 通过偏相关（partial Spearman correlation）检验声学特征独立解释神经差异的贡献。  
- **四种RSA模型对比**：  
  - M1: HFE | F0  
  - M2: MFCC | F0  
  - M3: HFE | F0 + MFCC  
  - M4: MFCC | F0 + HFE  
- 统计方法包括**基于簇的置换检验（cluster permutation test）**和多重比较FDR校正。  

---

## 三、实验设计  

### 1. 实验对象  
- 40名中国大陆普通话母语者（男女各半）。  
- 无语言、听觉或神经障碍。  

### 2. 刺激与语料  
- 来源于AI与人类说话者的共123句普通话句子。  
- 每位说话人以两种语调（自信/怀疑）朗读句子。  
- 使用**华为Celia语音系统**进行语音克隆，确保AI语音与原人声在说话人身份上一一对应。  
- 独立听众验证AI声音被感知为“较不人类化”，验证了刺激的感知有效性。  

### 3. 实验任务与流程  
- 共8个区块：前4块为人类语音、后4块为AI语音。  
- 参与者任务：将语音与说话者姓名配对（记忆任务），但未提示需判断语音来源或语调。  
- **EEG记录**：在训练阶段记录连续脑电数据。  
- **时间设计**：刺激长度约1.5–2.1秒，EEG采样率500 Hz。  

### 4. 数据分析  
- EEG预处理：带通滤波0.1–40 Hz、独立成分分析（ICA）去伪迹、基于听觉起始锁定。  
- 声学分析：通过librosa提取F0、HFE、MFCC特征。  
- 声学时间解码：随机森林分类器判断语调在时间上的可分性。

---

## 四、资源与算力  

- 文中未提及GPU或高性能计算设备，仅说明使用**MATLAB R2024b**与**Python 3.11.7**进行信号处理和机器学习分析。  
- 算法计算量相对有限（EEG信号处理 + 随机森林 + LDA），无需大规模算力。  

---

## 五、实验数量与充分性  

- **主实验**：EEG识别实验（40人 × 192刺激）。  
- **验证实验**：独立感知评分实验（48名听者）。  
- **声学控制分析**：基于F0轨迹的时间分辨分类。  
- **RSA模型比较**：4种声学模型组合 × 统计对比。  
- 实验层次完整，控制了说话人身份（通过AI克隆）与注意方向（任务无关）；总样本及试次数量达到神经科学常用标准。  
- 数据公开（OSF链接），透明性良好。  

---

## 六、主要结论与发现  

1. **大脑可在极短时间内（134–176毫秒）区分AI与人类语音**，此时尚未形成语调认知。  
2. **语调判别显著滞后**：仅在~1.3–2.0秒后（接近话语结束时）出现可分解活动。  
3. **语调信息需要整句整合**：声学分类显示语调差异只在语音末端（90%时长）变得可分。  
4. **神经区分的关键声学基础为谱包络（MFCC）而非高频能量**，表明大脑依赖更深层的声学特征。  
5. 语音来源解码时间（~150 ms）紧随MFCC独立贡献时间（~228 ms），暗示两者密切相关。  
6. 结论：人类大脑**隐性且自动**地识别AI声音，**并非依赖语调特征**，听众之所以报告因“语调不自然”识别AI系事后归因。  

---

## 七、研究优点  

- **实验控制严格**：  
  通过语音克隆消除了说话人身份差异，是首次在AI语音研究中严格匹配人声身份的设计。  
- **神经时间分辨率高**：  
  毫秒级EEG与MVPA结合，揭示识别发生在极早期神经加工阶段。  
- **声学–神经耦合分析新颖**：  
  RSA模型比较明确指出MFCC是最有解释力的声学特征。  
- **任务无关、反射性加工**：  
  参与者并未主动判断语音来源，确保捕获的是隐性处理。  
- **数据与代码开源**：  
  提升研究可复现性。  

---

## 八、不足与局限  

- **语言与样本范围有限**：  
  仅测试普通话母语者，结果需在其他语言背景下验证。  
- **语调刺激类型单一**：  
  仅包含“自信 / 怀疑”两类语调，未测试其他更自然的风格如愉快、悲伤或单调。  
- **区块顺序固定（人类→AI）**：  
  可能引入顺序效应或熟悉度偏差。  
- **未量化AI系统特性差异**：  
  研究仅使用单一语音引擎（Celia），不能代表所有AI语音系统。  
- **生理解释尚待拓展**：  
  EEG揭示了时序但缺乏明确脑区定位；尚不能确定哪一脑区实现初期识别。  
- **算力与重现性局限**：  
  未报告硬件资源与分析效率，外部复制需要重建同样的软件环境。  

---

**（完）**
