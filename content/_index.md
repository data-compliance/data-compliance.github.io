---
title: "Data Compliance"
---

# Can Performant LLMs Be Ethical?


<div style="text-align: center; background: var(--code-bg); padding: 1em; border-radius: 8px; margin: 1em 0; border: 1px solid var(--border);">
<strong>Developing Compliant LLM Training Data Respecting Content Owners Opt-out</strong>
</div>

<div style="text-align: center; margin: 1.5em 0;">
<div style="display: inline-flex; gap: 1em; flex-wrap: wrap; justify-content: center;">
<a href="https://arxiv.org/abs/2504.06219" target="_blank" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); color: white; padding: 12px 24px; text-decoration: none; border-radius: 8px; display: inline-flex; align-items: center; gap: 8px; font-weight: 600; box-shadow: 0 4px 15px rgba(102, 126, 234, 0.3); transition: transform 0.2s, box-shadow 0.2s;">
📄 Paper
</a>
<a href="#todo-github" style="background: linear-gradient(135deg, #24292e 0%, #1f2328 100%); color: white; padding: 12px 24px; text-decoration: none; border-radius: 8px; display: inline-flex; align-items: center; gap: 8px; font-weight: 600; box-shadow: 0 4px 15px rgba(36, 41, 46, 0.3); transition: transform 0.2s, box-shadow 0.2s;">
🐙 GitHub - TODO
</a>
<a href="https://huggingface.co/collections/swiss-ai/robots-txt-688d64b8e78f8c16284cf2e2" target="_blank" style="background: linear-gradient(135deg, #ff6b35 0%, #f7931e 100%); color: white; padding: 12px 24px; text-decoration: none; border-radius: 8px; display: inline-flex; align-items: center; gap: 8px; font-weight: 600; box-shadow: 0 4px 15px rgba(255, 107, 53, 0.3); transition: transform 0.2s, box-shadow 0.2s;">
🤗 Hugging Face
</a>
</div>
</div>

### 🎯 The Challenge

As more content owners opt-out of web crawling for AI training, a critical question emerges: **Can we build high-performing language models while respecting data usage restrictions?**


### 🛠️ Contribution

<div style="background: var(--entry); padding: 1.5em; border-radius: 8px; margin: 1em 0; border: 1px solid var(--border);">

We provide open-source tools and datasets to help the AI community:

- Check URL compliance and filter training data to respect robots.txt restrictions
- Compliant indexing of popular datasets (FineWeb, FineWeb2, FineWeb-Edu)
- 487K+ English and 333K+ multilingual domains that restrict AI crawlers

</div>

### 📊 Our Research

We introduce the Data Compliance Gap (DCG), a metric that quantifies the performance difference between:
<ul style="margin: 0.5em 0; list-style-type: none;">
<li>✅ Compliant models, trained only on data that respects robots.txt opt-outs.</li>
<li>❌ Non-compliant models, trained on all available web data.</li>
</ul>

### 🔍 Key Findings

**General Knowledge**: Close to 0% DCG, LLMs can achieve comparable performance using only openly available data

**Specialized Domains**: Noticeable gaps in areas like:
<ul style="margin: 0.5em 0; list-style-type: none;">
<li>🏥 Biomedical research</li>
<li>📰 Structural knowledge formats</li>
<li>🛡️ Robustness against adversarial examples</li>
</ul>

### Available Indices & Resources


<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 1em; margin: 2em 0;">

<div style="background: var(--code-bg); padding: 1.5em; border-radius: 8px; border: 1px solid var(--border);">
<h4>🗂️ Compliant Indexing</h4>
<p>Indices of compliant documents that respect robots.txt for FineWeb family datasets:</p>
<ul style="margin: 0.5em 0; list-style-type: none;">
<li><strong>🍷 FineWeb</strong></li>
<li><strong>🥂 FineWeb2</strong></li>
<li><strong>📚 FineWeb-Edu</strong></li>

</ul>
<a href="/datasets/" style="color: var(--primary);">Browse Indexings →</a>
</div>

<div style="background: var(--code-bg); padding: 1.5em; border-radius: 8px; border: 1px solid var(--border);">
<h4>🚫 Blocked Domain Lists</h4>
<p>Comprehensive lists of restricted domains:</p>
<ul style="margin: 0.5em 0;">
<li><strong>487K+ English domains</strong></li>
<li><strong>333K+ Multilingual domains</strong></li>
</ul>
<a href="/tools/#-coarse-grained-filtering" style="color: var(--primary);">Access Lists →</a>
</div>

</div>

<div style="text-align: center; margin: 2em 0;">
<a href="/tools/" style="background: var(--primary); color: var(--theme); padding: 12px 24px; text-decoration: none; border-radius: 5px; display: inline-block;">Get Started with Tool →</a>
</div>