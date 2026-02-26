# 🌸 Vision Transformer (ViT) for Flower Classification in PyTorch

### From Paper: *"An Image is Worth 16x16 Words"*

---

## 📄 Paper Reference

* **Title:** An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale
* **Authors:** Dosovitskiy et al.
* **Link:** [https://arxiv.org/abs/2010.11929](https://arxiv.org/abs/2010.11929)

<img width="952" height="490" alt="image" src="https://github.com/user-attachments/assets/abed34bc-99c1-42c6-a9d1-1ca5ffa6c4c2" />

```
@article{dosovitskiy2020vit,
  title={An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale},
  author={Dosovitskiy et al.},
  year={2020}
}
```

---

## 🎯 Objective

This repository provides a **from-scratch PyTorch implementation of Vision Transformer (ViT)** applied to a **Flower Image Classification task**.

The goal of this project is to understand how transformers can replace CNNs for vision tasks.

Key learning objectives:

* Understand patch embedding in vision
* Implement transformer encoder for images
* Apply self-attention to visual tokens
* Train ViT on real-world image dataset
* Evaluate transformer-based classification performance

---

## ✨ Features

* Patch Embedding from scratch
* Learnable Class Token
* Positional Encoding
* Multi-Head Self Attention (MSA)
* Transformer Encoder Blocks
* MLP Head for classification
* Full Training & Validation pipeline
* Test Evaluation
* Loss & Accuracy Visualization

---

## 🧠 Architecture Overview

Pipeline:

```
Image → Patches → Linear Embedding → Class Token
→ Positional Encoding → Transformer Encoder
→ Classification Token →  Output Class
```

The model closely follows **ViT-Base/16 architecture design** with adaptations for flower classification.

---

## 📂 Project Structure

```
flower-recognition-using-vit.ipynb
README.md
```

Inside Notebook:

* Data Loading
* Patch Embedding
* Multi-Head Attention
* Transformer Encoder
* ViT Model
* Training Loop
* Validation
* Testing
* Visualization

---

## ⚙️ Installation

Clone repository and install dependencies:

```bash
git clone https://github.com/Vishalrewaskar/vit-flower-classification.git
cd vit-flower-classification
pip install torch torchvision matplotlib numpy pandas
```

---

## 📊 Dataset

This project uses a **Flower Image Dataset** with:

* Train set
* Validation set
* Test set

Images are resized to:

```
224 × 224
```

Patch Size Used:

```
16 × 16
```

---

## 🚀 Training

Training performed using:

* **Optimizer:** Adam
* **Learning Rate:** 3e-3
* **Epochs:** 10
* **Batch Size:** 32

Run training via notebook cells.

---

### Hyperparameters

| Parameter     | Value |
| ------------- | ----- |
| Image Size    | 224   |
| Patch Size    | 16    |
| Embedding Dim | 768   |
| Heads         | 12    |
| Epochs        | 10    |
| Batch Size    | 32    |
| Optimizer     | Adam  |

---

## 📈 Results

Model trained successfully on flower dataset.

Tracked metrics:

* Training Loss
* Validation Loss
* Training Accuracy
* Validation Accuracy
* Test Accuracy

Visualizations included:

* Loss Curve 📉
* Accuracy Curve 📈

---

## 🔬 Experiments & Learnings

Key observations:

* Patch embeddings effectively replace convolutional filters
* Positional encoding is critical for spatial awareness
* Transformers can perform well even without CNNs
* Training stability improves with LayerNorm + residual connections

---

## 📌 Differences from Original Paper

| Paper                   | This Implementation       |
| ----------------------- | ------------------------- |
| Trained on ImageNet     | Trained on Flower Dataset |
| Large-scale pretraining | No pretraining            |
| Massive compute         | Lightweight training      |
| Huge dataset            | Small dataset             |

---

## 💡 Applications

* Plant classification 🌿
* Medical imaging 🧬
* Satellite image analysis 🛰️
* Object recognition 👁️

---

## 📚 References

1. Dosovitskiy, A. et al.
   *An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale*
   [https://arxiv.org/abs/2010.11929](https://arxiv.org/abs/2010.11929)

2. PyTorch Documentation
   [https://pytorch.org/docs/stable/index.html](https://pytorch.org/docs/stable/index.html)

3. Torchvision Datasets
   [https://pytorch.org/vision/stable/datasets.html](https://pytorch.org/vision/stable/datasets.html)

4. Attention Is All You Need (Transformer Foundation)
   Vaswani et al.
   [https://arxiv.org/abs/1706.03762](https://arxiv.org/abs/1706.03762)

---
