---
layout: archive
title: ""
permalink: experience/
author_profile: true
---

### Research Fellow, Microsoft Research, India <img style="float: right;" src="/images/microsoft.png" width="100">
<i>Advisor:</i> <a href="https://www.microsoft.com/en-us/research/people/padmanab/" style="color: black; text-decoration: underline;">Venkat Padmanabhan</a>
### HyWay

* Implemented face detection module to asynchronously detect faces from live video stream; telemetry module to extract and generate user-related analytics using Kusto Query Language
* Built an image-editing tool enabling users to create event spaces. The tool allows users to upload a custom image and edit it using drag/drop, group/ungroup, resize/rotate and duplicate different shapes (e.g., PowerPoint). The user actions are built using event listeners and use vector transformations. Implemented undo-redo functionality.
* **Performance Optimisations**: Fixed system memory leakage by performing in-place mutation instead of creating new objects for user actions. Migrated global variables from react state to redux store and reduced the number of re-renders. Maintained client synchronization using periodic server polling
* Our system hosted multiple internal events such as poster sessions supporting more than 300 users per session.

### Indoor User Localization and Representation
* Developed a computer-vision system to detect (YOLO), track (OCSORT), localize and represent (RetinaFace) multiple users present in an indoor environment using multiple cameras with non-overlapping views.
* Proposed an inter-camera matching algorithm to associate identical people across different camera viewpoints.
* Optimized an open-source face detection lib. (RetinaFace) and significantly reduced the total processing time
* Real world evaluations showed our mean inter-camera matching algorithm accuracy is around 90%, mean indoor localization error is 1.037m and the overall pipeline achieved 15 FPS, supporting real-time operations.

### Multi-Sensor User State Modeling for Distraction Detection

* Developed a windows-application for automatically determining whether a user is distracted or not during online meetings (e.g., Teams, Zoom etc..) in a privacy-preserving manner (user’s data shall not leave their device). The application collects data from multiple sources such as camera, microphone, speaker, and screen activity (e.g., mouse, keyboard) during the call.
* Implemented acoustic echo cancellation to filter local user’s speech using microphone and speaker streams.
* Proposed high-confidence rules to automatically generate supervised training data for distracted behavior.
* Our approach used temporal convolutional networks with resnet backbone for video-inputs and combined these predictions with rule-based outcomes for final predictions.
* This enabled different usecases such as: auto-mute A/V devices, recap missed-out content, meeting effectiveness.

Highlights:

* HyWay: Enabling Mingling in the Hybrid World got accepted into IMWUT / UbiComp 2023
* US Patent: "HYBRID ENVIRONMENT FOR INTERACTIONS BETWEEN VIRTUAL AND PHYSICAL USERS"
* Satya Nadella mentioned our project in the All Employees India Townhall!
* Bill Gates demoed our project in his visit to MSRI and got a [photo](https://www.linkedin.com/in/sirish-gambhira/overlay/background-image/)


### Data and Applied Scientist Intern, Microsoft <img style="float: right;" src="/images/microsoft.png" width="100">
<i>Advisor:</i> <a href="https://www.microsoft.com/en-us/research/people/vipinv/" style="color: black; text-decoration: underline;">Vipindeep Vangala</a>

* AI graph is a user-centric graph with user’s emails, meetings, documents as nodes and topics, associated people as edges. Developed a graph parsing algorithm to extract user’s topics and used heuristic scores to quantify user-topic relevance.
* Used Holt-Winters models for time-series analysis and visualized interactive spider & radar charts using D3.js

### Highlights:
* Obtained a Pre-Placement Offer (PPO) from the internship