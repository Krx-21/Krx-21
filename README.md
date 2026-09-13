# Hi, I'm Kritchaya Chaowajareun 👋

3rd-year Computer Engineering and Digital Technology student, Faculty of Engineering, Chulalongkorn University. I build applied AI and computer-vision systems and the data infrastructure behind them — two internships (Bank of Thailand, Charoen Pokphand Foods) and an ongoing quant-trading capstone.

## 📍 Now

Capstone project (in progress) — **Regime-Detection-Based Algorithmic Trading using HMM and Order Book Imbalance** (team of 4 CEDT students). My part is the data infrastructure: I designed and operate a 24/7 Binance level-2 market-data collector.

```text
Binance level-2 streams  (spot + USDⓈ-M perp, BTCUSDT / ETHUSDT)
  -> depth20@100ms order-book snapshots + trades + bookTicker + funding rate
  -> zstd-compressed Parquet, rotated every 10 min  (~1 GB/day)
  -> health checks + single-instance locking + clock-sync tuning
  -> daily rclone backup to Google Drive, checksum-verified
  -> reproducibility checks on Google Colab
```

Collecting since 27 July 2026 (collector code lives in a private repo).

---

## 💼 Experience

### Charoen Pokphand Foods PCL (CPF) — AI/ML Intern, Image Processing & Computer Vision
*AI Machine Development unit · 18 May – 10 July 2026 · 8 weeks · on-site, Bangkok · internal/private projects*

- **ThermalVision** — Windows desktop app (C# / .NET WPF) unifying a YOLOv8-seg (ONNX Runtime) detection mode with a classical image-processing mode to measure product temperature from thermal-camera images; integrates a Mettler Toledo weighing scale, RTSP cameras and Modbus TCP I/O; delivered as a self-contained installer.
- **Black Hot Vision** — classical image-processing pipeline (detector / tracker / de-dup / CSV logger) for thermal video, tested on factory footage; later merged into ThermalVision.
- **CPF_OCR** — production-line image-inspection web app (team project). Owned the frontend, a Preact + TypeScript SPA (scaffold, OCR/position config pages, ROI editor, run-inspection page, master-image registration, folder picker), and integrated a backend-trained YOLOv11n verification model with a confidence slider and de-duplication tracking.
- **AI_ML_CV** — desktop tool (Python, PyQt6/PySide6) for SAM-assisted annotation, YOLO training, evaluation and ONNX export, with an installer. Trained YOLO11-seg on a CPF chicken/duck dataset (2,013 train / 110 val / 111 test images) to mAP50 ≈ 0.99, exported to ONNX.
- **shrimp_counter** — SAM-assisted tool for counting and labeling shrimp larvae; client-server design using a remote GPU over Tailscale VPN; used to count and label 150 of 258 real images.
- **MeterMap** — WPF plant-map monitoring app for factory electricity meters (meter pins, 16 electrical values per meter, SQLite logging, alarms/thresholds, dashboard). My part: the Modbus RTU integration and register decoder on Node-RED, tested end-to-end with mock data only (not connected to real meters during the internship).

### Bank of Thailand — Intern
*Summer 2025 · internal project, private repo*

- Built **N'Book3**, an internal AI knowledge assistant for Bank of Thailand employees on Microsoft Copilot Studio, covering the financial and economic statistics bank teams use (financial-institution, real-sector, survey, payment, foreign-debt and import/export data). Published on Copilot Studio 30 May 2025.
- Defined the agent and topics in YAML — search and variable search, disambiguation when several topics match, conversation-context and history tracking, fallback, escalation, error handling, sign-in — with knowledge sources connected via SharePoint search; tuned intent recognition and disambiguation against written test scenarios.
- Built custom actions `FindVariables`, `CompareVariables` and `LocateVariableInDocument`; bilingual Thai/English with conversation-context memory.

---

## 🎓 Education

- **Chulalongkorn University**, Faculty of Engineering, Department of Computer Engineering — B.Eng. Computer Engineering and Digital Technology (CEDT 02 / INTANIA 108). Entered 2024; now in 3rd year (academic year 2026, first semester).
  - Coursework: Software-Defined Systems (Docker microservices, Kubernetes deployments), IoT, Computer Security, System Design, Software Engineering.
  - 2025: Software Development Practice II (Next.js / TypeScript course projects).
- **Princess Chulabhorn Science High School Satun** (PCSHSST 27), 2022–2024.

---

## 🧰 Skills

| Domain | Tools |
|---|---|
| Languages | Python, C#, TypeScript/JavaScript, C/C++, Java |
| AI / Computer Vision | OpenCV, YOLO (Ultralytics YOLOv8 / YOLO11), ONNX Runtime, Segment Anything (SAM), model training/eval/export pipelines |
| LLM / RAG | Google Gemini API, GraphRAG, retrieval (BM25 / TF-IDF / RRF), Microsoft Copilot Studio |
| Desktop | .NET WPF, PyQt6/PySide6, Electron |
| Web | Next.js, Preact, Angular, Tailwind CSS, Firebase, Streamlit |
| Data / Infra | pandas, Parquet, SQLite, Neo4j, Docker, Kubernetes, GitHub Actions, rclone, Node-RED, Modbus (TCP/RTU), Tailscale |
| Game | Unity, JavaFX |
| Environment | Git/GitHub, Windows, Linux |

---

## 🚀 Side projects

- [**Thai-Legal-GraphRAG**](https://github.com/Krx-21/Thai-Legal-GraphRAG) — Thai legal QA with GraphRAG: NetworkX/Neo4j knowledge graph, hybrid BM25 + dense retrieval with RRF, Gemini answers with section citations, Streamlit UI.
- [**AI_Vtube "Pailin"**](https://github.com/Krx-21/AI_Vtube) — Thai-speaking AI VTuber: Gemini chatbot + speech-to-text + edge-tts text-to-speech, fully async monorepo with GitHub Actions CI.
- [**beyond-depth-launcher**](https://github.com/Krx-21/beyond-depth-launcher) — standalone Electron launcher for a Minecraft (Forge 1.20.1) modpack, with offline mode and auto-update via a GitHub Releases manifest.

---

## 🏆 Awards & Activities

- ExxonMobil IT Bootcathon 2024 — selected participant, Analytics/ML track (21 June – 19 July 2024).
- KAGAYAKI Award 2023 (Kanazawa University science/research project competition, 24 July – 23 September 2023) — one of the top-6 finalist teams; physical-therapy equipment games for hand and leg physiotherapy for people with ALS (Unity game + ESP8266 board).
- POSN (Thai Academic Olympiad) Computer Science training camps 1 & 2, 2022 academic year (PSU Pattani center) — passed the criteria.
- First runner-up (gold medal), computer programming competition (grades 10–12), 70th Regional Student Art and Skill Competition 2022, Satun.
- Certificates: Samsung Innovation Campus Advanced Coding 2022; Chula MOOC (Python basics, data processing with NumPy/Matplotlib, data analytics & big data, 3D modeling); Thai MOOC.

---

## 📫 Contact

**Email:** 6733007821@student.chula.ac.th
