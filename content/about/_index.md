---
title: "About the Data Compliance Project"
---


<div style="background: var(--code-bg); padding: 1.5em; border-left: 5px solid var(--primary); margin-bottom: 2em; border-radius: 0 8px 8px 0;">
<h2 style="margin-top: 0; color: var(--primary);">🇨🇭 Swiss AI Initiative</h2>
<p style="font-size: 1.1em; margin-bottom: 0.8em;">
This project was developed as part of the <a href="https://www.swiss-ai.org/" target="_blank">Swiss AI Initiative</a> to create compliant training data for Swiss AI models. Our goal is to ensure that Swiss AI development adheres to the highest ethical standards by respecting content creators' rights and web crawling restrictions.
</p>
<p style="margin-bottom: 0.8em;">
The Swiss AI Initiative is the largest open science/open source effort for AI foundation models worldwide, leveraging the world's most AI-capable supercomputer Alps by the National Supercomputing Center (CSCS) with over 10,000 GPUs of the new NVIDIA Grace Hopper superchip.
</p>
<p style="margin-bottom: 0;">
Supported by a grant from the Swiss National Supercomputing Centre (CSCS) under project ID a06 on Alps, we provide the tools and datasets necessary for training performant yet ethical language models in compliance with Swiss values of privacy, transparency, and respect for intellectual property.
</p>
</div>

## The Research Behind the Tool

This project was part of the research paper **"Can Performant LLMs Be Ethical? Quantifying the Impact of Web Crawling Opt-Outs"** presented at COLM 2025, specifically developed to support the Swiss AI data pipeline.

### 📚 The Context

The success of Large Language Models (LLMs) heavily depends on web-scale data. However, as data becomes an increasingly valuable business asset, more content owners are restricting access through robots.txt files. This raises critical questions:

- Can we build high-performing AI systems while respecting data usage restrictions?
- What is the actual impact of excluding copyrighted content from training data?
- Which domains are most affected by compliance requirements?

### 🔬 Our Approach

We introduce the Data Compliance Gap (DCG), a metric that quantifies the performance difference between:

1. **Compliant models**: Trained exclusively on data that respects robots.txt opt-outs
2. **Non-compliant models**: Trained on all available web data

We measure DCG in two settings:
- **Pre-training from scratch**: Training models entirely on compliant vs. non-compliant data
- **Continual pre-training**: Integrating restricted data at later training stages

### 🎯 Key Findings

Our experiments with 1.5B parameter models reveal:

#### General Knowledge ✅
Near-zero DCG for models trained on fully open data perform comparably to those trained on all data. Even if all news publishers opt out, the impact remains minimal. Factual knowledge is often available from multiple sources and republications.

#### Specialized Domains ⚠️
Notable performance gaps appear in:
- **Biomedical research**: Major publishers' opt-outs affect domain-specific knowledge
- **Structural knowledge**: Information from tables, lists, and databases
- **Adversarial robustness**: Resistance to falsified or misleading information

#### Memorization Trade-offs ✍️
Compliant training reduces verbatim memorization of copyrighted content. However, it also limits acquisition of specific knowledge from restricted sources.

### 💡 Implications

Our findings suggest that General-purpose LLMs can be trained ethically without sacrificing overall performance. Specialized applications may require careful consideration of data sources. Overall, we believe that the AI community needs tools to navigate compliance requirements effectively.

### 🌟 Why This Matters

As the debate around AI and copyright continues, empirical evidence is crucial. Our research provides data on the trade-offs between compliance and performance, helping inform AI development practices and standards for ethical AI training.

### ⚖️ License - TODO
All datasets and tools are released under **TODO** license.

---

📄 [**Read the full paper →**](https://arxiv.org/abs/2504.06219)

🛠️ [**Get started with the tool →**](/tools/)

🗂️ [**Compliant Indexing →**](/datasets/)

👥 [**Meet the team →**](/team/)