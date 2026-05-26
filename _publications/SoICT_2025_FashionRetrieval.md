---
title: "Exploring Multi-Modal Large Language Models and Two-Stage Fine-Tuning for Fashion Image Retrieval"
collection: publications
permalink: /publications/ExploringFashionRetrieval/
date: 2025-12-13
venue: "Symposium on Information and Communication Technology (SoICT) 2025"
rank: Scopus-indexed
category: manuscripts
award: "Best Poster Award"
excerpt: "We investigate multi-modal large language models with a two-stage fine-tuning strategy for robust fashion image retrieval, demonstrating strong performance across standard benchmarks."
teaser: /images/papers/soict2025-teaser.jpg

paperurl: "files/soict.pdf"
certurl: "files/soict_cert.pdf"
tags:
  - MLLM
  - Fashion Retrieval
  - Fine-Tuning
  - Computer Vision
---

## Overview

This paper investigates the application of **Multi-Modal Large Language Models (MLLMs)** to the complex task of fashion image retrieval. We propose a robust **two-stage fine-tuning strategy** that bridges the gap between general domain knowledge and task-specific requirements. By first adapting the model to fashion-specific semantics and subsequently optimizing for retrieval objectives, we achieve highly accurate image–text matching.

🏆 **Awarded Best Poster at SoICT 2025.**

## Motivation

Fashion image retrieval inherently requires an acute understanding of fine-grained attributes—such as color, texture, pattern, and silhouette—while simultaneously aligning highly descriptive natural language queries with visual representations. Traditional contrastive pretraining paradigms (like CLIP) often exhibit vulnerabilities when confronted with the long-tail distribution of these specific fashion attributes. Our research addresses this limitation by leveraging the reasoning capabilities of MLLMs.

## Key Contributions

* **Two-Stage Fine-Tuning Pipeline**: 
    * *Stage 1 (Semantic Warm-up)*: Adapts the multi-modal backbone using specialized fashion captioning to establish domain familiarity.
    * *Stage 2 (Task Optimization)*: Applies retrieval-specific contrastive fine-tuning, incorporating hard negative mining to sharpen the model's discriminative boundaries.
* **Comprehensive MLLM Benchmarking**: We rigorously evaluate multiple state-of-the-art MLLM backbones (including LLaVA, InternVL, and MiniGPT-4) as visual encoders to determine optimal retrieval performance.
* **Empirical Validation**: Extensive experiments conducted on industry-standard datasets (FashionIQ and CIRR) demonstrate that our methodology consistently outperforms standard CLIP-only baselines.

## Results & Impact

The proposed two-stage approach yields significant and consistent **Recall@K improvements** across challenging FashionIQ sub-categories (Dress, Toptee, Shirt). By effectively parsing complex compositional queries, the model substantially outperforms single-stage fine-tuning baselines, proving the efficacy of semantic warm-ups in multi-modal retrieval tasks.