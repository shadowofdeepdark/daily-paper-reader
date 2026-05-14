---
title: Two Interacting Neural Processes Support Speech Planning during Naturalistic Conversation
title_zh: 两种相互作用的神经过程支持自然对话中的言语规划
authors: "Yamasaki, H., Blache, P., Schön, D."
date: 2026-05-07
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.06.723165v1.full.pdf"
tags: ["query:profile-1"]
score: 9.0
evidence: 记录自然对话中的脑电图，以测试听力与言语计划期间的神经活动
tldr: 本研究利用双人面对面对话的EEG记录，探讨说话者在听对方讲话时的脑活动如何支持言语计划。通过事件相关电位、振荡分析与多变量解码，发现听阶段的神经信号能提前一秒预测发话行为，揭示了言语计划的早期和晚期神经过程。
source: biorxiv
selection_source: fresh_fetch
motivation: 人类对话中说话者需在聆听时规划回应，但支持此过程的神经机制尚不明。
method: 研究通过记录参与者自然对话中的EEG信号，并进行ERP、频谱分析和多变量时间泛化解码。
result: 早期神经活动可预测发话持续时间，ERP成分和α/β功率变化与响应长度相关，延迟预测更接近转话边界。
conclusion: 研究表明言语计划在聆听阶段就已展开，早期活动反映持续的响应规划，后期过程与发话启动相关。
---

## 摘要
对话要求说话者在倾听对方时同时规划自己的回应，但支持这种重叠的神经动态机制仍不清楚。尤其是，不同的理论对于行为相关的准备是在理解过程的早期出现，还是仅在言语开始前才出现存在分歧。本研究记录了参与自然面对面对话的受试者配对的脑电图（EEG），并检验在倾听阶段的神经活动是否能够预测说话者开始回应的时间（潜伏期）以及发言的时长。通过事件相关电位（ERP）、振荡分析和多变量解码，我们发现发声前的神经活动在发声前一秒多就携带关于即将发生行为的可靠信息。最强且最早的效应与回应持续时间相关，持续的ERP成分以及α/β波段功率的调制能够预测参与者将说话的时长，即使在控制了行为变量之后仍然有效。相比之下，与回应潜伏期相关的神经预测指标在时间上更为局限，并且部分与对话伙伴的语轮边界对齐。时间泛化分析进一步揭示了连接准备早期与晚期阶段的稳定神经模式。总体而言，这些发现表明，会话规划在倾听阶段就展开，早期的神经活动反映了回应范围的持续表征，而后期的过程则与承诺和启动相关。这支持了一种关于语轮转换的时间结构化观点，其中准备过程包含早期的保持阶段与晚期的运动参与。

## Abstract
Conversation requires speakers to plan their responses while still listening to their partner, yet the neural dynamics supporting this overlap remain unclear. In particular, competing accounts differ on whether behaviourally relevant preparation emerges early during comprehension or only close to speech onset. Here, we recorded EEG from pairs of participants engaged in natural, face-to-face conversation and tested whether neural activity during listening predicts both when speakers begin their response (latency) and how long they speak (duration). Using event-related potentials, oscillatory analyses, and multivariate decoding, we show that pre-speech neural activity carries robust information about upcoming behaviour more than one second before articulation. The strongest and earliest effects tracked response duration, with sustained ERP components and alpha/beta power modulations predicting how long participants would speak, even after controlling for behavioural variables. In contrast, neural predictors of response latency were more temporally restricted and partly aligned with partner turn boundaries. Temporal generalisation analyses further revealed stable neural patterns linking early and late stages of preparation. Together, these findings indicate that conversational planning unfolds during listening and that early neural activity reflects the maintained specification of response extent, followed by later processes related to commitment and initiation. This supports a temporally structured account of turn taking in which preparation involves both early maintenance and late motor engagement.

---

## 论文详细总结（自动生成）

# 两种相互作用的神经过程支持自然对话中的言语规划 — 论文总结

---

## 一、核心问题与研究背景

- **研究动机**  
  人类在自然对话中能够在极短时间内完成语轮转换（约 200–300 毫秒），远快于语言生产所需的准备时间（通常超过 600 毫秒）。这表明说话者在听对方讲话的同时必须提前规划回应。  
- **科学背景与争议**  
  现有研究存在“早期规划”（Early Planning）与“晚期规划”（Late Planning）两种理论：
  - *早期规划假设*：听者在理解过程中即开始准备回应；
  - *晚期规划假设*：仅在伙伴语轮接近结束时才启动运动准备，以避免理解与生产冲突。  
- **研究目标**  
  本文旨在揭示自然面对面对话中，听阶段的神经动态是否能够预测说话者的行为（回应潜伏期与持续时长），并厘清言语计划的时间结构。

---

## 二、方法论与技术路线

- **总体思路**  
  通过记录双人自然对话的脑电（EEG），分析听者在自己发话前的神经活动是否携带未来言语行为的可预测信息。
- **关键技术步骤**
  1. **数据记录与分段**：实时 EEG + 对话录音；语音分割为 *Inter-Pausal Units (IPUs)*，由至少 200ms 的静音分隔；
  2. **事件对齐**：所有 EEG 信号对齐至发话者语轮开始（自我发言的 0 秒）；
  3. **信号处理**：
     - 独立成分分析（ICA）剔除肌肉、运动伪迹；
     - 高频滤波（0.1–30 Hz）、降采样、参考重设；
  4. **分析方法**：
     - 事件相关电位（ERP）分析：识别发声前的慢波成分；
     - 振荡分析：评估 α（8–12 Hz）/ β（13–30 Hz）功率变化；
     - 多变量时间泛化解码（Temporal Generalisation Decoding）：评估神经表征在时间上的稳定性；
     - 试次级线性混合效应模型（LMM）：量化神经变量对行为的预测力，并控制协变量（伙伴语轮长度、行为耦合项）。
- **统计方法**  
  使用非参数**簇基置换检验**（Maris & Oostenveld, 2007）控制多重比较；FDR 校正显著性水平；采用似然比检验评估模型改进。

---

## 三、实验设计

- **实验任务**
  - 使用 **Diapix** 协作任务（Van Engen et al., 2010；Baker & Hazan, 2011）：双人“找不同”游戏，自然诱发连续对话与频繁语轮切换。
- **数据集与规模**
  - 34 名受试者（17 对话对），最终有效数据为 32 人，共 **12,939 个语轮转换事件**；
  - 每位被试的试次数约 99–314 次。
- **行为指标**
  - *回应潜伏期*（partner offset → self onset）；
  - *回应持续时间*（self IPU 长度）。
- **Benchmark 与对比**
  - 本研究为首个针对自然对话条件的 EEG 预测分析；
  - 对比以往“控制式问答任务”研究（Bögels et al. 2015, 2018）作为参考框架，而非传统算法对比。

---

## 四、资源与算力

- 文中**未涉及显式算力信息**（如 GPU 型号或训练时长）。  
- 所有分析均在 **MNE-Python、R、scikit-learn** 上完成，通过 **Snakemake** 管理流程；计算负载为标准统计分析级，无大规模模型训练。

---

## 五、实验数量与充分性

- 实验层面包含：
  1. **ERP 与频谱对比实验**（长 vs 短回应；快 vs 慢潜伏期）
  2. **混合效应模型分析**（控制行为协变量；
     双时间窗 × 双区 ROI 的系统检验）
  3. **时间泛化解码实验**（两类行为变量均参与）
  4. **ERP–Alpha 耦合分析**（验证神经指标间关系）  
- **实验充分性**  
  - 统计覆盖 ERP、α/β 波段、以及解码；控制个体差与语境协变量；
  - 样本量与试次数充足（>1万语轮），结论较稳健；
  - 然而没有外部验证数据集或多任务测试，生态有效但可重复性尚待验证。

---

## 六、主要结论与发现

1. **早期神经预测**
   - 在发声前 >1 秒的听阶段，EEG 已能预测发言时长；
   - ERP 的持续负波与 α/β 功率下降均表征“回应范围”（duration）。
2. **潜伏期预测较晚**  
   - 与语轮边界时间更贴合，更多反映对转接时机的反应，而非早期规划。
3. **时间泛化结果**  
   - 与即将发声的行为相关的神经表征在整个听阶段稳定存在，表明“持续维持”而非瞬时触发。
4. **ERP 与 α/β 动力学的双过程模型**  
   - ERP 反映 **早期维持（maintenance）** 的响应表征；
   - α/β 去同步化对应 **晚期承诺（commitment）与运动准备**；
   - 二者相互作用，共同支持自然会话中的语轮规划。

---

## 七、方法与设计亮点

- **生态化 EEG 实验**：实现自然面对面对话中的双人同步脑电记录，突破以往实验室式问答限制。
- **行为建模与神经信号结合**：在混合效应模型中同时控制语境与协变量，提高统计因果解释力。
- **多层信号分析整合**：ERP、频谱、解码与耦合分析贯通验证，形成统一时间结构模型。
- **时间泛化技术的创新应用**：评估神经表征稳定性，为理解持续的计划过程提供定量证据。

---

## 八、不足与局限

- **时间和空间分辨率限制**：EEG 难以确定具体脑区来源，需结合 MEG 或 fMRI 进一步验证；
- **动作伪迹风险**：尽管排除发声相关成分，临近语轮开始仍可能受肌肉电影响；
- **任务结构化程度较高**：Diapix 虽为半自然任务，但仍具协作目标，可能影响对完全自发对话的推广；
- **缺乏外部验证与跨语言分析**：研究仅限法语母语者，跨语言普适性待验证；
- **推断层面**：神经预测信号与语言内容的关系尚不清晰，仅表征行为维度（时间与持续），未涉及语义或语法层级。

---

**（完）**
