---
title: "Intrusion detection without attack knowledge: generating out-of-distribution tabular data"
pubvenue: IEEE 34th International Symposium on Software Reliability Engineering (ISSRE)
authors: A. Ceccarelli, T. Zoppi
link: https://doi.org/10.1109/ISSRE59848.2023.00058
date: October 2023
tags: ids
---
Anomaly-based intrusion detectors are machine learners trained to distinguish between normal and anomalous data. The normal data is generally easy to collect when building the train set; instead, collecting anomalous data requires historical data or penetration testing campaigns. Unfortunately, the first is most often unavailable or unusable, and the latter is usually expensive and unfeasible, as it requires hacking the target system. It turns out that the possibility of training an intrusion detector without attack knowledge, i.e., without anomalies, is attractive. This paper reviews strategies to train anomaly detectors in the absence of anomalies, from shallow machine learning to deep learning and computer vision approaches, and applies such strategies to the domain of intrusion detection. We experimentally show that training an intrusion detector without attack knowledge is effective when normal and attack data distributions are distinguishable. Detection performance severely drops in the case of complex (but more realistic) datasets, making all the existing solutions inadequate for real applications. However, the recent advancements of out-of-distribution research in deep learning and computer vision show interesting prospective results.
