---
title: "AMD"
excerpt: "AI Frameworks Intern"
collection: collaborations
permalink: /collaborations/amd/
date: 2025-05-01
end_date: 2025-08-08
venue: "AMD"
location: "San Jose, CA, USA"
keywords: Quantization, GPU Parallelism, Mixture-of-Experts
---

### Model Optimization
- Proposed and implemented multi-gpu based solutions for GPTQ quantization of MoE models and model evaluation
- Bypassed GIL in python for quantization of experts and distributed the computation among GPU devices using model parallelism
- Achieved 1.65x and 10x speedup in quantization of Qwen1.5-MoE-A2.7B & DeepSeek-R1 with 0.5% improvement in perplexity
- Implemented data parallelism, partitioning the evaluation dataset across ranks and achieved 5.01x speedup in evaluation time

