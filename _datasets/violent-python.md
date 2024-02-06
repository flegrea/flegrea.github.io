---
name: Violent Python
paper: "AI Code Generators for Security: Friend or Foe?"
pubvenue: IEEE Security & Privacy Magazine
authors: R. Natella, P. Liguori, C. Improta. B. Cukic, D. Cotroneo
paperlink: https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10418104
date: February 2024
link: https://github.com/dessertlab/violent-python
---

This dataset has been designed for training and evaluating AI code generators for security. Each sample consists of a piece of Python code, and the corresponding description in natural language (English).

We built the dataset by using the popular book <i>Violent Python</i>, by T. J. O’Connor, which presents several examples of offensive programs using the Python language. The dataset covers multiple areas of offensive security, including penetration testing, forensic analysis, network traffic analysis, and OSINT and social engineering.

The dataset consists of 1,372 unique samples. We describe offensive code in natural language at granularity of individual lines, of groups of lines (blocks), and of entire functions.

In the paper, we used this dataset to experiment with three AI code generators (CodeBERT, Github Copilot, Amazon CodeWhisperer) at generating offensive Python code.
