<div align="center">
<img src="https://raw.githubusercontent.com/Mentora-Classroom-to-Career/.github/main/profile/cropped_circle_image (2).png" alt="Mentora Logo" width="160"/>

# Mentora
### A Smart Platform, From Classroom to Career
*Bridging Pakistan's exam preparation crisis and career guidance gap — with AI.*

[![Next.js](https://img.shields.io/badge/Frontend-Next.js_14-black?style=flat-square&logo=next.js)](https://nextjs.org/)
[![FastAPI](https://img.shields.io/badge/Backend-FastAPI-009688?style=flat-square&logo=fastapi)](https://fastapi.tiangolo.com/)
[![TensorFlow](https://img.shields.io/badge/ML-TensorFlow_2.15-FF6F00?style=flat-square&logo=tensorflow)](https://www.tensorflow.org/)
[![HuggingFace](https://img.shields.io/badge/Models-HuggingFace_Transformers-FFD21E?style=flat-square&logo=huggingface)](https://huggingface.co/)
[![PostgreSQL](https://img.shields.io/badge/Database-PostgreSQL_15-336791?style=flat-square&logo=postgresql)](https://www.postgresql.org/)
[![Docker](https://img.shields.io/badge/Deploy-Docker_Compose-2496ED?style=flat-square&logo=docker)](https://www.docker.com/)
[![License](https://img.shields.io/badge/License-MIT-blue?style=flat-square)](LICENSE)

</div>

---

## 🎯 What is Mentora?

**Mentora** is a unified intelligent platform built for Pakistani students that combines adaptive exam preparation with AI-powered career counseling — all from a single student profile.

Pakistan faces a dual crisis:
- **200,000+** students appear in MDCAT annually with no personalized guidance
- **CSS** has a historical pass rate **below 3%**, yet no intelligent prep system exists
- A large proportion of university graduates — especially from Tier-2 and Tier-3 institutions — receive **zero professional career counseling**

Mentora addresses both problems through a single integration layer called the **Student Intelligence Profile (SIP)** — where exam performance data continuously refines career recommendations, and career goals re-prioritize exam preparation focus areas.

---

## ✨ Core Features

| Feature | Description |
|---|---|
| 🧠 **Knowledge Gap Classifier** | Identifies weak sub-topics from MCQ answer patterns using DeBERTa-v3 |
| ✍️ **Adaptive Question Generator** | Generates new curriculum-aligned exam questions via fine-tuned FLAN-T5 + LoRA |
| 📈 **Performance Trajectory Predictor** | LSTM model that forecasts your exam score 7 days ahead and flags plateau risk |
| 💼 **Career-Skill Semantic Matcher** | Ranks 50+ career profiles against your academic profile using sentence embeddings |
| 📄 **CV / Transcript NER Extractor** | Extracts skills, GPA, certifications, and projects from uploaded documents |
| 🗺️ **6-Month Upskilling Roadmap** | Personalized, career-goal-linked skill-building plan auto-generated per student |
| 🤖 **3 Domain RAG Pipelines** | Retrieval-Augmented Generation for Exam, Career, and Interview knowledge bases |
| 🔗 **Student Intelligence Profile (SIP)** | A shared bidirectional data layer linking exam performance to career recommendations |

---

## 🏗️ System Architecture

```
┌─────────────────────────────────────────────────────┐
│                   FRONTEND LAYER                    │
│     Next.js 14 · Tailwind CSS · shadcn/ui           │
│  Dashboard · Exam UI · Career Explorer · Roadmap    │
└──────────────────────┬──────────────────────────────┘
                       │  REST API / JSON
┌──────────────────────▼──────────────────────────────┐
│                   BACKEND LAYER                     │
│   FastAPI · Auth · SIP Manager · Exam & Career API  │
└─────────────┬──────────────────────┬────────────────┘
              │                      │
┌─────────────▼──────────┐  ┌────────▼───────────────┐
│    ML MODELS LAYER     │  │    RAG + DATA LAYER     │
│  DeBERTa · FLAN-T5     │  │  ChromaDB · LangChain   │
│  LSTM · all-mpnet      │  │  Exam KB · Career KB    │
│  BERT NER              │  │  PostgreSQL (SIP/Users) │
└────────────────────────┘  └────────────────────────┘
```

---

## 🤖 ML Models at a Glance

| # | Model | Architecture | Target Metric |
|---|---|---|---|
| 1 | Knowledge Gap Classifier | DeBERTa-v3-base | F1 ≥ 0.85 |
| 2 | Adaptive Question Generator | FLAN-T5-Large + LoRA | BLEU-4 ≥ 0.35 |
| 3 | Performance Trajectory Predictor | LSTM (2-layer, 128 units) | MAE ≤ 5 pts |
| 4 | Career-Skill Semantic Matcher | all-mpnet-base-v2 | Precision@5 ≥ 0.75 |
| 5 | CV / Transcript NER Extractor | bert-base-uncased | Entity F1 ≥ 0.82 |

---

## 🛠️ Tech Stack

**Backend:** Python 3.11 · FastAPI · PostgreSQL 15 · LangChain · ChromaDB · Ollama (Mistral-7B)
**ML / AI:** TensorFlow 2.15 · HuggingFace Transformers · PEFT (LoRA) · Sentence-Transformers · SpaCy · Scikit-learn
**Frontend:** Next.js 14 · Tailwind CSS · shadcn/ui · Recharts
**DevOps:** Docker · Docker Compose · GitHub · Weights & Biases · Google Colab (T4 GPU)

---

## 🧰 Skills & Frameworks

<div align="center">

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)

**Frameworks & Libraries**

![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![HuggingFace](https://img.shields.io/badge/🤗_Transformers-FFD21E?style=for-the-badge)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)

**Tools & Platforms**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-121212?style=for-the-badge)
![Weights & Biases](https://img.shields.io/badge/Weights_&_Biases-FFBE00?style=for-the-badge&logo=weightsandbiases&logoColor=black)
![Google Colab](https://img.shields.io/badge/Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)

</div>

---

## 📊 GitHub Activity

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=RaimalRaja&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="GitHub Stats" width="49%"/>
<img src="https://streak-stats.demolab.com?user=RaimalRaja&theme=tokyonight&hide_border=true" alt="GitHub Streak" width="49%"/>

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=RaimalRaja&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" alt="Top Languages" width="49%"/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=RaimalRaja&theme=react-dark&hide_border=true" alt="Contribution Graph" width="98%"/>

</div>

> Replace `RaimalRaja` with the relevant GitHub username if these stats should track a different account or an org-wide aggregate.

---

## 📂 Repositories

| Repository | Description |
|---|---|
| [`mentora-backend`](https://github.com/Mentora-Classroom-to-Career/mentora-backend) | FastAPI backend — Auth, SIP Manager, Exam & Career APIs, RAG endpoints |
| [`mentora-frontend`](https://github.com/Mentora-Classroom-to-Career/mentora-frontend) | Next.js 14 student-facing web application |
| [`mentora-ml-models`](https://github.com/Mentora-Classroom-to-Career/mentora-ml-models) | All 5 ML model training scripts, notebooks, and model cards |
| [`mentora-rag-pipelines`](https://github.com/Mentora-Classroom-to-Career/mentora-rag-pipelines) | LangChain + ChromaDB pipelines for Exam, Career, and Interview KBs |
| [`mentora-data`](https://github.com/Mentora-Classroom-to-Career/mentora-data) | Data collection scripts, cleaning pipelines, and processed datasets |
| [`.github`](https://github.com/Mentora-Classroom-to-Career/.github) | Organization profile, issue templates, and contribution guidelines |

---

## 🗓️ Project Phases

```
Phase 1  ████░░░░░░░░░░░░░░░░  Setup & Research
Phase 2  ████░░░░░░░░░░░░░░░░  Data Collection & Cleaning
Phase 3  ████░░░░░░░░░░░░░░░░  RAG Pipeline Development
Phase 4  ████░░░░░░░░░░░░░░░░  ML Models 1 & 5 Training
Phase 5  ████░░░░░░░░░░░░░░░░  ML Models 2, 3 & 4 Training
Phase 6  ████░░░░░░░░░░░░░░░░  SIP Integration Layer
Phase 7  ████░░░░░░░░░░░░░░░░  Backend API Development
Phase 8  ████░░░░░░░░░░░░░░░░  Frontend Development
Phase 9  ████░░░░░░░░░░░░░░░░  User Study & Testing
Phase 10 ████░░░░░░░░░░░░░░░░  Documentation & Submission
```

*20-week development timeline · University of Sindh, Laar Campus Badin*

---

## 👨‍💻 Team

| | Name | Roll No. | Focus Area |
|---|---|---|---|
| 👤 | **Muhammad Haroon Abbas** | 2K23/BLCS/38 | Backend API · ML Models 1, 2, 3 · Exam RAG · Exam Frontend |
| 👤 | **Raimal Raja** | 2K23/BLCS/49 | Backend API · Career API · ML Models 4, 5 · Career & Interview RAG · Career Frontend |

**Supervisor:** Sir Dileep Kumar
**Program:** BS Computer Science · University of Sindh, Laar Campus Badin

---

## 🚀 Getting Started

```bash
# Clone the main repository
git clone https://github.com/Mentora-Classroom-to-Career/mentora-backend.git

# Copy environment variables
cp .env.example .env

# Start all services with Docker Compose
docker-compose up --build
```

> Full setup guide available in each repository's `README.md`.

---

## 📊 Datasets Used

MDCAT Past Papers (2008–2025) · CSS Past Papers · NTS Past Papers · SQuAD 2.0 · O\*NET Occupation Database · Pakistan Job Postings (Rozee.pk) · Career Recommendation Dataset · Resume/CV Dataset · DigiSkills Course Catalog

---

<div align="center">

*Built with ❤️ for Pakistan's students — from classroom to career.*

**University of Sindh, Laar Campus Badin · BS Computer Science · Final Year Project 2025**

</div>
