# ⚡ FocusFlow AI: In-Browser Smart ToDoozie Assistant

> *A privacy-first, serverless productivity tool powered by client-side WebGPU AI and procedural Web Audio.*

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Tech Stack](https://img.shields.io/badge/tech-HTML5%20%7C%20CSS3%20%7C%20JS%20%7C%20Transformers.js-orange)
![Hosting](https://img.shields.io/badge/hosting-GitHub%20Pages-brightgreen)

---

## 💡 The Vision: Lightweight, Frictionless AI & Soundscapes

For a long time, I wanted to explore a simple question:  
**"Can we build useful, modern AI tools that run 100% inside the user's browser without complex backends, heavy cloud infrastructure, or expensive API keys?"**

Most productivity and AI tools rely on server-side APIs, requiring users to log in, supply API keys, or deal with server latency and data privacy concerns.

**FocusFlow AI** is my answer to that challenge. It combines a classic **ToDoozie focus timer**, an **in-browser LLM** (via `@huggingface/transformers` and ONNX runtime), a **procedural Web Audio sound engine**, and **local persistent state**—all packed into a zero-backend static Web app.

---

## ✨ Features

- ⏱️ **ToDoozie Focus Engine:** Customizable Work/Break intervals with simple control toggles.
- 🤖 **In-Browser AI Task Breakdown:** Uses **Gemma-3 270M (ONNX)** running locally to decompose major goals into actionable, 25-minute ToDoozie steps.
- 🎵 **Procedural AI Soundscapes:** Real-time, algorithmic ambient audio generated entirely via the Web Audio API (no external MP3 downloads required). Choose between:
  - 🎷 **Smooth Jazz:** Mellow chord progressions with warm triangle waves.
  - ⚡ **Electric Energy:** Punchy, fast-paced synth loops to energize rapid sprints.
  - 🧠 **Extreme Focus:** Deep ambient drones designed for distraction-free deep work.
- 📊 **Dynamic Task Status Management:** Cycle tasks between **Not Started**, **In Progress**, and **Done** with visual badges.
- 💾 **LocalStorage Persistence:** Saves your task list, subtasks, and progress automatically across browser sessions.
- 🔒 **100% Local & Private:** Your task list, prompts, and audio generation never leave your device. Zero server calls, zero telemetry.
- ⚡ **WebGPU / WASM Accelerated:** High-performance local inference directly through your browser graphics card.
- 💸 **$0 Cost to Host:** Single-file static architecture natively hosted on GitHub Pages.

---

## 🛠️ How It Works Under the Hood
<img width="1024" height="559" alt="image" src="https://github.com/user-attachments/assets/4db65002-9365-4e75-8318-9620461d1994" />
1. **No Backend Required:** The app is written in plain HTML, CSS, and modern JavaScript.
2. **Model Caching:** On first load, the lightweight quantized model (~270M parameters) is cached locally in the browser (`IndexedDB`), allowing instant execution on subsequent visits.
3. **Zero Audio File Overhead:** Instead of streaming heavy MP3 files, ambient soundscapes are synthesized mathematically in real time using the browser's native `AudioContext` oscillators and gain nodes.
4. **Hardware Acceleration:** Uses **WebGPU** when available, automatically falling back to CPU WebAssembly (WASM).

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

Audio Engine: Web Audio API (Synthesized Oscillators)

Persistence: HTML5 localStorage API

Hosting: GitHub Pages

## 🔮 Future Roadmap
[ ] Custom soundscape tempo and frequency controls
[ ] Export task lists & session summaries to Markdown
[ ] Customizable model selection (e.g., Qwen / SmolLM variants)
[ ] Offline PWA (Progressive Web App) manifest and service worker integration

## 🤝 Contributing
Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

## 📄 License
Distributed under the MIT License. See LICENSE for more information.
