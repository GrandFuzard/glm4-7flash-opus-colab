[![link](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/GrandFuzard/GLM_4_7Flash_fine_tune_Opus_4_5_xhigh.ipynb)

# glm4-7flash-opus-colab

Ready-to-run colab notebook for running a **GLM-4.7-Flash × Claude Opus 4.5 high-reasoning distill (GGUF)** model.

This project focuses on making large GGUF models usable on **free Colab T4** by supporting GPU/CPU layer splitting and a User friendly Gradio web UI.

---

## ✨ Features

- GGUF inference via llama.cpp (CUDA + CPU split)
- Gradio chat interface with streaming
- Multiple chats with rename / delete / export
- Token/sec and latency display
- One-click launch from Colab

---

## 🚀 Quick start

1. Click **Open in Colab** at the top of this page.
2. Run the cells in order.
3. Choose a quantized model in the dropdown.
4. Adjust GPU layers if needed.
5. Open the Gradio public link.

No local setup is required.

---

## 💻 Requirements

- Free Colab T4 (15 GB VRAM) is enough to run upto Q3_K_M.
- GPU / CPU splitting is controlled manually using the GPU layers slider.

---

## 📦 Models

Models and quantized files are downloaded at runtime from their specific repositories

This repository does **not** redistribute any model weights or datasets.

---

## ⚠️ Important note

This repository contains **only the Colab notebook and UI / glue code**.

Models and datasets are fetched from their original sources and remain under their
respective licenses.

---

## 🙏 Credits

- Base model and derivatives are provided by their respective authors on Hugging Face.
- Inference backend: llama.cpp
- UI: Gradio

---

## 📄 License

MIT License – applies only to the notebook and code in this repository.
