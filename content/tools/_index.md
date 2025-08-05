---
title: "Compliance Filtering Tool"
---

We provide a comprehensive tool to help the AI community filter training data in compliance with robots.txt restrictions. Our tool is designed to be easy to use while ensuring respect for content creators' wishe via robots.txt.



### Why Use This Tool?

- **Ethical AI Development**: Build models that respect content creators' rights
- **Legal Compliance**: Avoid potential copyright issues in your training data
- **Transparency**: Know exactly what data you're using

### Retrospective Compliance Filtering

We first rank domains based on the amount of data they provide to the corpus. Then, we select the top 1 million English domains and the top 1 million non-English domains. Some of these domains are now offline, and there is some overlap between the two lists. As a result, the total number of robots.txt files we could successfully download is much less than 2 million.

For every domain that is still reachable we retrieve the robots.txt file as of January 2025 and evaluate the rules that are relevant for AI training. Specifically, we look at the directives that apply to the AI-specific user agents listed below. 

```
"AI2Bot",                       # AI2  
"Applebot-Extended",            # Apple  
"Bytespider",                   # Bytedance  
"CCBot",                        # Common Crawl  
"CCBot/2.0",                    # Common Crawl  
"CCBot/1.0",                    # Common Crawl  
"ClaudeBot",                    # Anthropic  
"cohere-training-data-crawler", # Cohere  
"Diffbot",                      # Diffbot  
"Meta-ExternalAgent",           # Meta  
"Google-Extended",              # Google  
"GPTBot",                       # OpenAI  
"PanguBot",                     # Huawei  
"*"
```

## 🚫 Pre-filtered Domain Lists

We provide curated lists of URL domains that restrict AI crawlers in their robots.txt files. If any subdomain of a given domain disallows crawling by any AI training user agent, that domain is included in the list.

<div style="background: var(--code-bg); padding: 1.5em; border-radius: 8px; margin: 1em 0; border: 1px solid var(--border);">

#### 🇬🇧 English Corpus
**[Download English Blocked Domains](https://huggingface.co/datasets/swiss-ai/robots-txt-blocked-domains-english)** 🤗 - 487K+ blocked domains

#### 🌍 Multilingual Corpus  
**[Download Multilingual Blocked Domains](https://huggingface.co/datasets/swiss-ai/robots-txt-blocked-domains-multilingual)** 🤗 - 333K+ blocked domains

</div>



## 🔍 URL Compliance Checker

A single domain can host many sub‑domains—and each one may follow a different robots.txt policy. Our [`robots-checker`](https://pypi.org/project/robots-checker/1.2.3/) package lets you zoom in to the exact URL and instantly see whether it plays by the rules.

### Installation

```bash
pip install robots-checker==1.2.3
```

### Usage

```python
import url_checker
checker = url_checker.RobotsTxtComplianceChecker()
status = checker.is_compliant("https://blog.example.com/some-page")
print(status)   # ➜  "Compliant"  or  "NonCompliant"
```

Additionally, we offer fine-grained data filtering codes using the checker in our [github](https://github.com/swiss-ai/robots-txt-compliance), which is based on [Datatrove](https://github.com/huggingface/datatrove). 


## 🗂️ Document-wise Compliance Tag

Due to data distribution restrictions, we are unable to directly upload the filterd dataset, however, we provide a document-wise compliance tag for easy filtering. For each document in the FineWeb family, we tag it as either compliant or non-compliant.

<div style="background: var(--code-bg); padding: 1.5em; border-radius: 8px; margin: 1em 0; border: 1px solid var(--border);">

### 🍷 FineWeb Compliant Tag
**[swiss-ai/fineweb-compliant-tag](https://huggingface.co/datasets/swiss-ai/fineweb-compliant-tag)** 🤗

- Base Dataset: [HuggingFaceFW/fineweb](https://huggingface.co/datasets/HuggingFaceFW/fineweb) 🤗

</div>

<div style="background: var(--code-bg); padding: 1.5em; border-radius: 8px; margin: 1em 0; border: 1px solid var(--border);">

### 🥂 FineWeb2 Compliant Tag
**[swiss-ai/fineweb-2-compliant-tag](https://huggingface.co/datasets/swiss-ai/fineweb-2-compliant-tag)** 🤗

- Base Dataset: [HuggingFaceFW/fineweb-2](https://huggingface.co/datasets/HuggingFaceFW/fineweb-2) 🤗

</div>

<div style="background: var(--code-bg); padding: 1.5em; border-radius: 8px; margin: 1em 0; border: 1px solid var(--border);">

### 📚 FineWeb-Edu Compliant Tag
**[swiss-ai/fineweb-edu-compliant-tag](https://huggingface.co/datasets/swiss-ai/fineweb-edu-compliant-tag)** 🤗

- Base Dataset: [HuggingFaceFW/fineweb-edu](https://huggingface.co/datasets/HuggingFaceFW/fineweb-edu) 🤗

</div>

## 📄 Citation

```bibtex
@inproceedings{fan2025datacompliance,
  title={Can Performant LLMs Be Ethical? Quantifying the Impact of Web Crawling Opt-Outs},
  author={Fan, Dongyang and Sabolčec, Vinko and Ansaripour, Matin and 
          Tarun, Ayush Kumar and Jaggi, Martin and Bosselut, Antoine and Schlag, Imanol},
  booktitle={Conference on Language Modeling (COLM)},
  year={2025}
}
```