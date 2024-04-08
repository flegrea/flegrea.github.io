---
title: Workshop on AI for addressing Advanced Persistent Threats (AI-APT)
subtitle: |-
    co-located with the Italian Conference on Cybersecurity (ITASEC24)
    April 8th, 2024, Salerno, Italy
---

# Motivation and background

Cyber-attacks have become a severe threat for critical services in several domains, such as healthcare, manufacturing, telecom, energy, transportation, where the impact can be exceedingly high (e.g., in terms of service outages, private data breaches, intellectual property theft). Modern attacks are today very challenging, as they evolved into "Advanced Persistent Threats" (APTs). APT actors are typically cybercriminal or state-sponsored groups, which perform carefully-planned, stealthy attacks that span over a long period of time. A well-known example is the Stuxnet attack, which has been sabotaging Iran's nuclear centrifuges since 2005, and was uncovered in 2010.

Unfortunately, the APT threat landscape is continuously evolving, as attackers develop new tactics and techniques. This trend puts both researchers and organizations at disadvantage, since it is difficult for them to stay up-to-date with emerging APT attacks. Moreover, most organizations are unwilling to share data about attacks they have experienced, because of concerns about disclosing sensitive data. This is a huge opportunity loss, both for the scientific community and for the organizations themselves: scientists are unable to assess new countermeasures on real-world attacks, which hinders scientific progress; organizations are unable to timely update their attack detectors against emerging APT campaigns.

This workshop aims to provide a forum for researchers from academia and industry about the use of AI to address these challenges, with emphasis on Generative AI. Recent advances in Generative AI, such as Large Language Models, provides a valuable opportunity to generate new representative datasets of APT attacks, without forcing organizations to disclose their sensitive information.

# Workshop program

<table>
  <tr>
    <td nowrap="nowrap">10:00 - 10:15</td>
    <td><b>Introduction</b></td>
  </tr>
  <tr>
    <td nowrap="nowrap">10:15 - 10:35</td>
    <td><b>Analyzing Cyber Threat Intelligence for Adversary Emulation</b><br/>D. Cotroneo, R. Natella, V. Orbinato, L. Pianese - U. Napoli Federico II<br/><details><summary>Abstract</summary>Nowadays, organizations are facing sophisticated cybersecurity attacks, known as Advanced Persistent Threats (APTs), in terms of the number of stages and variety of techniques. Knowledge about APTs can be gained from sources of Cyber Threat Intelligence (CTI), such as incident reports and leaked documents. Unfortunately, these sources are often in unstructured natural language and are not actionable for automated testing of cybersecurity defenses (Adversary Emulation). This work investigates Machine Learning (ML) techniques to extract CTI from unstructured sources to support Adversary Emulation. We analyze several ML models and strategies and evaluate their accuracy on real-world CTI documents. The experimental results show that the best accuracy can be achieved by fine-tuning Large Language Models (LLM) with our dataset of CTI, in combination with sentence clustering and summarization.</details></td>
  </tr>
  <tr>
    <td nowrap="nowrap">10:35 - 10:55</td>
    <td><b>Measuring attack latency of anomaly detectors: Definition of target metrics and construction of datasets</b><br/>A. Ceccarelli, T. Puccetti - U. Firenze<br/><details><summary>Abstract</summary>The ever-evolving landscape of attacks, coupled with the growing complexity of ICT systems, makes crafting anomaly-based intrusion detectors (ID) a difficult task: they must accurately detect attacks, and they should promptly perform detections. Although improving and comparing the detection capability is the focus of most research works, the timeliness of the detection is less considered and often insufficiently evaluated or discussed. In this presentation, we argue the relevance of measuring the temporal latency of attacks, and we propose an evaluation approach for detectors to ensure a pragmatic trade-off between correct and in-time detection. Briefly, the approach relates the false positive rate with the temporal latency of attacks and errors, and this ultimately leads to guidelines for configuring a detector. We apply our approach by evaluating different solutions in two industrial cases: i) an embedded railway on-board system that optimizes public mobility, and ii) an edge device for the Industrial Internet of Things. Our results show that considering latency in addition to traditional metrics like the false positive rate, precision, and coverage gives an additional fundamental perspective on the actual performance of the detector and should be considered when assessing and configuring anomaly detectors.</details></td>
  </tr>
  <tr>
    <td nowrap="nowrap">10:55 - 11:30</td>
    <td>Break</td>
  </tr>
  <tr>
    <td nowrap="nowrap">11:30 - 11:50</td>
    <td><b>Towards Robotpsychlogy: new exploitation opportunities for AI's subtle prejudices</b><br/>G. Costa, M. Cerreta - IMT Lucca<br/><details><summary>Abstract</summary>Machine Learning includes several powerful techniques that are revolutionizing our society in many ways. As a result, several activities that once were regarded as prerogatives of the human brain, can now be delegated to computers. The main promise is that these algorithms are free from many flaws typical of the human nature.  In this talk we will discuss this assumption and show that, in fact, some critical weaknesses of human beings are also affecting ML, perhaps in new, surprising and subtle ways. Moreover, we will understand some of the reasons why these mistakes are difficult to be spotted out and possible techniques to detect them.</details></td>   
  </tr>
  <tr>
    <td nowrap="nowrap">11:50 - 12:10</td>
    <td><b>Transformer or Autoencoder? Who is the ultimate adversary for attack detectors?</b><br/>S. Laudanna, A. Di Sorbo, P. Vinod, C.A. Visaggio, G. Canfora - U. Sannio<br/><details><summary>Abstract</summary>In recent years, Machine Learning (ML) approaches have been widely adopted for computer security tasks, including network intrusion detection and malware detection. However, linear and non-linear MLbased classifiers are vulnerable to adversarial examples created to deceive the classifiers. Generative Adversarial Networks (GAN) are architectures based on neural networks capable of successfully producing adversarial samples. In this study, we compare the performance of two GAN architectures based on either Transformer or Autoencoder networks in two distinct domains: Network Intrusion Detection Systems (NIDS) and mobile malware detection. We aim to evaluate their performance in terms of both effectiveness (i.e., the ability of the GAN-generated samples to reduce the detection rate of the targeted classifier) and efficiency (i.e., the capability of achieving the desired goal with fewer training epochs). Our findings reveal that the Transformerbased GAN outperforms the Autoencoder-based GAN, generating high-quality adversarial samples able to deceive both ML-based NIDS and ML-based malware detectors. Furthermore, in both scenarios, the Transformerbased architecture achieves a high deception efficacy through a reduced number of training epochs. This research sheds light on the relevance of GAN architectures, particularly Transformer-based models, and the need to consider samples produced by this architecture for improving the robustness of ML-based security solutions.</details></td>
  </tr>
  <tr>
    <td nowrap="nowrap">12:10 - 12:30</td>
    <td><b>Handling cyber risks through an automated approach for control-based mitigation identification</b><br/>S. Bonomi, M.P. Carello, L. Querzoni - U. Roma La Sapienza<br/><details><summary>Abstract</summary>Identifying, assessing and managing cyber risks is a critical task for managing the overall cyber security of every company. The risk management process is currently well defined and supported by several standards and guidelines but it currently requires a significant effort from human operators that manually analyze vulnerabilities, identify the related risks and define the most appropriate treatment to contain the organization exposure to cyber attacks. Thus, the current implementation of the process is time consuming and requires well experienced analyst. Recently, some MAPE-K based Architectures have been proposed to partially automate the risk management process but they still rely on a preconfigured list of mitigation actions that need to be defined by humans. In our research, we take a step in this direction and we propose a method to (semi)-automatically identify and suggest the implementation of specific security controls with the aim of mitigating the identified risks. To this aim, we rely on two NLP models, based on the BERT architecture, to quantify the relevance of security controls to solve specific vulnerabilities and it turns to reduce the overall risk level.</details></td>
  </tr>
  <tr>
    <td nowrap="nowrap">12:30 - 12:50</td>
    <td><b>Will individuals believe AI's threat intelligence?</b><br/>F. Massacci, S. Van Gerwen, K. Tuma - U. Trento/Vrije Universiteit<br/><details><summary>Abstract</summary>The uncertainty that comes with diverse intelligence sources leaves room for biased judgements, which is still not well understood. We present a controlled experiment with two groups of participants, one who is knowledgeable of the security domain and one that is knowledgeable of the AI domain to measure the bias introduced by the source of intelligence (human vs algorithmic). Each of the 𝑛 = 19 + 21 participants analyzed eight threat intelligence reports from the Dutch National Cyber Security Center where a final recommendation was manipulated as for coming from a human expert or an AI algorithm. Our findings revealed that the type of source had only an impact on the agreement with a recommendation when knowledge of the AI domain was present. The perceived bias significantly differed only when knowledge about the decision domain was present. The difference in knowledge by the groups yielded a skewed preference for AI (for the security group) and for humans (for the AI group) but not significantly. This work is supported by the NWO KIC project HEWSTI and the European Project Sec4AI4Sec.
</details></td>
  </tr>
  <tr>
    <td nowrap="nowrap">12:50 - 13:00</td>
    <td><b>Conclusion</b></td>
  </tr>
</table>


# Call for talks (expired)

The workshop is open to <b>your proposal for a talk</b> at the workshop. To submit a proposal, please send an email to the organizers (see below), with subject <i>"[ITASEC 24] Workshop Talk Proposal"</i>. Please include a title, abstract, and biography of the speaker(s). Please submit your proposal by March 17, 2024.

Proposals will be evaluated based on the relevance and timeliness of the proposed topic, on the potential impact of insights and results on the research community, and on the background and experience of the speakers.

We do not require the submission of papers for the workshop, in order to also include presentations of early-stage ideas and results that are not yet mature for publication. The workshop will aim for lightweight exchange of ideas and networking.


# Topics of interest

Topics of interest include, but are not limited to:
<ul>
<li>Generative AI for cybersecurity datasets (logs, network traces, exploits, payloads, and others)</li>
<li>Privacy-preserving techniques for sharing cybersecurity datasets</li>
<li>Generative AI for training and evaluation of attack detectors</li>
<li>Generative AI for incident handling and response</li>
<li>Generative AI for cybersecurity training and cyber-ranges</li>
<li>Applications of Generative AI for IT/OT cybersecurity</li>
<li>Benchmarks and experiments on Generative AI for cybersecurity</li>
<li>Practical case studies</li>
</ul>



# Attending the workshop

The workshop will be held in conjunction with the Italian Conference on Cybersecurity (ITASEC), on April 8th, 2024. Participants need to register to the conference, either for just the day of the workshop (one-day registration) or for the full period of the conference (April 8-12). For more information about the conference, please refer to <a href="https://itasec.it">https://itasec.it</a>.


# Technical Programme Committee

Organizers:
<ul>
<li>Roberto Natella, Università di Napoli Federico II (roberto.natella AT unina.it)</li>
<li>Andrea Ceccarelli, Università di Firenze (andrea.ceccarelli AT unifi.it)</li>
<li>Massimo Ficco, Università di Salerno (mficco AT unisa.it)</li>
</ul>


