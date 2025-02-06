---
title: "Better and safer autonomous driving with predicted object relevance"
pubvenue: IEEE 35th International Symposium on Software Reliability Engineering Workshops (ISSREW)
authors: A. Ceccarelli, L. Montecchi
link: https://doi.org/10.1109/ISSREW63542.2024.00099
arxiv: 
date: October 2024
dataset: "Object detection in autonomous driving"
---
Object detection in autonomous driving consists in perceiving and locating instances of objects in multi-dimensional data, such as images or LIDAR scans. Very recently, multiple works are proposing to evaluate object detectors by measuring their ability to detect the objects that are most likely to interfere with the driving task. Detectors are then ranked according to their ability to detect objects that are relevant, rather than the general accuracy of detection. However, there is little evidence so far that isolating the most relevant objects may contribute to improvements in the safety and effectiveness of the driving task. This paper defines and exercises a strategy to i) set-up and deploy object detectors that successfully extract knowledge on object relevance, and ii) use such knowledge to improve the trajectory planning task. We show that, given the output of an object detector, filtering objects based on their predicted relevance, in combination with the usual confidence threshold, improves the quality of trajectories produced by the downstream trajectory planner. We conclude the paper showing that information on object relevance should be further exploited and we sketch some directions for future work.

