---
title: "Web-based eye-tracking for remote cognitive assessments: The anti-saccade task as a case study"
title_zh: 基于网络的眼动追踪用于远程认知评估：以反向扫视任务为案例研究
authors: "Juantorena, G. E., Figari, F., Petroni, A., Kamienkowski, J. E."
date: 2026-04-30
pdf: "https://www.biorxiv.org/content/10.1101/2023.07.11.548447v2.full.pdf"
tags: ["query:q5"]
score: 9.0
evidence: 用于远程认知评估的摄像头眼动追踪技术
tldr: 本文提出了一种改进的基于网络的远程摄像头眼动追踪系统，用于认知评估。研究在反向眼跳任务中测试其可靠性与空间时间分辨率，结果显示该系统能稳定复现传统实验室结果，为远程认知与临床评估提供了可行方案。
source: biorxiv
selection_source: fresh_fetch
motivation: 随着远程实验和远程医疗需求增长，需要验证基于网络的眼动追踪在认知任务中的可行性与可靠性。
method: 研究提出改进的远程摄像头眼动追踪原型，并通过反向眼跳任务评估其性能。
result: 系统稳定性与反向眼跳实验结果与实验室高质量设备一致，表现出较好的空间时间分辨率和可靠性。
conclusion: 该原型验证了远程基于网络的眼动追踪在认知评估中具有稳定性与临床应用潜力。
---

## 摘要
近年来，基于远程网络摄像头的眼动追踪（ET）原型得到了多项发展，用以测试其在网络实验中的可行性和潜力。这一日益增长的兴趣主要源于远程执行任务的可能性，能够研究更大规模且难以接触的人群，并具备远程医疗等潜在应用。然而，摄像头质量下降以及环境噪声增加带来了新的实现挑战。本研究提出了一种新的基于远程网络摄像头的ET原型。首先，我们在现有最先进的远程ET原型基础上进行改进，使其适用于认知和临床任务，例如无需持续的鼠标交互。其次，我们评估了其时空分辨率及其实验内的可靠性。第三，我们运行了经典实验——反向扫视任务（anti-saccade task），以评估其功能性与局限性。该认知测试比较了注视目标方向的水平眼动（顺向扫视，pro-saccades）与朝远离目标方向的水平眼动（反向扫视，anti-saccades），用于衡量抑制控制能力。我们的结果重现了以高质量实验室ET获得的先前发现。简而言之，相较于顺向扫视，反向扫视中观察到更高的错误率，且错误反应的反应时间更短。我们的网络ET原型在时间上显示出稳定的校准性能，并在经典认知实验中表现良好。最后，我们讨论了该原型在临床应用中的潜力及其在实验应用中的限制。

## Abstract
Over the last years, several developments of remote webcam-based eye tracking (ET) prototypes have emerged, testing their feasibility and potential for web-based experiments. This growing interest is mainly explained by the possibility to perform tasks remotely, which allows the study of larger and hard-to-reach populations and potential applications in telemedicine. Nevertheless, a decrease in the quality of the camera and a noisier environment brings new implementation challenges. In this study, we present a new prototype of remote webcam-based ET. First, we introduced improvements to the state-of-the-art remote ET prototypes for cognitive and clinical tasks, e.g. without the necessity of constant mouse interactions. Second, we assessed its spatiotemporal resolution and its reliability within an experiment. Third, we ran a classical experiment, the anti-saccade task, to assess its functionality and limitations. This cognitive test compares horizontal eye movements toward (pro-saccades) or away from (anti-saccades) a target, as a measure of inhibitory control. Our results replicated previous findings obtained with high-quality laboratory ETs. Briefly, higher error rates in anti-saccades compared to pro-saccades were observed, and incorrect responses presented faster reaction times. Our web-ET prototype showed a stable calibration over time and performed well in a classic cognitive experiment. Finally, we discussed the potential of this prototype for clinical applications and its limitations for experimental use.

---

## 论文详细总结（自动生成）

# 基于网络的眼动追踪用于远程认知评估：以反向扫视任务为案例研究  
**Web-based eye-tracking for remote cognitive assessments: The anti-saccade task as a case study**  
作者：G. E. Juantorena、F. Figari、A. Petroni、J. E. Kamienkowski（阿根廷布宜诺斯艾利斯大学）  
发布时间：2026 年 4 月 30 日  
来源：bioRxiv  

---

## 一、研究核心问题与整体含义

- **研究动机：**  
  随着远程实验与远程医疗的需求持续增长，传统实验室眼动追踪设备（如 EyeLink、Tobii）价格昂贵且操作受限，难以在大规模或跨地域人群中使用。  
  作者希望验证一种**基于网络的摄像头眼动追踪（Web-ET）**技术是否能在无需专用硬件的情况下实现可靠的认知测试。  

- **研究目标：**  
  1. 开发一个改进的远程摄像头眼动追踪原型。  
  2. 评估其在认知任务（尤其是反向扫视任务）中的空间与时间分辨率。  
  3. 探讨其在临床应用与远程认知评估中的可行性。  

---

## 二、方法论与技术实现

### 1. 核心思想
在现有开源库 WebGazer 的基础上改进算法与架构，使其能独立于鼠标交互进行精确的眼动估计，从而适用于典型认知任务。

### 2. 关键技术细节

- **面部识别与眼位定位（FaceMesh 模型）：**  
  使用 TensorFlowJS 的 `@tensorflow-models/face-landmarks-detection` 代替原 WebGazer 的旧版 Facemesh，实现实时三维面部建模与眼部区域定位。  
  - 有效避免旧 Facemesh 模型 10 分钟后崩溃的问题。  
  - 输出 3D 网格节点，以提取双眼矩形区域。

- **显式校准（Explicit Calibration）：**  
  代替 WebGazer 原本的连续鼠标校准方式：  
  - 用户注视屏幕上依次出现的 9 个校准点并按下空格键；  
  - 基于每个点的图像与屏幕坐标计算岭回归（Ridge Regression）模型。  
  - 校准结束后一次性计算回归系数，降低实时计算压力。  

- **头部运动检测模块（Head Movement Detection）：**  
  - 记录校准阶段眼部位置；  
  - 若后续帧中检测到偏移，则触发“需重新校准”的提示事件。  

- **虚拟下巴托（Virtual Chinrest）集成：**  
  来源于 Li et al. 2020 方法：通过信用卡尺寸标定屏幕分辨率及盲点测量视距。  
  - 计算公式：  
    (1) 逻辑像素密度 LPD = 屏幕像素距离 / 实际毫米距离  
    (2) 视距 d = 实际盲点到中心距离 / tan(13.5°)  
  - 自动计算像素与视角度转换因子，实现视觉度量标准化。  

- **软件兼容性：**  
  - 与 jsPsych 实验框架整合；  
  - 提供浏览器自由访问接口与 HTML/JS playground 以便测试与开发。

---

## 三、实验设计

### 1. 实验场景与任务

- **实验 1：准确度评估（Accuracy Assessment）**
  - 对照 9 点校准与多次验证，测定空间与时间误差。
  - 重复 8 个区块（calibration + validation），共 576 次试验。
  - 两位参与者（作者本人）在多种摄像头上测试。

- **实验 2：反向扫视任务（Anti-saccade Task）**
  - 典型的认知测试：受试者根据提示，需**抑制自动注视并看向目标相反方向**。
  - 共 26 名参与者，单次实验含 160 个反扫试次与 160 个顺扫试次（共约 320 条记录）。
  - 使用 Logitech C270（30 FPS，720p）摄像头，Chrome 浏览器。  
  - 每个区块后需重新校准，以保证头位一致。

### 2. 数据处理与分析流程

- 使用 Python 开源库 **Pyxations** 管理眼动数据（转换为 BIDS 标准格式）。  
- 数据预处理：  
  - 采样率归一化至 30 Hz；  
  - 基线减去中心注视阶段均值；  
  - 正常化坐标并镜像左侧试次。  
- 使用**阈值法**判定扫视方向与反应时间。  
- 统计分析：采用非参数 Wilcoxon 秩和检验比较各条件误差率与反应时间（RT）。

### 3. Benchmark 与对照参考
- 与传统实验室高精度设备的数据进行概念性对照。  
- 重现文献中的典型结果（Currie 1991；Hallett 1978；Munoz 2004 等）。  

---

## 四、资源与算力

- 文中明确说明所有实验均在标准桌面机上执行：  
  - CPU：Intel Core i5‑4460 @ 3.20 GHz × 4  
  - 内存：16 GB  
  - 操作系统：Ubuntu 20.04.5 LTS  
  - 无 GPU 加速提及；所有模型在浏览器端以 JavaScript / TensorFlowJS 推理。  
- 未报告训练时长、算力测度或能耗估算。  

---

## 五、实验数量与充分性

- **实验数量：**  
  - 两个主要实验：准确度评估（576 次点测） + 反向扫视任务（约 320 试次 × 26 人）。  
- **充分性与公平性评估：**  
  - 对于可行性验证而言，实验数量较充分，可反映系统稳定性。  
  - 尽管反扫实验样本量适中，但比传统实验略少。  
  - 校准稳定性与采样率分析覆盖不同摄像头/运行模式，测试范围较全面。  

---

## 六、主要结论与发现

- **系统性能：**
  - 采样率稳定在约 23 Hz（理论 30 Hz 下的实际值），波动小。  
  - 水平方向误差小于垂直方向；中央区域误差低、边角误差高。  
  - 校准后误差随时间稳定，无显著漂移。

- **任务表现：**
  - 反向扫视错误率高于顺向扫视（5.8% vs 3.5%）。  
  - 反扫正确反应时间显著更长（约 461 ms vs 416 ms），反映抑制控制负荷。  
  - 错误反扫具有更快的反应时间（“快速错误”现象），提示抑制失效的自动化机制。  
  - 使用约半量数据（约 10 分钟实验）即可稳定复现上述差异。  

- **总体结论：**  
  改进的 Web‑ET 原型可在无专用硬件的环境下复现实验室眼动实验的关键结果，具备远程认知与临床评估潜力。

---

## 七、优点与创新亮点

1. **显式无鼠标校准机制：**  
   解决了 WebGazer 依赖鼠标输入的局限，使眼动实验更贴近实验室流程。  
2. **实时头位监测与自动重校建议：**  
   提高长期稳定性。  
3. **集成虚拟下巴托：**  
   实时测量屏幕尺寸与视距，实现跨设备的视觉角度标准化。  
4. **开放源代码与 jsPsych 兼容性：**  
   方便研究者复现与定制实验。  
5. **首次在 Web‑ET 中系统测试经典反扫任务并成功复现实验室结果。**

---

## 八、不足与局限

- **硬件限制：**
  - 摄像头帧率低（30 Hz）导致时间分辨率不足，难以捕捉快速扫视或注视变化。  
- **空间精度：**
  - 水平约 2–4°视觉角，低于实验室级设备（≈ 0.5°）。  
- **算法局限：**
  - 使用简单的岭回归模型，未探索更高级的机器学习模型（如深度神经网络）。  
- **样本与环境：**
  - 实验多在可控环境中进行，尚未评估家庭或低光条件下的稳定性。  
- **Blink（眨眼）检测未实现：**
  - 缺乏对眨眼或数据丢失的校正模块。  
- **浏览器影响与平台兼容性：**
  - 实验仅在 Chrome 上测试，其他浏览器（Firefox/Safari）未验证。  

---

**（完）**
