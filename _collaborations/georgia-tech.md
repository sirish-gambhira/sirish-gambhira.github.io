---
title: "Georgia Tech - SAIL Lab"
excerpt: "Student Researcher"
collection: collaborations
permalink: /collaborations/georgia-tech/
date: 2024-08-01
venue: "Georgia Institute of Technology"
location: "Atlanta, GA, USA"
gpa: 4.0/4.0
keywords: "LLM Inference Optimizations, GPU Programming"
---

### Vajra: Serving System For Next-Gen AI Workloads
- Implemented support to serve FP8 quantized models
- Designed a custom weight loader to read fp8 quantized weights. Implemented custom kernels to dequantize and requantize loaded
weights. Utilized flashinfer kernels to perform the forward pass

### KV optimization for disaggregated LLM inference 
- Disaggregated prefill and decode stages of LLM inference using two different LLMs (e.g., Llama-3-3B and Llama-3-1B)
- Created a hybrid network using ‘stitch-layers‘ to transfer KV cache between prefill and decode during inference
- Two stage training: a) stitch-layer warmup between the predicted and actual KV caches b) end-to-end LoRA based finetuning.
- Observed interpolation in rogue scores for different LLM series (e.g., Llama, Qwen, Minitron)


### SEAM: Stitchable Efficient Architectures for ResNet Models 
- Created intermediate architectures using stitching and interpolated the compute, performance of ResNet34 and ResNet50
- 92.16% of our stitches achieved interpolation upon fine-tuning the end-to-end network on ImageNet
- Served lighter competitive models compared to baselines 100% of the time for a given accuracy constraint

### Caching policies using L2 persistence for DNN inference 
- Started with hypothesis that default hardware caching policy is sub-optimal for weight-shared DNNs inference (metric: latency)
- Implemented dynamic prefetching, fetch next layer’s weights during current layer’s computation [CUDA stream concurrency]
- Observed latency improvement for hand-written CUDA kernels for linear and convolutional networks on RTX 3070 GPU
- Extended policies for custom PyTorch models (e.g., OFA MobileNet) and observed selective gains 8.27% compared to default
hardware policy. Justified latency performance using DRAM read/write measurements from Nsight compute.

### Can DB Queries Exploit Tensor Cores? 
- Implemented hash join operation between tables of size 1M rows using matrix multiplication in Triton on H100 GPU
- Implemented hash lookup as an alternative approach in CUDA and compared its performance against Triton
- Results indicated that average run-time for CUDA kernel is 90.65us and for triton is 13.78ms (150x faster)
- Speedup achieved is due to higher occupancy of CUDA (74.14%) compared to Triton (18.67%), obtained using Nsight Compute

### Parallel bitonic sort using CUDA 
- Implemented parallel bitonic sort algorithm over 10M array elements on L40S GPU
- Reduced memory access time by utilizing shared memory instead of global memory, improving throughput from 67% to 93%
- Explored host-device data transfer optimizations such as pinned-memory to reduce transfer time from 15ms to 5ms
- Proposed approach achieved 110x speedup over CPU based sorting.
