---
layout: page
title: "Prescriptive AI: Automated Optimal-Value Recommendation"
description: Naver BoostCamp AI Tech 7th Final Project · 2025.01–2025.02
img:
importance: 1
category: Deep Learning
github: https://github.com/kkyungyoon/level4-cv-finalproject-hackathon-cv-06-lv3
---

**Period**: 2025.01–2025.02 · **Affiliation**: Naver BoostCamp AI Tech 7th (Computer Vision Track) — Final Project

## Background

In most machine learning settings, models learn a forward mapping from inputs to outputs (X → Y). In practice, however, businesses often have the opposite need: given a *desired* output value (Y), what input values (X) should be chosen to achieve it? This is an inverse problem — for a single target Y there may exist many valid candidates X — and it must be solved automatically across diverse datasets while respecting strict response-time constraints.

## Problem Definition

Build an automated **Prescriptive AI** system that analyzes a given dataset and recommends the optimal input values (X) needed to reach a customer-specified target output (Y), all within a bounded inference time. The system was validated on multiple datasets, each requiring its own preprocessing and feature-engineering pipeline.

## Approach

🔗 [View the repository](https://github.com/kkyungyoon/level4-cv-finalproject-hackathon-cv-06-lv3)

We decoupled the problem into a two-model framework that balances predictive accuracy with computational efficiency:

- **Surrogate Model** — learns the forward mapping (X → Y), serving as a fast, differentiable approximation of the true environment.
- **Search Model** — explores the input space within the learned surrogate environment to find the optimal X for a target Y.

The full pipeline — dataset preprocessing, feature engineering, model training, and search — was wrapped into a deployable end-to-end service. The system was served via a FastAPI (Python) backend and a JavaScript frontend, containerized with Docker Compose and fronted by Nginx.

## Role

Collaborated as part of a 6-member team, contributing to data preprocessing / feature engineering and the surrogate–search modeling pipeline.

## Lessons Learned

I learned how to frame and tackle an inverse (prescriptive) problem rather than a standard forward prediction task, and how to design a system that trades off model accuracy against latency. Building the project end-to-end — from preprocessing through modeling to a deployed, containerized service — also gave me hands-on experience turning a research idea into a usable product.
