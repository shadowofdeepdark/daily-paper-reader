---
title: The human language processing system straightens natural speech
title_zh: 人类语言处理系统会将自然语音“拉直”
authors: "Xu, J., Nguyen, T. D., Tang, J., Huth, A. G., Goris, R. L. T."
date: 2026-07-02
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.30.735613v1.full.pdf"
tags: ["query:q1"]
score: 7.5
evidence: 人类大脑在自然语言处理过程中的时间预测机制
tldr: 论文研究人脑语言系统是否通过“拉直”语音表征轨迹来提升时间预测能力。作者提出一种利用fMRI估计神经表征轨迹曲率的新方法，并分析受试者聆听自然语音时的大脑活动，同时比较WavLM模型对自然与扰动语音的响应。结果发现，语音表征在低级听觉区更弯曲，而沿皮层层级逐渐变直；类似现象也出现在更接近自然语音统计结构的模型表征中，揭示了时间预测、表征几何与语言层级加工之间的联系。
source: biorxiv
selection_source: fresh_fetch
motivation: 虽然大语言模型显示时间预测对语言处理至关重要，但预测目标如何塑造人脑语音表征结构仍缺乏直接证据。
method: 研究提出一种基于fMRI的表征轨迹曲率测量方法，并结合自然语音刺激与WavLM模型分析不同层级脑区和模型中的轨迹几何变化。
result: 结果发现，低级听觉区的表征轨迹最弯曲，而沿皮层层级逐渐变直；在统计结构更接近自然语音的刺激中，WavLM也表现出更强的层级拉直效应。
conclusion: 研究表明，人脑语言系统会沿皮层层级逐步“拉直”自然语音表征轨迹，从而提升时间预测能力，并揭示了预测目标、表征几何与层级时间尺度之间的直接联系。
---

## 摘要
基于下一词预测训练的大型语言模型展现出了令人瞩目的语言能力。这表明，时间预测这一目标对于语言处理至关重要，但这一目标如何影响人脑中语音表征的结构仍不清楚。在本研究中，我们检验了这样一种假设：预测是通过语音处理层级中表征轨迹在时间维度上的“拉直”而得到促进的。我们开发了一种利用功能性磁共振成像（fMRI）测量这些轨迹曲率的方法。该方法利用了单神经元响应时间尺度与群体轨迹曲率之间一种此前未知的联系。我们考察了受试者聆听自然语音时的大脑响应。结果发现，响应轨迹在低层次听觉区域中弯曲程度最高，并沿皮层层级逐渐变得平直。我们将相同的语音刺激及其扰动版本输入 wavLM——一种与人脑响应高度一致的语音表征模型——结果发现，对于统计结构更接近自然语音的刺激，层级式“拉直”效应最为显著。综合来看，我们的结果建立了时间预测目标、神经语音表征几何结构以及表征时间尺度皮层层级之间的直接联系。

## Abstract
Large language models trained on next-word prediction have impressive linguistic capabilities. This suggests that the goal of temporal prediction is essential to language processing, but how this goal impacts the structure of speech representations in the human brain remains unknown. Here, we test the hypothesis that prediction is facilitated by the temporal straightening of representational trajectories along the speech processing hierarchy. We developed a methodology for measuring the curvature of these trajectories using fMRI. Our method exploits a previously unknown connection between the timescale of single-unit responses and the curvature of population trajectories. We examined brain responses of subjects listening to natural speech. Response trajectories were most curved in lower-level auditory areas and progressively straightened along the cortical hierarchy. We presented the same speech stimuli and perturbed versions thereof to wavLM--a speech representation model that is well aligned with human brain responses--and found that hierarchical straightening effects are strongest for stimuli whose statistical structure resembles natural speech. Together, our results establish a direct connection between the goal of temporal prediction, the geometry of neural speech representations, and the cortical hierarchy of representational timescales.