## 🧠 AI Fact-Check & Multimedia Generator

An AI-powered web platform that allows users to verify trending news or social media content. It extracts factual claims, runs NLP analysis, and generates visual content like infographics and optional videos to present credibility.

---

### 🔧 Architecture Overview

| Layer                 | Tech Stack                               |
| --------------------- | ---------------------------------------- |
| **Frontend**          | React (Vite) for fast, interactive UI    |
| **Backend**           | FastAPI to serve NLP and generation APIs |
| **NLP**               | Hugging Face Transformers, spaCy         |
| **Fact-Checking**     | Bing Search API                          |
| **Visual Generation** | Stable Diffusion (via Diffusers)         |
| **Optional Video**    | Coqui TTS + Text2Video (bonus)           |
| **Deployment**        | Vercel (frontend), Render (backend)      |

---

### 🚀 Features

* 🧾 **Claim Extraction & Verification**
  Automatically detects and verifies claims in posts or URLs.

* 🔍 **NLP Analysis**
  Includes topic classification, sentiment analysis, and named entity recognition.

* 🖼️ **AI Visual Generation**
  Generates infographics or illustrative images based on the content.

* 🎙️ **(Optional)** Narrated video summaries with lip-syncing.

* 📊 **Dashboard View**
  Results shown with evidence, visuals, and credibility mapping.

---

### ⚙️ Setup Instructions

#### 1. Clone the Repository

```bash
git clone https://github.com/your-username/ai-fact-checker.git
cd ai-fact-checker
```

---

#### 2. Backend Setup (FastAPI)

```bash
cd backend/
pip install -r requirements.txt
uvicorn main:app --host 0.0.0.0 --port 8000
```

> ✅ Replace API keys in `fact_check.py` and `image_generation.py`

---

#### 3. Frontend Setup (React)

```bash
cd frontend/
npm install
npm start
```

Then open `http://localhost:3000` in your browser.

---

### 🧪 Usage Guide

1. Input a **URL or custom text** into the homepage form.
2. The system:

   * Extracts key claims
   * Runs fact-checking logic
   * Applies NLP processing (sentiment, NER, topics)
   * Generates an AI image/infographic
   * (Optional) Produces a narrated video
3. Results are shown in an interactive dashboard, including:

   * Verdict (True/False/Unverified)
   * Extracted evidence + sources
   * Generated visuals
   * Timeline or source map

---

### 👨‍💻 For Development

* **Frontend Styles**: Customize `frontend/src/styles.css`
* **CORS Config**: Ensure backend allows your frontend domain
* **Infographic Prompt Logic**: Tweak prompts in `image_generation.py`
* **Claim Logic**: Modify `fact_check.py` for custom verification behavior

> Optional: Integrate TTS/video generation in `video/` directory

---

### 📦 Deployment

* **Frontend**:
  Push to GitHub and link to [Vercel](https://vercel.com/)

* **Backend**:
  Deploy `backend/` to [Render](https://render.com/) or use Hugging Face Spaces

---

### ✅ Rubric Mapping

| Requirement               | Covered               |
| ------------------------- | --------------------- |
| ✅ Claim Verification      | Bing Search           |
| ✅ NLP Analysis            | Transformers + spaCy  |
| ✅ AI Visuals              | Stable Diffusion      |
| ✅ UI/UX                   | React dashboard       |
| ✅ Deployment              | Vercel + Render ready |
| ✅ Documentation           | Full README + PDF     |
| 🔁 Bonus Video (Optional) | Wav2Lip + TTS         |

---

### 📄 License

This project is open-sourced under the MIT License.

---
[AI_FactCheck_Project_Report (1).pdf](https://github.com/user-attachments/files/20635206/AI_FactCheck_Project_Report.1.pdf)


