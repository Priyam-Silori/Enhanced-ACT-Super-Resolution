# Enhanced ACT for Single Image Super-Resolution

## Overview

This repository presents an enhanced version of the Adaptive Cross Transformer (ACT) for Single Image Super-Resolution (SISR). The proposed model improves feature representation by integrating a Dual Attention Module and an Adaptive Feature Fusion Gate while employing an improved training strategy based on Smooth L1 + MS-SSIM loss and Cosine Annealing Learning Rate Scheduling.

This work was developed as part of a research project on transformer-based image super-resolution.

---

## Features

- Adaptive Cross Transformer (ACT) backbone
- Dual Attention Module (Channel + Spatial Attention)
- Adaptive Feature Fusion Gate (AFFG)
- Smooth L1 + MS-SSIM Loss
- Cosine Annealing Learning Rate Scheduler
- Fine-tuning from pretrained ACT weights
- Evaluation on Set5, Set14 and BSD100 datasets

---

## Repository Structure

```
Enhanced-ACT-Super-Resolution/
│── Enhanced-ACT-Super-Resolution.ipynb
│── README.md
```

---

## Experimental Setup

- Framework: PyTorch
- Training Dataset: DIV2K
- Evaluation Datasets:
  - Set5
  - Set14
  - BSD100
- Scale Factor: ×2
- Optimizer: Adam
- Scheduler: Cosine Annealing LR

---

## Results

The proposed architecture maintains competitive performance with the baseline ACT model while introducing a more flexible attention and feature fusion framework.

| Dataset | PSNR (dB) | SSIM |
|---------|----------:|------:|
| Set5 | 38.424 | 0.9520 |
| Set14 | 34.516 | 0.9116 |
| BSD100 | 32.508 | 0.9052 |

---

## Future Work

- Training on DF2K
- Evaluation on Urban100 and Manga109
- ×3 and ×4 Super-Resolution
- Lightweight attention mechanisms

---

## Author

**Priyam Silori**

Department of Computer Science and Engineering

Graphic Era Deemed to be University

---

## License

This repository is intended for academic and research purposes.
