---
title: "Tools"
---

# Filtering Tools
We provide a tool designed to filter out data from URL domains that are restricted by robots.txt rules. This helps ensure compliance with web scraping policies by automatically excluding content from domains that prohibit crawler access.

Our curated URL lists are based on the FineWeb corpus. We identify the top 1 million URL domains and retrieve their corresponding robots.txt files as of January 2025. If any of the following crawlers are disallowed, we mark the associated data as blocked by robots.txt:

```
"AI2Bot",                        # AI2  
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

## Coarse-Grained Tool
We offer two URL domain lists. If any of the listed crawlers are blocked in a domain’s robots.txt file, the domain is added to the list. We offer the robotstxt blocked URL domains for both [English 🤗](https://huggingface.co/datasets/swiss-ai/robots-txt-blocked-domains-english) and [Multilingual 🤗](https://huggingface.co/datasets/swiss-ai/robots-txt-blocked-domains-multilingual) pretraining corpus. 

## Fine-Grained Tool
Since a single domain can include many subdomains—and not all subdomains necessarily follow the same robots.txt restrictions—we also support a more fine-grained filtering approach. (API to be added)