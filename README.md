# 📄 ATS Resume Expert — AI-Powered Applicant Tracking System

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge&logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-Web%20App-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![Gemini](https://img.shields.io/badge/Google%20Gemini-1.5%20Flash-4285F4?style=for-the-badge&logo=google&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-Agent%20Workflow-purple?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

---

## 📌 Project Overview

**ATS Resume Expert** is an AI-powered Applicant Tracking System that uses **Google Gemini 1.5 Flash** to analyse resumes against job descriptions. It evaluates how well a candidate's resume matches a given role — mimicking the behaviour of real ATS systems used by HR departments.

The project also includes a **LangGraph** agentic workflow experiment (`LangraphExm.ipynb`) demonstrating multi-step AI agent orchestration.

---

## 🎯 Features

- 📤 **Upload PDF Resume** — Converts the first page to an image for Gemini to analyse
- 📝 **Paste Job Description** — Enter any job description for comparison
- 🤖 **AI-Powered Analysis** — Uses Gemini 1.5 Flash multimodal to evaluate the resume
- 📊 **ATS Match Score** — Returns percentage match, missing keywords, and improvement suggestions
- 🔑 **Google Makersuite API** — Simple API key setup via Google AI Studio

---

## 🏗️ How It Works

```
User uploads PDF Resume + Paste Job Description
            ↓
PDF → First Page → JPEG Image (via pdf2image)
            ↓
Image + Job Description → Gemini 1.5 Flash (multimodal)
            ↓
AI Response: Match %, Missing Keywords, Profile Summary
```

---

## 🖥️ Application Interface

The Streamlit app provides:
1. A **Job Description** text area
2. A **PDF file uploader** for the resume
3. Two action buttons:
   - **Tell Me About the Resume** — General profile evaluation
   - **Percentage Match** — ATS-style scoring against the job description

---

## 📁 Project Structure

```
Applicatin-tracking-system/
│
├── app.py                 # Streamlit application (main entry point)
├── LangraphExm.ipynb      # LangGraph agentic workflow experiment
├── requirements.txt       # Python dependencies
├── README.md
└── LICENSE
```

---

## 🚀 How to Run

### 1. Clone the repository
```bash
git clone https://github.com/homeshwarnelakurthi/Applicatin-tracking-system.git
cd Applicatin-tracking-system
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Get your Google API Key
- Visit [Google AI Studio](https://makersuite.google.com/app/apikey)
- Generate a free Gemini API key

### 4. Set environment variable
```bash
# Create a .env file
echo "GOOGLE_API_KEY=your_api_key_here" > .env
```

### 5. Run the app
```bash
streamlit run app.py
```

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python 3.10+ | Core language |
| Streamlit | Web application UI |
| Google Gemini 1.5 Flash | Multimodal AI analysis |
| pdf2image | PDF → image conversion |
| Pillow (PIL) | Image processing |
| python-dotenv | Environment variable management |
| LangGraph | Agentic AI workflow (experimental) |

---

## 👨‍💻 Author

**Homeswar Rao Nelakurthi**
[![GitHub](https://img.shields.io/badge/GitHub-homeshwarnelakurthi-181717?style=flat&logo=github)](https://github.com/homeshwarnelakurthi)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
