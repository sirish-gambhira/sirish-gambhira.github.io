---
layout: archive
title: ""
permalink: /code/
author_profile: true
redirect_from:
  - 
---

Here's a list of papers in the machine-learning and systems domains that I implemented from scratch and their corresponding code respositories.

1. "Llama 2: Open Foundation and Fine-Tuned Chat Models" [[code](https://github.com/sirish-gambhira/llama2-pytorch)]: Implemented Llama 2 architecture, loaded pretrained weights from meta repository and performed inference on prompts using top_k selection strategy. I found an interesting way to [jailbreak](https://github.com/sirish-gambhira/llama2-pytorch/blob/main/README.md) Llama-2.

2. "Attention is all you need" [[code](https://github.com/sirish-gambhira/attention-pytorch)]: Implemented and trained a Transformer (encoder-decoder) architecture for neural machine translation task between english (source) to italian (target) using [opus_books](https://huggingface.co/datasets/Helsinki-NLP/opus_books) dataset.