---
title: Changes in perceptual sampling contribute to representational drift
title_zh: 知觉采样的变化促进表征漂移
authors: "Yuan, Y., Aoi, M. C., Serences, J."
date: 2026-07-01
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.24.734121v2.full.pdf"
tags: ["query:q5"]
score: 6.5
evidence: 测量注视点偏移的纵向眼动追踪实验
tldr: 该研究探讨视觉皮层中的“表征漂移”是否可能由行为变化而非纯神经机制引起。研究者对14名受试者进行了持续2至4周的纵向眼动实验，分析其观看自然图像时的注视模式变化，并将注视遮罩后的图像输入CORnet-S视觉模型。结果发现，随着时间推移，注视分布逐渐漂移，并在模型各层引发表征距离显著增大，说明细微且持续的视觉采样变化足以造成表征漂移。
source: biorxiv
selection_source: fresh_fetch
motivation: 以往研究多将表征漂移归因于神经可塑性等内在机制，作者希望检验行为变化尤其是视线与注意漂移是否也会驱动这一现象。
method: 研究对14名成年人进行跨2至4周的纵向眼动实验，比较不同时间点的注视分布差异，并将注视遮罩后的图像输入CORnet-S模型评估神经表征距离变化。
result: 不同实验阶段之间的注视模式会随时间间隔增大而逐渐偏离，且这些变化能够在CORnet-S各视觉层级中产生显著增加的表征距离，并通过统计检验验证其显著性。
conclusion: 视觉场景采样方式会随时间系统性漂移，而这种行为层面的细微变化本身就可能导致视觉表征漂移，无需完全归因于神经回路内部重构。
---

## 摘要
对同一刺激的神经响应模式随时间逐渐发生变化的现象，被称为表征漂移（representational drift），这一现象已在多个皮层区域中被广泛观察到。表征漂移通常被归因于由突触可塑性或突触更新驱动的内在神经动力学。在本研究中，我们检验了一个互补性假设：表征漂移源于行为的系统性变化，例如注意力或凝视的转移。我们开展了一项纵向眼动追踪实验，14名成年人在持续2至4周的6个实验阶段中自由观看自然场景图像，其中部分图像在阶段内及阶段间重复呈现。对于每位参与者，我们利用Wasserstein距离量化不同阶段配对之间注视密度图的相似性。随着实验阶段时间间隔的增加，注视模式变得越来越不相似，表明凝视行为存在系统性且具有方向性的漂移。为评估这些行为变化是否足以诱发神经表征变化，我们将经过注视掩蔽处理的图像输入CORnet-S——一种模拟灵长类腹侧视觉通路的层级深度神经网络模型。通过成对激活差异的Frobenius范数所量化的表征距离，在模型的四个层级（V1、V2、V4、IT）中均随着注视图之间间隔实验阶段数量的增加而增大。基于核方法的最大均值差异（maximum mean discrepancy）检验进一步证实，表征距离的经验分布与随机打乱对照之间存在显著差异。这些发现表明，随着时间推移，对视觉场景采样方式中微小但系统性的变化，已足以导致视觉皮层中的表征漂移。更广泛地说，这些结果表明，即使在简单任务中，行为随时间发生细微变化也是不可避免的，而这些变化可能足以在不存在神经编码内在重构的情况下驱动表征漂移。

作者摘要：在关于视觉皮层表征漂移的研究中，在重复刺激呈现过程中注意力和凝视的变化，能够产生类似漂移的神经模式。尽管当前研究重点关注视觉采样变化对漂移的贡献，但结果也提出了一种可能性：其他许多难以量化的细微行为变化，也可能在其他领域驱动表征漂移。

## Abstract
Gradual changes in neural response patterns to the same stimulus over time, termed representational drift, have been widely observed across cortical areas. Drift is typically attributed to intrinsic neural dynamics driven by synaptic plasticity or turnover. Here we test a complementary hypothesis that drift arises due to systematic changes in behavior such as shifts in attention or gaze. We conducted a longitudinal eye-tracking experiment in which fourteen adults freely viewed naturalistic images across 6 experimental sessions spanning 2-4 weeks, with a subset of images repeated within and across sessions. For each participant, we quantified the similarity of fixation density maps between session pairs using the Wasserstein distance. Fixation patterns became increasingly dissimilar with greater temporal separation between sessions, indicating systematic and directional drift in gaze behavior. To assess whether these behavioral changes could plausibly induce changes in neural representations, we passed fixation-masked images through CORnet-S, a hierarchical deep neural network model of the primate ventral visual stream. Representational distances, quantified as the Frobenius norm of pairwise activation differences, increased with the number of sessions that separated the fixation maps across all four model layers (V1, V2, V4, IT). A kernel-based maximum mean discrepancy test further confirmed that the empirical distribution of representational distances differed significantly from shuffled controls. These findings suggest that small but systematic shifts in the sampling of a visual scene over time are sufficient to cause representational drift in visual cortex. More generally, these results suggest that subtle changes in behavior over time are inevitable, even in simple tasks, and that these changes may be sufficient to drive representational drift in the absence of intrinsic reconfigurations of neural codes.

Author summaryIn studies of representational drift in visual cortex, shifts in attention and gaze across repeated stimulus exposures can produce drift-like neural patterns. While the current focus is on contributions of changes in visual sampling to drift, the results raise the possibility that other subtle changes in behavior, many that are hard to quantify, could drive drift in other domains.