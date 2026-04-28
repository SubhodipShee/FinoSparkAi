# 🚀 FinoSpark AI

[![Next.js](https://img.shields.io/badge/Next.js-15-black?logo=next.js)](https://nextjs.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.109-009688?logo=fastapi)](https://fastapi.tiangolo.com/)
[![Gemini](https://img.shields.io/badge/Google_Gemini-AI-blue?logo=google-gemini)](https://ai.google.dev/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-v4-38B2AC?logo=tailwind-css)](https://tailwindcss.com/)

**FinoSpark AI** is a cutting-edge personal finance cockpit that leverages Google Gemini to transform how you track, analyze, and optimize your financial life. Featuring a sleek neon-green aesthetic, it combines a powerful Next.js dashboard with a high-performance FastAPI backend for image-based receipt analysis.

🏆 **MumbaiHacks 2026:** Secured a spot in the **Top 10%** of teams.

🔗 **Live Demo:** [finospark-finance.onrender.com](https://finospark-finance.onrender.com/)

---

## ✨ Features

### 📊 Financial Dashboard
- **Live Insights:** Real-time visualizations of spending trends and categories using Recharts.
- **Smart Budgeting:** Track credits vs. debits with interactive bar charts.
- **Goal Planner:** Plan and monitor your investment goals.

### 🤖 AI Finance Advisor
- **Gemini Engine:** Powered by Google's generative AI for spending summaries, future predictions, and personalized advice.
- **AI Chat Panel:** Interact with a financial specialist bot for instant insights.

### 🧾 Receipt Analyzer
- **Vision AI:** Upload receipt images to extract structured data (vendor, total, items, date) via Gemini Vision.
- **OCR Fallback:** Robust Tesseract integration ensures data extraction even without high-end vision models.
- **Sample Picker:** Quickly test the analyzer with pre-generated receipt samples.

---

## 🏗️ Project Structure

```text
AiFino/
├── finospark-dashboard/   # Next.js Frontend & Core API
├── uploadimage/           # Python FastAPI Backend & Receipt UI
└── scripts/               # Automation & Sample Generation
```

---

## 🧰 Tech Stack

| Domain | Technologies |
| :--- | :--- |
| **Frontend** | Next.js 15, React, TypeScript, Tailwind CSS v4, Framer Motion |
| **UI Components** | shadcn/ui, Lucide Icons, Recharts |
| **Backend (Web)** | Next.js API Routes (Node.js) |
| **Backend (Vision)** | FastAPI, Python 3.13+ |
| **Database** | SQLite (Lightweight, file-based) |
| **AI / ML** | Google Gemini SDK, Tesseract OCR |

---

## 🚀 Getting Started

### 1. Prerequisites
- Node.js 18+ & npm
- Python 3.12+
- Google AI Studio API Key ([Get it here](https://aistudio.google.com/))

### 2. Setup the Dashboard (Web Application)
```bash
cd finospark-dashboard
npm install
```
Create a `.env.local` file:
```env
SQLITE_DB_PATH="app.db"
SESSION_SECRET="your-random-secret"
GEMINI_API_KEY="your_google_gemini_key"
```
Run the dev server:
```bash
npm run dev
```

### 3. Setup the Receipt Analyzer (Vision Backend)
```bash
cd uploadimage/server
pip install -r requirements.txt
```
Create a `server/.env` file:
```env
GEMINI_API_KEY="your_google_gemini_key"
```
Launch the API:
```bash
uvicorn app.main:app --reload
```

---



---

## 🛠️ Installation & Setup

### 1️⃣ Clone the repository
```bash
git clone https://github.com/SubhodipShee/FinoSparkAi.git
cd FinoSparkAi
cd finospark-dashboard
npm install
cd ../uploadimage
npm install
cd uploadimage
npm start
cd finospark-dashboard
npm start


