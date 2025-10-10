---
layout: project
title: ABR-Arena
subtitle: Into the Wild – Real-World Testing for ML-Based ABR
permalink: /projects/2025_into_the_wild.html
---

<p style="text-align: center; margin-bottom: 30px;">
<b>Benjamin Hoffman</b>, Alexander Dietmüller, Ayush Mishra, Laurent Vanbever<br/>
<i>ETH Zürich</i><br/>
PACMI@SOSP, 2025
</p>

**Abstract.**
Machine learning (ML)-based Adaptive Bitrate (ABR) algorithms often struggle to bridge the gap between simulation and reality. Their strong performance in synthetic environments frequently fails to generalize to real-world conditions. Researchers have therefore begun testing these algorithms over the Internet to incorporate real-world feedback into their design. In this paper, we show that since network conditions vary significantly across the globe, testing in individual real-world environments can suffer from the same generalization issues as lab-based testing. Existing testing platforms face (and might even be oblivious to) this limitation because they cover a small geographical region and rely on a narrow set of users affected by survivorship bias. As a result, their insights on an algorithm's performance generalize poorly to other deployments across the Internet, hindering the widespread adoption of ML-based ABR methods in practice. 
<br/> &nbsp;&nbsp;&nbsp;&nbsp;
To address this gap, we present ABR-Arena, a global testing platform that enables researchers to evaluate the performance of ABR algorithms across a diverse set of regions around the globe. As a result of its worldwide coverage, ABR-Arena can reveal the performance shortcomings of several state-of-the-art ML-based approaches. It is extensible and easy to deploy in additional locations. We will make ABR-Arena available to the community to support the development of new ML-based approaches and to facilitate meaningful improvements to existing algorithms.

**ABR-Arena.** <br/>
ABR-Arena is a Python-based testing infrastructure for the efficient evaluation and comparison of ABR algorithm performance across diverse real-world environments (see the figure below). By containerizing streaming servers and deploying them to cloud instances worldwide, we design ABR-Arena to be easy to use and to extend to new locations. We mitigate the impact of survivorship bias on our data by not relying on returning users, but rather stream to random users sourced via Amazon Mechanical Turk (MTurk), a popular crowdsourcing marketplace.

{%
	include image_with_caption.html
	url="/assets/projects/2025_into_the_wild/abr_arena_diagram.jpg"
	width="100%"
%}

**Results.** <br/>
Overall, our results highlight both the value and necessity of ABR-Arena: QoE performance varies significantly across real-world environments, and comparisons with prior work reveal how much ML-based ABR performance can diverge between training and deployment. A reliable evaluation of these algorithms can only be done by testing them across diverse regions with varying network conditions.

{%
	include image_with_caption.html
	url="/assets/projects/2025_into_the_wild/results.jpg"
	width="100%"
%}

**Availability.** <br/>
We will open-source ABR-Arena to facilitate the development of new ML-based ABR algorithms and to enable meaningful improvements to existing algorithms. We are currently cleaning up all of our code and documenting every step to make it as easy to replicate and build as possible.

**Citation.** <br/>
```
@inproceedings{hoffman2025into,
  title={Into the Wild: Real-World Testing for ML-Based ABR},
  author={Hoffman, Benjamin and Dietm{"u}ller, Alexander and Mishra, Ayush and Vanbever, Laurent},
  booktitle={PACMI '25: Proceedings of the 4th Workshop on Practical Adoption Challenges of ML for Systems},
  year={2025}
}
```
