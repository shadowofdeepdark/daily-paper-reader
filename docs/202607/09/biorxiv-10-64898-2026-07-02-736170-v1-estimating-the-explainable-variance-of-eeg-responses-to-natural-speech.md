---
title: Estimating the Explainable Variance of EEG Responses to Natural Speech
title_zh: 自然语音 EEG 响应中可解释变异的估计
authors: "Dou, J., Lalor, E."
date: 2026-07-03
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.02.736170v1.full.pdf"
tags: ["query:profile-1"]
score: 8.5
evidence: 脑电对自然语言及语言特征的反应
tldr: 本文研究自然语音条件下EEG脑响应中可被语音输入解释的方差上限问题。作者基于19名受试者聆听同一有声读物时的EEG数据，利用跨被试建模、维度约简和外推方法估计可解释方差，并将其与基于声学和语言特征的线性时序响应函数模型进行比较。结果表明，现有语音特征模型已能解释大部分EEG响应，但仍存在未被捕获的可解释脑活动信息。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-736170-v1/fig-001.webp\", \"caption\": \"Figure 1 Estimating the explainable variance in EEG responses to natural speech using inter-subject modeling. A 19 native speakers of English listened to the same audiobook while their (128-channel) EEG was recorded. One of these subjects was chosen as the target subject. A subset of the other subjects were source subjects (in the figure we show a case with all the other subjects as the source subjects). Multiway canonical correlation analysis was used to reduce the 128 channel EEG to 3 components for each source subject that were maximally correlated with those of all the other source subjects. A temporal response function was then fit that aimed to\", \"page\": 7, \"index\": 1, \"width\": 902, \"height\": 962}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-736170-v1/fig-002.webp\", \"caption\": \"Figure 4: The explainable variance in EEG responses to natural speech aggregated across subjects and channels. Each dot represents the accuracy of decoding one target subject’s EEG from a group of source subjects’ EEG. Greycolored lines indicate curves fitted during each iteration of hierarchical bootstrapping. The dashed line indicates the median of the fitted curves during hierarchical bootstrapping. The blue horizontal line indicates the speech-EEG model’s prediction accuracy averaged across subjects. The dotted horizontal line indicates the median of the estimated explainable variance aggregated across all subjects and channels.\", \"page\": 18, \"index\": 2, \"width\": 902, \"height\": 452}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-736170-v1/fig-003.webp\", \"caption\": \"Figure 5 Estimated noise ceiling cannot be fully explained by the speech-to-EEG model. Left: The median of the confidence interval of the group-level channel-wise noise ceiling. Middle: The lower bound of the confidence interval of the group-level channel-wise noise ceiling. Right: The estimated noise ceiling minus the speech-toEEG prediction accuracy. Channels with significant positive differences are labeled with white dots.\", \"page\": 19, \"index\": 3, \"width\": 892, \"height\": 244}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-736170-v1/fig-004.webp\", \"caption\": \"Figure 3 The prediction accuracy of speech-to-EEG TRF.\", \"page\": 17, \"index\": 4, \"width\": 458, \"height\": 348}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-736170-v1/fig-005.webp\", \"caption\": \"Figure 2 Simulations showing that temporal response functions can be used to model one EEG timeseries based on another EEG timeseries, even when those\", \"page\": 16, \"index\": 5, \"width\": 810, \"height\": 760}]"
motivation: 已有大量研究使用语音声学和语言特征建模EEG脑响应，但尚不清楚自然语音条件下EEG信号中究竟有多少方差是可由语音输入解释的。
method: 研究利用19名受试者在收听同一有声读物时的EEG数据，构建跨被试预测模型并通过维度约简与外推方法估计EEG响应中的总可解释方差。
result: 跨被试EEG模型可有效估计自然语音诱发EEG中的可解释方差，且基于时序响应函数的常见语音特征模型能够解释其中大部分但并非全部方差。
conclusion: 自然语音驱动的EEG响应存在可估计的可解释方差上限，而现有基于声学与语言特征的线性模型虽已能解释大部分脑响应，但仍无法完全覆盖全部可解释信息。
---

## 摘要
近年来，人们在理解人脑如何解析和处理自然语音方面取得了显著进展。这些进展很大程度上依赖于对脑活动与语音不同声学和语言学特征之间关系的建模。通过拟合和测试基于这些特征的模型，可以检验关于大脑将语音声音转化为理解过程中所使用的计算机制与表征形式的假设。尽管大量研究集中于利用功能性神经影像或颅内电生理信号对 BOLD 活动进行建模，但这种方法同样已被证明适用于 MEG 和 EEG。事实上，在语音处理研究的转化研究与应用方面，非侵入式 EEG 具有一定优势。过去十余年的研究表明，EEG 可以基于众多声学、语言学及副语言学语音特征进行成功建模。然而，一个重要且尚未解决的问题始终存在于这些研究之中：究竟什么样的模型才算是自然语音 EEG 响应的优秀模型？换言之，在自然语音聆听过程中记录到的 EEG 变异中，有多少是可以解释为来源于语音输入的？本研究旨在解决这一问题。我们基于如下假设展开研究：对于某个人的自然语音 EEG 响应而言，最佳模型应当是一组来自其他聆听相同语音个体的 EEG 响应。在这一假设下，我们利用 19 名健康成年英语母语者在聆听同一本有声读物时采集的 EEG 数据构建被试间模型。针对每位被试，模型通过使用来自不同数量其他被试的（降维后的）EEG 数据来预测其 EEG 数据，并进一步外推估计目标个体对语音响应中的总可解释变异。随后，我们表明，基于若干常用声学和语言学语音特征的线性模型（时间响应函数）能够预测跨被试 EEG 响应中估计总可解释变异的大部分——但重要的是，并不能预测其全部。

## Abstract
Substantial progress has been made in recent years on understanding how the human brain parses and processes natural speech. Much of this progress has been based on modeling how brain activity relates to the different acoustic and linguistic features of speech. By fitting and testing models based on those features, one can test hypotheses about the kinds of computations and representations the brain uses to convert speech sounds into understanding. While much of this work has focused on modeling BOLD activity using functional neuroimaging or intracranially recorded electrophysiological signals, the approach has also proven useful with MEG and EEG. Indeed, noninvasive EEG has certain advantages for studying speech processing in terms of translational research and application. Research over the last decade or so has shown that EEG can be successfully modeled based on numerous acoustic, linguistic, and paralinguistic speech features. However, an important unanswered question hangs over all of this work: namely, what constitutes a good model of EEG responses to natural speech? Or, to put it another way, how much variance in EEG recorded during natural speech listening is explainable as having derived from that speech input? The present study aims to tackle this issue. We do so under the assumption that the best model for a persons EEG response to natural speech is a set of EEG responses from other people listening to the same speech. Using this assumption, we construct inter-subject models using EEG from 19 healthy adult native speakers of English who all listened to the same audiobook. The model for each subject involves predicting their EEG data using (dimensionality-reduced) EEG from different numbers of other subjects and then extrapolating to estimate the total explainable variance in the target individuals response to speech. Following this, we show that linear models (temporal response functions) based on several commonly used acoustic and linguistic speech features can predict most - but importantly not all - of the estimated total explainable variance in EEG responses across subjects.

---

## 论文详细总结（自动生成）

# 论文总结：Estimating the Explainable Variance of EEG Responses to Natural Speech

## 1. 核心问题与整体含义（研究动机与背景）

这篇论文关注一个在“自然语音 EEG 建模”领域长期存在但缺少明确答案的问题：

> 在人类聆听自然语音时，EEG 信号中究竟有多少方差是真正由语音输入驱动、因此“可以被解释”的？

过去大量研究已经能够利用：
- 声学特征（如 speech envelope）
- 语言学特征（如 lexical surprisal）
- 更高层语言表示

去预测 EEG/MEG/fMRI 对自然语音的响应。

但这些研究一直缺少一个“上限”概念：
- 当前模型到底已经解释了多少真正与语音相关的脑活动？
- 模型预测效果低，是模型不好，还是 EEG 本身信噪比太低？
- 还剩多少“可解释脑活动”尚未被建模？

作者将这个问题定义为：
- EEG responses to speech 的 explainable variance
- 即 EEG 中由语音刺激所驱动、理论上可以被模型解释的部分
- 类似神经科学中的 noise ceiling（噪声上限）

传统估计 explainable variance 的方法通常依赖：
- 同一刺激重复呈现
- 比较重复试次之间脑活动一致性

但作者指出：
- 自然语言刺激重复后会改变语言预测性、注意力和语义加工
- 因此不适用于自然语音理解研究

于是论文提出：
- 用“其他听同一故事的人”的 EEG 来预测目标被试 EEG
- 并通过跨被试外推估计无限被试情况下的可解释方差

这是本文的核心贡献。

---

# 2. 方法论

## 2.1 核心思想

论文建立如下假设：

> 对一个人的自然语音 EEG 最好的模型，是其他人在听相同语音时的 EEG。

方法总体流程：

1. 多个 source subjects 听同一语音
2. 用 source EEG 预测 target EEG
3. 随着 source subjects 数量增加，预测能力提高
4. 拟合“被试数量 → 预测准确率”的增长曲线
5. 外推到“无限被试”
6. 得到 target EEG 的 explainable variance（noise ceiling）

---

## 2.2 方法结构

整体模型：

```text
Source EEG
   ↓
MCCA 降维
   ↓
TRF 时滞回归
   ↓
预测 Target EEG
   ↓
不同人数外推
   ↓
估计 Explainable Variance
```

---

## 2.3 为什么不能直接跨被试平均 EEG

作者指出 EEG 有两个核心问题：

### （1）空间分布差异

不同人：
- 头骨厚度不同
- cortical folding 不同
- electrode projection 不同

导致：
- 同一脑活动在 scalp 上空间分布不同

因此不能直接：
- channel-by-channel averaging

---

### （2）时间响应差异

不同人：
- ERP latency 不同
- response morphology 不同

因此：
- 即便响应同一语音
- 时间结构也不一致

---

## 2.4 MCCA（Multi-way Canonical Correlation Analysis）

为解决空间差异，作者使用：

### 多路典型相关分析（MCCA）

目的：
- 从多个被试 EEG 中提取“共享成分”
- 保留跨被试一致的 speech-related EEG

具体做法：
- 128 channels → 3 canonical components

特点：
- 最大化多个被试之间相关性
- 比 PCA 更适合提取共享神经活动

作者还加入：
- ±2 samples 的 temporal shifts
- 允许不同被试之间存在约 ±31ms latency 偏差

最终：
- 每个 source subject 只保留 3 个 canonical components

这是重要的降维步骤。

---

## 2.5 TRF（Temporal Response Function）

随后作者使用：

### Ridge Regression TRF

建立：

```text
(source MCCA components with time lags)
                ↓
          target EEG
```

时间窗：
- -400 ms 到 +400 ms

作用：
- 允许 source 与 target EEG 存在时间形态差异
- 本质上是时间卷积线性模型

形式：

\[
\hat r(t)=\sum_\tau h(\tau)s(t-\tau)+b
\]

其中：
- s：source MCCA 成分
- h：TRF 权重
- r：target EEG

通过 ridge regression 求解。

---

## 2.6 Explainable Variance 的外推

作者重复如下过程：

- 使用 1 个 source subject
- 使用 2 个 source subjects
- ...
- 使用 18 个 source subjects

得到：

```text
source人数 → EEG预测准确率
```

随后拟合指数曲线：

\[
f(x)=v_0(1-e^{-x/\tau_0})
\]

其中：
- x：source 数量
- v₀：无限被试时的极限值
- v₀ 被定义为 explainable variance

这是全文最核心的数学定义。

---

## 2.7 Benchmark Speech-to-EEG 模型

作者使用经典 speech feature TRF 作为 benchmark。

包含三个特征：

### （1）Acoustic envelope

Hilbert envelope。

---

### （2）Lexical surprisal

用 GPT-2 计算：

\[
-\log P(word|context)
\]

context 最大长度：
- 1024 words

---

### （3）Word onset impulses

词开始时单位脉冲。

用于：
- 捕获额外词级时锁定活动。

---

# 3. 实验设计

## 3.1 数据集

使用公开 EEG 数据集：

Broderick et al. (2019)

数据：
- 19 名英语母语者
- 听同一本 audiobook
- 20 段自然语音
- 每段约 180s

EEG：
- 128 channels
- BioSemi ActiveTwo
- 原始采样率 512Hz
- 最终：
  - bandpass: 0.5–8 Hz
  - downsample 到 64Hz

---

## 3.2 实验任务

主要任务：

### （1）跨被试 EEG-to-EEG 预测

目标：
- 估计 explainable variance

---

### （2）Speech-to-EEG benchmark

目标：
- 测试现有 speech feature 模型能解释多少 explainable variance

---

## 3.3 对比与消融

### PCA vs MCCA

作者测试：
- PCA 降维
- MCCA 降维

结果：
- MCCA 更高效
- 用更少维度达到类似甚至更好性能

---

### TRF 时间窗模拟实验

比较：
- 窄时间窗
- 宽时间窗

结果：
- 大时间窗显著改善跨 temporal morphology 解码能力

---

## 3.4 评估指标

主要指标：
- Pearson correlation (r)

使用：
- nested 10-fold CV
- 内层调 λ
- 外层 unbiased evaluation

设计较规范。

---

# 4. 资源与算力

论文没有明确给出：
- GPU 型号
- GPU 数量
- 训练时间
- FLOPs

仅提到：

- 使用 CuPy
- 在 NVIDIA GPU 上加速
- 重写了：
  - MCCA
  - mTRFpy

说明：
- 计算量较大
- 尤其是高维 time-lag EEG regression

但没有详细硬件配置。

---

# 5. 实验数量与充分性

## 实验内容较丰富

主要包括：

### （1）模拟实验

验证：
- TRF 是否能处理 temporal morphology 差异

---

### （2）跨被试 explainable variance 实验

核心主实验。

---

### （3）group-level noise ceiling

---

### （4）channel-wise noise ceiling

---

### （5）single-subject analysis

展示：
- 正常案例
- 局部化案例
- failure case

---

### （6）PCA vs MCCA

---

### （7）bootstrap confidence interval

---

## 客观性与公平性

优点：
- nested CV
- bootstrap CI
- group + subject 两层分析
- failure cases 主动展示

但也存在限制：

- 数据集仅 19 人
- 单一 audiobook
- 单一语言（英语）
- benchmark speech features 较有限

整体而言：
- 实验设计较认真
- 统计处理规范
- 但规模偏小。

---

# 6. 主要结论与发现

## 核心发现

### （1）自然语音 EEG 的 explainable variance 可以估计

通过：
- EEG-to-EEG inter-subject modeling
- source-number extrapolation

可以得到 noise ceiling。

---

### （2）现有 speech-feature TRF 已解释大部分 variance

group-level：
- speech-EEG 平均 r ≈ 0.0507
- explainable variance 中位数 ≈ 0.0608

说明：
- 当前模型已经接近上限

---

### （3）但仍存在未解释脑活动

尤其：
- centroparietal
- right temporal regions

speech model 仍低于 noise ceiling 下界。

意味着：
- 仍有 speech-related neural activity 未被建模

---

### （4）跨被试 temporal variability 很重要

大时间窗 TRF 可显著改善 EEG-to-EEG decoding。

---

### （5）MCCA 优于 PCA

因为：
- 能提取 shared neural structure
- 更适合 inter-subject EEG

---

# 7. 优点与亮点

## 理论贡献明显

这是少见直接讨论：

> “自然语音 EEG 模型上限”的工作。

其意义很大：
- 能重新解释 EEG encoding model 的好坏
- 提供统一 benchmark

---

## 方法设计巧妙

关键创新：
- EEG-to-EEG 建模
- source subject extrapolation
- MCCA + TRF 结合

很适合 EEG 的：
- 低 SNR
- 高个体差异

---

## 统计设计规范

包括：
- nested CV
- hierarchical bootstrap
- CI estimation

方法学较扎实。

---

## 主动分析 failure cases

不是只展示成功案例。

这一点提升了可信度。

---

# 8. 不足与局限

## 数据规模较小

仅：
- 19 subjects

而 explainable variance 的外推本身依赖：
- “趋于无限被试”

因此外推稳定性有限。

---

## 单语种、单刺激

只有：
- 英语
- 单 audiobook

泛化性不明确。

---

## benchmark 不够强

speech model 仅包含：
- envelope
- lexical surprisal
- word onset

未包含：
- phoneme features
- semantic embeddings
- syntactic representations
- LLM contextual states
- nonlinear models

因此：

“现有模型尚未达到 noise ceiling”
并不意味着更先进模型做不到。

---

## 线性假设限制明显

无论：
- EEG-to-EEG
- speech-to-EEG

都依赖线性 TRF。

但脑活动显然非线性。

---

## 对弱响应被试不稳定

部分被试：
- noise ceiling 估计失败
- 或低于 speech benchmark

说明：
- 方法依赖较强 inter-subject similarity

---

## 高频 EEG 未分析

仅研究：
- 0.5–8 Hz

未涉及：
- alpha
- beta
- gamma

而这些频段也可能包含语言加工信息。

---

# 总体评价

这篇论文的重要性在于：

它首次较系统地回答了：

> “自然语音 EEG 中到底有多少是真正可解释的？”

论文提出了一套适配 EEG 特性的：
- 跨被试 noise ceiling estimation framework

并证明：
- 当前经典 speech-feature TRF 已接近但尚未达到 EEG 可解释上限。

对于：
- EEG speech neuroscience
- neural encoding
- language neuroscience
- brain benchmark evaluation

都具有较强的方法学意义。

（完）
