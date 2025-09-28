---
title: "Detection Latencies of Anomaly Detectors - An Overlooked Perspective?"
pubvenue: IEEE 35th International Symposium on Software Reliability Engineering (ISSRE)
authors: T. Puccetti, A. Ceccarelli
link: https://doi.org/10.1109/ISSRE62328.2024.00015
arxiv: 
date: October 2024
dataset: "Detection Latencies of Anomaly Detectors"
tags: ids
---
The ever-evolving landscape of attacks, coupled with the growing complexity of ICT systems, makes crafting anomaly-based intrusion detectors and error detectors difficult: they must accurately detect attacks and promptly perform detections. Although improving and comparing the detection capability is the focus of most research works, the timeliness of the detection is less considered and often insufficiently evaluated or discussed. In this paper, we argue the relevance of measuring the temporal latency of attacks and errors, and we propose an evaluation approach for detectors to ensure a trade-off between correct and in-time detection. Briefly, the approach relates the false positive rate with the temporal latency of attacks and errors, ultimately leading to guidelines for configuring a detector. We apply our approach by evaluating different intrusion and error detectors in two industrial cases: i) an embedded railway on-board system that optimizes public mobility, and ii) an edge device for the Industrial Internet of Things. Our results show that considering latency in addition to traditional metrics like the false positive rate, precision, and coverage gives an additional fundamental perspective on the actual performance of the detector and should be considered when assessing and configuring anomaly detectors.
