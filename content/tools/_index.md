---
title: "Tools"
---

To quantify the impact of web crawling opt-outs, we developed a methodology centered around the **data compliance gap (DCG)**. This metric serves as a tool to evaluate how respecting `robots.txt` directives affects LLM performance.

### Data Compliance Gap (DCG)

The DCG is calculated as the performance difference between two models:

1.  A model trained on a dataset that **ignores** web crawling opt-outs (including data from sources that have a `robots.txt` disallow rule).
2.  A model trained on a **compliant** dataset that respects these opt-outs (excluding data from restricted sources).

A larger DCG indicates a greater performance loss when adhering to data compliance standards.

### Datasets

Our research utilized datasets derived from **Common Crawl**, a publicly available web crawl corpus. We curated two versions of a pre-training dataset to measure the DCG:

-   **Open-License Text:** This dataset contains content exclusively from domains with permissive licenses, fully compliant with web standards.
-   **Opt-Out Text:** This dataset includes content from domains that have explicitly opted out of web crawling via `robots.txt`.

By training models on different combinations of these datasets, we can isolate and measure the impact of data compliance on model capabilities in various domains. These datasets are foundational tools for our analysis. 