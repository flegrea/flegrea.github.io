---
title: "Fail-Controlled Classifiers: A Swiss-Army Knife Toward Trustworthy Systems"
pubvenue: Empirical Software Engineering
authors: Khokhar, F. A., Zoppi, T., Ceccarelli, A., Montecchi, L., & Bondavalli, A.
link: https://doi.org/10.1002/spe.70033
date: November 2025
tags: ids
---
**Background.** Modern critical systems often require to take decisions and classify data and scenarios autonomously without having detrimental effects on people, infrastructures or the environment, ensuring desired dependability attributes. Researchers typically strive to craft classifiers with perfect accuracy, which should be always correct and as such never threaten the encompassing system. Unfortunately, this is a very unrealistic goal, as classification tasks are typically complex and may encounter a wide variety of unexpected operating conditions and unknown inputs.

**Methods.** Classifiers should be considered as building blocks that interact with other components that help rejecting those predictions that are suspected to be misclassifications, triggering system-level mitigation strategies instead. Fail-Controlled Classifiers (FCCs) are software components that can either correctly classify, misclassify, or reject outputs: ideally, they would reject all and only outputs that correspond to misclassifications. Nine different FCCs are presented: Self-Checking Classifiers (SCC), Watchdog Timers (WT), Input Processor (IP), Output processor (OP), Safety Wrapper (SW), Recovery Blocks (RB), weighted and non-weighted Voting (VT, WVT) and Stacking (STK).

**Results.** These 9 FCCs are instantiated in experiments with tabular and image classifiers, showing their potential in rejecting most misclassifications and paving the ways for trustworthy decisions to be deployed in critical systems. If the system can tolerate more omissions, the IP FCC is a good choice. On the other hand, if achieving the highest accuracy is the priority, RB FCC performs better.

**Conclusions.** Findings show that FCCs do not primarily aim at improving correct classifications, but allow for transforming many misclassifications into rejections, which may be easily handled by the encompassing system and paving the way for trustworthy decisions to be deployed in critical systems.
