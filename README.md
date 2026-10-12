# ⚡ ToDoozAI: In-Browser Smart Task & Focus Assistant

> *A privacy-first productivity dashboard with task-bound ToDoozie timers, local WebGPU AI breakdowns, and an integrated Spotify player.*

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Tech Stack](https://img.shields.io/badge/tech-HTML5%20%7C%20CSS3%20%7C%20JS%20%7C%20Transformers.js-orange)
![Hosting](https://img.shields.io/badge/hosting-GitHub%20Pages-brightgreen)

---

## 💡 The Vision: Lightweight, Frictionless AI & Focus Tools

**ToDoozAI** explores a simple question:  
**"Can we build useful, modern productivity tools with local AI that run 100% inside the browser without backend servers, subscription costs, or exposed API keys?"**

Most AI utilities rely on heavy cloud APIs or server infrastructure. **ToDoozAI** shifts everything to the client side. By pairing **Task-Bound ToDoozie Timers**, an **in-browser LLM** (`@huggingface/transformers`), **LocalStorage persistence**, and an **embedded Spotify Focus widget**, it offers a complete focus workspace hosted directly on GitHub Pages for $0.

---

## ✨ Key Features

- ⏱️ **Task-Associated ToDoozie Timers:** Each task features its own dedicated 25-minute countdown timer. Starting a timer automatically shifts task status to *In Progress* and auto-completes it upon session finish.
- 🤖 **In-Browser AI Task Breakdown:** Uses **Gemma-3 270M (ONNX)** running locally to decompose complex, daunting tasks into 3 actionable 25-minute steps.
- 🎵 **Floating Spotify Focus Widget:** Fixed in the upper-right corner for quick access to curated lo-fi and focus playlists while working.
- 📊 **Three-State Task Lifecycle:** Track progress across **Not Started**, **In Progress**, and **Done** with clickable status badges.
- 💾 **LocalStorage Persistence:** All tasks, active subtasks, and remaining timer states persist automatically across browser refreshes.
- 🔒 **100% Local & Private:** Prompts and task data never leave your browser. Zero backend telemetry, zero API key requirements.
- ⚡ **WebGPU / WASM Accelerated:** High-performance local AI execution powered by your browser's graphics processing or WASM fallback.
- 💸 **$0 Cost to Host:** Single-file static architecture native to GitHub Pages.

---

## 🛠️ How It Works Under the Hood
<img width="1024" height="559" alt="image" src="https://github.com/user-attachments/assets/0ac6b0b3-14b1-4174-8ad6-abc31ad3c3d8" />



1. **Client-Side Architecture:** The entire app runs out of a single `index.html` file using standard web APIs and CDN-loaded ES modules.
2. **Model Caching:** On first execution, the quantized ~270M parameter model is cached locally in `IndexedDB`, allowing subsequent task breakdowns to generate quickly.
3. **Smart State Management:** Starting a focus timer on one task automatically pauses any other running timer to keep you focused on a single priority at a time.

---

## 🚀 Live Demo & Quickstart

### 1. View Live
Try the live app on GitHub Pages:  
👉 **https://zachncurry.github.io/**

### 2. Run Locally
No `npm install`, Node.js server, or build step required!

1. Clone the repository:
   ```bash
   git clone [https://github.com/](https://github.com/)<zachncurry>/<zachncurry.github.io>.git


## 📊 Tech Stack
Frontend: HTML5, CSS3 (CSS Variables & Flexbox), Vanilla JavaScript (ES6 Modules)
AI Engine: @huggingface/transformers v3
Model: onnx-community/gemma-3-270m-it-ONNX
Integrations: Spotify Embed iFrame API
Persistence: HTML5 localStorage & IndexedDB
Hosting: GitHub Pages

## 🔮 Future Roadmap
[ ] Custom ToDoozAI duration sliders per task
[ ] Drag-and-drop task reordering
[ ] Export completed tasks & session logs to Markdown/CSV
[ ] Custom Spotify playlist URL input in widget settings

## 🤝 Contributing
Contributions, feature requests, and bug reports are welcome! Feel free to open an issue or submit a pull request.
