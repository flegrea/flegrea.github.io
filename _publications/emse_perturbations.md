---
title: "Enhancing robustness of AI offensive code generators via data augmentation"
pubvenue: Empirical Software Engineering
authors: C. Improta, P. Liguori, R. Natella, B. Cukic, D. Cotroneo
link: https://doi.org/10.1007/s10664-024-10569-y
arxiv: https://arxiv.org/abs/2306.05079
date: October 2024
dataset: Robustness of AI Code Generators
tags: ai-code-generators
---
Since manually writing software exploits for offensive security is time-consuming and requires expert knowledge, AI-base code generators are an attractive solution to enhance security analysts’ productivity by automatically crafting exploits for security testing. However, the variability in the natural language and technical skills used to describe offensive code poses unique challenges to their robustness and applicability. In this work, we present a method to add perturbations to the code descriptions to create new inputs in natural language (NL) from well-intentioned developers that diverge from the original ones due to the use of new words or because they miss part of them. The goal is to analyze how and to what extent perturbations affect the performance of AI code generators in the context of offensive code. First, we show that perturbed descriptions preserve the semantics of the original, non-perturbed ones. Then, we use the method to assess the robustness of three state-of-the-art code generators against the newly perturbed inputs, showing that the performance of these AI-based solutions is highly affected by perturbations in the NL descriptions. To enhance their robustness, we use the method to perform data augmentation, i.e., to increase the variability and diversity of the NL descriptions in the training data, proving its effectiveness against both perturbed and non-perturbed code descriptions.
