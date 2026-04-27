---
title: "Brain2VLM: Hierarchical Alignment Between Cortical Representations and Vision-Language Latent Spaces"
title_zh: Brain2VLM：皮层表征与视觉—语言潜在空间之间的分层对齐
authors: "Pritam, N. A. A., O, J. S., Jain, S."
date: 2026-04-23
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.23.720313v1.full.pdf"
tags: ["query:profile-1"]
score: 6.5
evidence: 皮层表征与视觉语言潜空间的对齐研究
tldr: 本文提出Brain2VLM框架，研究fMRI信号与预训练视觉-语言模型潜在空间的分层对齐关系。采用线性与非线性解码方法分析不同皮层区域的映射特征，发现视觉皮层与结构潜变量线性对应，高级视觉区需非线性映射。结果显示非线性解码显著提升语义空间对齐和重建质量，揭示脑-潜变量对齐是脑图像重建的关键因素。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有脑成像到模型潜变量映射效果良好但机制不清楚，需探究皮层与模型潜空间的分层对齐。
method: 通过线性岭回归和非线性残差MLP从fMRI数据中解码扩散潜变量和CLIP嵌入。
result: 非线性解码对扩散潜变量提升较小，但对语义嵌入显著提高分布对齐和预测性能。
conclusion: 研究验证了大脑皮层表征与视觉-语言模型潜在空间之间存在分层映射关系，脑-潜变量接口是脑解码系统的关键瓶颈。
---

## 摘要
本研究提出了 Brain2VLM 框架，用于分析皮层表征如何与基于扩散模型的预训练视觉—语言模型的潜在空间对齐，从而实现从脑信号到图像的重建。尽管近年来的方法通过将功能性磁共振成像（fMRI）信号映射到模型潜变量取得了良好性能，但这一映射的结构仍缺乏深入理解。我们假设脑到潜变量的对齐具有分层特征：早期视觉皮层与结构性扩散潜变量之间呈近似线性对应，而高阶视觉区域则需要非线性映射才能与语义嵌入空间对齐。为验证这一点，我们在 Natural Scenes Dataset 上使用线性岭回归与非线性残差 MLP 从 fMRI 信号中解码扩散潜变量与 CLIP 嵌入。结果显示，对于扩散潜变量，非线性解码仅带来轻微提升（相关系数增量 Δ ≈ 0.05–0.06），但在语义嵌入上则取得显著改进（Δ ≈ 0.47），显著提升了分布对齐度（MMD：0.042 vs 0.358）。然而，更高的解码器表达能力可能引入潜变量分布偏移，表明预测精度与生成兼容性之间存在权衡。尽管采用了简单的重建流程，Brain2VLM 仍取得了较强的表现（PixCorr：0.33，CLIP：85%），暗示脑与潜变量的对齐改进在重建质量中与生成建模同样重要。这些发现提供了皮层表征与模型潜在空间之间分层对齐的实证依据，将脑到潜变量的接口定位为脑解码系统的主要瓶颈。代码可在 https://github.com/adarsh-crafts/Brain2VLM 获取。

## Abstract
This work introduces Brain2VLM, a framework for analyzing how cortical representations align with latent spaces of pretrained diffusion-based vision-language models for brain-to-image reconstruction. While recent approaches achieve strong performance by mapping functional Magnetic Resonance Imaging (fMRI) signals to model latents, the structure of this mapping remains poorly understood. We hypothesize that brain-to-latent alignment is hierarchical, with early visual cortex exhibiting approximately linear correspondence to structural diffusion latents, and higher-order visual areas requiring nonlinear mappings to align with semantic embedding spaces. To test this, we decode diffusion latents and CLIP embeddings from fMRI signals using both linear ridge regression and a nonlinear residual MLP on the Natural Scenes Dataset. Our results reveal that nonlinear decoding provides only marginal improvements for diffusion latents ({Delta} {approx} 0.05 - 0.06 in correlation), but yields substantial gains for semantic embeddings ({Delta} {approx} 0.47), significantly improving distributional alignment (MMD: 0.042 vs 0.358). However, increased decoder expressivity can introduce shifts in latent distributions, highlighting a trade-off between prediction accuracy and generative compatibility. Despite using a simple reconstruction pipeline, Brain2VLM achieves strong performance (PixCorr: 0.33, CLIP: 85%), suggesting that improvements in brain-to-latent alignment play an important role in reconstruction quality alongside generative modeling. These findings provide empirical evidence for hierarchical alignment between cortical representations and model latent spaces, positioning the brain-to-latent interface as a primary bottleneck in brain decoding systems. Our code can be found at https://github.com/adarsh-crafts/Brain2VLM