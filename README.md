# 📰 NewsCRED – AI-Powered News Verification

NewsCRED is a real-time AI fact-checking web app that detects fake, misleading, or unverifiable news claims.
It combines **Google News search (via SerpAPI)** with **Google Gemini reasoning**, and outputs:

✔ Final Verdict
✔ Explanation / Reasoning
✔ Confidence Score
✔ Article Source References

This project was built to combat digital misinformation and provide transparent, evidence-based news validation.

---

## 🚀 Features

* ✔ Enter a headline OR full news article paragraph
* ✔ Live news search using Google News (via SerpAPI)
* ✔ AI-based credibility analysis using Google Gemini
* ✔ Verdict labels:

  * 🟢 True / Verified
  * 🔴 False / Likely Fake
  * 🟡 Unverified
  * ⚪ Not a news
* ✔ Confidence bar (0–100%)
* ✔ Displays real clickable news sources
* ✔ Clean, minimal Streamlit-based UI

---

## 🧠 How It Works (Pipeline)

1. User enters a news claim
2. App sends query → Google News via SerpAPI
3. Fetches top real news articles
4. Claim + articles are sent to Gemini AI
5. Gemini outputs:

   * Verdict
   * Reasoning
   * Confidence score
6. UI displays:

   * verdict
   * reasoning
   * confidence bar
   * sources

---

## 🛠️ Tech Stack

| Component          | Technology              |
| ------------------ | ----------------------- |
| Frontend + Backend | Streamlit               |
| News Search        | SerpAPI (Google News)   |
| AI Reasoning       | Google Gemini 2.0 Flash |
| Language           | Python                  |
| Regex parsing      | Python `re` module      |

---

## 📦 Installation & Setup

### 1️⃣ Clone the repository

```bash
git clone https://github.com/yourusername/newscred.git
cd newscred
```

### 2️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

Required libraries include:

```
streamlit
serpapi
google-generativeai
```

---

## 🔑 API Keys Required

You need:

✔ SerpAPI Key
✔ Gemini API Key

Edit in the script:

```python
SERPAPI_KEY = "your-serpapi-key-here"
GEMINI_API_KEY = "your-gemini-key-here"
```

Get keys from:

* [https://serpapi.com](https://serpapi.com)
* [https://ai.google.dev](https://ai.google.dev)

---

## ▶️ Running the App

```bash
streamlit run app.py
```

---

## 📝 Example Inputs For Testing

```
India wins 2024 T20 World Cup  
Google is shutting down Gmail in 2025  
Reliance to acquire Disney Star India  
NASA confirms the sun will rise from the west  
Apple launches iPhone 16  
```

---

## 📄 Sample Output

```
🟢 True / Verified  
Reasoning: This news has been widely covered by multiple credible sources.
Confidence: 94%
```

---

## 📚 Project Motivation

With the rapid spread of misinformation on digital platforms, individuals often struggle to verify news credibility.
This project aims to:

✔ provide automated fact-checking
✔ show transparent reasoning
✔ reference real sources
✔ combine search + LLM inference

---

## 🧩 Future Improvements (100% Milestone)

* Web UI redesign with branding & styling
* PDF export of reports
* Browser extension for instant news verification
* Database logging for input history
* Multilingual news analysis
* API endpoints for external integration

---

## 🧑‍💻 Author

**Ishpreet Singh**
https://github.com/ishpreet7226

---

## ⭐ Contribute

Pull requests are welcome.

If using this for research or academic purpose, kindly reference the repository.

---

## 📣 Disclaimer

This tool assists in evaluating news credibility but does not guarantee absolute factual accuracy.
Users should cross-verify using official sources.

---
