# MicroMPoxNet


**MicroMPoxNet: A Lightweight CNN for Interpretable Monkeypox Classification in Dermoscopic Images with Comparative Transfer Learning Evaluation** <br>

**Authors**  
A. A. M. Mustahid, A. A. M. Muzahid*, Md. Sadekur Rahman, Hua Han, Yujin Zhang, Ferdous Sohel  

📄 **Status:** Paper Under Review

<p align="center">
  <img src="assests/Final_JournalGraph.png" width="95%">
</p>

---

[![Paper](https://img.shields.io/badge/Paper-Under%20Review-blue)](#)
[![Dataset](https://img.shields.io/badge/Dataset-Google%20Drive-green)](https://drive.google.com/file/d/1P3ZZ01TSJS4v9uhBy0USzfbMXWbO8QIh/view?usp=sharing)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

---

## Repository Structure

```
MicroMPoxNet/
│
├── README.md
├── LICENSE
├── CITATION.cff
│
├── assets/
│   ├── pipeline.png
│   ├── architecture.png
│   ├── dataset_samples.png
│   ├── TLModel_Diagram.jpg
│   ├── XAI_n.jpg
│   ├── conf_roc_curve.png
│   ├── model_performance_tradeoffs.png
│   └── Final_JournalGraph.png
│
├── models/
│
├── training/
│
└── dataset/
    └── dataset_links.md
```

---

## Table of Contents

- [Overview](#overview)
- [Highlights](#highlights)
- [Research Pipeline](#research-pipeline)
- [Architecture Overview](#architecture-overview)
- [Dataset](#dataset)
- [Explainability (XAI)](#explainability-xai)
- [Code Availability](#code-availability)
- [Citation](#citation)
- [Contact](#contact)

---

## Research Pipeline

<p align="center">
  <img src="assests/pipeline.png" width="95%">
</p>


---

## Overview

Monkeypox (Mpox) has recently emerged as a global public health concern, highlighting the need for fast, accessible, and reliable diagnostic tools. Traditional diagnostic methods such as PCR testing require specialized laboratory infrastructure and trained personnel, which can limit timely diagnosis in resource-constrained environments.

Recent deep learning approaches have shown promising results for automated skin lesion classification. However, many existing methods rely on large and computationally expensive transfer learning models, making real-time deployment difficult in practical healthcare settings.

To address these limitations, this work introduces **MicroMPoxNet**, a lightweight convolutional neural network designed for efficient and interpretable Mpox classification from dermoscopic images. The proposed architecture integrates depthwise separable convolutions, residual connections, Swish activation functions, and squeeze-and-excitation blocks to achieve a strong balance between predictive performance and computational efficiency.

Extensive experiments were conducted using both transfer learning baselines and the proposed MicroMPoxNet model. The results demonstrate that MicroMPoxNet achieves highly competitive performance while maintaining significantly lower computational complexity, making it suitable for deployment in low-resource clinical environments.

---

## Highlights

- Proposed **MicroMPoxNet**, a lightweight CNN architecture for Monkeypox skin lesion classification.
- Designed for **efficient deployment in resource-constrained clinical environments**.
- Integrates **depthwise separable convolutions, residual connections, Swish activation, and squeeze-and-excitation blocks**.
- Achieves **high classification performance with significantly reduced computational complexity**.
- Evaluated against **11 state-of-the-art transfer learning models**.
- Includes **explainable AI methods (Grad-CAM, LIME, Integrated Gradients)** for improved clinical interpretability.

---

## Architecture Overview
MicroMPoxNet is designed with the following goals:

- Efficient Mpox skin lesion classification from dermoscopic images  
- Lightweight architecture suitable for real-time deployment in resource-constrained environments  
- Reduced computational complexity while maintaining strong predictive performance  
- Improved interpretability for clinical decision support  

The architecture emphasizes efficient feature extraction and compact network design to ensure reliable Mpox classification while enabling deployment on low-resource medical devices and edge computing platforms.

---

***<p align="center">Architecture of MircoMPoxNet***<br><br>
<img src="assests/architecture.png" width="90%" height="100%"><br><br>
***<p align="center">Architecture of Transfer Learning***<br><br>
<img src="assests/TLModel Diagram.jpg" width="90%" height="90%"><br><br>
***<p align="center">Classification results on Binary and Multi-class dataset***<br><br>
<img src="assests/conf_roc_curve.png" width="90%" height="90%"><br><br>
***<p align="center">Model Performance Tradeoffs (MicroPoxNet vs Transfer Learning)***<br><br>
<img src="assests/model_performance_tradeoffs.png" width="90%" height="90%"><br><br> 

---

## Dataset

### Mpox2025 Dataset (Proposed)

The **Mpox2025 dataset** was constructed to support reliable Mpox classification using dermoscopic images.

Dataset characteristics:

- Total images: **696**
- Mpox images: **337**
- Normal images: **359**
- Image format: **PNG**
- Color space: **RGB / Grayscale**

After applying data augmentation techniques, the dataset was expanded to **34,555 images** for robust model training.

### Sample Images from Mpox2025

<p align="center">
  <img src="assests/dataset_samples.png" width="95%">
</p>

### Dataset Download

The **Mpox2025 dataset** used in this study is available at:

Google Drive:  
https://drive.google.com/file/d/1P3ZZ01TSJS4v9uhBy0USzfbMXWbO8QIh/view?usp=sharing

External dataset used in this study:

Kaggle Dataset:  
https://www.kaggle.com/datasets/maxmelichov/monkeypox-2022-remastered

---


## Explainability (XAI)

To improve clinical interpretability, this study employs several explainability techniques:

- Grad-CAM
- LIME
- Integrated Gradients

These methods help visualize which regions of the dermoscopic images contribute most to the model’s predictions, supporting more transparent AI-assisted diagnosis.

<p align="center"> <br>
<img src="assests/XAI_n.jpg" width="90%" height="90%"><br><br>

---

## Code Availability

The complete implementation of **MicroMPoxNet**, including model architecture and training scripts, will be made publicly available upon acceptance of the paper.

The **Mpox2025 dataset** used in this study is currently accessible via the Google Drive link provided in the dataset section.

---

## Citation

If you find this work useful for your research, please consider citing:

```
@article{micrompoxnet2026,
  title={MicroMPoxNet: A Lightweight CNN for Interpretable Monkeypox Classification in Dermoscopic Images with Comparative Transfer Learning Evaluation},
  author={Mustahid, A. A. M. and Muzahid, A. A. M. and Rahman, Md. Sadekur and Han, Hua and Zhang, Yujin and Sohel, Ferdous},
  journal={},
  year={2026}
}
```

---

## Contact

For questions or collaboration inquiries, please contact:

**A. A. M. Mustahid**  
Email: *mustahid34@gmail.com*


---
