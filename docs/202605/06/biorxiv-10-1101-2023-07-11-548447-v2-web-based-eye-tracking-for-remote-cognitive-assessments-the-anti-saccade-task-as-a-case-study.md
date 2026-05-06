---
title: "Web-based eye-tracking for remote cognitive assessments: The anti-saccade task as a case study"
title_zh: 基于网络的眼动追踪用于远程认知评估：以反眼跳任务为案例研究
authors: "Juantorena, G. E., Figari, F., Petroni, A., Kamienkowski, J. E."
date: 2026-04-30
pdf: "https://www.biorxiv.org/content/10.1101/2023.07.11.548447v2.full.pdf"
tags: ["query:q5"]
score: 9.0
evidence: 用于远程认知评估和实验的网页端眼动追踪
tldr: 本研究提出改进的基于网络摄像头的远程眼动追踪原型，优化了无需鼠标交互的实验流程，并通过经典抗眼跳任务验证了其时空分辨率与可靠性，结果与实验室高质量眼动仪一致，显示其在远程认知评估和临床应用中的可行性。
source: biorxiv
selection_source: fresh_fetch
motivation: 为了实现远程认知评估并扩大研究人群，亟需验证网络摄像头眼动追踪在实验和临床中的可行性。
method: 研究开发改进后的基于网络摄像头的眼动追踪原型，并通过抗眼跳任务评估其时空分辨率和可靠性。
result: 系统稳定，校准可靠，成功复现实验室中抗眼跳任务的典型结果。
conclusion: 该研究验证了远程网络式眼动追踪在经典认知任务中的可靠性和潜力，同时指出其在实验精度方面的局限。
---

## 摘要
近年来，基于远程网络摄像头的眼动追踪（ET）原型经历了多项发展，探索其在网络实验中的可行性与潜力。这一日益增长的研究兴趣主要源于任务可远程执行的可能性，使得更大、难以触及的人群得以研究，并为远程医疗应用提供了潜力。然而，摄像头质量下降和环境噪声增加带来了新的实施挑战。本研究提出了一种新的远程网络摄像头基础的眼动追踪原型。首先，我们改进了现有远程ET原型在认知和临床任务中的技术，例如无需持续的鼠标操作。其次，我们评估了该系统的时空分辨率及其实验内的可靠性。第三，我们进行了一个经典实验——反眼跳任务，以评估其功能和局限性。该认知测试比较了眼睛向目标方向移动（顺眼跳）或远离目标方向移动（反眼跳）的水平运动，以测量抑制控制能力。我们的结果重复了使用高质量实验室ET所得的先前发现。简而言之，在反眼跳任务中的错误率高于顺眼跳，而错误反应的反应时间更快。我们的网络ET原型在时间上保持了稳定的校准，并在经典认知实验中表现良好。最后，我们讨论了该原型在临床应用中的潜力以及在实验使用中的局限性。

## Abstract
Over the last years, several developments of remote webcam-based eye tracking (ET) prototypes have emerged, testing their feasibility and potential for web-based experiments. This growing interest is mainly explained by the possibility to perform tasks remotely, which allows the study of larger and hard-to-reach populations and potential applications in telemedicine. Nevertheless, a decrease in the quality of the camera and a noisier environment bring new implementation challenges. In this study, we present a new prototype of remote webcam-based ET. First, we introduced improvements to the state-of-the-art remote ET prototypes for cognitive and clinical tasks, e.g. without the necessity of constant mouse interactions. Second, we assessed its spatiotemporal resolution and its reliability within an experiment. Third, we ran a classical experiment, the anti-saccade task, to assess its functionality and limitations. This cognitive test compares horizontal eye movements toward (pro-saccades) or away from (anti-saccades) a target, as a measure of inhibitory control. Our results replicated previous findings obtained with high-quality laboratory ETs. Briefly, higher error rates in anti-saccades compared to pro-saccades were observed, and incorrect responses presented faster reaction times. Our web-ET prototype showed a stable calibration over time and performed well in a classic cognitive experiment. Finally, we discussed the potential of this prototype for clinical applications and its limitations for experimental use.

---

## 论文详细总结（自动生成）

# 基于网络的眼动追踪用于远程认知评估：以反眼跳任务为案例研究 — 中文总结

---

## 一、核心问题与总体背景

- **研究动机**：近年来，远程心理与认知评估的需求急升，尤其在无法到实验室的群体（如老年人、患者或分布广泛的样本）中开展实验成为重要方向。  
- **技术背景**：传统实验级眼动仪设备价格高昂（约 1–5 万美元）且需要实验室环境；而基于普通摄像头的网络眼动追踪技术具有低成本、便捷和可远程执行的优势。  
- **核心问题**：如何在无专用硬件、无实验员监督的网络环境下，实现足够**时空分辨率与稳定性**的眼动追踪，以支撑认知任务或临床评估。  
- **目标**：构建并验证一个改进的网络摄像头眼动追踪原型，评估其在典型认知任务——**反眼跳（Anti-saccade）任务**中的可靠性与可用性，为远程认知与神经精神病学应用奠定基础。

---

## 二、方法论：核心思想与技术实现

1. **整体架构**  
   - 在现有 *WebGazer.js* 框架基础上进行改进，形成新版 **web-based eye-tracker prototype**。  
   - 系统通过普通网页浏览器（Chrome）和标准摄像头定位眼睛并预测视线位置，兼容 *jsPsych* 在线实验库。

2. **关键模块与技术细节**

   - **Facemesh 模型升级**：
     - 使用最新版 `@tensorflow-models/face-landmarks-detection` 替代旧版 `@tensorflow-models/facemesh`；
     - 改进了实时眼部坐标提取逻辑，解决旧模型 10 分钟后崩溃的问题。

   - **显式校准（Calibration）机制**：
     - 采用 **空间点校准 + 空格键确认** 的方式（类似实验室ET），替代原 WebGazer 的“鼠标点击校准”；
     - 每个校准点采样眼部图像并更新岭回归模型（Ridge Regression）；
     - 特征维度：每只眼睛图像 10×6 像素灰度处理 → 拼接为 120 维输入向量；输出为屏幕坐标 (x, y)。

   - **头部运动检测（Head movement checking）**：
     - 在每帧检测眼坐标变化，若偏离校准状态则自动触发“建议重新校准”的提示；
     - 通过自定义 JS 事件导出坐标数据，供外部模块调用。

   - **虚拟下巴托（Virtual Chin-Rest）**：
     - 两步校准：  
       ① 用标准银行卡校准屏幕实际尺寸，计算像素密度；  
       ② 盲点实验估算用户眼距（基于 13.5°视觉角公式）；
     - 提供像素到视觉角度转换因子（px→deg），实现跨设备一致刺激呈现。

   - **兼容性与接口**：  
     - 提供两种接口：jsPsych任务调用接口和浏览器独立测试 playground；
     - 所有代码开源于 GitHub。

---

## 三、实验设计与对比场景

### 1. 实验一：**系统准确性评估**

- **目的**：验证系统的时间稳定性与空间精度（横向、纵向误差）。  
- **参与者**：作者两人（正常视觉）。  
- **任务流程**：
  - 9 点校准 + 9 点验证，8 个区块 × 8 轮 × 每轮 9 点 → 共 576 试次；
  - 记录采样率与误差分布。
- **硬件条件**：
  - 电脑：Intel i5-4460 CPU, 16 GB RAM, 显示器 1920×1080。
  - 比较 4 种摄像头（Logitech C270、C925e、Kelyx LM16、Redragon Fobos），均为 30 FPS。
- **分析指标**：
  - 水平误差 x、垂直误差 y、总误差（单位：像素）、采样频率（Hz）。

### 2. 实验二：**反眼跳任务验证**

- **目的**：验证网络ET在经典认知任务中的有效性。  
- **任务说明**：
  - 呈现中心提示符号（交叉=反眼跳；空心圆=顺眼跳），随后出现侧边目标点；
  - 测量眼跳方向是否正确及启动时延（反应时，RT）。
- **参与者**：26 名成年人（31.8±6.1 岁，7 女）。
- **运行环境**：远程在线，使用 Logitech C270 摄像头（720p, 30 FPS）。
- **数据处理**：
  - 预处理与分析由 Python 库 *Pyxations* 执行，转为 BIDS 格式；
  - 采样率重采样为 30 Hz，滤除离群试次；
  - 采用四分类法分析：
    - 正确顺眼跳、错误顺眼跳、正确反眼跳、错误反眼跳；
  - 统计方法：Wilcoxon 秩和检验，报告中位数与 IQR。

- **Benchmark 对照**：实验室级结果（反眼跳错误率更高、反应时间更长）作为理论标准。

---

## 四、资源与算力

- 本研究为**行为实验与统计分析**，并未涉及模型训练或大规模计算。  
- 文中未提及 GPU 型号、训练时间或算力指标；仅指出运行环境为标准桌面电脑与 Chrome 浏览器。  
- Facemesh 模型通过 TensorFlowJS 在客户端实时运行，推理时间随浏览器性能而变。

---

## 五、实验数量与充分性

- 共执行 **两大类实验**：
  1. **精度与稳定性测试**（8 块 × 576 试次 × 多摄像头对比）；
  2. **反眼跳任务验证**（26 受试者 × 320 次试次）。  
- 数据量对于可行性验证较充分；试验覆盖不同硬件与远程条件。  
- 分析采用非参数统计与显著性检验，结果报告详实。  
- 客观性较高，但样本量仍偏小（尤其精度实验仅 2 人），因此结论为验证性质而非大规模统计。

---

## 六、主要结论与发现

- 改进后的网络摄像头眼动追踪系统可在网页端实现稳定校准与较一致采样率（约 22–25 Hz）。  
- 空间误差主要集中在垂直方向（较高），但总体误差可控（约 4°视觉角）。  
- 在反眼跳任务中成功复现实验室结果：
  - 反眼跳错误率高于顺眼跳（5.8% vs 3.5%，p≈0.09，呈趋势）；  
  - 正确反眼跳反应时间明显更长（约 461 ms vs 416 ms，p = 0.00019）；  
  - 错误反眼跳具有更快的反应时间（“快速错误”现象），提示抑制失败机制。  
- 实验结论显示 10 分钟左右的远程任务即可获得与实验室近似数据。  
- 系统在无鼠标交互与远程环境中仍保持良好稳定性与实验复现性。

---

## 七、优点与亮点

- **技术融合与改进显著**：
  - 修复 WebGazer 10 分钟崩溃问题；
  - 采用显式校准、增加头动检测、整合虚拟下巴托实现屏幕距校验。
- **开放与可重复性强**：
  - 全部代码与数据公开（GitHub 链接）；
  - 支持 *jsPsych* 实验脚本，可复用。
- **实验设计合理**：
  - 使用经典反眼跳任务作为验证 benchmark；
  - 同时展示系统在时间稳定性与空间误差上的表现。
- **临床潜力明确**：
  - 可用于认知抑制评估、Alzheimer/MCI 等远程诊断前景。

---

## 八、不足与局限

- **采样率与分辨率限制**：
  - 典型 webcam 仅 30 FPS，空间精度约 4°视觉角，低于专业设备的 0.5°。  
  - 可能不足以处理高速眼跳或微细注视检测任务。
- **环境与设备差异**：
  - 不同浏览器与硬件可能影响算法稳定性；
  - 研究仅基于 Chrome 测试，缺少 Firefox、Safari 等比较。
- **样本规模有限**：
  - 精度实验参与者过少（2 人）；临床群体尚未验证。
- **缺乏眨眼检测功能**：
  - 当前系统未包含眼闭合检测，限制部分任务分析。
- **算法简化**：
  - 使用岭回归模型，未来可探索神经网络或更强鲁棒算法。

---

（完）
