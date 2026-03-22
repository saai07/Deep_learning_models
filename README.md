# 🧠 Deep Learning Models

A personal collection of deep learning model implementations built from scratch using Jupyter Notebooks. Covers classic CNN architectures, generative models, and modern transformer-based vision models

---

## 📁 Repository Structure

```
Deep_learning_models/
│
├── computer_vision/
│   ├── resnet50.ipynb       # ResNet-50 — Deep Residual Network
│   ├── vit.ipynb            # Vision Transformer (ViT)
│   ├── gan.ipynb            # Generative Adversarial Network
│   └── ...
│
└── README.md
```

---

## 🗂️ Models

### 🔷 ResNet-50
> *Deep Residual Learning for Image Recognition* — He et al., 2015

ResNet-50 is a 50-layer CNN that solves the vanishing gradient problem using **skip (residual) connections**, allowing much deeper networks to train effectively.

- 50-layer architecture with bottleneck residual blocks
- Batch Normalization + ReLU throughout
- Supports fine-tuning on custom datasets
- 📌 **Use case:** Image Classification

---

### 🔷 Vision Transformer (ViT)
> *An Image is Worth 16×16 Words* — Dosovitskiy et al., 2020

ViT applies the **Transformer architecture** directly to sequences of image patches — no convolutions needed. Achieves state-of-the-art results when pre-trained on large datasets.

- Image split into fixed-size patches (e.g. 16×16)
- Patch + positional embeddings fed into Transformer encoder
- Multi-head self-attention across all patches
- MLP head for final classification
- 📌 **Use case:** Image Classification

---

### 🔷 GAN (Generative Adversarial Network)
> *Generative Adversarial Nets* — Goodfellow et al., 2014

GANs pit two networks against each other — a **Generator** that learns to create realistic images from random noise, and a **Discriminator** that learns to distinguish real from fake.

- Generator: noise vector → synthetic image
- Discriminator: binary real/fake classification
- Trained adversarially in a minimax game
- 📌 **Use case:** Image Generation / Synthetic Data

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python 3.x | Core language |
| PyTorch / TensorFlow | Model building & training |
| NumPy | Numerical computation |
| Matplotlib | Visualizations & training curves |
| Jupyter Notebook | Interactive experiments |

---

## 🚀 Getting Started

```bash
# 1. Clone the repo
git clone https://github.com/saai07/Deep_learning_models.git
cd Deep_learning_models

# 2. Install dependencies
pip install torch torchvision tensorflow numpy matplotlib jupyter

# 3. Launch Jupyter
jupyter notebook
```

Open any notebook inside `computer_vision/` and run cells top to bottom.

> 💡 **GPU recommended** — especially for ViT and GAN training. CUDA-enabled GPU significantly reduces training time.

---

## 📖 Papers

| Model | Paper |
|-------|-------|
| ResNet-50 | [Deep Residual Learning for Image Recognition](https://arxiv.org/abs/1512.03385) |
| ViT | [An Image is Worth 16x16 Words](https://arxiv.org/abs/2010.11929) |
| GAN | [Generative Adversarial Nets](https://arxiv.org/abs/1406.2661) |

---

## 👤 Author

**saai07** — [@saai07](https://github.com/saai07)

> ⭐ Star this repo if you find it useful!
