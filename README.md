# 🚀 MLOps Final Assignment Repository


## 📁 Folder Structure

| Folder        | Description                                                                                   |
|---------------|-----------------------------------------------------------------------------------------------|
| `devops`      | AWS EC2 (public/private), Dockerized Flask app, Kubernetes deployment (Kind & EKS)            |
| `kserve`      | ML model for crop disease risk prediction (RandomForest + joblib)                             |
| `kubeflow`    | Kubeflow Pipelines (KFP) with MinIO and custom YAML pipeline for model training and prediction |
| `observability` | Flask app with real-time Elasticsearch logging using Bonsai cloud                           |
| `python`      | Data science projects (Titanic, House Prices, Wine, etc.) with FastAPI & object-oriented design |
| `streamlit`   | Interactive dashboards: CSV Visualizer, Weather App, Sentiment Analysis                       |

---

## 🔧 Tools & Technologies

- **Python**, **Pandas**, **Scikit-learn**, **Matplotlib**, **Seaborn**
- **FastAPI**, **Streamlit**, **TextBlob**, **joblib**
- **Docker**, **Kubernetes (Kind & EKS)**, **KServe**
- **Elasticsearch**, **MinIO**
- **AWS EC2**, **Custom VPC**

---

## 🌐 Project Highlights

### ✅ DevOps (EC2 + Docker + K8s)
- Launched EC2 instances inside a custom VPC (no default VPC/NAT Gateway).
- Deployed Flask apps inside Docker containers.
- Built Kubernetes manifests and deployed Flask app using `kind`.

### ✅ KServe Model
- Random Forest model for disease risk prediction.
- Saved and exported `model.joblib`, encoders, and scaler.
- Output: model accuracy and classification report.

### ✅ Kubeflow Pipelines
- Pipeline with:
  - Data preparation
  - Model training
  - Prediction
- Integrated with MinIO to store pipeline artifacts.

### ✅ Observability
- Flask app with `LogisticRegression` model.
- Logs predictions to **Elasticsearch** in real time.
- Integrated with Bonsai for hosted Elasticsearch.

### ✅ Python Mini Projects
- Titanic EDA visualizations
- House Price Prediction with FastAPI
- Wine filter and visualizations
- Custom iterator for Mall customers
- Decorator for sales analysis
- Iris filtering with FastAPI & plots

### ✅ Streamlit Dashboards
- Upload CSV and visualize charts.
- Live weather data fetch via API.
- Text-based sentiment analysis with emoji feedback.

---

## 🧠 Skills Demonstrated

| Area            | Skills & Concepts                       |
|------------------|-----------------------------------------|
| MLOps Pipeline   | Model Dev ➝ Docker ➝ K8s ➝ Kubeflow     |
| Monitoring       | Real-time Logs ➝ Elasticsearch          |
| API Design       | FastAPI, Flask                          |
| Visualization    | Streamlit, Matplotlib, Seaborn          |
| Automation       | OOP, Decorators, Iterators              |

---

## 📌 How to Run (Example for Docker)

```bash
# Flask App
docker build -t flask-app .
docker run -d -p 5000:5000 flask-app

# Streamlit App
streamlit run app.py

# FastAPI App
uvicorn main:app --reload
