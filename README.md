# EffiCAT — Skin Disease Classification via Multi‑Dataset Fusion & Attention

[![CI](https://github.com/sasithradevia-ux/EffiCAT-SkinDisease-Classification/actions/workflows/ci.yml/badge.svg)](https://github.com/sasithradevia-ux/EffiCAT-SkinDisease-Classification/actions/workflows/ci.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Python](https://img.shields.io/badge/python-3.9|3.10|3.11-blue.svg)](#)

**EffiCAT** is a research codebase for robust skin disease classification that combines multi‑dataset training and attention mechanisms.

## ✨ Key Features
- Multi‑dataset ingestion & harmonization
- Attention modules (e.g., SE/CBAM/Channel‑Spatial) — plug‑and‑play
- Solid training/eval loops with metrics (Acc/F1/AUC) and plots (ROC/CM)
- Reproducible configs (`configs/`) and scripts (`scripts/`)

## 🏁 Quickstart
```bash
# 1) Create & activate a virtualenv
python -m venv .venv
# Linux/Mac
source .venv/bin/activate
# Windows (PowerShell)
# .venv\Scripts\Activate.ps1

# 2) Install deps
pip install -U pip
pip install -r requirements.txt

# 3) Train / Evaluate (examples)
python scripts/train.py --config configs/base.yaml
python scripts/eval.py --weights checkpoints/best.pth
```

## 📦 Project Layout
```
EffiCAT/
├── src/efficat/          # Library: models/, data/, engine/, utils/
├── scripts/              # Entry points: train.py, eval.py, etc.
├── configs/              # YAML/JSON config files
├── notebooks/            # Experiments / analysis
├── data/                 # (gitignored) datasets
├── checkpoints/          # (gitignored) weights/outputs
├── .github/workflows/    # CI
├── requirements.txt
├── README.md
├── .gitignore
└── LICENSE
```

## 🗂 Datasets
Add precise instructions here for each dataset (links, MD5s, folder layout). Optionally provide a helper script `scripts/prepare_datasets.py`.

## 🧪 Reproducibility
- Seeded training, config‑driven experiments
- Save best checkpoints and logs
- Determinism toggles (where feasible)

## 🔖 Citation
If this repo helps your research, please cite:
```bibtex
@article{EffiCAT2025,
  title={EffiCAT: A synergistic approach to skin disease classification through multi-dataset fusion and attention mechanisms},
  author={Rajendran, Sushmetha Sumathi and H, Kiranchandran and H, Vishal and Sasithradevi, A. and Seemakurthy, Karthik and Poornachari, Prakash and Vijayalakshmi, M.},
  journal={arXiv},
  year={2025}
}
```

## 📜 License
This project is licensed under the MIT License — see [LICENSE](LICENSE) for details.