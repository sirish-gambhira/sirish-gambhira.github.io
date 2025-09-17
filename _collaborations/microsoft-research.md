---
title: "Microsoft Research India"
excerpt: "Research Engineer"
collection: collaborations
permalink: /collaborations/microsoft-research/
date: 2022-07-01
end_date: 2024-07-15
venue: "Microsoft Research India"
location: "Hyderabad, India"
keywords: Applied Computer Vision, Software Engineering
---

### Highlights
- **IMWUT/ACM UbiComp 2023**: [HyWay: Enabling Mingling in the Hybrid World](https://www.microsoft.com/en-us/research/publication/hyway-enabling-mingling-in-the-hybrid-world/)
- **Patent Filed**: US Patent application filed in July 2023
- **Bill Gates Demo**: Bill Gates personally demonstrated our project during his visit to Microsoft Research India
- **CEO Recognition**: Our work was praised by Satya Nadella during the All Employees India Townhall in January 2023

### HyWay: Hybrid Hallway

- Primary contributor to HyWay - an interactive communication platform for in-person and remote participants.
- Built an image editor powered by CosmosDB to create/edit event-spaces. Contributed to core-fixes such as memory-leakage:
in-place mutation of game-objects, re-renders: migration from react state to redux store.

### Indoor User Localization and Representation

- Developed a computer-vision system to detect, track, localize and represent using multiple cameras.
- Proposed an inter-camera matching algorithm to associate identical people across different camera viewpoints.
- Optimized an open-source face detection lib (RetinaFace) and significantly reduced the end-to-end processing time of our system.
- Real world evaluations showed our mean inter-camera matching algorithm accuracy is around 90%, mean indoor localization error
is 1.037m and the overall pipeline achieved 15 FPS, supporting real-time operations.

### Continual Learning for User State Modeling

- Developed a heuristic + ResNet based continual learning framework for determining whether a user is distracted or not using
multiple data sources in a privacy-preserving manner.
- Implemented a data-processing module to collect and synchronize data from multiple sensors (e..g, cam, mic, keyboard, screen).
- Implemented an acoustic echo cancellation module to facilitate usability of the tool in a headset-free setting.
- Proposed a continual learning framework to generate annotated video data on fly and trained a ResNet to model each user.