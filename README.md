# 🧠 MindPulse AI — Student Mental Health Prediction Web App

[![Live App](https://img.shields.io/badge/Render-Live%20Demo-brightgreen?style=for-the-badge&logo=render)](YOUR_RENDER_LIVE_LINK_HERE)

**MindPulse AI** ek Machine Learning-powered full-stack web application hai jo students ke daily habits (sleep, study hours, social media usage, physical activity) ke aadhar par unke Mental Health Score ko predict karta hai.

---

## 🌐 Live Demo & UI Preview

- **Live Application:** [Click Here to Access MindPulse AI](YOUR_RENDER_LIVE_LINK_HERE)

### 📸 Application Interface

![MindPulse AI UI Preview](YOUR_IMAGE_LINK_OR_PATH_HERE)
_(Apni screenshots/UI ki image ka link ya path upar paste karein)_

---

## 🚀 Old Flow vs. New Flow (My Progress)

Is project me maine apne ML workflow ko ek naye production-ready level par upgrade kiya hai:

| Feature / Step       | 🔴 Old Flow                   | 🟢 New Flow (Upgraded)                                                    |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------ |
| **Deployment**       | Streamlit UI                  | **Render Web Service** (FastAPI Backend + HTML/JS Frontend)               |
| **Preprocessing**    | Manual Ad-hoc Transformations | **Scikit-learn `ColumnTransformer`** (Automated & Leak-free)              |
| **Model Training**   | Manual Loops & Loose Scripts  | **Integrated ML Pipelines** (`Pipeline([('prep', ...), ('model', ...)])`) |
| **API & Validation** | Raw JSON / Basic Flask        | **FastAPI + Pydantic Schema Validation**                                  |
| **Frontend**         | Streamlit Default UI          | **Custom UI** (Vanilla HTML5, Modern CSS, JavaScript Fetch API)           |

---

## 🔮 Future Integration Plan (Upgrading Legacy Projects)

Maine is project ke zariye production-grade Machine Learning pipeline aur deployment seekha hai. **Aage chal kar main apne jitne bhi puraane ML aur Deep Learning (DL) projects hain, un sabhi me in same features ko integrate/upgrade karunga:**

- ⚙️ **End-to-End Pipeline & Column Transformers:** Preprocessing aur model fitting ko single Sklearn pipeline me migrate karna.
- ⚡ **FastAPI Migration:** Puraane Streamlit / Flask endpoints ko fast, async, aur modular FastAPI backend se replace karna.
- 🛡️ **Pydantic Validation & Security:** Strict schema checks, error handling, aur environment variables (`.env` / config) se API keys aur URLs ko secure & hide karna.

---

## 🛠️ Project Architecture & Tech Stack

1. **Machine Learning Pipeline (`notebook.ipynb`)**:
   - Data cleaning, log transformations, outlier removal.
   - Categorical feature encoding & scaling using `ColumnTransformer`.
   - Model comparison: Linear Regression vs. Random Forest (Default & Tuned).
   - Pipeline serialization via `joblib`.

2. **Backend API (`main.py`)**:
   - **FastAPI**: Asynchronous & high-performance Web API framework.
   - **Pydantic**: Input schema validation and field-level constraint enforcement (`age`, `study_hours`, `stress_level`, etc.).
   - **CORS Middleware**: Secure cross-origin requests.

3. **Frontend (`index.html`, `script.js`, `style.css`)**:
   - Interactive gauge dashboard for visual score representation.
   - Dynamic error messaging & client/server validation handling.

---

## 📊 Model Performance Metrics

| Model                       | Test $R^2$ | Training $R^2$ | MAE        | RMSE       |
| :-------------------------- | :--------- | :------------- | :--------- | :--------- |
| **Linear Regression**       | 0.7397     | 0.7236         | 0.5361     | 0.6760     |
| **Random Forest (Default)** | 0.8775     | 0.9808         | 0.3472     | 0.4636     |
| **Random Forest (Tuned)**   | **0.8650** | **0.9547**     | **0.3689** | **0.4869** |

---

## ⚡ Local Setup Instructions

1. **Clone the repository**:
   ```bash
   git clone [https://github.com/your-username/mindpulse-ai.git](https://github.com/your-username/mindpulse-ai.git)
   cd mindpulse-ai
   ```

MindPulse AI: A production-grade ML web app predicting student mental health scores based on daily lifestyle habits. Features an upgraded workflow: Scikit-learn Pipeline &amp; ColumnTransformer for leak-free training, FastAPI + Pydantic for schema validation, and an interactive HTML/JS frontend live deployed on Render.
