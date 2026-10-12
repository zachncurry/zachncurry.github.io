# ⚡ FocusFlow AI — In-Browser Smart ToDoozie Assistant

> *A privacy-first, serverless productivity tool powered by client-side WebGPU AI.*

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Tech Stack](https://img.shields.io/badge/tech-HTML5%20%7C%20CSS3%20%7C%20JS%20%7C%20Transformers.js-orange)
![Hosting](https://img.shields.io/badge/hosting-GitHub%20Pages-brightgreen)

---

## 💡 The Vision: Lightweight, Frictionless AI

For a long time, I wanted to explore a simple question:  
**"Can we build useful, modern AI tools that run 100% inside the user's browser without complex backends, heavy cloud infrastructure, or expensive API keys?"**

Most AI features today rely on server-side APIs, requiring users to log in, supply API keys, or deal with server latency and data privacy concerns. 

**FocusFlow AI** is my answer to that challenge. It combines a classic **ToDoozie focus timer** with an **in-browser LLM** (via `@huggingface/transformers` and ONNX runtime) to automatically break down large, daunting tasks into actionable, 25-minute ToDoozie steps.

---

## ✨ Features

- ⏱️ **ToDoozie Focus Engine:** Customizable Work/Break intervals with simple control toggles.
- 🤖 **In-Browser AI Task Breakdown:** Uses **Gemma-3 270M (ONNX)** running locally to decompose tasks into actionable sub-steps.
- 🔒 **100% Local & Private:** Your task list and prompts never leave your device. Zero server calls, zero telemetry.
- ⚡ **WebGPU / WASM Accelerated:** High-performance local inference directly through your browser graphics card.
- 💸 **$0 Cost to Host:** Single-file architecture natively hosted on GitHub Pages.

---

## 🛠️ How It Works Under the Hood

<img width="678" height="367" alt="image" src="https://github.com/user-attachments/assets/6e19fe62-af37-444f-a382-6b9a2f42a7c3" />



1. **No Backend Required:** The app is written in plain HTML, CSS, and modern JavaScript.
2. **Model Caching:** On first load, the lightweight quantized model (~270M parameters) is cached locally in the browser (`IndexedDB`), allowing instant execution on subsequent visits.
3. **Hardware Acceleration:** Uses **WebGPU** when available, automatically falling back to CPU WebAssembly (WASM).

---

## 🚀 Live Demo & Quickstart

### 1. View Live
Try the live demo on GitHub Pages:  
👉 **`https://<your-username>.github.io/<your-repo-name>/`**

### 2. Run Locally
No `npm install` or node server setup needed!

1. Clone the repository:
   ```bash
   git clone [https://github.com/](https://github.com/)<your-username>/<your-repo-name>.git




## 📊 Tech Stack
Frontend: Vanilla HTML5, CSS3, JavaScript (ES6 Modules)

AI Runtime: @huggingface/transformers v3

Model: onnx-community/gemma-3-270m-it-ONNX

Hosting: GitHub Pages

## 🔮 Future Roadmap
[ ] LocalStorage persistence for completed tasks & streaks
[ ] Customizable model selection (e.g., Qwen / SmolLM variants)
[ ] Web Audio synthesized ambient noise generator (Lo-Fi / White Noise)
[ ] Mobile PWA offline mode integration

## 🤝 Contributing
Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

## 📄 License
Distributed under the MIT License. See LICENSE for more information.
