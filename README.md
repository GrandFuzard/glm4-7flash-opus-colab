<a href="https://colab.research.google.com/github/GrandFuzard/glm4-7flash-opus-colab/blob/main/GLM_4_7Flash_fine_tune_Opus_4_5_xhigh.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

# glm4-7flash-opus-colab

> Run **GLM-4.7 Flash × Claude Opus reasoning distill** on **FREE Google Colab (T4)** using GGUF + Gradio UI. No local setup required.

---

## ✨ Features

- GGUF inference via llama.cpp (CUDA + CPU split)
- Flash Attention enabled (`flash_attn=True`)
- Optimized batching (`n_batch=512`)
- Gradio chat UI with streaming
- Multi-chat (rename / delete / export)
- Copy button for responses
- Token/sec + latency display
- Web search (DuckDuckGo) integration
- One-click Colab launch

---

## 🚀 Quick start

1. Click **Open in Colab**
2. Run cells **1 → 4**
3. Select quant in Cell 2
4. Adjust GPU layers (start at 48)
5. Open the Gradio public link

---

## 🔧 Configuration Notes

- Default context: `4096`
- GPU layers: `48` (adjust if needed for your quant)
- Higher quants may require CPU offloading

---

## 🎛️ Sampling Presets (Fixed)

Based on model card:

| Mode | Temperature | Top-P |
|------|------------|------|
| General | `1.0` | `0.95` |
| Tool-calling | `0.7` | `1.0` |
| Research | `0.7` | `0.95` |

---

## 🆕 Recent Updates

- Increased `n_batch` from 384 → 512 (better throughput)
- Enabled `flash_attn=True` (faster inference)
- Fixed sampling presets to match model card
- Added **copy button** in chat UI
- Fixed upload status clearing after responses
- Improved stability for free Colab T4 usage

---

## 💻 Requirements

- Free Colab T4 (~15GB VRAM)

| Quant | Behavior |
|------|--------|
| IQ2_M → Q3_K_M | Fully GPU |
| IQ4_XS → Q6_K | GPU + CPU split |
| Q8_0+ | Not suitable for T4 |

---

## 📦 Models

Models are downloaded at runtime from Hugging Face.

This repository does **not** host model weights.

---

## ⚠️ Notes

- Performance depends on context length and quant
- Flash attention may slightly increase VRAM usage
- CPU splitting affects token generation speed

---

## 🙏 Credits

- Base model: GLM-4.7-Flash (zai-org)
- Fine-tunes: Unsloth, TeichAI
- Quantization: TeichAI
- Inference: llama.cpp
- UI: Gradio
- Development assistance: Claude Opus 4.6 (Anthropic)

---

## 📄 License

MIT License (applies only to notebook and code)
