---
title: "Exploring Multi-Modal Large Language Models and Two-Stage Fine-Tuning for Fashion Image Retrieval"
collection: publications
permalink: /publications/ExploringFashionRetrieval/
date: 2025-12-13
venue: "Symposium on Information and Communication Technology (SoICT) 2025"
rank: Scopus-indexed
category: manuscripts
excerpt: "We investigate multi-modal large language models with a two-stage fine-tuning strategy for robust fashion image retrieval, demonstrating strong performance across standard fashion retrieval benchmarks."
teaser: /images/papers/soict2025-teaser.jpg

paperurl: "https://doi.org/10.1145/3805622.3810590"
codeurl: "https://github.com/HNg0303/VietFashion"
projecturl: "https://hng0303.github.io/VietFashion/"
---

## Overview

This paper investigates the application of **Multi-Modal Large Language Models (MLLMs)** for fashion image retrieval. We propose a **two-stage fine-tuning strategy** that first adapts the model to general fashion semantics, then fine-tunes on task-specific retrieval objectives for robust image–text matching.

## Motivation

Fashion image retrieval is challenging due to the need to understand fine-grained attributes (color, texture, pattern, silhouette) while aligning natural language queries with visual content. Standard contrastive pretraining (CLIP-style) often struggles with the long-tail distribution of fashion attributes.

## Contributions

- **Two-Stage Fine-Tuning**: Stage 1 warms up the multi-modal backbone on fashion captioning; Stage 2 applies retrieval-specific contrastive fine-tuning with hard negative mining.
- **MLLM Backbone Exploration**: We benchmark multiple MLLM backbones (LLaVA, InternVL, MiniGPT-4) as visual encoders for retrieval.
- **Evaluation**: Comprehensive experiments on FashionIQ and CIRR showing consistent improvements over CLIP-only baselines.

## Key Results

The proposed two-stage approach yields consistent Recall@K improvements across FashionIQ sub-categories (Dress, Toptee, Shirt) and outperforms single-stage fine-tuning baselines.

## Citation

```bibtex
@inproceedings{cao2025fashionretrieval,
  title     = {Exploring Multi-Modal Large Language Models and Two-Stage Fine-Tuning for Fashion Image Retrieval},
  author    = {Cao, Hoang-Nguyen and others},
  booktitle = {Proceedings of the Symposium on Information and Communication Technology (SoICT)},
  year      = {2025},
  doi       = {10.1145/3805622.3810590}
}
```
