---
title: Neural Tracking of Speech Envelope as an Index of Spatial Release from Masking
title_zh: 作为空间释放掩蔽指标的语音包络神经追踪
authors: "Galeano-Otalvaro, J.-D., Dieudonne, B., Francart, T., Wouters, J."
date: 2026-07-02
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.29.734758v1.full.pdf"
tags: ["query:q9"]
score: 7.5
evidence: 使用脑电图进行语音神经追踪以量化加工过程
tldr: 研究探讨EEG神经语音追踪能否反映空间释放掩蔽效应，从而客观评估双耳空间听觉能力。研究招募19名正常听力受试者，在不同信噪比下聆听共址与空间分离条件中的连续语音，并采用包络重建与时间响应函数分析EEG数据。结果发现，空间分离可显著增强目标语音的神经追踪，并改善晚期皮层响应特征，且与行为层面的语音理解提升一致，表明神经语音追踪可作为评估空间听觉收益的客观指标。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-29-734758-v1/fig-001.webp\", \"caption\": \"Figure 1 SRTs per subject for the collocated and separated conditions obtained with the Matrix sentence test (Twosided Wilcoxon sign-rank test; p<0.001).\", \"page\": 11, \"index\": 1, \"width\": 494, \"height\": 330}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-29-734758-v1/fig-002.webp\", \"caption\": \"Figure 2 A. Behavioural scores and envelope tracking for each SNR and spatial condition. Points show individualsubject averages, and dashed lines indicate the predictive trends from a sigmoidal nonlinear mixed-effects model. ( p < 0.05, p < 0.01, p < 0.001; two-sided Wilcoxon signed-rank test, FDR corrected).B. Differences between separated and collocated conditions for both untransformed measures, shown per SNR and subject. R and p-values correspond to Pearson’s correlation. C. Relationship between behavioural scores and envelope tracking for collocated and separated conditions. Behavioural scores were logit-transformed to reduce ceiling effects, and envelope tracking (Spearman correlations) was normalised using a Fisher Z transform.\", \"page\": 14, \"index\": 2, \"width\": 904, \"height\": 1124}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-29-734758-v1/fig-003.webp\", \"caption\": \"Table 1. Statistical values for pairwise comparison between envelope tracking values for separated and collocated 437 conditions per SNR (Two-sided Wilcoxon sign-rank test). 438\", \"page\": 13, \"index\": 3, \"width\": 904, \"height\": 256}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-29-734758-v1/fig-004.webp\", \"caption\": \"Figure 3 A. Average TRFs across subjects for each SNR and spatial condition. Shaded ribbons indicate the standard error of the mean. The marked peak corresponds to P2, with its latency (ms) indicated separately for the collocated and separated conditions. Coloured horizontal bars indicate time windows where the TRF amplitude differed reliably from zero across subjects (cluster-permutation test); grey bars mark the overlap between conditions, identifying windows where both retained a significant cluster around the P2 peak. These windows were used to define the time regions for the spatial analysis shown in the bottom panel.\", \"page\": 17, \"index\": 4, \"width\": 1014, \"height\": 993}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-29-734758-v1/fig-005.webp\", \"caption\": \"Table 2. Statistical values for pairwise comparison for P2 latencies and amplitudes for separated and collocated 488 conditions per SNR (Two-sided Wilcoxon sign-rank test, FDR corrected). 489\", \"page\": 16, \"index\": 5, \"width\": 860, \"height\": 519}]"
motivation: 传统双耳听觉收益测量依赖行为反应，因此需要一种能够客观评估空间听觉与空间释放掩蔽效应的神经指标。
method: 研究让19名正常听力受试者在不同信噪比下聆听共址与空间分离条件中的连续荷兰语语音，并利用EEG结合包络重建和TRF分析量化神经语音追踪。
result: 空间分离条件显著增强了目标语音包络的神经追踪能力，尤其在低信噪比下更明显，同时TRF表现出更高幅度和更短潜伏期的晚期皮层响应。
conclusion: EEG神经语音追踪能够客观反映空间释放掩蔽带来的双耳收益，可作为评估复杂听觉环境中空间听觉能力的潜在神经指标。
---

## 摘要
在嘈杂环境中理解语音高度依赖双耳线索，例如双耳时间差和双耳电平差（ITD 和 ILD），这些线索有助于空间听觉以及对竞争性声源的分离。当这些线索受到削弱时，听者在复杂声学环境中的理解会变得十分困难。

双耳获益的行为学测量方法，如双耳掩蔽电平差、双耳可懂度电平差以及空间释放掩蔽（SRM），已在正常听力（NH）听者中得到充分研究，但这些方法都需要受试者主动做出行为反应。基于脑电图（EEG）的神经语音追踪已成为量化连续语音神经加工的一种有前景的方法，但其对空间听觉线索的敏感性仍缺乏充分表征。

我们采用基于 EEG 的神经语音追踪，在正常听力受试者中研究空间释放掩蔽的神经相关机制。19 名参与者在多种信噪比（SNR）条件下，聆听带有掩蔽噪声的连续荷兰语语音故事，实验包含两种空间配置：共位条件（S0N0）和空间分离条件（S0N90）。通过语音包络重建和时间响应函数（TRF）分析两种方法，对语音包络的神经追踪进行量化。

空间分离增强了对目标语音包络的神经追踪，尤其是在具有挑战性的低信噪比条件下，此时行为学上也观察到了空间释放掩蔽效应。TRF 分析进一步揭示，晚期皮层成分的幅度增加且潜伏期缩短，这与空间去掩蔽效应一致。

这些发现表明，神经语音追踪能够捕捉空间去掩蔽的皮层特征，并与语音理解的行为学改善密切对应。在正常听力受试者中建立这些关系，有助于开发用于评估双耳获益的客观神经测量方法，尤其适用于难以进行行为测试的人群。

## Abstract
Understanding speech in noisy environments relies strongly on binaural cues such as interaural time and level differences (ITDs and ILDs), which support spatial hearing and the segregation of competing sound sources. When these cues are degraded, listeners experience substantial difficulty in complex acoustic environments.

Behavioural measures of binaural benefit, such as binaural masking level differences, binaural intelligibility level differences, and spatial release from masking (SRM), are well established in normal-hearing (NH) listeners, but they require an active behavioural response. Neural speech tracking using electroencephalography (EEG) has emerged as a promising approach for quantifying neural processing of continuous speech, yet its sensitivity to spatial hearing cues remains insufficiently characterised.

We investigated the neural correlates of spatial release from masking in NH listeners using EEG-based neural speech tracking. Nineteen participants listened to continuous Dutch speech stories presented with masking noise under two spatial configurations, collocated (S0N0) and spatially separated (S0N90), across multiple signal-to-noise ratios (SNRs). Neural tracking of the speech envelope was quantified using both envelope reconstruction and temporal response function (TRF) analyses.

Spatial separation enhanced neural tracking of the target speech envelope, particularly at challenging SNRs where behavioural SRM was also observed. TRF analysis further revealed increased amplitudes and decreased latencies of late cortical components consistent with spatial unmasking effects.

These findings demonstrate that neural speech tracking captures cortical signatures of spatial unmasking and closely reflects behavioural improvements in speech understanding. Establishing these relationships in NH listeners supports the development of objective neural measures for evaluating binaural benefit in difficult-to-test populations.