---
layout: page
title: Object Detection for Recycling Waste Classification
description: Naver BoostCamp AI Tech 7th (CV Track) · 2024.10
img:
importance: 4
category: Deep Learning
github: https://github.com/kkyungyoon/level2-objectdetection-cv-01
---

**Period**: 2024.10 · **Affiliation**: Naver BoostCamp AI Tech 7th (Computer Vision Track)

## Background

When waste is sorted correctly, it can be recycled as a resource, but when it is sorted incorrectly, it is classified as waste and is either landfilled or incinerated. To address this, we aim to develop a model that automatically detects waste in photos.

## Problem Definition

The goal is to develop a model that detects 10 types of waste objects in images. The input consists of images containing the 10 types of waste objects, along with bounding box coordinates and category information in COCO format, and the output returns bounding box coordinates, categories, and scores. Model performance is evaluated by mAP50: when the IoU (Intersection over Union) between a predicted bounding box and a ground-truth box is 0.5 or higher, it is treated as True, and the average precision is computed accordingly.

## Role

Experiments to improve model performance (addressing the low mAP of small bounding boxes).

## Approach

🔗 [View individual experiments & contributions](https://github.com/kkyungyoon/level2-objectdetection-cv-01/tree/main/individual_project_summary)

To address the low mAP of small bounding boxes:

- **Small bbox detection via backbone change** — Changed the backbone to a Swin Transformer to improve small bbox detection performance.
- Small bbox detection via image resolution change
- Building a model that detects only small bboxes and then ensembling it
- **Experiment assigning weights by bbox size** — Defined a loss function (SizeWeightedLoss) that applies different weights depending on bbox size, then trained the model.

## Lessons Learned

I learned the importance of redefining the criteria for "small bboxes" to fit the dataset, the need for caution when tuning weights, and the limited effectiveness of resolution changes and Mosaic augmentation. The key takeaway was that, rather than simply changing techniques, it is important to use strategies tailored to the characteristics of the dataset and to maintain the training stability of the model.
