---
title: "About"
---

This project explores the impact of web crawling opt-outs on the performance of Large Language Models (LLMs). As more copyright holders restrict access to their online content, it's crucial to understand how these limitations affect the capabilities of AI models trained on web data.

Our research introduces the concept of the **data compliance gap (DCG)**, which measures the performance difference between models trained on datasets that respect web crawling opt-outs and those that do not.

### Key Findings

Our experiments with 1.5B parameter models (as of January 2025) show:

- **General Knowledge:** For general knowledge acquisition, there is a negligible data compliance gap (close to 0%). This suggests that general-purpose LLMs can be trained effectively using fully open data without a loss in performance.
- **Specialized Domains:** In specialized fields, such as biomedical research, excluding data from major publishers leads to a noticeable decline in model performance.

These findings indicate a trade-off between data compliance and model performance in specialized domains, suggesting that access to high-quality, copyrighted sources may be beneficial later in the training process. This study provides empirical data to inform future discussions on AI training practices and policy.

The research was conducted by Dongyang Fan, Vinko Sabolčec, Matin Ansaripour, Ayush Kumar Tarun, Martin Jaggi, Antoine Bosselut, and Imanol Schlag. 