# BMVA Summer School — Computer Vision Practicals

Hands-on deep learning practicals for the [BMVA](https://www.bmva.org/) Computer Vision Summer School.

Everything runs on **Google Colab** — nothing to install. Click a badge below, sign in with a Google account, and you're coding. All datasets download automatically inside the notebooks.

---

## 🟢 Beginner — From Image Classification to Semantic Segmentation

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Adaptive-Intelligence-Lab/BMVA-summer-school/blob/main/BMVA_CVSS_Beginner.ipynb)

Two practicals in one notebook, designed to be worked through in order:

1. **Your first CNN** — build, train, and evaluate a convolutional neural network that recognises handwritten digits (MNIST). Covers the complete deep learning workflow: data loading, convolutions, defining models with `torch.nn`, the training loop, and evaluation with confusion matrices and error inspection.
2. **Fully Convolutional Networks for semantic segmentation** — go from one label per *image* to one label per *pixel*. Take a pretrained VGG16 classifier apart, turn it into an FCN, and train it to segment real photos of cats and dogs (Oxford-IIIT Pet dataset).

**You will learn:** images as tensors · convolutions and kernels · CNNs · loss functions and optimisers · training loops · evaluation · transposed convolutions · FCN-32s / FCN-16s and skip connections · pixel accuracy and mean IoU

*No prior deep learning experience required.*

---

## 🔴 Advanced — Knowledge Distillation

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Adaptive-Intelligence-Lab/BMVA-summer-school/blob/main/BMVA_CVSS_Advanced.ipynb)

What if you barely have any labels — but you do have a big, accurate model? **Knowledge distillation** lets a large "teacher" network teach a tiny "student": on CIFAR-10, the same 24k-parameter student (44× smaller than its teacher) gains **≈15–20 accuracy points** when the only change is learning from the teacher's soft predictions — and reaches ≈78% having seen *zero* ground-truth labels. You will implement the distillation loss and training loop yourself, and *see* why it works through dark-knowledge, t-SNE, confusion-matrix, and attention visualisations.

**You will learn:** teacher–student training · soft targets, temperature, and "dark knowledge" · the KD loss (and its classic pitfalls) · label-scarce training · hard pseudo-labels vs soft distillation · Decoupled KD (optional extension)

*Assumes the beginner practical (or equivalent PyTorch familiarity).*

---

## How to use the notebooks

1. Click an **Open in Colab** badge above.
2. In Colab: **File → Save a copy in Drive** so your progress is kept.
3. **Runtime → Change runtime type → T4 GPU** — do this *before* running any cells (switching later restarts the session).
4. Run the cells top to bottom:
   - **✏️ Exercises** contain `# TODO` skeletons — try them yourself first.
   - Each exercise is followed by a **✅ Reference solution**, so the notebook always runs end-to-end even if you skip one.
   - **🧠 Quick checks** ask a short question — think first, then click to reveal the answer.

All data is fetched inside the notebooks (MNIST, Oxford-IIIT Pet, CIFAR-10 — the latter from a fast mirror in this repository's [releases](https://github.com/Adaptive-Intelligence-Lab/BMVA-summer-school/releases), with automatic fallback to the official source).

---

## Credits

These practicals were created by the [Adaptive Intelligence Lab](http://adaptive-intelligence.co.uk/):

| | GitHub |
|:---|:---|
| [Dr Shuang (Chris) Chen](http://adaptive-intelligence.co.uk/dr-shuang-chris-chen/) | [@ChrisChen1023](https://github.com/ChrisChen1023) |
| [Dr Ruochen Li](http://adaptive-intelligence.co.uk/dr-ruochen-li/) | [@Carrotsniper](https://github.com/Carrotsniper) |
| [Dr Guodong Shen](http://adaptive-intelligence.co.uk/dr-guodong-shen/) | [@SGD95](https://github.com/SGD95) |
| [Dr Wenke E](http://adaptive-intelligence.co.uk/wenke-tom-e/) | [@Tom-E-Durham](https://github.com/Tom-E-Durham) |
