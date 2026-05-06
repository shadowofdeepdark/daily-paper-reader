---
title: Transformed reactivation of latent working memory enables hierarchical language processing
title_zh: 潜在工作记忆的转换性再激活使层级语言加工成为可能
authors: "Li, J., Pan, Y., Park, H., Hagoort, P., Luo, H., Jensen, O."
date: 2026-05-04
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.02.722174v1.full.pdf"
tags: ["query:profile-1"]
score: 9.0
evidence: 层次化语言加工与记忆重激活的神经机制
tldr: 本研究探讨语言理解中工作记忆的维持与提取机制。通过脑磁图追踪句子中主语在从句嵌入结构中的神经表征，发现其在从句期间静默维持并在主句动词处以变换的编码形式重现，激活由前额叶到语言区的网络，揭示静默工作记忆与结构依赖的检索机制。
source: biorxiv
selection_source: fresh_fetch
motivation: 研究旨在揭示语言处理中早期词汇保持依赖持续神经活动还是静默工作记忆机制，以及记忆提取涉及哪些脑区网络。
method: 研究使用脑磁图与时间分辨解码技术跟踪句子中主语的神经表征变化。
result: 主语表征在嵌入从句期间衰减，在主句动词出现时以变换形式重新激活，首先出现在右背外侧前额叶再扩展至语言相关区域。
conclusion: 该研究表明语言理解中存在活动静默式工作记忆维持与结构依赖的记忆提取，且域通用与语言特异性网络协同工作。
---

## 摘要
人类的语言理解需要在跨越插入材料时追踪词语，以构建语法结构。然而，两个基本问题仍未解决：早期词语的维持是依赖于持续的神经活动，还是依赖于无活动（activity-silent）的工作记忆机制；在整合过程中，记忆检索是涉及一般认知网络还是语言选择性网络。使用磁脑图（magnetoencephalography, MEG）的时间分辨解码方法，我们追踪了受试者在听带有嵌入从句的句子（例如：“The dog, who chases the cat, jumps over the mud.”）时的主句主语处理过程。主语（“dog”）的神经表征在嵌入从句期间衰减至基线，但在主句动词（“jumps”）出现后重新激活，且神经编码形式为转换的（transformed），而非简单再现的（reinstated）。关键的是，重新激活首先出现在右背外侧前额叶皮层（right dorsolateral prefrontal cortex），随后才涉及额颞语言区域，且重新激活的强度受到句法结构的调节，并可预测理解准确度。这些发现表明，层级语言加工过程中存在无活动工作记忆的维持、依赖结构的检索机制，以及一般认知网络与语言选择性网络的协作功能。

## Abstract
Human language comprehension requires tracking words across intervening material to construct grammatical structures, yet two fundamental questions remain unresolved: whether maintenance of earlier words relies on sustained neural activity or activity-silent working memory mechanisms, and whether memory retrieval during integration engages domain-general or language-selective networks. Using magnetoencephalography with time-resolved decoding, we tracked main-clause subjects as participants heard sentences with embedded clauses (e.g., "The dog, who chases the cat, jumps over the mud."). The subject representation ("dog") decayed to baseline during the embedded clause but reactivated after the main-clause verb ("jumps"), with transformed rather than reinstated neural codes. Critically, reactivation emerged first in right dorsolateral prefrontal cortex before engaging frontotemporal language regions, and reactivation strength was modulated by syntactic structure and predicted comprehension accuracy. These findings demonstrate activity-silent working memory maintenance, structure-dependent retrieval, and cooperative function of domain-general and language-selective networks during hierarchical language processing.

---

## 论文详细总结（自动生成）

# 《潜在工作记忆的转换性再激活使层级语言加工成为可能》论文总结

---

## 一、核心问题与研究背景

- **研究动机**：  
  人类语言理解需要在短时间内整合分散在句子不同部分的词语信息，形成符合语法的层级结构。然而，当句子中出现插入成分（如从句）时，早期输入的词语在被再次调用前，如何在脑中被维持和提取，是认知神经科学中的核心问题。

- **核心科学问题**：
  1. 语言中早期词语的表征是否依赖持续的神经活动，还是通过“无活动（activity-silent）工作记忆机制”被暂时存储？
  2. 当理解者需要检索和整合早期词语时，这一过程涉及的是通用认知网络（如前额叶控制系统），还是语言特异性网络（额颞语言区）？

- **整体含义**：  
  该研究揭示了语言理解中“潜在工作记忆（latent working memory）”的存在，说明人类在句法层级处理时，可以通过非持续活动的方式保持语义单元，并在需要时以不同编码形式重新激活。这为工作记忆与语言系统的交互模型提供了新证据。

---

## 二、方法论：核心思想与技术路线

- **研究思路**：  
  通过脑磁图（MEG）追踪受试者在听句子时特定词语（如主语）的神经表征变化，判断其在从句插入期间的动态模式及再激活形式。

- **关键技术步骤**：
  1. **刺激材料设计**：构造含嵌套从句的句子，例如“The dog, who chases the cat, jumps over the mud.”。
  2. **时间分辨解码（time-resolved decoding）**：在不同时间点训练分类器，用于识别特定目标词的神经表征模式。
  3. **动态表示检测**：
     - 测量主语词在从句期间的神经活动变化；
     - 在主句动词出现时检测主语表征是否重新出现；
     - 比较再激活信号与最初编码之间的向量相似性，判断是“再现（reinstated）”还是“转换（transformed）”。
  4. **脑区定位分析**：利用源定位（source reconstruction）技术确定信号起源，重点分析右背外侧前额叶（DLPFC）与额颞语言区的时序激活关系。

- **算法/统计框架**：
  - 多变量模式分析（MVPA）用于判别主语表征；
  - 时间广义解码（temporal generalization）矩阵用于可视化跨时间点的相似性；
  - 统计显著性通过置换检验与集群校正（cluster-based permutation test）完成；
  - 行为相关性：再激活强度与理解正确率之间的回归分析。

---

## 三、实验设计

- **数据来源与样本**：
  - 受试者为健康成年人；
  - 实验条件为听力理解任务，材料为英文句子；
  - 采用被试内设计，包含主句–从句结构对比。

- **对比设置**：
  - **条件变量**：句法嵌入复杂度（含/不含从句）；
  - **分析对象**：语义主语的表征强度变化；
  - **对比方法**：与基线期（无相关表征）和非目标词激活比较。

- **Benchmark 与验证**：
  - 并非传统机器学习基准，而是以“是否存在再激活信号”及“时空分布是否符合预测模型”为验证依据；
  - 比较不同脑区、不同时间窗信号强度的显著差异。

---

## 四、资源与算力

- 文中未具体说明计算资源（例如 GPU 型号、数量、运行时长）。
- 由于使用的是 MEG 数据解码分析，计算负荷主要来自神经信号处理与统计分析，而非深度学习训练，因此估计算力需求较低。

---

## 五、实验数量与充分性

- **实验数量**：
  - 单一主实验，包含若干条件（如句法复杂度差异、不同从句位置）。
  - 辅助分析包括：
    - 主语表征时间动态分析；
    - 再激活编码形式（reinstated vs transformed）比较；
    - 脑区时序分析；
    - 与行为正确率的关联。
  - 未报告多数据集复现，但实验在被试内多试次、严格控制语言材料。

- **充分性评估**：
  - 实验控制合理，变量独立；
  - 结果稳定且有统计显著；
  - 缺乏跨任务、跨语言验证，外推性有限。

---

## 六、主要结论与发现

1. **静默工作记忆的存在证据**：  
   早期词语神经表征在从句期间并不依赖持续活动维持，而处于“活动静默”状态。

2. **转换性再激活（transformed reactivation）**：  
   主语在主句动词出现后重新激活，编码形式不同于初始表征，表明记忆检索涉及编码转换。

3. **脑区时序机制**：  
   记忆再激活动作首先发生在右侧背外侧前额叶（DLPFC），随后传播至额颞语言相关区域，显示出“域通用控制—语言特异处理”的协作模式。

4. **句法依赖与行为预测**：  
   再激活强度受句法结构调节，并可预测理解准确率，揭示层级语法处理对记忆机制的依赖性。

---

## 七、优点与创新点

- 首次提供**直接神经生理证据**支持“语言理解中存在活动静默工作记忆”。
- 创新使用 MEG 时间分辨解码技术，能够**以毫秒级精度追踪语义表征的动态变化**。
- 提出现象级新发现：记忆表征并非简单再现，而是“转换性再激活”，提示复杂的神经表征变换机制。
- 揭示前额叶与语言区的**跨网络协作模式**，打通“工作记忆—语言加工”两大认知领域。

---

## 八、不足与局限

- **样本与语言材料局限**：研究仅使用英语句子，受试者范围有限，跨语言普适性待验证。
- **任务复杂度控制不足**：嵌句任务可能包含注意与语义整合的交互效应，难以完全区分记忆维持与句法处理。
- **未复现于其他模态**（如阅读或视觉呈现），限制结果的跨感知通用性。
- **神经机制层面解释仍非因果**：MEG 提供时序信息但空间分辨率有限，无法证明前额叶对语言区的因果调控。
- **缺乏模型化分析**：未与神经网络语言模型或计算记忆模型进行直接对比。

---

**（完）**
