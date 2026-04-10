---
title: Human brains implicitly and rapidly distinguish AI from human voices before decoding prosodic meaning
title_zh: 在人类解码韵律意义之前，大脑会以隐式且快速的方式区分人工智能与人类声音
authors: "Chen, W., Pell, M., Jiang, X."
date: 2026-04-09
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.08.716483v1.full.pdf"
tags: ["query:q8"]
score: 9.0
evidence: 区分人类与AI语音中的韵律线索和脑电图
tldr: 本研究利用EEG和语音克隆技术探究人类大脑区分AI声音与人类声音的神经时间过程，发现这种区分发生得极快，早于语调的理解，说明听觉系统能在语义处理之前自动识别声音来源。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-08-716483-v1/fig-001.webp\", \"caption\": \"Figure 2. Validation of training stimuli. (A) Mean F0 comparison between AI and human voices in two prosodies. Connecting lines link matched audio pairs (same prosody, statement, speaker). (B) Perceptual ratings of humanlikeness and vocal confidence (1-7 scale; error bars: SE). (C) Machine learning classification of confident vs. doubtful prosody at 5% intervals (5- 100% normalized duration). Filled markers indicate FDR-corrected significance (p < 0.05).\", \"page\": 15, \"index\": 1, \"width\": 892, \"height\": 627}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-08-716483-v1/fig-002.webp\", \"caption\": \"Figure 4. Partial RSA: Independent Acoustic Contributions to Neural Voice Source Structure. Partial Spearman correlations between neural and acoustic RDMs (N = 40, 2 ms resolution, 0–1500 ms). Each panel shows mean partial r (±1 SEM, shaded) after controlling for the specified features. Bottom colored bars: significant clusters vs. 0 (one-sided cluster permutation, p < .05); onset latencies annotated with downward arrows. Top bars: significant between-model differences (two-sided, p < .05); onset latencies annotated with upward arrows. Gray shading: MVPA source decoding onset (134–176 ms). Dashed line: mean stimulus duration (1559 ms). HFE = high-frequency energy (>4 kHz); MFCC = melfrequency cepstral coefficients.\", \"page\": 18, \"index\": 2, \"width\": 892, \"height\": 400}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-08-716483-v1/fig-003.webp\", \"caption\": \"Figure 1. Experimental Design and Analysis Pipeline. (A) Speaker identity learning task across 8 blocks (4 Human, 4 AI), each comprising a Training phase (24 trials; EEG recorded) and a Checking phase (12 trials). (B) MVPA was applied to EEG patterns (59 channels) from the Training phase to decode voice source (Human vs. AI) at each timepoint using linear discriminant analysis, yielding temporal decoding curves (AUC) and time generalization matrices. (C) Partial RSA compared neural RDMs (4×4, correlation distance; 2 ms resolution, 0–1500 ms) with acoustic feature RDMs (F0, HFE, MFCC). Four models assessed independent contributions of HFE and MFCC controlling for F0 and each other (M1: HFE|F0; M2: MFCC|F0; M3: HFE|F0+MFCC; M4: MFCC|F0+HFE). Schematic time courses illustrate the expected pattern of results.\", \"page\": 8, \"index\": 3, \"width\": 892, \"height\": 831}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-08-716483-v1/fig-004.webp\", \"caption\": \"Figure 3. Mel spectrograms and temporal decoding of voice source and prosody. (A-D) Spectrograms of an exemplar sentence across conditions. (E-H) Time-generalization matrices (TGM) showing decoding performance. (I-J) Temporal decoding curves. Shaded areas: SE. Colored bars: significant clusters (p < 0.05, cluster-based permutation). Dashed lines: mean (1559 ms) and maximum (2103 ms) stimulus duration.\", \"page\": 16, \"index\": 4, \"width\": 892, \"height\": 462}]"
motivation: 人们常通过语调判断声音真伪，但尚不清楚这种判断是否驱动大脑区分AI与人类声音。
method: 研究者通过EEG记录被试听人类与AI声音的反应，并用多变量模式分析检测脑信号差异。
result: EEG数据显示，参与者在约134-176毫秒内即可区分AI与人类声音，这种区分远早于对语调的识别。
conclusion: 大脑对AI与人类声音的快速区分说明语调并非决定性因素，而是后期整合的结果。
---

## 摘要
人们每天都会接触到人工智能（AI）生成的语音。现有的行为研究表明，听众依赖如语调和表现力等韵律线索来识别音频深度伪造，并报告称AI语音在韵律上比人类语音更缺乏丰富性。为检验在语音加工的神经时间进程中，韵律加工是否驱动深度伪造的辨识，我们记录了被试在聆听人类与AI生成的说话者以自信与怀疑两种韵律（语气）发声时的脑电（EEG）数据，并要求他们注意记忆说话者姓名。我们使用语音克隆技术控制人类与AI语音之间的说话者身份混杂因素。多变量模式分析（MVPA）结果显示，无论韵律类型如何，大脑对人类与AI语音的神经区分都快速出现（自信语气：176毫秒；怀疑语气：134毫秒），明显早于韵律识别阶段（在人类语音中区分自信与怀疑：2066毫秒；在AI语音中：1366毫秒）。声学分析进一步表明，韵律差异仅在语句结束时（归一化时长的90%）才能被分类，这与神经证据一致，表明韵律加工需要几乎完整的时间整合。这种快速的语音来源区分与较晚出现的韵律解码之间的时间分离，暗示韵律在音频深度伪造检测中所起的作用比听众事后报告的要小。表征相似性分析（RSA）进一步揭示，驱动人类与AI语音神经区分的，是谱包络特征（mel频率倒谱系数，MFCC），而非视觉上更显著的高频能量差异。MFCC的最早独立贡献（228毫秒）紧随MVPA解码起点（134–176毫秒）之后。未来的研究可操控特定声学成分，以确定这种快速且持续的神经区分的因果来源。

## Abstract
People encounter AI voices daily. Existing behavioral studies suggest listeners rely on prosodic cues such as intonation and expressiveness to detect audio deepfakes, reporting that AI voices sound prosodically less rich than human voices. To test whether prosodic processing drives deepfake discrimination in the neural time course of voice processing, we recorded electroencephalographic (EEG) data while participants listened to human and AI-generated speakers producing utterances in confident vs. doubtful prosody (tone of voice), with attention directed toward memorizing speaker names. We used voice cloning to control for speaker identity confounds between human and AI voices. Multivariate pattern analysis revealed that neural discrimination of human vs. AI voices emerged rapidly regardless of prosody (confident: 176 ms; doubtful: 134 ms), substantially preceding prosody discrimination (confident vs. doubtful within human voices: 2066 ms; within AI voices: 1366 ms). Acoustic analysis confirmed that prosodic distinctions became classifiable only at utterance offset (90% normalized duration), converging with neural evidence that prosody requires near-complete temporal integration. This temporal dissociation between rapid voice source discrimination and late-emerging prosody decoding suggests that prosody plays a smaller role in audio deepfake detection than listeners retrospectively report. Representational similarity analysis further revealed that spectral envelope features (mel-frequency cepstral coefficients; MFCC), rather than the visually salient high-frequency energy differences, drove neural human-AI discrimination, with MFCC's earliest independent contribution (228 ms) closely following the MVPA decoding onset (134-176 ms). Future studies may manipulate specific acoustic components to establish the causal sources of this rapid and sustained neural discrimination.

---

## 论文详细总结（自动生成）

# 在人类解码韵律意义之前，大脑会以隐式且快速的方式区分人工智能与人类声音  

---

## 一、研究背景与核心问题

- **核心问题**：人类如何在神经层面区分人工智能（AI）生成的语音与人类真实语音？这种区分是否依赖语调（韵律）特征？  
- **研究动机**：随着语音合成与深度伪造技术广泛应用，人们在日常生活中不断接触AI声音（电话提示、导航语音、客服机器人等），但行为层面研究显示听众往往认为“AI声调较单一”“表现力不足”。作者希望弄清这一感知差异是否真的是大脑区分AI声音的依据，还是一种**事后归因**。  
- **整体含义**：通过神经时间过程（EEG）分析发现，人类大脑能在语义和韵律理解之前**自动、迅速区分语音来源**，说明听觉系统内部存在“来源识别”的早期通道，而这种能力不依赖意识注意。

---

## 二、方法论与技术流程

### 核心思想
- 运用**隐式脑电解码范式**检测人类聆听语音时的自动加工过程，而非让被试显性判断“是不是AI声音”。
- 将人类与AI语音对齐为同一说话者身份（通过语音克隆），排除个体声纹差异的影响，确保任何差异都能归因于**声音来源（source）**。

### 技术与算法流程
1. **语音数据准备**：
   - 使用 Huawei Celia 系统进行语音克隆。
   - 生成自信（confident）与怀疑（doubtful）两种韵律的语音样本。
2. **EEG数据采集**：
   - 64通道EEG（Brain Products ActiCap系统），采样率500 Hz。
   - 记录被试在**“记忆说话者姓名任务”**中的脑电活动，语音来源与韵律均为非任务相关特征。
3. **数据处理**：
   - 使用 EEGLAB 进行预处理与独立成分分析（ICA）。
   - 去除眼动、肌肉伪迹，低通滤波（30 Hz）。
4. **多变量模式分析（MVPA）**：
   - 采用线性判别分析（LDA）对每个时间点的脑电进行分类。
   - 解码目标：①人类 vs. AI 语音；②自信 vs. 怀疑语调。
   - 输出指标：AUC（area under curve）。
5. **表征相似性分析（RSA）**：
   - 构建声学特征模型（F0、HFE >4kHz、MFCC）。
   - 建立神经表征矩阵（neural RDM，4×4）。
   - 使用**偏相关分析（partial Spearman correlation）**探测各声学特征与神经模式的独立关联。

---

## 三、实验设计与数据集

- **受试者**：40名普通大学生（男女各半），均为普通话母语者，无神经或听觉障碍。  
- **语料**：192条语音刺激，来自24名说话者。每名说话者均录制人类版与AI克隆版语音。  
- **韵律条件**：自信 vs. 怀疑，每个说话者均对应两种版本。  
- **实验任务**：说话者姓名记忆学习（Training阶段记录EEG），随后进行选择测试（Checking阶段验证注意力水平）。  
- **对比**：  
  - 对比维度一：**声音来源（Human vs. AI）**  
  - 对比维度二：**韵律类型（Confident vs. Doubtful）**  
- **评价指标**：  
  - 行为层面：识记准确率（平均94.2%，确认被试专注）。  
  - 声学层面：F0均值、感知人类性与自信度评分。  
  - 神经层面：AUC解码曲线、RSA相关系数分布。

---

## 四、资源与算力使用

- 文中**未提及GPU或算力配置**。  
- 语音处理与机器学习部分使用 Python（librosa、scikit-learn）与 MATLAB（MVPA-Light、EEGLAB）。  
- 由于为非深度学习实验，主要依赖 CPU 数据处理和统计分析；未出现训练模型计算量描述。

---

## 五、实验数量与充分性评估

- **实验数量**：
  - 192条语音刺激 × 40名被试，共约7443个有效脑电试次。
  - 多维度解码（4条件 × 时间点 × 声学模型）。
  - 包括多轮 MVPA 与 RSA 对照实验，共呈现十余个显著时窗。
- **实验充分性**：
  - 控制人类-说话者匹配与韵律对称非常严格。
  - 包含行为验证、声学分析、脑电时间过程三重证据。
- **公平性**：
  - 声音强度、句子长度、音高等被系统平衡；被试性别均衡。
  - 分析使用基于聚类的置换检验控制假阳性风险（Maris & Oostenveld, 2007）。

---

## 六、主要结论与发现

1. **快速神经区分**：  
   - 人类大脑在听到语音约 **134–176毫秒** 就能自动区分 AI 与人类声音。  
   - 该时间窗口远早于韵律（语调）解码阶段（约 **1366–2066毫秒**）。  
2. **韵律非决定性因素**：  
   - 韵律差异仅在语句接近结束（时长的90%）才可声学分类。  
   - 大脑对语音来源的敏感度并不依赖语调丰富度。  
3. **声学驱动机制**：  
   - 虽视觉上高频能量差异较明显，但真正与神经区分相关的是**谱包络特征（MFCC）**。  
   - MFCC在约 **228毫秒** 出现独立神经贡献，与快速区分时间紧密相邻。  
4. **社会认知含义**：人们自认为依靠语调识别AI声音的策略，其实是**事后解释**，而大脑早已在潜意识中完成区分。

---

## 七、优点与亮点

- **跨层验证设计**：行为 + 声学 + 神经证据三者互相印证。  
- **语音克隆匹配**：在人类与AI模型间精确控制说话者身份，极大减少混杂。  
- **隐式任务范式**：避免被试的主观判断干扰，揭示真实的早期神经加工机制。  
- **高时间分辨率分析**：EEG的毫秒级解析配合MVPA，实现动态认知过程追踪。  
- **创新性结论**：首次明确证实“大脑能在韵律理解前区分AI语音”，具有社会与技术双重意义。

---

## 八、不足与局限

- **语言与样本局限**：仅使用普通话语音，尚未验证多语言或非母语听者的普适性。  
- **任务顺序固定**：人类语音始终在前、AI语音在后，可能存在学习顺序偏差。  
- **韵律范围有限**：仅研究“自信 vs. 怀疑”情绪维度，未包含更丰富的情感或表现性语调。  
- **声学因果不明**：MFCC仅为复合特征，尚未解析具体哪个声学维度驱动区分。  
- **外部生态效度**：实验室条件与真实交互环境（电话、语音助手）仍有差距。  

---

（完）
