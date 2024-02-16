---
name: PoisonPy
paper: "Vulnerabilities in AI Code Generators: Exploring Targeted Data Poisoning Attacks"
pubvenue: 32nd IEEE/ACM International Conference on Program Comprehension
authors: D. Cotroneo, C. Improta, P. Liguori, R. Natella
paperlink: https://doi.org/10.1145/3643916.3644416
date: April 2024
link: https://github.com/dessertlab/Targeted-Data-Poisoning-Attacks
---

This dataset has been designed to perform a targeted data poisoning attack on AI code generators, leading them to generate vulnerable code. Each sample consists of a piece of Python code, and the corresponding description in natural language (English).

The dataset contains 823 unique pairs of code description--Python code snippet, including both safe and unsafe (i.e., containing vulnerable functions or bad patterns) code snippets. 

The detailed organization of the dataset is described in the [README.md](https://github.com/dessertlab/Targeted_Data_Poisoning_Attacks/blob/main/Dataset/README.md) file.

To build the dataset, we combined the only two available (at the time) benchmark datasets for evaluating the security of AI-generated code, [*SecurityEval*](https://doi.org/10.1145/3549035.3561184) and [*LLMSecEval*](https://doi.ieeecomputersociety.org/10.1109/MSR59073.2023.00084). Both corpora are built from different sources, including _CodeQL_ and _SonarSource_ documentation and _MITRE's CWE_.

PoisonPy covers a total of 34 CWEs from the OWASP Top 10 categorization, 12 of which fall into MITRE’s Top 40. 

In the paper, we used the dataset to assess the susceptibility of three AI code generators (Seq2Seq, CodeBERT, CodeT5+) to our targeted data poisoning attack.
