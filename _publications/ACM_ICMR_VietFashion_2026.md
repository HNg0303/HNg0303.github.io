---
title: "VietFashion: Benchmarking Sketch–Text Composed Image Retrieval for Cultural Outfits"
collection: publications
permalink: /publications/VietFashion/
date: 2026-04-25
venue: "ACM International Conference on Multimedia Retrieval (ICMR) 2026"
rank: B-rank
category: manuscripts
excerpt: "We introduce VietFashion, the first benchmark for sketch–text composed image retrieval targeting culturally-specific Vietnamese traditional outfits, enabling fine-grained cross-modal retrieval via domain-adapted encoder fine-tuning."
teaser: /images/papers/vietfashion-teaser.jpg

paperurl: "https://doi.org/10.1145/3805622.3810590"
codeurl: "https://github.com/HNg0303/VietFashion"
projecturl: "https://hng0303.github.io/VietFashion/"
---

## Overview

**VietFashion** is a novel cross-modal retrieval benchmark focused on Vietnamese cultural fashion (Áo Dài, Áo Bà Ba, and similar traditional garments). The dataset supports **Sketch–Text Composed Image Retrieval (STCIR)** — a task where a user provides both a sketch and a free-form text description to retrieve visually matching outfit images from a gallery.

## Motivation

Existing composed image retrieval benchmarks (FashionIQ, CIRR, CIRCO) focus on Western fashion and lack cultural diversity. We observed that models trained on these benchmarks perform poorly on culturally-specific Vietnamese garments due to the large domain gap in visual patterns, textures, and silhouettes.

## Contributions

- **Dataset**: Curated a large-scale benchmark with paired sketch–image–text triplets covering major Vietnamese traditional outfits.
- **Encoder Fine-tuning**: Adapted sketch and text encoders via domain-specific contrastive fine-tuning to bridge the modality gap.
- **Benchmark Design**: Designed evaluation protocols (Recall@K) and established strong baselines for future research.
- **Manuscript**: Full research pipeline from data collection to experimental validation.

## Results

Our domain-adapted model significantly outperforms general-purpose CLIP-based baselines on Recall@1, Recall@5, and Recall@10 across all outfit categories in the VietFashion benchmark.

## Citation

```bibtex
@inproceedings{cao2026vietfashion,
  title     = {VietFashion: Benchmarking Sketch–Text Composed Image Retrieval for Cultural Outfits},
  author    = {Cao, Hoang-Nguyen and others},
  booktitle = {Proceedings of the ACM International Conference on Multimedia Retrieval},
  year      = {2026},
  doi       = {10.1145/3805622.3810590}
}
```
