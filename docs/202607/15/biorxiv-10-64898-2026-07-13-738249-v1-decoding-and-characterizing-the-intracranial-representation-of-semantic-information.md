---
title: Decoding and Characterizing the Intracranial Representation of Semantic Information
authors: "Smith, C., Inchyna, S., Barrentine, B., Nelson, M. J."
date: 2026-07-15
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.13.738249v1.full.pdf"
tags: ["query:q1"]
score: 7.5
evidence: 在语言任务中从人类皮层活动中解码高级语义表征
tldr: 研究语言处理任务期间用于解码语义信息的颅内神经活动。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738249-v1/fig-001.webp\", \"caption\": \"Table 1. Stimulus categories and their associated hierarchy.\", \"page\": 11, \"index\": 1, \"width\": 595, \"height\": 585}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738249-v1/fig-002.webp\", \"caption\": \"Figure 2. Schematic showing the 5 tasks studied.\", \"page\": 13, \"index\": 2, \"width\": 670, \"height\": 662}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738249-v1/fig-003.webp\", \"caption\": \"Figure 3. Single channel neural activity recorded in two locations from the same patient. (A) High levels of discrimination shown between animate semantic categories. (B) High levels of discrimination shown between inanimate categories. Both locations show separation between superordinate categories.\", \"page\": 20, \"index\": 3, \"width\": 893, \"height\": 914}]"
motivation: 在语言任务中从人类皮层活动中解码高级语义表征。
method: 方法与实现细节请参考摘要与正文。
result: 结果与对比结论请参考摘要与正文。
conclusion: 总体而言，该工作在所述任务上展示了有效性，并提供了可复用的思路或工具。
---

## Abstract
Brain-computer interfaces (BCIs) have achieved impressive performance by decoding motor and articulatory signals associated with speech production. However, considerably less is known about whether higher-level semantic representations can be decoded from human cortical activity. Demonstrating semantic decoding would advance both our understanding of language organization and the development of BCIs that rely on conceptual rather than purely articulatory information. We recorded intracranial neural activity from patients undergoing stereotactic electroencephalography (sEEG) for clinical epilepsy monitoring while they performed language tasks requiring semantic processing. High-gamma power was extracted from local field potentials and used to generate trial-level features for supervised machine-learning classification. Classification performance was evaluated using cross-validation. Semantic category information was decoded significantly above chance, with mean classification accuracy reaching 29.8% across 15 semantic categories (chance = 6.7%). These findings demonstrate that high-gamma activity contains information about conceptual category membership that can be extracted on individual trials. These results provide evidence that semantic information is accessible from intracranial population recordings and support the feasibility of semantic decoding as a complementary direction for future language BCIs. Beyond neuroprosthetic applications, this work contributes to understanding how conceptual knowledge is represented in the distributed human language network.