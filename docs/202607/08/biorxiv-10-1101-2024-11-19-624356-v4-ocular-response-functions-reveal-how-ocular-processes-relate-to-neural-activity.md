---
title: Ocular Response Functions reveal how ocular processes relate to neural activity
title_zh: 眼部响应函数揭示眼动过程如何与神经活动相关
authors: "Gehmacher, Q., Schubert, J., Kaltenmaier, A., Weisz, N., Press, C."
date: 2026-07-08
pdf: "https://www.biorxiv.org/content/10.1101/2024.11.19.624356v4.full.pdf"
tags: ["query:q5"]
score: 8.0
evidence: 眼动活动与神经活动及认知的关系
tldr: 该研究针对传统脑成像分析中将眼动视为噪声的问题，提出利用静息态MEG结合眼动追踪，通过时间分辨回归建模眼动响应函数（ORFs），系统刻画扫视、眨眼与瞳孔变化对应的神经活动。结果发现眼动与感觉皮层、小脑及额叶活动密切相关，并能由脑信号重建眼动事件；进一步表明部分被认为源于感觉加工的神经标记，可能实际上受到眼动过程影响，为认知与临床神经科学研究提供了新框架。
source: biorxiv
selection_source: fresh_fetch
motivation: 传统神经数据分析常将眼动视为需去除的伪迹，导致与认知和疾病相关的重要神经机制被忽视。
method: 研究结合静息态MEG与眼动追踪，利用时间分辨回归方法建模扫视、眨眼和瞳孔扩张等眼动事件对应的Ocular Response Functions。
result: 研究发现多种感觉皮层、小脑与额叶活动会在眼动事件前后出现特征性响应，并可利用脑活动重建眼动事件，同时证明部分任务相关神经信号可能来源于眼动贡献。
conclusion: 研究提出了可解释眼动与脑活动关系的ORF框架，表明眼动信号不仅是噪声来源，还能为认知与临床神经科学提供重要信息。
---

## 摘要
眼动活动为认知与健康提供了关键洞见，越来越多的证据表明，其参与了注意、记忆和感觉处理等多种认知功能，并且是精神病理学与神经系统疾病的重要指示指标。尽管其在多个领域具有重要意义，但支持眼动的神经机制长期以来研究不足，主要原因在于眼动通常被视为需要从神经信号中去除的伪迹。尽管这种方法有助于数据清理，但也可能丢弃有关眼动控制的有价值信息，因此近年来研究者开始关注对这些信号进行建模，以加深对其机制的理解。在本研究中，我们结合静息态下的脑磁图（MEG）与眼动追踪，并采用时间分辨回归方法，对眼部响应函数（Ocular Response Functions，ORFs）进行建模，以刻画不同眼动事件——特别是扫视、眨眼和瞳孔扩张——对应的神经特征。我们揭示了眼部动作与神经活动之间的关系（编码过程），发现这些眼动事件发生前后存在一系列感觉皮层、小脑及额叶相关的神经特征。反过来，我们还展示了如何利用脑活动重建眼动事件，并进一步将基于静息态得到的ORF应用于被动聆听任务，表明一些原本被解释为直接与感觉相关的神经标记，原则上可能间接来源于眼动对任务相关神经处理的贡献。通过提供一个便于研究眼动与神经过程相互作用的框架，我们提出了一系列见解，具有广泛应用于认知神经科学与临床神经科学的潜力。

## Abstract
Oculomotor activity provides critical insights into cognition and health, with growing evidence demonstrating its involvement in various cognitive functions such as attention, memory, and sensory processing, and that it is a significant indicator of psychopathologies and neurological disorders. Despite its crucial importance across domains, the neural mechanisms supporting oculomotion have been underexplored, largely because eye movements are typically treated as artefacts to be removed from the neural signal. While useful for data cleaning, this approach risks discarding valuable information about oculomotor control, and there has been recent interest in modelling these signals instead to understand them. Using time-resolved regression methods with magnetoencephalography (MEG) and eye tracking during the resting state, we thus here sought to model Ocular Response Functions (ORFs), that characterise the neural signatures of distinct oculomotor events, specifically saccades, blinks, and pupil dilation. We demonstrate the relationships between ocular action and neural activity (encoding), revealing a range of sensory cortical, cerebellar and frontal signatures preceding and following such ocular events. We conversely show how we can reconstruct ocular events from brain activity, and further apply resting-state derived ORFs to a passive listening task - demonstrating how some neural markers interpreted as directly related to sensation may in principle indirectly result from oculomotor contributions to task-related neural processing. By providing an accessible framework for examining the interplay between eye movements and neural processes, we offer a range of insights with potential applications across cognitive and clinical neuroscience.