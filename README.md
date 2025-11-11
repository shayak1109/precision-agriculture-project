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
| **Hosting (optional)** | Gunicorn / Render / Heroku |

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

