<h1 align="center">Cheah Ken Win</h1>

<p align="center">
  <b>Computer Vision · AI Engineering · Software Engineering</b><br>
  Computer Science graduate, First Class Honours (Distinction), Universiti Tunku Abdul Rahman (UTAR), 2026 · Malaysia
</p>

<p align="center">
  <a href="mailto:wincheahken@gmail.com"><img src="https://img.shields.io/badge/Email-wincheahken%40gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white" alt="Email"></a>
  <a href="https://github.com/kwincheah"><img src="https://img.shields.io/badge/GitHub-kwincheah-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub"></a>
  <img src="https://img.shields.io/badge/Open_to-Graduate_roles_·_Malaysia_&_Singapore-2EA44F?style=flat-square" alt="Open to graduate roles in Malaysia and Singapore">
</p>

---

### 👋 About me

- I build **computer vision and AI software that runs outside the notebook**: trained models, inspection tools, APIs and desktop apps
- I care about the whole pipeline: **datasets → training → evaluation → deployment**
- Industry experience as an **Application Engineer Intern in machine vision** (Bitmap Engineering, Oct 2025 – Jan 2026)
- 🎯 Looking for **graduate roles in Computer Vision, AI Engineering or Software Engineering**, available now

---

### 💼 Experience

**Application Engineer Intern (Machine Vision / Deep Learning)**, Bitmap Engineering · Oct 2025 – Jan 2026

- Trained and evaluated **5 deep learning defect-detection models** for glove manufacturing (stain, hole, tear and more) with Hikrobot VisionMaster, on a ~20,000-image dataset
- Cut the longest training run from **~26 hours to 1.5 hours** (about 94% faster)
- Built the [**Glove AI Performance Tracker**](https://github.com/kwincheah/Glove-AI-Performance-Tracker): a C# / WPF app running up to **11 concurrent inspection flows across 12 production lines at ~12 ms per image**

---

### 🔬 Featured research: Final Year Project

#### [Hybrid YOLO + Vision-Language Model framework for out-of-distribution PCB defects](https://github.com/kwincheah/FYP-PCB-Inspection)

**Question:** can a vision-language model (VLM) reliably judge a detector's uncertain defect calls, and cut false rejections (overkill) caused by harmless marks?

**Key finding:** across **7 VLM configurations**, general accuracy did **not** predict adjudication value. **Qwen3-VL-30B-A3B (Mixture-of-Experts)** cut the detector's false rejections by **52.7%**, despite lower diagnostic accuracy than GPT-5.5. I proposed the **Overkill Reduction Rate (ORR)** as a system-level metric for this.

<p align="center">
  <code>YOLOv11n Observer</code> &nbsp;→&nbsp; <code>Agentic Gateway</code> &nbsp;→&nbsp; <code>VLM Judge</code><br>
  <sub>fast defect localisation &nbsp;·&nbsp; class- and confidence-aware routing &nbsp;·&nbsp; semantic check of escalated crops</sub>
</p>

<table align="center">
  <tr>
    <th>Overkill reduction (ORR)</th>
    <th>VLM configurations tested</th>
    <th>Baseline mAP@0.5</th>
    <th>Precision</th>
    <th>Recall</th>
  </tr>
  <tr align="center">
    <td><b>52.7%</b></td>
    <td>7</td>
    <td>0.962</td>
    <td>0.972</td>
    <td>0.968</td>
  </tr>
</table>

- Extended a TDD-Net-derived dataset (6 defect classes) with **11 synthetic anomaly categories**; fixed 1,443-image test set
- Escalated detections reach the VLM as **high-resolution crops with bounding-box guidance** and return structured judgements
- Mixture-of-Experts variants clearly beat Dense variants on overkill reduction

`YOLOv11` `PyTorch` `Vision-Language Models` `GPT-5.5` `Qwen3-VL` `Python` &nbsp;·&nbsp; [Full report](https://github.com/kwincheah/FYP-PCB-Inspection/tree/main/report)

---

### 🏭 Featured project: Apex Industrial Vision Studio

#### [Desktop machine vision platform](https://github.com/kwincheah/vision-studio): build inspections by wiring blocks, or describe them and let AI build them

<p align="center">
  <a href="https://github.com/kwincheah/vision-studio"><img src="https://github.com/kwincheah/vision-studio/raw/main/docs/screenshots/qml/workspace_flow.png" alt="Apex Vision Studio flow editor" width="85%"></a>
</p>

- Node-based flow editor with **40 image processing, measurement and location tools** plus **YOLO inference** from PyTorch, ONNX or TensorRT engines
- **Hikrobot GigE / USB3 industrial cameras**, RTSP streams, OpenCV lens calibration, and a TCP/IP tool that sends OK/NG results to PLCs and robots
- **AI Gen**: a tool-using LLM agent that turns plain-language requests into validated inspection flows, checking against a JSON Schema and repairing its own errors (Claude, OpenAI, Gemini, DeepSeek, local Ollama and more)
- Plugin SDK, **1,300+ automated tests** in GitHub Actions CI, packaged Windows installer

`Python` `Qt Quick / QML` `OpenCV` `PyTorch` `ONNX` `TensorRT` `pytest`

---

### 🚀 More projects

<table>
  <tr>
    <td width="50%" valign="top">
      <b><a href="https://github.com/kwincheah/Glove-AI-Performance-Tracker">🧤 Glove AI Performance Tracker</a></b><br>
      <sub>Multi-line inspection and AI model validation app (internship)</sub>
      <ul>
        <li>Up to 11 concurrent inspection flows across 12 production lines, ~12 ms per image</li>
        <li>Thread-safe procedure pool, rate limiting, live views and per-line yield summaries</li>
        <li>Background export of false positives / negatives for retraining</li>
      </ul>
      <code>C#</code> <code>.NET</code> <code>WPF</code> <code>Hikrobot VisionMaster SDK</code>
    </td>
    <td width="50%" valign="top">
      <b><a href="https://github.com/kwincheah/whatsapp_transcript_service">🎙️ WhatsApp Voice & Document Assistant</a></b><br>
      <sub>Deployed AI assistant on WhatsApp</sub>
      <ul>
        <li>Transcribes, summarises and translates voice notes and videos (built for Manglish)</li>
        <li><b>OCR for scanned PDFs</b>; answers questions about documents; web search with sources</li>
        <li>SQL data layer with FTS5 search and cost reporting; Docker on Railway, pytest in CI</li>
      </ul>
      <code>Python</code> <code>FastAPI</code> <code>SQLite</code> <code>OpenAI</code> <code>DeepSeek</code> <code>Docker</code>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <b><a href="https://github.com/kwincheah/FinanceReportAnalyzer">📈 Bursa Intelligence</a></b><br>
      <sub>Financial analysis terminal for Bursa Malaysia equities</sub>
      <ul>
        <li>Automated quarterly report ingestion, financial statements and interactive charts</li>
        <li><b>4-stage RAG pipeline</b>: table-aware chunking, hybrid BM25 + ChromaDB retrieval (RRF), cross-encoder reranking, cited answers</li>
        <li>Web app and Tauri desktop build</li>
      </ul>
      <code>Python</code> <code>FastAPI</code> <code>RAG</code> <code>ChromaDB</code> <code>Next.js</code> <code>Tauri</code>
    </td>
    <td width="50%" valign="top">
      <b><a href="https://github.com/kwincheah/superres-ai">🖼️ SuperResAI</a></b><br>
      <sub>AI image super-resolution platform</sub>
      <ul>
        <li>4× upscaling with <b>Real-ESRGAN</b> on <b>GPU workers</b> (Modal)</li>
        <li>Asynchronous job processing, so the UI never blocks</li>
        <li>FastAPI backend, Next.js frontend with a before/after view, Supabase for jobs and storage</li>
      </ul>
      <code>PyTorch</code> <code>Real-ESRGAN</code> <code>FastAPI</code> <code>Next.js</code> <code>Supabase</code>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <b><a href="https://github.com/kwincheah/tailscaleNotify">🔔 TailscaleNotify</a></b><br>
      <sub>Native desktop alert and quick-action overlay for Tailscale Taildrop</sub>
      <ul>
        <li>Real-time file watcher with debounced arrival detection on macOS, Windows and Linux</li>
        <li>Filters out browser downloads using macOS quarantine xattrs and Windows Zone.Identifier</li>
        <li>Floating macOS panel over full-screen apps, image previews, safe scoped file opening</li>
      </ul>
      <code>Rust</code> <code>Tauri</code> <code>TypeScript</code>
    </td>
    <td width="50%" valign="top">
      <b><a href="https://github.com/kwincheah/TFContainerDockerCodebase">🐳 RunPod CV Environment</a></b><br>
      <sub>GPU-ready container for CV and VLM work</sub>
      <ul>
        <li>Version-pinned PyTorch + CUDA 12.6, Ultralytics YOLO, Transformers, JupyterLab and SSH</li>
        <li>Model and dataset caches on a persistent network volume, so new pods start ready to train</li>
        <li>Automated build, GPU smoke test and publishing via GitHub Actions</li>
      </ul>
      <code>Docker</code> <code>PyTorch</code> <code>CUDA</code> <code>GitHub Actions</code> <code>Linux</code>
    </td>
  </tr>
</table>

**Other projects**

- [BuildIt Construction](https://github.com/kwincheah/ConstructionLandingPage): responsive business website with a projects gallery, contact form and light/dark theme · `Next.js` `React` `TypeScript` `Tailwind CSS`

---

### 🛠️ Tech stack

<p>
  <img src="https://skillicons.dev/icons?i=py,pytorch,opencv,cs,dotnet,qt,fastapi,rust,tauri,ts,react,nextjs,postgres,sqlite,docker,githubactions,linux,git&perline=18" alt="Tech stack icons">
</p>

| Area | Skills |
|---|---|
| **Computer vision** | Object detection (YOLOv11), vision-language models (GPT-5.5, Qwen3-VL), industrial cameras and calibration, OCR, super-resolution (Real-ESRGAN), synthetic data, evaluation (mAP, precision/recall, F1) |
| **Machine learning** | PyTorch, Ultralytics, ONNX, TensorRT, scikit-learn, NumPy |
| **AI engineering** | Tool-using LLM agents, structured outputs (JSON Schema), RAG, MCP, LLM APIs (Claude, OpenAI, DeepSeek), GPU inference |
| **Software** | Python, C# / .NET (WPF), TypeScript, Rust, FastAPI, Qt (PyQt6 / QML), Next.js, Tauri, SQL (PostgreSQL, SQLite) |
| **Tools** | Git, Docker, GitHub Actions, pytest, Linux, Hikrobot VisionMaster |

---

<p align="center">
  📫 Let's connect: <a href="mailto:wincheahken@gmail.com">wincheahken@gmail.com</a>
</p>
