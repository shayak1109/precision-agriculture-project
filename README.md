# 🌾 Web-Based Precision Agriculture using Machine Learning and Deep Learning

### An Integrated Platform for Crop Recommendation, Fertilizer Suggestion, and Disease Detection

---

## 🧭 Overview

Agriculture in India faces challenges like **poor crop selection**, **inefficient fertilizer use**, and **late disease detection**, leading to lower productivity and financial losses.  
This project introduces an **AI-driven web platform** that integrates **Machine Learning (ML)** and **Deep Learning (DL)** to assist farmers through three major modules:

1. 🌱 **Crop Recommendation System** – Suggests the most suitable crop based on soil nutrients (NPK), pH, temperature, humidity, and rainfall.  
2. 🌾 **Fertilizer Recommendation System** – Provides fertilizer suggestions by comparing soil nutrient levels with ideal crop requirements.  
3. 🍃 **Disease Detection System** – Identifies plant leaf diseases using a **ResNet-9 CNN** trained on thousands of leaf images.

Developed as part of the **B.E. Minor Project** at **RV College of Engineering (ECE Dept)** under the guidance of **Dr. Veena Devi S.V.**

---

## 🧠 Tech Stack

| Category | Tools & Frameworks |
|-----------|--------------------|
| **Frontend** | HTML5, CSS3, JavaScript, Bootstrap |
| **Backend** | Python (Flask) |
| **Database** | SQLite / SQLAlchemy ORM |
| **Machine Learning** | scikit-learn, NumPy, Pandas |
| **Deep Learning** | PyTorch, TorchVision |
| **APIs** | OpenWeatherMap API (for real-time weather) |

---

## 📊 Model Details

| Module | Algorithm / Model | Accuracy |
|--------|--------------------|-----------|
| **Crop Recommendation** | Random Forest | 97% |
| **Fertilizer Suggestion** | Rule-based (NPK comparison) | – |
| **Disease Detection** | ResNet-9 CNN | 89% |

The Random Forest model outperformed Decision Tree, SVM, and Logistic Regression models in terms of accuracy and stability.

---

## ⚙️ Installation & Setup

### 1️⃣ Clone this repository
```bash
git clone https://github.com/shayak1109/precision-agriculture-project.git
cd precision-agriculture-project
```

### 2️⃣ Create and activate a virtual environment
```bash
python -m venv myenv
myenv\Scripts\activate        # (Windows)
# or
source myenv/bin/activate     # (Linux/Mac)
```
### 3️⃣ Install dependencies
```bash
pip install -r requirements.txt

```
### 4️⃣ Add your OpenWeatherMap API key
Create a *config.py* file in the root directory and add:
```bash
weather_api_key = "API_KEY"
```
### 5️⃣ Run the Flask app
```bash
python app.py
```

## 🧩 Folder Structure
```bash
precision-agriculture-using-machine-learning/
│
├── README.md
├── app.py                    # Main Flask app
├── requirements.txt          # Dependencies
├── .gitignore
├── config.py                 # Contains your API key
├── crop_rec.zip              # crop recommendation dataset
├── models.zip
├── Data/                     # Fertilizer data (CSV)
├── models/                   # ML & DL model files (.pkl, .pth)
├── static/                   # CSS, JS, and images
├── templates/                # HTML files
├── utils/                    # Helper Python modules
└── database.db               # Auto-created SQLite DB
```

## 🧪 Features Demonstration

🌱 Crop Recommendation

- Inputs: N, P, K, pH, temperature, humidity, rainfall, and location.

- Output: Recommended crop suitable for the conditions.

🌾 Fertilizer Recommendation

- Inputs: Crop name, N, P, K values.

- Output: Suggests fertilizer corrections and organic alternatives.

🍃 Disease Detection

- Inputs: Image of a crop leaf (JPG/PNG).

- Output: Detects disease and suggests treatment measures.

## 📈 Results Summary

| Algorithm           | Accuracy |
| ------------------- | -------- |
| Decision Tree       | 90%      |
| Logistic Regression | 94.3%    |
| SVM                 | 97%      |
| Random Forest       | ~97-99%  |
| ResNet-9 (DL model) | 89%      |

## 👨‍💻 Contributors

**Guide:** Dr. Veena Devi S.V., Associate Professor, Dept. of ECE, RVCE

| Name               | Role                                        |
| ------------------ | ------------------------------------------- |
| **Shayak Bose**    | Frontend, Flask Integration, Documentation  |
| **Shubh Bafna**    | Backend, ML Integration                     |
| **Siddhant Sinha** | Database, Flask Authentication              |
| **Yash Naik**      | DL Model Training & Documentation           |
