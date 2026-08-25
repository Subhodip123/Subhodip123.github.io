---
title: "📝 f-INE: Influence Estimation using Hypothesis Testing"
collection: publications
permalink: /publication/2025-07-18-f-ine-dataworld
excerpt: '🎯 A hypothesis-testing definition of influence that explicitly captures training-time randomness, enabling consistent estimation of the influence of training data in a single training run.'
date: 2025-07-18
venue: 'ICML 2025 Workshop on DataWorld: Unifying Data Curation Frameworks Across Domains'
authors: 'Subhodip Panda, Shashwat Sourav, Prathosh A. P., Sai Praneeth Reddy Karimireddy'
venue_short: 'ICML 2025'
year: 2025
type: 'workshop'
image: 'f-INE.drawio.png'
paperurl: 'https://icml.cc/virtual/2025/48726'
citation: ''
---
👥 **Co-authors:** [Shashwat Sourav](https://scholar.google.com/citations?user=sC-lJr4AAAAJ&hl=en), [Prathosh A.P](https://sites.google.com/view/prathosh/home), [Sai Praneeth Karimireddy](https://spkreddy.org/).

🔑 **Keywords:** data attribution, privacy, explainability.

![f-INE](/images/f-INE.drawio.png#right)

Understanding the influence of individual or groups of training examples on a model's predictions lies at the core of data valuation, attribution, debugging, and privacy. Yet, due to the inherent randomness and complexity of modern ML training pipelines, reliably measuring this influence remains elusive. In fact, we show that existing influence estimation methods fail to account for this, leading to highly inconsistent results — small changes in data ordering can result in drastically different influence estimates. Instead, we introduce **f-influence** — a new definition of influence grounded in hypothesis testing that explicitly captures training-time randomness. We define the influence of a data subset as the statistical ease of distinguishing between the outputs of models trained with and without that subset. We prove that f-influence satisfies desirable properties such as compositionality and asymptotic normality, analogous to central limit theorems. Leveraging these properties, we design a new algorithm **f-INfluence Estimation (f-INE)** that efficiently estimates the influence of training data *in a single training run*. Our approach is a theoretically sound, highly scalable, and empirically robust alternative to prior methods, enabling consistent influence estimation. ⏩ [Full Paper](https://icml.cc/virtual/2025/48726)
