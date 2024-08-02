---
title: "The Power of Words: Generating {PowerShell} Attacks from Natural Language"
pubvenue: 18th USENIX WOOT Conference on Offensive Technologies (WOOT 24)
authors: P. Liguori, C. Marescalco, R. Natella, V. Orbinato, L. Pianese
link: https://www.usenix.org/conference/woot24/presentation/liguori
arxiv: https://arxiv.org/abs/2404.12893
date: August 2024
dataset: Powershell
---
As the Windows OS stands out as one of the most targeted systems, the \textit{PowerShell} language has become a key tool for malicious actors and cybersecurity professionals (e.g., for penetration testing). This work explores an uncharted domain in AI code generation by automatically generating offensive PowerShell code from natural language descriptions using Neural Machine Translation (NMT). For training and evaluation purposes, we propose two novel datasets with PowerShell code samples, one with manually curated descriptions in natural language and another code-only dataset for reinforcing the training. We present an extensive evaluation of state-of-the-art NMT models and analyze the generated code both statically and dynamically. Results indicate that tuning NMT using our dataset is effective at generating offensive PowerShell code. Comparative analysis against the most widely used LLM service ChatGPT reveals the specialized strengths of our fine-tuned models.