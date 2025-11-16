# 📰 Fake News Detector 101 — Browser Extensions

**Fake News Detector 101** is an AI-powered tool designed to help users identify misleading, biased, or false online news.  
This repository contains the **Chrome** and **Firefox** browser extensions, along with supporting files.

The system connects to a **private backend API** to analyze article content using machine learning and explainable AI.

---

## Features

- **Scan any online article** instantly  
- **AI-powered classification** (Fake / Real / Uncertain)  
- **Confidence scoring**  
- **Explainability output** (keywords, tone, reasoning)  
- **English + Malay language support**  
- **Fast & lightweight browser extension**  
- **Secure API communication (HTTPS + JWT)**  
- **Chrome & Firefox versions included**

---

## How It Works

1. User opens any news article  
2. Clicks **Scan** in the extension  
3. Extension extracts readable text  
4. Sends it to the backend endpoint:  
   `POST /analyze`  
5. Backend returns:  
   - Classification  
   - Confidence  
   - Explanation  
   - Model used  
6. Result is displayed in the UI

---

## Backend API (Required)

The browser extensions require the Fake News Detector backend:

**Backend API:**  
`https://fakenewsdetector-zjzs.onrender.com`



---

## Official Links

| Resource | URL |
|---------|-----|
| Website | https://www.fakenewsdetector101.com |
| Backend API | https://fakenewsdetector-zjzs.onrender.com |
| Frontend Source | *(to be added)* |
| Privacy Policy | https://www.fakenewsdetector101.com/privacy-policy |
| Terms of Service | https://www.fakenewsdetector101.com/terms-of-service |
| Contact | **jazlizharfan@outlook.com** |

---

## Technical Stack

| Component | Technology |
|----------|------------|
| **Backend** | Python (Flask), SQLite |
| **Models** | Logistic Regression + TF-IDF |
| **Frontend** | Chrome & Firefox Extensions |
| **Explainability** | Keyword heuristics, confidence scoring |
| **Deployment** | Render.com |
| **Security** | HTTPS, JWT, Environment Protection |

---

## Dataset Usage & Credits

This project uses publicly available datasets for research and evaluation purposes.  
Please credit the original dataset creators:

1. **Zolkepli, Husein — Malay Dataset**  
   https://github.com/huseinzol05/Malay-Dataset

2. **Zolkepli, Husein — Malaya NLP Toolkit**  
   https://github.com/huseinzol05/Malaya

3. **Gor Abaghyan — Fake News Dataset (Kaggle)**  
   https://www.kaggle.com/datasets/abaghyangor/fake-news-dataset

---

## Publication & Academic Reference

This project is connected to the following research publication:

**"A Benchmark Evaluation Study for Malay Fake News Classification Using Neural Network Architectures"**  
Kazan Digital Week 2020 — Methodical and Informational Science Journal,  
Vestnik NTsBZhD (4), pp. 5–13, 2020.

**Links:**

- PDF: https://ncbgd.tatarstan.ru/rus/file/pub/pub_2610566.pdf  
- Journal Site: http://www.vestnikncbgd.ru/index.php?id=1&lang=en  
- Event: https://kazandigitalweek.com/  
- Related GitHub Work: https://github.com/AsyrafAzlan/malay-fake-news-classification.git

---

## Developer Installation (Local Testing)

```bash
# Clone the repository (replace if your URL differs)
git clone https://github.com/JazLOT/FakeNewsDetector101_Extensions.git
cd FakeNewsDetector101_Extensions

# Chrome installation
# Open chrome://extensions → Enable Developer Mode → Load unpacked
# Select: /FakeNewsDetector101_Chrome/

# Firefox installation
# Open about:debugging#/runtime/this-firefox → Load Temporary Add-On
# Select the manifest.json inside: /FakeNewsDetector101_Firefox/
