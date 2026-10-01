<h1 align="center">Cheah Ken Win</h1>

<p align="center">
  <b>Computer Vision · AI Engineering · Software Engineering</b><br>
  Final-year Computer Science student at Universiti Tunku Abdul Rahman (UTAR), completing my degree in October 2026 · Malaysia
</p>

<p align="center">
  <a href="mailto:wincheahken@gmail.com"><img src="https://img.shields.io/badge/Email-wincheahken%40gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white" alt="Email"></a>
  <a href="https://github.com/kwincheah"><img src="https://img.shields.io/badge/GitHub-kwincheah-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub"></a>
  <img src="https://img.shields.io/badge/Open_to-Graduate_roles-2EA44F?style=flat-square" alt="Open to graduate roles">
</p>

---

### 👋 About me

- I build **computer vision** systems: object detection, vision-language models and image enhancement
- I care about the whole pipeline: **datasets → training → evaluation → deployment**
- 🎯 Looking for **graduate roles in Computer Vision, AI Engineering or Software Engineering**, available from **October 2026**

---

### 🔬 Featured: Final Year Project

#### Hybrid PCB Defect Inspection with YOLO and Vision-Language Models

A PCB inspection framework that keeps YOLO's speed and uses a VLM to **reduce false rejections (overkill)** caused by harmless visual anomalies.

<p align="center">
  <code>YOLOv11n Observer</code> &nbsp;→&nbsp; <code>Agentic Gateway</code> &nbsp;→&nbsp; <code>VLM Judge</code><br>
  <sub>fast defect localisation &nbsp;·&nbsp; class- and confidence-aware routing &nbsp;·&nbsp; semantic check of escalated crops</sub>
</p>

<table align="center">
  <tr>
    <th>mAP@0.5</th>
    <th>mAP@0.5:0.95</th>
    <th>Precision</th>
    <th>Recall</th>
    <th>Overkill reduction</th>
    <th>VLM configurations tested</th>
  </tr>
  <tr align="center">
    <td><b>0.962</b></td>
    <td>0.599</td>
    <td>0.972</td>
    <td>0.968</td>
    <td><b>52.7%</b></td>
    <td>7</td>
  </tr>
</table>

- Extended a **TDD-Net**-derived dataset (6 defect classes) with **11 synthetic anomaly categories** to test behaviour beyond known defects. Evaluated on a fixed **1,443-image** test set.
- Escalated detections go to the VLM as **high-resolution crops with bounding-box guidance**, which returns structured judgements on structural damage and conductor interaction
- **GPT-5.5** achieved the best diagnostic accuracy. **Qwen3-VL-30B-A3B (MoE)** achieved the highest overkill reduction, and MoE variants clearly beat Dense variants on it
- Proposed the **Overkill Reduction Rate (ORR)** as a system-level metric: a VLM's general accuracy did **not** predict how well it adjudicates

`YOLOv11` `PyTorch` `Vision-Language Models` `GPT-5.5` `Qwen3-VL` `Python` &nbsp;·&nbsp; *Computer Vision, AI for Smart Manufacturing*

---

### 🚀 Projects

<table>
  <tr>
    <td width="50%" valign="top">
      <b><a href="https://github.com/kwincheah/superres-ai">🖼️ SuperResAI</a></b><br>
      <sub>AI image super-resolution platform</sub>
      <ul>
        <li>4× upscaling with <b>Real-ESRGAN</b> (RRDBNet) on <b>GPU workers</b> (Modal)</li>
        <li>Asynchronous job processing, so the UI never blocks</li>
        <li>FastAPI backend, Next.js frontend with a before/after view, Supabase for jobs and storage</li>
      </ul>
      <code>PyTorch</code> <code>Real-ESRGAN</code> <code>FastAPI</code> <code>Next.js</code> <code>Supabase</code>
    </td>
    <td width="50%" valign="top">
      <b><a href="https://github.com/kwincheah/whatsapp_transcript_service">🎙️ WhatsApp Voice & Document Assistant</a></b><br>
      <sub>AI assistant on WhatsApp</sub>
      <ul>
        <li>Transcribes, summarises and translates voice notes and videos</li>
        <li><b>OCR for scanned PDFs</b> with a vision model; answers questions about documents; web search</li>
        <li>Docker on Railway, with CI running a pytest suite</li>
      </ul>
      <code>Python</code> <code>FastAPI</code> <code>OpenAI</code> <code>DeepSeek</code> <code>Docker</code>
    </td>
  </tr>
</table>

**Other projects**

- [BuildIt Construction](https://github.com/kwincheah/ConstructionLandingPage): responsive business website with a projects gallery, contact form and light/dark theme · `Next.js` `React` `TypeScript` `Tailwind CSS`
- [RunPod CV Environment](https://github.com/kwincheah/TFContainerDockerCodebase): GPU-ready Docker image (PyTorch + CUDA, YOLO, Transformers, JupyterLab, SSH) for computer vision training on RunPod, with caches kept on the network volume · `Docker` `PyTorch` `CUDA` `GitHub Actions`

---

### 🛠️ Tech stack

<p>
  <img src="https://skillicons.dev/icons?i=py,pytorch,tensorflow,sklearn,fastapi,ts,react,nextjs,tailwind,postgres,sqlite,supabase,docker,githubactions,linux,git&perline=16" alt="Tech stack icons">
</p>

| Area | Skills |
|---|---|
| **Computer vision** | Object detection (YOLOv11), vision-language models (GPT-5.5, Qwen3-VL), super-resolution (Real-ESRGAN), OCR, synthetic data, evaluation (mAP, precision/recall) |
| **Machine learning** | PyTorch, TensorFlow, scikit-learn, NumPy, Pillow |
| **AI engineering** | GPU inference (Modal), LLM and speech APIs (OpenAI, DeepSeek), asynchronous job pipelines |
| **Software** | Python, TypeScript, FastAPI, REST APIs, React, Next.js, PostgreSQL, SQLite |
| **Tools** | Git, Docker, GitHub Actions, Linux |

---

<p align="center">
  📫 Let's connect: <a href="mailto:wincheahken@gmail.com">wincheahken@gmail.com</a>
</p>
