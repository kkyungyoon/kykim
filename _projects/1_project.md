---
layout: page
title: Hand Bone Image Segmentation
description: Naver BoostCamp AI Tech 7th (CV Track) · 2024.11
img:
importance: 2
category: Deep Learning
github: https://github.com/kkyungyoon/level2-cv-semanticsegmentation-cv-06-lv3
---

**Period**: 2024.11 · **Affiliation**: Naver BoostCamp AI Tech 7th (Computer Vision Track)

## Background

Bones have a significant impact on the structure and function of our bodies, so accurate bone segmentation is essential for developing medical diagnoses and treatment plans.

## Problem Definition

An image containing a hand bone X-ray object is used as the model's input. The model performs a multi-channel prediction that produces a probability map over 29 classes, and then assigns each pixel to its corresponding class based on this map. Finally, the predicted results are converted into Run-Length Encoding (RLE) format for submission.

## Role

Experiments to improve model performance.

## Approach

🔗 [View individual experiments & contributions](https://github.com/kkyungyoon/level2-cv-semanticsegmentation-cv-06-lv3/tree/main/individual_project_summary)

- Attempted returning the loss of an auxiliary classifier
- Searched for the optimal loss suited to the metric and the data
- Attempted pseudo labeling
- Attempted pixel shuffling / unshuffling to compensate for pixels lost due to interpolation
- Attempted adding a 1×1 convolution layer to improve accuracy in the overlapping regions of the back-of-hand bones

## Lessons Learned

- The importance of being careful when selecting a model before running experiments
- For some experiments, running follow-up experiments such as weight tuning can be more effective than running a wide variety of experiments
- When working on a project within a limited time, time must be allocated well across the experiments you want to run, and it is worth moving on if an approach shows no effect or remains unsolved within a few days
