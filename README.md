# Lane Departure Anomaly Detection Using U-Net with Feature Cross Attention

## Overview

This repository presents an implementation of a lane departure anomaly detection system based on a modified U-Net architecture enhanced with Feature Cross Attention (FCA). The model is designed to improve lane segmentation accuracy and anomaly sensitivity under challenging driving conditions such as occlusions, illumination changes, and lane distortions.

The implementation focuses on the core experimental pipeline and visual analysis, as described in the associated research work.

---

## Methodology

The proposed approach extends the standard U-Net architecture by integrating Feature Cross Attention modules at the bottleneck and decoder stages. The attention mechanism enhances both spatial and channel-wise feature interactions, enabling more precise lane boundary representation and improved anomaly awareness.

Key characteristics:
- Backbone: U-Net (encoder–decoder with skip connections)
- Attention mechanism: Feature Cross Attention (spatial + channel attention)
- Input resolution: 128 × 128
- Output: Binary lane segmentation mask
- Framework: PyTorch

Lane departure anomalies are identified based on spatial deviation between predicted lane boundaries and ground truth masks.

---

## Dataset

This project uses the **Comma2k19-LD** dataset, a publicly available lane detection dataset containing annotated highway driving scenes.

Dataset source (Kaggle):
- https://www.kaggle.com/datasets

Due to size considerations, the dataset is **not included** in this repository.

Expected directory structure:
