---
layout: project
title: ABR-Arena
subtitle: Into the Wild Real-World Testing for ML-Based ABR
permalink: /projects/2025_into_the_wild.html
---
<h5>Abstract</h5>

<p>
Machine learning (ML)-based Adaptive Bitrate (ABR) algorithms often struggle to bridge the gap between simulation and reality. Their strong performance in synthetic environments frequently fails to generalize to real-world conditions. Researchers have therefore begun testing these algorithms over the Internet to incorporate real-world feedback into their design. In this paper, we show that since network conditions vary significantly across the globe, testing in individual real-world environments can suffer from the same generalization issues as lab-based testing. Existing testing platforms face (and might even be oblivious to) this limitation because they cover a small geographical region and rely on a narrow set of users affected by survivorship bias. As a result, their insights on an algorithm's performance generalize poorly to other deployments across the Internet, hindering the widespread adoption of ML-based ABR methods in practice. 

To address this gap, we present ABR-Arena, a global testing platform that enables researchers to evaluate the performance of ABR algorithms across a diverse set of regions around the globe. As a result of its worldwide coverage, ABR-Arena can reveal the performance shortcomings of several state-of-the-art ML-based approaches. It is extensible and easy to deploy in additional locations. We will make ABR-Arena available to the community to support the development of new ML-based approaches and to facilitate meaningful improvements to existing algorithms.
</p>

<h5>ABR-Arena</h5>
ABR-Arena is a Python-based testing infrastructure for the efficient evaluation and comparison of ABR algorithm performance across diverse real-world environments (see the figure below). By containerizing streaming servers and deploying them to cloud instances worldwide, we design ABR-Arena to be easy to use and to extend to new locations. We mitigate the impact of survivorship bias on our data by not relying on returning users, but rather stream to random users sourced via Amazon Mechanical Turk (MTurk), a popular crowdsourcing marketplace.

<h5>Results</h5>


<h5>Citation</h5>
<p>
<b>Benjamin Hoffman</b>, Alexander Dietmüller, Ayush Mishra, Laurent Vanbever. PACMI@SOSP, 2025.
</p>
