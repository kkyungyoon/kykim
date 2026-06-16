---
layout: page
title: Sketch Image Data Classification
description: Naver BoostCamp AI Tech 7th (CV Track) · 2024.09
img:
importance: 5
category: Deep Learning
github: https://github.com/kkyungyoon/level1-imageclassification-cv-01
---

**Period**: 2024.09 · **Affiliation**: Naver BoostCamp AI Tech 7th (Computer Vision Track)

## Background

A sketch is an abstract, simplified form of image that lacks color, texture, and fine detail but focuses on basic shape and structure. By understanding these characteristics and developing a model that learns the basic structure of objects from sketch images, we aimed to recognize the differences from ordinary images and to strengthen our model-development skills from diverse perspectives.

## Problem Definition

Out of 1,000 classes in total, we selected the top 500 objects with the largest number of images and used 25,035 image samples. The data was split into 15,021 training samples and 10,014 public & private evaluation samples. The input is the file names of the 10,014 images, and the output is the predicted probabilities over the 500 objects for each image.

## Role

Experiments to improve model performance.

## Approach

🔗 [View individual experiments & contributions](https://github.com/kkyungyoon/level1-imageclassification-cv-01/tree/main/individual_project_summary)

I extracted feature vectors from the early and middle stages of `Swin_base_patch4_window7_224`, computed coarse-category and mid-category losses respectively, and performed backpropagation by taking a weighted sum with the original fine-category loss. I hypothesized that stage-by-stage classification would be more effective than predicting all 500 classes directly.

## Lessons Learned

I learned the importance of systematic experimentation.
