---
title: Classification of Smartphone Interaction Using Multimodal Physiological Signals with a Brain-Body Spatio-Temporal Transformer
title_zh: 基于脑-身体时空 Transformer 的多模态生理信号智能手机交互分类
authors: "Mishra, P., Kagathara, V., Gandhi, T. K."
date: 2026-05-07
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.03.722573v1.full.pdf"
tags: ["query:q5"]
score: 7.5
evidence: 包含脑电和眼动追踪的多模态信号用于认知反应研究
tldr: 本研究提出一种脑-身体时空Transformer模型（BB-STT），利用脑电、皮电、光体积脉搏和眼动等多模态生理信号识别不同智能手机交互行为。模型在区分智能手机及其具体使用场景（短视频、游戏等）中表现出较高准确率，揭示了跨模态注意力和生理特征的层次性贡献。
source: biorxiv
selection_source: fresh_fetch
motivation: 不同智能手机交互方式会引发差异明显的认知与生理反应，当前研究往往未能细致区分这些差异。
method: 提出BB-STT深度学习框架，通过跨模态注意力整合多源生理信号进行交互行为分类。
result: "模型区分智能手机与非智能手机活动准确率达83.51%，在短视频、游戏和基线三分类任务上达74.13%。"
conclusion: 多模态生理信号能够用于实时、客观地评估自然场景下的数字交互参与程度。
---

## 摘要
不同的智能手机交互行为（如短视频滚动和手机游戏）会引发在认知和生理反应上显著不同的特征。然而，将智能手机使用视为单一行为的研究方法往往忽略了这些差异。本文提出了脑-身体时空 Transformer（BrainBody Spatio-Temporal Transformer, BB-STT），一个统一的深度学习框架，用于从多模态信号（包括 EEG、EDA、PPG 和眼动追踪数据）中分类交互特定的生理特征。BB-STT 在区分智能手机活动与非智能手机活动时达到 83.51% 的准确率，在三分类任务（短视频观看、游戏和基线观看）中取得 74.13% 的准确率。模型在留一被试交叉验证（LOSO）下表现出强泛化能力，其性能与五折交叉验证结果相当。跨模态注意机制是关键组件，它通过动态整合多模态信号，将三分类准确率提高了 16.74 个百分点。可解释性分析表明生理反应具有层级性结构。眼动特征，尤其是凝视深度，可实现智能手机活动与非智能手机活动的粗粒度区分；相反，对于区分被动视频观看与主动游戏，双侧瞳孔扩张与中央 EEG 特征的协同作用更为关键。总体而言，这些结果展示了多模态生理信号在自然环境中实现对数字参与进行客观、实时评估的潜力。

## Abstract
Distinct smartphone interaction behaviors, like short-form video scrolling and mobile gaming, elicit qualitatively different cognitive and physiological responses. However, such distinctions is often overlooked by approaches that treat smartphone use as a monolithic behavior. This paper presents BrainBody Spatio-Temporal Transformer (BB-STT), a unified deep learning framework for classifying interaction-specific physiological signatures from multimodal signals, including EEG, EDA, PPG, and eye-tracking. BB-STT achieves 83.51% accuracy in distinguishing smartphone from non-smartphone activity and 74.13% accuracy in three-class classification of short-form video, gaming, and baseline viewing. The model demonstrates strong generalization with leave-one-subject-out (LOSO) performance that is also comparable to 5-fold cross-validation accuracy. Crossmodal attention emerges as the key component, improving three-class accuracy by 16.74 points through dynamic integration of multimodal signals. Interpretability analysis indicates a hierarchical organization of physiological responses. Eye-tracking features, particularly gaze depth, enable coarse separation between smartphone and non-smartphone activity. In contrast, finer discrimination between passive video viewing and active gaming on smartphones relies on the joint contribution of bilateral pupil dilation and central EEG features. Together, these results demonstrate the potential of multimodal physiological signals for objective, real-time assessment of digital engagement in naturalistic settings.