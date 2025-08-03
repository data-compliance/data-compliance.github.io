---
title: "Compliance Filtering Tool"
---

We provide a comprehensive tool to help the AI community filter training data in compliance with robots.txt restrictions. Our tool is designed to be easy to use while ensuring respect for content creators' wishe via Robots.txt.



## 🎯 Why Use This Tool?

- **Ethical AI Development**: Build models that respect content creators' rights
- **Legal Compliance**: Avoid potential copyright issues in your training data
- **Transparency**: Know exactly what data you're using

### Retrospective Compliance Filtering

 We identify the top 1 million URL domains and retrieve their corresponding robots.txt files as of January 2025. Based on the robots.txt content, we provide coarse-grained and fine-grained compliance filtering. By compliance filtering, we evaluates robots.txt rules specifically for AI training user agents, as shown in the list below. 

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

## 🚫 Coarse-Grained Filtering

### Pre-filtered Domain Lists

We offer curated lists of URL domains that restrict AI crawlers in their robots.txt files. These lists are based on the top 1 million URL domains from the FineWeb corpus, checked as of January 2025. If any of the sub-domains are restricted, the URL domain is added to the list. 

<div style="background: var(--code-bg); padding: 1.5em; border-radius: 8px; margin: 1em 0; border: 1px solid var(--border);">

#### 🇬🇧 English Corpus
**[Download English Blocked Domains](https://huggingface.co/datasets/swiss-ai/robots-txt-blocked-domains-english)** 🤗 - 487K+ blocked domains

#### 🌍 Multilingual Corpus  
**[Download Multilingual Blocked Domains](https://huggingface.co/datasets/swiss-ai/robots-txt-blocked-domains-multilingual)** 🤗 - 333K+ blocked domains

</div>




## 🔍 Fine-Grained Checking

### URL Compliance Checker

A single domain can host many sub‑domains—and each one may follow a different robots.txt policy. Our `robots-checker` package lets you zoom in to the exact URL and instantly see whether it plays by the rules.

### Installation

```bash
pip install robots-checker==1.2.0
```

### Usage

```python
import url_checker
checker = url_checker.RobotsTxtComplianceChecker()
status = checker.is_compliant("https://blog.example.com/some-page")
print(status)   # ➜  "Compliant"  or  "NonCompliant"
```

Additionally, we offer fine-grained data filtering codes in our [github](https://github.com/swiss-ai/robots-txt-compliance), which is based on [Datatrove](https://github.com/huggingface/datatrove). 


### Document-wise compliance tag

Due to data distribution restrictions, we are unable to directly upload the filterd dataset, however, we provide a document-wise compliance tag for easy filtering. For each document in the FineWeb family, we tag it as either compliant or non-compliant. 

## 📄 Citation

```bibtex
@inproceedings{fan2025compliance,
  title={Can Performant LLMs Be Ethical? Quantifying the Impact of Web Crawling Opt-Outs},
  author={Fan, Dongyang and Sabolčec, Vinko and Ansaripour, Matin and 
          Tarun, Ayush Kumar and Jaggi, Martin and Bosselut, Antoine and Schlag, Imanol},
  booktitle={Conference on Language Modeling (COLM)},
  year={2025}
}
```