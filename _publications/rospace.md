---
title: "ROSPaCe: Intrusion Detection Dataset for a ROS2-Based Cyber-Physical System and IoT Networks"
pubvenue: Scientific Data, Vol. 11.1, Article no. 481
authors: Tommaso Puccetti, Simone Nardi, Cosimo Cinquilli, Tommaso Zoppi, Andrea Ceccarelli
link: https://doi.org/10.1038/s41597-024-03311-2
date: May 2024
dataset: ROSPaCe
tags: iot ids
---
Most of the intrusion detection datasets to research machine learning-based intrusion detection systems (IDSs) are devoted to cyber-only systems, and they typically collect data from one architectural layer. Often the attacks are generated in dedicated attack sessions, without reproducing the realistic alternation and overlap of normal and attack actions. We present a dataset for intrusion detection by performing penetration testing on an embedded cyber-physical system built over Robot Operating System 2 (ROS2). Features are monitored from three architectural layers: the Linux operating system, the network, and the ROS2 services. The dataset is structured as a time series and describes the expected behavior of the system and its response to ROS2-specific attacks: it repeatedly alternates periods of attack-free operation with periods when a specific attack is being performed. This allows measuring the time to detect an attacker and the number of malicious activities performed before detection. Also, it allows training an intrusion detector to minimize both, by taking advantage of the numerous alternating periods of normal and attack operations.
