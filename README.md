# 🎵 Music Mood Prediction (Sentiment Analysis)

This project is a **machine learning-based web application** that predicts the **mood of a song (Happy or Sad)** based on its lyrics.

It leverages **Natural Language Processing (NLP)** and **classification models** to analyze text input and determine sentiment, with support for **Hindi (Devanagari) lyrics via translation**.

---

## 🚀 Live Demo

🌐 **App Hosted on Heroku**  
https://mood-prediction.herokuapp.com/

---

## 📘 Documentation

📖 https://codelabs-preview.appspot.com/?file_id=1guBB6MdRZQEfGpmeTlHPv2Z4a1uChJaGpvSrs7uUKU4#6

---

## 🎥 Demo Video

▶️ https://youtu.be/jPBI4o8b-Gc

---

## 🎯 Features

- 🎤 Predict song mood: **Happy / Sad**
- 🌐 Supports **Hindi lyrics** (auto-translated to English)
- ⚡ Real-time prediction via web interface
- 🧠 Multiple ML models experimented
- 📊 NLP preprocessing pipeline

---

## 🛠️ Tech Stack

- **Language:** Python  
- **ML Models:** MLP, SVM, Random Forest, Bagging, Boosting  
- **NLP:** Text preprocessing, stopword removal  
- **Web Framework:** Flask  
- **Frontend:** HTML, AJAX  
- **Deployment:** Heroku  

---

## 🧠 Model Development

The model development phase includes two main notebooks:

### 📓 1. Main Notebook
- `MusicMood_SongClassification`
- Implements the **MLP (Multi-Layer Perceptron)** model used in production

### 📓 2. Experimental Notebook
- `Implementing Multiple Classifiers`
- Includes:
  - Support Vector Machine (SVM)
  - Random Forest (RF)
  - Bagging
  - Boosting

---

## 📂 Project Structure
├── Code/
│ ├── MusicMood_SongClassification.ipynb
│ └── Implementing Multiple Classifiers.ipynb
│
├── Data/
│ ├── train_lyrics_1000
│ ├── valid_lyrics_200
│ └── stopwords_eng
│
├── Model/
│ └── (Pickled model + preprocessing components)
│
├── app.py
├── templates/
│ └── index.html
└── README.md



---

## 📊 Dataset

- **Training Data:** `train_lyrics_1000`  
- **Validation Data:** `valid_lyrics_200`  
- **Stopwords Corpus:** `stopwords_eng`  

---

## ⚙️ Model Deployment Flow

1. User inputs lyrics (Hindi or English)
2. If Hindi → translated to English using Google Translator
3. Processed text passed to trained ML model
4. Model predicts sentiment (**Happy / Sad**)
5. Response returned as JSON
6. Frontend updates UI dynamically using AJAX

---

## 🔄 Application Workflow

### Backend (Flask API)
- Loads pickled model and preprocessing pipeline
- Accepts input lyrics
- Translates (if required)
- Predicts mood
- Returns JSON response

### Frontend
- User enters lyrics in text area
- AJAX request sent to backend API
- Receives prediction result
- Displays corresponding image/output

---

## ▶️ How to Run Locally

### 1. Clone Repository
```bash
git clone <your-repo-url>
cd Music-Mood-Prediction-Sentiment-Analysis
