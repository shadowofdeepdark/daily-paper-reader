---
title: Classification of Smartphone Interaction Using Multimodal Physiological Signals with a Brain-Body Spatio-Temporal Transformer
title_zh: 基于脑-身体时空 Transformer 的多模态生理信号智能手机交互分类
authors: "Mishra, P., Kagathara, V., Gandhi, T. K."
date: 2026-05-07
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.03.722573v1.full.pdf"
tags: ["query:q9"]
score: 7.5
evidence: 包括脑电和眼动在内的多模态生理信号用于分类认知反应
tldr: 本文针对智能手机不同交互行为的生理差异，提出融合脑电、皮电、光体积和眼动信号的脑-身体时空Transformer模型BB-STT，用于识别视频浏览、游戏和基线活动，实现高准确率与强泛化能力，为自然场景下数字行为的客观评估提供新方法。
source: biorxiv
selection_source: fresh_fetch
motivation: 不同智能手机使用行为引发丰富的认知和生理差异，但现有研究常将其视为单一行为。
method: 提出脑-身体时空Transformer（BB-STT），融合EEG、EDA、PPG和眼动信号，通过跨模态注意机制分类智能手机使用类型。
result: "模型在区分智能手机与非智能手机活动上达83.51%准确率，在三类任务上达74.13%，跨模态注意提升16.74个百分点。"
conclusion: 多模态生理信号能有效用于数字交互识别，BB-STT展现了良好的泛化和解释性，为实时评估人机交互提供新途径。
---

## 摘要
不同的智能手机交互行为，如短视频滚动浏览和移动游戏，会引发显著不同的认知与生理反应。然而，将智能手机使用视为单一行为的传统方法往往忽视了这些差异。本文提出了一种名为 BrainBody Spatio-Temporal Transformer (BB-STT) 的统一深度学习框架，用于从包含 EEG、EDA、PPG 和眼动追踪等多模态信号中分类识别交互特定的生理特征。BB-STT 在区分智能手机与非智能手机活动时达到了 83.51% 的准确率，在短视频、游戏与基线观看三分类任务中达到了 74.13% 的准确率。模型在留一受试者交叉验证（LOSO）中的泛化能力强，其表现与五折交叉验证的准确率相当。跨模态注意力机制是关键组件，通过对多模态信号的动态整合，使三分类准确率提升了 16.74 个百分点。可解释性分析表明，生理反应呈层级化组织结构。眼动特征，尤其是注视深度，有助于对智能手机与非智能手机活动进行粗粒度区分；而在区分智能手机上的被动视频观看与主动游戏时，则主要依赖双侧瞳孔扩张与中部 EEG 特征的共同作用。总体而言，这些结果展示了多模态生理信号在自然环境中对数字参与进行客观、实时评估的潜力。

## Abstract
Distinct smartphone interaction behaviors, like short-form video scrolling and mobile gaming, elicit qualitatively different cognitive and physiological responses. However, such distinctions is often overlooked by approaches that treat smartphone use as a monolithic behavior. This paper presents BrainBody Spatio-Temporal Transformer (BB-STT), a unified deep learning framework for classifying interaction-specific physiological signatures from multimodal signals, including EEG, EDA, PPG, and eye-tracking. BB-STT achieves 83.51% accuracy in distinguishing smartphone from non-smartphone activity and 74.13% accuracy in three-class classification of short-form video, gaming, and baseline viewing. The model demonstrates strong generalization with leave-one-subject-out (LOSO) performance that is also comparable to 5-fold cross-validation accuracy. Crossmodal attention emerges as the key component, improving three-class accuracy by 16.74 points through dynamic integration of multimodal signals. Interpretability analysis indicates a hierarchical organization of physiological responses. Eye-tracking features, particularly gaze depth, enable coarse separation between smartphone and non-smartphone activity. In contrast, finer discrimination between passive video viewing and active gaming on smartphones relies on the joint contribution of bilateral pupil dilation and central EEG features. Together, these results demonstrate the potential of multimodal physiological signals for objective, real-time assessment of digital engagement in naturalistic settings.