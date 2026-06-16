---
layout: page
title: Multilingual Receipt OCR
description: Naver BoostCamp AI Tech 7th (CV Track) · 2024.10
img:
importance: 3
category: Deep Learning
github: https://github.com/kkyungyoon/level2-cv-datacentric-cv-01
---

**Period**: 2024.10 · **Affiliation**: Naver BoostCamp AI Tech 7th (Computer Vision Track)

## Background

There are generally two perspectives when doing deep learning. One is the model-centric perspective, and the other is the data-centric perspective. In this project, we carried out a receipt-related OCR task with a focus on the data-centric perspective.

## Problem Definition

We participated in an OCR competition to detect text regions in receipt images written in multiple languages (Chinese, Japanese, Thai, and Vietnamese). The input consisted of 400 JPG images for training and 120 for testing, and the output was provided in the UFO format, which includes the bounding box coordinates indicating the positions of text in the images. The goal of the competition was to accurately predict text regions using only the given data, without developing a model.

## Role

Experiments to improve model performance.

## Approach

🔗 [View individual experiments & contributions](https://github.com/kkyungyoon/level2-cv-datacentric-cv-01/tree/main/individual_project_summary)

To improve model performance, I applied Salt and Pepper noise, Binarization, Binarization (Adaptive Threshold), and Normalization.

## Lessons Learned

I learned that adding noise can produce a more robust model, and that applying thresholding and normalization suited to the characteristics of the data contributes greatly to performance improvement.
