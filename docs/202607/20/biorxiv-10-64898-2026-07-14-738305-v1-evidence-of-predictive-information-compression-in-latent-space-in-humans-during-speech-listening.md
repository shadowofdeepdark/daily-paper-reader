---
title: Evidence of predictive information compression in latent space in humans during speech listening
authors: "Corsini, A., Schneider, S., Tomassini, A., Pedani, L., Fadiga, L., D'Ausilio, A."
date: 2026-07-15
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.14.738305v1.full.pdf"
tags: ["query:profile-1"]
score: 8.5
evidence: 语音听解过程中的预测信息表征
tldr: 探讨人类语音感知过程中神经系统是否在潜空间中使用预测编码。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738305-v1/fig-001.webp\", \"caption\": \"\", \"page\": 3, \"index\": 1, \"width\": 1277, \"height\": 1098}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738305-v1/fig-002.webp\", \"caption\": \"\", \"page\": 5, \"index\": 2, \"width\": 1274, \"height\": 857}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738305-v1/fig-003.webp\", \"caption\": \"\", \"page\": 7, \"index\": 3, \"width\": 1273, \"height\": 890}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738305-v1/fig-004.webp\", \"caption\": \"\", \"page\": 9, \"index\": 4, \"width\": 1271, \"height\": 1194}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738305-v1/fig-005.webp\", \"caption\": \"\", \"page\": 23, \"index\": 5, \"width\": 1276, \"height\": 1018}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738305-v1/fig-006.webp\", \"caption\": \"\", \"page\": 24, \"index\": 6, \"width\": 1273, \"height\": 1248}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738305-v1/fig-007.webp\", \"caption\": \"\", \"page\": 25, \"index\": 7, \"width\": 1270, \"height\": 781}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738305-v1/fig-008.webp\", \"caption\": \"\", \"page\": 26, \"index\": 8, \"width\": 1270, \"height\": 583}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738305-v1/fig-009.webp\", \"caption\": \"\", \"page\": 27, \"index\": 9, \"width\": 1276, \"height\": 1158}]"
motivation: 语音听解过程中的预测信息表征。
method: 方法与实现细节请参考摘要与正文。
result: 结果与对比结论请参考摘要与正文。
conclusion: 总体而言，该工作在所述任务上展示了有效性，并提供了可复用的思路或工具。
---

## Abstract
Speech perception requires transforming acoustic input into neural representations that support linguistic understanding, yet its underlying computational principles remain unclear. Classical efficient coding theories posit optimal compression of sensory input, whereas alternative accounts propose that neural systems preferentially encode information that supports prediction. A key open question is whether such predictive encoding operates on fixed inputs or on flexible internal representations. We instantiated three hypothesis models of speech processing: (i) optimal compression with deep autoencoders, (ii) predictive reconstruction with predictive autoencoders, and (iii) predictive information representation via latent-space prediction using contrastive learning. We compared resulting speech latent representations to electroencephalographic (EEG) activity during speech listening. Representations learned under the predictive information objective best explained neural latents. Crucially, only representations that selectively compressed predictive information predicted behavioral performance, suggesting that neural speech representations are structured to encode predictive information in latent space rather than to maximize compression or input prediction.