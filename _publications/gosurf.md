---
title: "GoSurf: Identifying Software Supply Chain Attack Vectors in Go"
pubvenue: ACM Workshop on Software Supply Chain Offensive Research and Ecosystem Defenses (SCORED)
authors: Carmine Cesarano, Vivi Andersson, Roberto Natella, Martin Monperrus
link: https://doi.org/10.1145/3689944.3696166
date: November 2024
dataset: GoSurf
tags: apt static-analysis
---
In Go, the widespread adoption of open-source software has led to a flourishing ecosystem of third-party dependencies, which are often integrated into critical systems. However, the reuse of dependencies introduces significant supply chain security risks, as a single compromised package can have cascading impacts. Existing supply chain attack taxonomies overlook language-specific features that can be exploited by attackers to hide malicious code. In this paper, we propose a novel taxonomy of 12 distinct attack vectors tailored for the Go language and its package lifecycle. Our taxonomy identifies patterns in which language-specific Go features, intended for benign purposes, can be misused to propagate malicious code stealthily through supply chains. Additionally, we introduce GoSurf, a static analysis tool that analyzes the attack surface of Go packages according to our proposed taxonomy. We evaluate GoSurf on a corpus of 500 widely used, real-world Go packages. Our work provides preliminary insights for securing the open-source software supply chain within the Go ecosystem, allowing developers and security analysts to prioritize code audit efforts and uncover hidden malicious behaviors.
