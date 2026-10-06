---
title: "Journey Clustering — Unsupervised User Journeys from Clickstream"
collection: portfolio
permalink: /portfolio/journey-clustering/
date: 2026-10-01
status: "Active"
excerpt: "Clusters 250M+ unlabeled mobile clickstream events into named user journeys. A Kafka sink connector and a daily Airflow job feed an ML pipeline with HDBSCAN, Markov anomaly scoring and drift monitoring."

codeurl: "https://github.com/HNg0303/Unsupervised-Journey-Clustering"
projecturl: "https://hng0303.github.io/Unsupervised-Journey-Clustering/"
tags:
  - Unsupervised Learning
  - HDBSCAN
  - Kafka
  - Airflow
  - DuckDB
  - Python
  - Kotlin
  - Swift
---

**[Open the interactive project page →](https://hng0303.github.io/Unsupervised-Journey-Clustering/)**

## Overview

A production pipeline that turns raw mobile app click logs into goal-level **user journeys**, clusters them without labels, and maps each cluster to a business taxonomy of about 500 intents. The product team uses it to see what customers come to the app for, where they struggle, and how iOS and Android differ.

## Data Pipeline

- **MongoDB → Kafka → SQL.** I built the sink connector that pulls clickstream topics from Kafka into SQL.
- **Daily Airflow cron job.** Each day it partitions, clusters, scores, names and summarises the previous day's events. Every task runs one CLI in the same Docker image.
- **Out-of-core and idempotent.** PyArrow and DuckDB keep memory bounded on 250M+ rows, and versioned data and model runs make reruns safe.

## ML Pipeline

1. **Data processing.** Role-correct canonicalisation, ID masking, a 5-level semantic ladder that aligns iOS and Android, and rule-based journey segmentation.
2. **Model development.** A multi-channel TF-IDF/SVD and behavioural embedding, HDBSCAN archetypes, a Markov chain per cluster for anomaly and next-action scoring, and taxonomy naming with a human review queue.
3. **Monitoring.** Data and model drift signals trigger challenger retraining with promotion gates and rollback.

## Results

- About 17M journeys scored and about 2,800 journey archetypes across Android and iOS.
- The same model runs on-device on Android (Kotlin + ONNX Runtime) and iOS (Swift).
