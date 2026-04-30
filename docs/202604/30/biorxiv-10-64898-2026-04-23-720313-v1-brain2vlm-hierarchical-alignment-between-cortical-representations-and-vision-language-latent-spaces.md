---
title: "Brain2VLM: Hierarchical Alignment Between Cortical Representations and Vision-Language Latent Spaces"
title_zh: Brain2VLM：皮层表征与视觉-语言潜在空间的分层对齐
authors: "Pritam, N. A. A., O, J. S., Jain, S."
date: 2026-04-23
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.23.720313v1.full.pdf"
tags: ["query:q7"]
score: 7.5
evidence: 皮层表征与视觉-语言潜空间之间的对齐
tldr: 本文提出Brain2VLM框架，探讨大脑皮层表征与扩散式视觉语言模型潜在空间的层次对应关系。研究通过线性与非线性模型解码fMRI，发现早期视觉区与结构潜变量线性对应，而高级视觉区需非线性映射，从而显著提升语义对齐与脑图像重建质量。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有脑-图像重建虽表现优异，但脑信号与模型潜在空间对齐的层次结构仍未明晰。
method: 通过线性岭回归和非线性残差MLP从fMRI信号解码扩散潜变量及CLIP嵌入，并评估其分布对齐与重建性能。
result: "非线性解码对扩散潜变量仅带来微小提升，但对语义嵌入显著改善0.47相关，同时提高分布对齐；总体重建表现达到PixCorr 0.33与CLIP 85%。"
conclusion: 脑皮层表征与视觉语言模型潜在空间之间存在分层对应关系，脑到潜在空间的对齐是当前脑解码系统的主要瓶颈。
---

## 摘要
本研究提出了 Brain2VLM 框架，用于分析皮层表征如何与基于扩散的预训练视觉-语言模型的潜在空间对齐，从而实现从大脑到图像的重建。尽管近期的方法通过将功能性磁共振成像（fMRI）信号映射到模型潜变量取得了较强的性能，但这种映射的结构仍然理解不足。我们提出假设，大脑到潜变量的对齐是分层的：早期视觉皮层与结构性扩散潜变量呈近似线性对应，而高级视觉区域则需要非线性映射才能与语义嵌入空间对齐。为验证该假设，我们使用线性岭回归和非线性残差多层感知机（residual MLP）在自然场景数据集（Natural Scenes Dataset）上从 fMRI 信号解码扩散潜变量和 CLIP 嵌入。结果表明，对于扩散潜变量，非线性解码仅带来微小提升（相关性约 Δ0.05–0.06），但对于语义嵌入则获得显著提升（Δ≈0.47），显著改善了分布对齐（MMD：0.042 对 0.358）。然而，更高的解码器表达能力可能导致潜变量分布的偏移，揭示了预测精度与生成兼容性之间的权衡。尽管采用了简单的重建管线，Brain2VLM 仍实现了较强的性能（PixCorr 0.33，CLIP 85%），说明改进大脑与潜变量之间的对齐在重建质量中与生成建模同样重要。这些发现为皮层表征与模型潜在空间之间的分层对齐提供了实证依据，表明大脑到潜变量的接口是大脑解码系统中的主要瓶颈。我们的代码可在 https://github.com/adarsh-crafts/Brain2VLM 获取。

## Abstract
This work introduces Brain2VLM, a framework for analyzing how cortical representations align with latent spaces of pretrained diffusion-based vision-language models for brain-to-image reconstruction. While recent approaches achieve strong performance by mapping functional Magnetic Resonance Imaging (fMRI) signals to model latents, the structure of this mapping remains poorly understood. We hypothesize that brain-to-latent alignment is hierarchical, with early visual cortex exhibiting approximately linear correspondence to structural diffusion latents, and higher-order visual areas requiring nonlinear mappings to align with semantic embedding spaces. To test this, we decode diffusion latents and CLIP embeddings from fMRI signals using both linear ridge regression and a nonlinear residual MLP on the Natural Scenes Dataset. Our results reveal that nonlinear decoding provides only marginal improvements for diffusion latents ({approx}{Delta} 0.05 - 0.06 in correlation), but yields substantial gains for semantic embeddings ({Delta}{approx}0.47), significantly improving distributional alignment (MMD: 0.042 vs 0.358). However, increased decoder expressivity can introduce shifts in latent distributions, highlighting a trade-off between prediction accuracy and generative compatibility. Despite using a simple reconstruction pipeline, Brain2VLM achieves strong performance (PixCorr 0.33, CLIP 85%), suggesting that improvements in brain-to-latent alignment play an important role in reconstruction quality alongside generative modeling. These findings provide empirical evidence for hierarchical alignment between cortical representations and model latent spaces, positioning the brain-to-latent interface as a primary bottleneck in brain decoding systems. Our code can be found at https://github.com/adarsh-crafts/Brain2VLM