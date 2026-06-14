# 🎓 EduMind — AI-Powered Academic Tutor

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Streamlit-1.30+-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white"/>
  <img src="https://img.shields.io/badge/Ollama-Mistral-0A0A0A?style=for-the-badge&logo=ollama&logoColor=white"/>
  <img src="https://img.shields.io/badge/License-MIT-22C55E?style=for-the-badge"/>
</p>

<p align="center">
  A sleek, local AI tutor web app that delivers structured, step-by-step academic answers — with a system prompt engineered to minimize hallucinations.
</p>

---

## ✨ Features

- 🧠 **Multi-turn conversation** — remembers context across the full chat session
- 📚 **Subject-aware responses** — choose from Math, Physics, Chemistry, Biology, CS, History, English, and more
- 🎯 **Difficulty levels** — Beginner, Intermediate, or Advanced explanations on demand
- 🛡️ **Anti-hallucination system prompt** — instructs the model to say "I don't know" rather than guess
- 💬 **Step-by-step reasoning** — forces the model to show its work for every problem
- 📊 **Session stats** — tracks questions asked and exchanges in the sidebar
- 🗑️ **Clear chat** — reset the session with one click
- 🌑 **Dark professional UI** — custom-styled with CSS, Google Fonts, and gradient accents

---

## 🖥️ Demo

> _App running locally via Streamlit_

```
Ask: "Explain Newton's Second Law with a real-world example"

EduMind: Newton's Second Law states that F = ma — the net force on an object
equals its mass times its acceleration. Here's a step-by-step breakdown...
```

---

## 🏗️ Tech Stack

| Layer       | Technology                        |
|-------------|-----------------------------------|
| **Frontend**| Streamlit + Custom CSS            |
| **LLM**     | Mistral 7B (via Ollama, local)    |
| **Language**| Python 3.10+                      |
| **Fonts**   | Inter + Poppins (Google Fonts)    |

---

## ⚙️ Installation

### Prerequisites

Make sure you have the following installed:

- [Python 3.10+](https://www.python.org/downloads/)
- [Ollama](https://ollama.com/) — to run the Mistral model locally

### 1. Clone the repository

```bash
git clone https://github.com/your-username/edumind-ai-tutor.git
cd edumind-ai-tutor
```

### 2. Install Python dependencies

```bash
pip install streamlit ollama
```

### 3. Pull the Mistral model via Ollama

```bash
ollama pull mistral
```

### 4. Run the app

```bash
streamlit run ai_assistant.py
```

The app will open in your browser at `http://localhost:8501`

---

## 📁 Project Structure

```
edumind-ai-tutor/
│
├── ai_assistant.py      # Main Streamlit app
└── README.md            # Project documentation
```

---

## 🛡️ Anti-Hallucination Design

The system prompt follows 10 strict rules to improve factual accuracy:

| Rule | Purpose |
|------|---------|
| Confidence gating | Only states facts the model is certain about |
| "I don't know" fallback | Explicit permission to admit uncertainty |
| No invented data | Blocks fabrication of names, dates, formulas |
| Step-by-step enforcement | Makes reasoning transparent and verifiable |
| False-assumption correction | Detects and fixes errors in the user's question |
| Level-matched output | Tailors depth to Beginner / Intermediate / Advanced |
| Topic scoping | Keeps the model focused on academic subjects |

---

## 🚀 Future Improvements

- [ ] Add PDF/image upload for document-based Q&A
- [ ] Export chat history as PDF
- [ ] Support more models (LLaMA 3, Gemma, etc.)
- [ ] Voice input support
- [ ] Dark/Light theme toggle

---

## 🙋 Author

**Ibrahim** — Data Analyst & AI Developer  
[LinkedIn](https://linkedin.com/in/mohammad-ibrahim-sofi) · [GitHub](https://github.com/Mohammad-Ibrahim-Sofi)

---

## 📄 License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
