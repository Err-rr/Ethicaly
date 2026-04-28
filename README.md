# Ethicly

**Ethicly – Detect, Explain, and Fix AI Bias**

Ethicly is a full-stack AI fairness audit platform that helps users identify, validate, and understand bias in datasets and model outcomes. It provides statistical fairness metrics, AI-driven explanations, comparison analysis, and professional report generation in a clean, intuitive interface.

---

## 🚀 Features

### 🔍 Bias Detection Engine
- Detects bias using fairness metrics:
  - Statistical Parity  
  - Approval Gap  
  - Fairness Score  
  - Disparate Impact Ratio  

### 📊 Statistical Validation
- Uses Chi-Square testing to verify if bias is statistically significant  
- Ensures reliable and data-backed fairness evaluation  

### 🤖 AI Explanation Layer
- Converts statistical outputs into human-readable insights  
- Provides actionable suggestions to improve fairness  

### 📈 Comparison Mode
- Compare two datasets (before vs after)  
- Track fairness improvements visually  

### 📄 Smart PDF Reports
- Generates branded reports with:
  - Metrics  
  - Graphs  
  - Verdict  
  - Fix recommendations  

---

## 🧠 Core Logic

Ethicly evaluates fairness using both mathematical metrics and statistical testing:

### Parity
Parity = min(P(Y=1|G)) / max(P(Y=1|G))

### Approval Gap
Approval Gap = max(P(Y=1|G)) - min(P(Y=1|G))

### Chi-Square Test
χ² = Σ((O - E)² / E)

### Disparate Impact Ratio
DIR = min(Group Rate) / max(Group Rate)

---

## 🛠 Tech Stack

### Frontend
- React (Vite)  
- Tailwind CSS  
- React Router  
- Recharts  
- react-dropzone  

### Backend
- Flask (Python)  
- REST APIs  

### Data & Analytics
- Pandas  
- NumPy  
- SciPy (Chi-Square testing)  

### AI Integration
- Google Gemini API  

### Reporting
- ReportLab (PDF generation)  

### Deployment
- Firebase Hosting (Frontend)  
- Render (Backend)  

---

## 📁 Project Structure

```bash
Ethicly/
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── assets/
│   │   └── App.jsx
│   └── package.json
│
├── backend/
│   ├── app.py
│   ├── requirements.txt
│   └── utils/
│
└── README.md

---

## ⚙️ Getting Started

### 1. Clone the Repository

git clone https://github.com/your-username/ethicly.git  
cd ethicly

---

### 2. Setup Frontend

npm install  
npm run dev  

App runs on:  
http://127.0.0.1:5173/

---

### 3. Setup Backend

cd backend  
pip install -r requirements.txt  
python app.py  

Backend runs on:  
http://127.0.0.1:5000/

---
```

## 📂 CSV Guidelines

Ethicly automatically detects:

### Group Columns
gender, race, age, group, segment  

### Outcome Columns
approved, label, target, prediction, outcome  

If not found:  
First column → group  
Last column → outcome  

---

## 🌐 Deployment

### Frontend (Firebase)

npm run build  
npx firebase deploy  

---

### Backend (Render)

- Push backend to GitHub  
- Connect repo to Render  
- Set start command:  

python app.py  

Ensure:

app.run(host="0.0.0.0", port=10000)

---

## 📊 API Endpoints

Upload CSV  
POST /upload  

Get AI Explanation  
POST /explain  

Download Report  
POST /download-report  

---

## 💡 Why Ethicly?

- End-to-end fairness pipeline  
- Combines statistics with AI  
- Easy to use for all users  
- Real-time insights  
- Production-ready architecture  

---

## 🔮 Future Scope

- Real-time model monitoring  
- Automated bias correction  
- Enterprise API integration  
- Fairness benchmarking  

---

## 👨‍💻 Author

Shivam Kumar  

---