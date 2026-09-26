## Hi, I'm Cheah Ken Win 👋

Final-semester **Computer Science** student at **Universiti Tunku Abdul Rahman (UTAR)**, completing my degree in **October 2026**.
I work on **computer vision** and **AI engineering**, especially detection models, vision-language models, and getting models into working products.

🎯 **Looking for:** graduate roles in **Computer Vision**, **AI Engineering** or **Software Engineering**, available from October 2026<br>
📫 **Email:** [wincheahken@gmail.com](mailto:wincheahken@gmail.com)

---

### Projects

**Hybrid PCB Defect Inspection with YOLO and Vision-Language Models**: Final Year Project, UTAR
- Designed a three-stage inspection framework:
  - a **YOLOv11n Observer** localises defects quickly
  - an **Agentic Gateway** routes each detection by class and confidence, either rejecting it or escalating it
  - a **VLM Judge** re-examines escalated high-resolution crops with bounding-box guidance and structured responses (structural damage, conductor interaction)
- Extended a **TDD-Net**-derived dataset (6 defect classes) with **11 synthetic anomaly categories**, to test behaviour beyond known defects
- Observer: **0.962 mAP@0.5**, 0.599 mAP@0.5:0.95, 0.972 precision and 0.968 recall on a 1,443-image test set
- Benchmarked **7 VLM configurations**, a pure-YOLO baseline and ablations:
  - **GPT-5.5** gave the best diagnostic accuracy
  - **Qwen3-VL-30B-A3B (MoE)** cut Observer overkill (false rejections) by **52.7%**
- Proposed the **Overkill Reduction Rate (ORR)** as a system-level metric. A VLM's general accuracy did not predict how well it adjudicates, and MoE variants beat Dense variants on ORR
- `YOLOv11` `PyTorch` `Vision-Language Models` `GPT-5.5` `Qwen3-VL` `Python` · *Computer Vision, AI for Smart Manufacturing*

**[SuperResAI](https://github.com/kwincheah/superres-ai)**: AI image super-resolution platform
- Upscales low-resolution images 4× with **Real-ESRGAN** (RRDBNet), using the general and anime model variants
- Runs **PyTorch** inference on serverless **GPU workers (Modal)**, with asynchronous job processing so the UI never blocks
- **FastAPI** backend, **Next.js** frontend with a before/after comparison view, and **Supabase** for job tracking and image storage
- `PyTorch` `Real-ESRGAN` `Pillow` `NumPy` `FastAPI` `Next.js` `Supabase` `Modal`

**[WhatsApp Voice & Document Assistant](https://github.com/kwincheah/whatsapp_transcript_service)**: AI assistant on WhatsApp
- Transcribes voice notes and videos, summarises and translates them, and answers questions about forwarded files
- **OCR for scanned PDFs**: renders pages without a text layer to images and reads them with a vision model, OCR-ing only the pages that need it
- Reads PDF and Word documents and can search the web, showing the latency and cost of every reply
- Deployed with **Docker on Railway**, with **CI** running a pytest suite
- `Python` `FastAPI` `OpenAI API` `DeepSeek` `pypdfium2` `SQLite` `Docker` `GitHub Actions`

**[TensorFlow ML Container](https://github.com/kwincheah/TFContainerDockerCodebase)**: reproducible training environment
- Ubuntu + Python + TensorFlow image with NumPy, Pandas, Matplotlib and scikit-learn
- A **GitHub Actions** workflow publishes it to GitHub Container Registry
- `Docker` `TensorFlow` `GitHub Actions`

**[BuildIt Construction](https://github.com/kwincheah/ConstructionLandingPage)**: responsive business website
- Services, projects gallery, contact form and light/dark theme
- `Next.js` `React` `TypeScript` `Tailwind CSS`

---

### Skills

- **Computer vision:** object detection (YOLOv11), vision-language models (GPT-5.5, Qwen3-VL), image super-resolution (Real-ESRGAN), OCR pipelines, synthetic data generation, evaluation (mAP, precision/recall)
- **ML frameworks:** PyTorch, TensorFlow, scikit-learn, NumPy, Pillow
- **AI engineering:** model deployment on GPU workers, LLM & speech APIs (OpenAI, DeepSeek), asynchronous job queues
- **Backend:** Python, FastAPI, REST APIs, PostgreSQL (Supabase), SQLite
- **Frontend:** TypeScript, React, Next.js, Tailwind CSS
- **Tools:** Git, Docker, GitHub Actions, Linux

---

### Contact

📫 [wincheahken@gmail.com](mailto:wincheahken@gmail.com)
