📄 README.md Content (Full Markdown)
# SUMMERINTERNSHIP2025_22AIML003

> **Role:** AI–ML Intern  
> **Company:** Trionic LLP, Ahmedabad  
> **Domain:** Agentic AI (Single-Agent & Multi-Agent Systems)  
> **Duration:** 19 May 2025 – 28 June 2025

---

## 📌 Introduction
This repository documents my work, learnings, and project deliverables from my **Summer Internship 2025** at **Trionic LLP**.  
The internship focused on **Agentic AI** — learning agent concepts, building a **single-agent app** (YouTube URL → Blog Generator), and designing a **multi-agent system** for the **education** domain.  
Tech stack: **Python, LangChain, LLMs, Streamlit, YouTube API, Vector DB (Chroma/FAISS)**.

---

## 🧭 Internship Overview
At Trionic LLP, I worked on two core tracks:

1. **Single-Agent System**
   - **Project:** *YouTube URL → Blog Generator*
   - **Stack:** Python, LangChain, LLMs, YouTube API, Streamlit
   - **Output:** Transcript extraction → summarization → blog generation with headings/subheadings in a web UI.

2. **Multi-Agent System (Education)**
   - **Project:** *Faculty Assistance Platform*
   - **Agents:** Content Agent, Exam Agent, Tutor Agent, Video/Script Agent
   - **Stack:** Python, LangChain (agent/tool orchestration), Streamlit, Vector DB (Chroma/FAISS)
   - **Output:** Automated content creation, question generation, coding help, and script generation.

---

## 🎯 Responsibilities
- Studied **Agentic AI** fundamentals (perception → reasoning → action; single vs multi-agent).
- Implemented **LangChain**-based agents with role prompts and tools.
- Integrated **YouTube API** for transcript fetch and preprocessing.
- Built **Streamlit** UIs for both projects.
- Implemented **vector search** (Chroma/FAISS) for syllabus/notes grounding.
- Performed **prompt engineering**, evaluation, and iterative refinement.
- Wrote **technical documentation** and demo notes.

---

## 🗂️ Repository Structure


.
├── single_agent_youtube_blog/
│   ├── app.py
│   ├── requirements.txt
│   ├── README.md
│   └── images/
│       └── ui_screenshot.png
├── multi_agent_edu/
│   ├── app.py
│   ├── agents/
│   │   ├── content_agent.py
│   │   ├── exam_agent.py
│   │   ├── tutor_agent.py
│   │   └── video_agent.py
│   ├── data/
│   │   └── sample_docs/
│   ├── requirements.txt
│   ├── README.md
│   └── images/
│       ├── architecture.png
│       └── dashboard.png
└── README.md  <-- (this file)

## 🚀 How to Run (Quick Start)

> **Prerequisites:** Python 3.10+, a supported LLM provider key (e.g., `OPENAI_API_KEY`) in your environment, and (optionally) a YouTube Data API key.

### 1) Single-Agent: YouTube URL → Blog
```bash
cd single_agent_youtube_blog
python -m venv .venv && source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
export OPENAI_API_KEY="your-key"                     # Windows: set OPENAI_API_KEY=your-key
export YT_API_KEY="your-youtube-key"                 # optional if using transcript libs
streamlit run app.py

2) Multi-Agent: Education Assistant
cd multi_agent_edu
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
export OPENAI_API_KEY="your-key"
streamlit run app.py

```

## 📅 Weekly Progress

### **Week 1: 19 May – 24 May 2025**
- Orientation at Trionic LLP; environment setup and access.
- Studied **Agentic AI fundamentals**: perception, reasoning, action loops.
- Compared **single vs. multi-agent** design patterns.
- Explored **LangChain agents, tools, memory**, and example blueprints.
- Drafted scopes for **Single-Agent Project** and **Multi-Agent System**.  
✅ **Outcome**: Project plans finalized; tech stack confirmed.

---

### **Week 2: 26 May – 31 May 2025**
- Implemented **YouTube transcript ingestion and preprocessing**.
- Built **LangChain summarization → blog format generator**.
- Developed **Streamlit UI** for blog preview.  
✅ **Outcome**: Single-Agent app MVP functional.  
📷 ![UI Screenshot](single_agent_youtube_blog/images/ui_screenshot.png)

---

### **Week 3: 2 June – 7 June 2025**
- Designed **Multi-Agent architecture** and defined agent roles.
- Developed **Content Agent** and **Exam Agent**.
- Integrated **Chroma / FAISS** for RAG (retrieval-augmented generation).  
✅ **Outcome**: Core pipeline functional with two agents.  
📷 ![Architecture Diagram](multi_agent_edu/images/architecture.png)

---

### **Week 4: 9 June – 14 June 2025**
- Added **Tutor Agent** for syllabus-grounded Q&A.
- Prototyped **Video/Script Agent**.
- Integrated agent flows and validations.  
✅ **Outcome**: Four-agent flow working end-to-end.

---

### **Week 5: 16 June – 21 June 2025**
- Refined prompts and reduced hallucinations via RAG.
- Added **export options**: Markdown, CSV, TXT.
- UI polish and **caching** for performance.  
✅ **Outcome**: Faster, more reliable, low-cost outputs.  
📷 ![Dashboard Screenshot](multi_agent_edu/images/dashboard.png)

---

### **Week 6: 23 June – 28 June 2025**
- Final tests, bug fixes, documentation, and demos.
- Prepared **internship report** content and deliverables.  
✅ **Outcome**: Project ready for demo and submission.

---

## 🔧 Tech Stack

- **Language**: Python  
- **Framework**: LangChain  
- **Models**: LLMs (via `OPENAI_API_KEY`)  
- **UI**: Streamlit  
- **APIs**: YouTube API (optional TTS/Video APIs)  
- **Vector DB**: ChromaDB / FAISS  
- **Utilities**: Pydantic, Requests, tiktoken, python-dotenv  

---

## 🧪 Key Deliverables

### **1. Single-Agent – YouTube URL → Blog**
- Transcript → Summary → Blog generator pipeline
- Streamlit UI with copy/download functionality

### **2. Multi-Agent – Education Assistant**
- **Content Agent**: Notes, lecture outlines  
- **Exam Agent**: MCQs, coding tasks, difficulty tagging  
- **Tutor Agent**: Contextual Q&A (syllabus-based)  
- **Video/Script Agent**: Draft lesson scripts, TTS hooks  
- Modular agents coordinated via **LangChain orchestration**

---

## 📊 Results & Insights

- **Single-Agent**: Fast to build; best for narrow, focused tasks.  
- **Multi-Agent**: Scalable, modular design handles complexity.  
- **RAG**: Reduced hallucinations, improved alignment with syllabus.  
- **Prompt Engineering**: Roles + constraints significantly improved output accuracy and latency.  
- **Caching**: Reduced token cost and boosted speed.

---

## 🧠 Learnings

- Hands-on experience with **agent design & orchestration**
- Mastery of **prompt engineering** and **RAG techniques**
- Integrated **UI + API** workflows
- Built **export-ready academic content** pipelines

---

## 📸 Screenshots (Placeholders)

> Replace these placeholder paths with real screenshots using the same filenames:

- `single_agent_youtube_blog/images/ui_screenshot.png`  
- `multi_agent_edu/images/architecture.png`  
- `multi_agent_edu/images/dashboard.png`

---

## 🙌 Acknowledgements

Grateful to the **mentors and team at Trionic LLP** for continuous support, constructive feedback, and knowledge sharing throughout the internship.

---

## 📄 License

This repository is intended **for academic and demonstration purposes only** as part of the **Summer Internship 2025** at **Trionic LLP**.

---

