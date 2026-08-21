<img src="https://capsule-render.vercel.app/api?type=waving&height=300&color=0:0077b6,50:00b4d8&text=Siva%20S&fontColor=ffffff&desc=CAE%20Engineer%20building%20Healthcare%20AI%20%E2%80%A2%20Agentic%20Systems%20%E2%80%A2%20RAG%20%E2%80%A2%20Medical%20Imaging&descAlign=50&fontAlign=50&fontAlignY=38&descAlignY=58" alt="header" />

<p align="center">
  <a href="https://github.com/sivasoundhar?tab=followers"><img src="https://img.shields.io/github/followers/sivasoundhar?style=for-the-badge&color=00b4d8&labelColor=0d1117&label=Followers" alt="followers" /></a>
  <img src="https://komarev.com/ghpvc/?username=sivasoundhar&style=for-the-badge&color=00b4d8&labelColor=0d1117&label=Profile+Views" alt="views" />
  <a href="https://linkedin.com/in/YOUR-HANDLE"><img src="https://img.shields.io/badge/LinkedIn-0077b6?style=for-the-badge&logo=linkedin&logoColor=white" alt="linkedin" /></a>
  <a href="mailto:sivasoundhar93@gmail.com"><img src="https://img.shields.io/badge/Email-0d1117?style=for-the-badge&logo=gmail&logoColor=00b4d8" alt="email" /></a>
</p>

---

## About Me

| | | |
|---|---|---|
| 🧠 | **Currently building** | Healthcare AI — agentic RAG, multi-agent clinical pipelines, medical imaging |
| 🏥 | **Domain focus** | Medical & healthcare AI — clinical documents, diagnostic imaging, HIPAA-aware design |
| ⚙️ | **Bridging** | Physics-based simulation ↔ Generative AI |
| 🤝 | **Open to** | AI / ML Engineer roles, healthcare AI collaborations |
| 📬 | **Contact** | <sivasoundhar93@gmail.com> |

---

## Featured Work

### 🧬 UniRAG — Universal Adaptive Agentic RAG Platform
Production RAG engine with adaptive routing and self-correction — not a vector-search wrapper.

- **Hybrid retrieval** — BM25 + dense (BAAI/bge-large-en-v1.5), RRF fusion, cross-encoder reranking
- **Agentic layer** — corrective RAG loops and adaptive query routing; the system decides *how* to retrieve
- **Resilient gateway** — Groq primary, local Ollama fallback; runs fully offline
- **Production concerns** — NeMo Guardrails, eval harness, structured logging, versioned FastAPI, Docker Compose

`LangGraph` `ChromaDB` `FastAPI` `Groq` `Ollama` `Docker`

**[→ Repository](https://github.com/sivasoundhar/unirag)**

---

### 🫁 Medical Imaging AI Copilot
Dual-modality diagnostic prototype — 2D chest X-ray classification and 3D CT nodule detection.

- ResNet50 fine-tune for pneumonia classification with **Grad-CAM explainability**
- Custom 3D CNN on LUNA16 CT volumes — ROC-AUC 0.777 on a sparse-positive split
- Multi-candidate report generation, PDF export, SQLite-backed report history
- 188/188 passing test suite; clean `tsc` / `vite build` / `oxlint`

> Research prototype, not a clinical device. The 3D precision numbers are statistically fragile on a 9-positive test split — documented in the repo rather than hidden.

`PyTorch` `FastAPI` `React` `TypeScript` `Grad-CAM`

**[→ Repository](https://github.com/sivasoundhar/medical-imaging-copilot)**

---

### 🩺 MedIntel AI — Multi-Agent Clinical Document Intelligence
Four specialized reasoning agents under a LangGraph supervisor.

| Agent | Reasoning task |
|---|---|
| **PHI Reasoner** | Context-aware detection — is "Smith" the patient or the attending physician? |
| **De-ID Strategist** | Selective masking that preserves clinical readability |
| **Clinical Analyzer** | Prioritizes diagnoses and medications over administrative noise |
| **QA Verification** | Cites source or refuses — hallucination-resistant by design |

Multi-clinician access control with a full HIPAA-style audit trail.

`LangGraph` `FastAPI` `HTMX` `Tailwind` `SQLite` `Docker`

**[→ Repository](https://github.com/sivasoundhar/medintel-ai)**

---

## Tech Stack

**AI & Agents**

![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langgraph&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![Groq](https://img.shields.io/badge/Groq-F55036?style=flat-square&logo=groq&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6F00?style=flat-square)

**ML & Data**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)

**Backend & Ops**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

**Simulation & CAE**

![ABAQUS](https://img.shields.io/badge/ABAQUS-005386?style=flat-square)
![NASTRAN](https://img.shields.io/badge/NASTRAN-0B5FA5?style=flat-square)
![FEMFAT](https://img.shields.io/badge/FEMFAT-4A7C59?style=flat-square)
![ANSA](https://img.shields.io/badge/ANSA-7B2D8E?style=flat-square)
![HyperMesh](https://img.shields.io/badge/HyperMesh-1F4E79?style=flat-square)

---

## GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=sivasoundhar&show_icons=true&count_private=true&hide_border=true&title_color=00b4d8&icon_color=00b4d8" alt="stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=sivasoundhar&layout=compact&langs_count=8&hide_border=true&title_color=00b4d8" alt="top languages" />
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com/?user=sivasoundhar&hide_border=true&ring=00b4d8&fire=00b4d8&currStreakLabel=00b4d8" alt="streak" />
</p>

---

### 🚀 Designing intelligent healthcare systems with AI, agents and engineering rigour.

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0077b6,100:00b4d8&height=120&section=footer" alt="footer" />
