---
name: PowerShell Offensive Code Generation
paper: "The Power of Words: Generating PowerShell Attacks from Natural Language"
pubvenue: 18th USENIX WOOT Conference on Offensive Technologies (WOOT 24)
authors: P. Liguori, C. Marescalco, R. Natella, V. Orbinato, L. Pianese
paperlink: https://www.usenix.org/conference/woot24/presentation/liguori
date: August 2024
link: https://github.com/dessertlab/powershell-offensive-code-generation
---

This repo provides a replication package for the paper <b>The Power of Words: Generating PowerShell Attacks from Natural Language</b>, presented at the 18th USENIX WOOT Conference on Offensive Technologies (WOOT 2024).

![PowerShell Offensive Code Generation](https://raw.githubusercontent.com/dessertlab/powershell-offensive-code-generation/refs/heads/main/imagesmd/001.jpg)

In this paper, we present an extensive evaluation of state-of-the-art NMT models in generating PowerShell offensive commands.

We also contribute with a large collection of unlabeled samples of general-purpose PowerShell code to pre-train NMT models to refine their capabilities to comprehend and generate PowerShell code. Then we build a manually annotated labelled dataset consisting of PowerShell code samples specifically crafted for security applications which we pair with curated Natural language descriptions in English.

We use this dataset to pre-train and fine-tune:

- CodeT5+
- CodeGPT
- CodeGen

We also evaluate the model with:

- Static Analysis in which the generated code is assessed to ensure that it adheres to PowerShell programming conventions
- Execution Analysis which evaluates the capabilities of the generated offensive PowerShell code in executing malicious action

The project includes scripts and data to repeat the training/testing experiments and replicate evaluations.



