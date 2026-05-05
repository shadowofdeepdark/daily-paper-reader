---
title: The language network responds robustly to sentences across diverse tasks
title_zh: 语言网络在多样任务中对句子的强烈响应
authors: "Gao, R., Cheung, C., Siegelman, M., Pongos, A. L. A., Kean, H. H., Tanner, A., Fedorenko, E., Ivanova, A. A."
date: 2026-04-27
pdf: "https://www.biorxiv.org/content/10.64898/2025.12.02.691902v2.full.pdf"
tags: ["query:profile-1"]
score: 9.0
evidence: 检查包括深度语义参与在内的多种任务中对句子的神经反应
tldr: 本研究探讨语言网络在不同任务情境下对句子的稳定响应，比较其与通用多需求（MD）网络的任务敏感性。通过六种阅读任务的fMRI实验，发现语言网络在任务变化下仍能稳定地响应语言刺激，表明语言加工具有任务独立性，而MD网络主要响应任务需求。
source: biorxiv
selection_source: fresh_fetch
motivation: 研究旨在了解语言网络在语言处理中的任务稳定性及其与多需求网络的功能差异。
method: 研究采用fMRI测量52名参与者在六种阅读任务中对句子与非词的脑区反应。
result: 结果显示语言网络在所有任务中对句子反应强烈且稳定，而MD网络在任务存在时对语言和非语言刺激均有反应。
conclusion: 语言网络在不同任务中稳定响应语言输入，而MD网络则主要反映任务驱动的认知过程。
---

## 摘要
左额叶和颞叶脑区组成的网络支持语言理解与产生，执行与词汇提取及组合性语言加工相关的计算。本文探讨：语言网络对语言刺激的反应在不同任务情境中有多稳定，以及这种稳定性与一般域多需求（MD）网络的任务敏感性相比如何？52 名被试在六种任务条件下阅读句子和非词列表，包括被动阅读、阅读后进行记忆检测以及需要深层语义参与的阅读问答任务。句子>非词的对比在所有任务中均隔离出同一组语言响应体素；这些体素的位置因个体而异，彰显了个体特异性功能定位的价值。因此，我们认为语言定位对任务变化具有稳健性。随后，我们进一步分析这些语言响应体素（语言网络）以及一般域 MD 网络的响应强度和精细激活模式，以检验任务要求是否调制语言计算或招募不同的脑系统。语言网络在所有任务中对句子均表现出强劲的响应，并在语义参与更深的任务中响应略高。相较之下，MD 网络在存在任务情况下对句子和非词均有响应，这提示在使用包含任务要求的语言范式时需谨慎，因为此类范式会同时激活两个独立网络。多变量分析进一步表明，语言网络中更容易解码刺激信息，而 MD 网络中更容易解码任务信息。结果表明，语言网络与 MD 网络在任务驱动的语言理解过程中发挥互补作用：语言网络主要提取语言输入中的信息，而 MD 网络则决定与任务相关的适当响应。

## Abstract
A network of left frontal and temporal brain areas supports language comprehension and production, implementing computations related to word retrieval and combinatorial linguistic processing. Here, we ask: to what extent are responses to language in this language network stable across task contexts, and how does this stability compare to task sensitivity in the domain-general multiple demand (MD) network? Participants (n=52) read sentences and nonword lists under six task conditions, including passive reading, reading with a memory probe after each stimulus, and reading and answering questions that require deep semantic engagement. The sentences>nonwords contrast isolated the same set of language-responsive voxels across all tasks; the locations of those voxels were participant-specific, highlighting the value of individual-specific functional localization. We therefore conclude that language localization is robust to task variation. We then examined the magnitudes and fine-grained activation patterns in these language-responsive voxels (the language network) and in the domain-general MD network, to test whether task demands modulate linguistic computations and/or recruit a distinct brain system. The language network responded robustly to sentences across all tasks, with somewhat higher responses to semantically engaging tasks. In contrast, the MD network responded to both sentences and nonwords in the presence of a task, which warrants caution when using language paradigms that include task demands, as such paradigms engage two independent networks. A multivariate analysis further revealed that stimulus information is more easily decodable in the language network, whereas task information is more decodable in the MD network. These results suggest that the language and MD networks perform complementary functions during task-driven language comprehension, with the language network primarily extracting information from linguistic input and the MD network determining the appropriate response to the task.

---

## 论文详细总结（自动生成）

## 一、核心问题与研究背景

- **研究动机**：人脑中的“语言网络”（主要分布于左额叶和颞叶）负责语言理解与生成，但过去研究多忽略任务情境对语言网络活动的影响。  
- **核心问题**：语言网络在不同任务条件下（被动阅读、记忆检测、语义判断等）对语言刺激的反应是否稳定？其稳定性与域通用的“多需求网络（MD network）”相比如何？  
- **理论意义**：通过探讨语言网络的任务独立性，可以更好地理解它在大脑层级中的位置——是像感知区那样稳定响应刺激，还是像认知控制区那样受任务强烈调制。  
- **实践意义**：评估语言网络功能定位方法的鲁棒性，确保脑成像语言实验不被任务因素混淆。

---

## 二、方法论与技术路线

### 1. 核心思想
- 对比“句子 vs. 非词列表”这一经典语言刺激对比，在不同任务情境下观察其稳定性。  
- 同时对比“语言网络”与“多需求（MD）网络”的活动模式，评估任务敏感性与刺激敏感性。

### 2. 技术关键点
- **fMRI 数据获取与分析框架**：使用个体化功能区（fROI）定义方法——Group-Constrained Subject-Specific (GSS) 方法，保证参与者层面的空间一致性。  
- **实验建模**：采用一般线性模型（GLM）分析各任务条件的血氧变化（BOLD 信号），并通过跨任务交叉验证确保独立性。  
- **空间重叠分析**：通过 Dice 系数评估不同任务下语言区域的空间一致性。  
- **多变量模式分析（MVPA）**：使用线性分类器（如 SVM、kNN、相关分类器等）进行语义内容与任务类型的解码测试。  
- **统计工具**：基于混合效应模型（R 的 lmerTest 包）进行全脑区域比较，控制个体与区域的随机效应。

---

## 三、实验设计与对比方案

### 1. 数据与场景
- **被试**：52 名成年英语母语者（MIT及周边地区）。  
- **刺激材料**：  
  - 句子：取自英语语言语料库（Brown Corpus）。  
  - 非词列表：使用 Wuggy 软件将单词转化为可发音的伪词。  
- **任务版本（共六种）**：  
  1. **V1**：被动阅读 + 按钮检测图标。  
  2. **V2**：困难记忆检测（任意单词匹配）。  
  3. **V3**：简单记忆检测（最后一个单词匹配）。  
  4. **V4**：问答配对 + 按钮检测。  
  5. **V5**：阅读后回答理解问题（Yes/No）。  
  6. **V6**：语义情感判断（积极/消极）。  
- **控制条件**：非词列表使用统一的困难记忆检测任务以匹配认知负荷。  
- **额外任务**：空间工作记忆任务用于定位 MD 网络。

### 2. 对比与Benchmark
- 对比维度：
  - **语言网络 vs. MD 网络**；
  - **不同任务之间（V1–V6）**；
  - **句子 vs. 非词**；
- 无外部Benchmark模型（研究为神经实验性质），但参考了经典语言定位范式（Fedorenko et al., 2010）。

---

## 四、资源与算力

- 文中未涉及任何 GPU 或计算硬件的使用细节。  
- 算力信息有限，仅说明在 MIT 进行 fMRI 数据采集与分析，使用 SPM12、CONN 模块和定制 MATLAB/R 脚本。  
- 无训练或计算时长描述——本研究基于神经影像数据分析而非模型训练。

---

## 五、实验数量与充分性

- **主要实验集**：52名被试 × 六种任务版本（共472个实验运行），其中少量因准确率等因素被剔除。  
- **补充实验**：
  - 行为准确率与反应时分析。  
  - 多任务空间重叠与空间相关性。
  - 多变量解码（21名完成所有关键任务的被试）。  
- **实验充分性**：任务覆盖广（从被动到高语义参与），样本量较大（超过以往语言任务标准），分析维度多（空间重叠、响应幅度、模式相似性、解码准确率），结论稳健。  
- **公平性**：所有比较均在同一被试组内完成，控制了个体差异，对比设计合理。

---

## 六、主要结论与发现

1. **语言网络的任务稳健性**  
   - 在所有六种任务中均表现出显著的“句子 > 非词”效应。  
   - 同一被试不同任务下语言区空间位置高度重合（平均 Dice 系数 0.50），说明定位方法可靠。  

2. **语言网络与任务的关系**  
   - 高认知负荷（如语义判断任务）时语言区响应略增强，但核心选择性（句子>非词）不变。  
   - 表明语言网络主要受语言输入驱动，而非任务操作驱动。

3. **MD 网络的任务依赖性强**  
   - 在所有含任务的条件中，MD 网络对语言和非语言刺激均有明显反应。  
   - 任务难度（准确率下降）显著预测MD区域激活。  
   - 说明MD网络主要承担与任务控制或工作记忆相关的域通用计算。

4. **多变量解码结果**  
   - 在语言网络中，**刺激类型（句子 vs. 非词）**更易被解码。  
   - 在MD网络中，**任务类型**更易被解码。  
   - 两者功能互补：语言网络编码语言内容，MD网络编码任务信息。

---

## 七、研究优点

- **系统性设计**：首次在同一组被试中系统比较六类语言任务，排除跨实验差异。  
- **个体级分析**：采用个体化功能定位（fROI-GSS），避免群体平均带来的空间误差。  
- **多层次分析**：结合单变量、空间模式、多变量解码，验证结果稳定。  
- **理论拓展**：使语言网络在大脑层级中的性质更明确——更接近感知系统而非任务驱动系统。

---

## 八、不足与局限

- **实验任务范围有限**：仅覆盖句子级阅读与简单问答，未探讨语篇、推理或社会语用加工。  
- **样本群体单一**：为年轻、健康的英语母语者，结果泛化到儿童、老年人或多语言人群仍需验证。  
- **任务与刺激不可完全分离**：复杂任务可能诱发额外语言复述或重处理，从而混淆任务效应与语言效应。  
- **算力与动态成像精度受限**：所用标准fMRI时序分辨率较低，难以捕捉快速语言神经动态。

---

**（完）**
