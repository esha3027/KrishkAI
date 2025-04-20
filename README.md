# 🌾 KrishkAI – AI-Powered Farming Assistant

KrishkAI is a technology platform powered by AI, designed to empower farmers by providing smart crop suggestions, disease analysis, financial services, and an interactive multilingual knowledge base.

---

## 🚀 Features

### 🧠 Knowledge Hub
- Pose agriculture-related questions in natural language
- Open-source LLMs (LLaMA 3 / DeepSeek) powered
- Multilingual support for local users

### 🌱 Crop Recommendation
- Recommends the best crops based on:
- Soil fertility
- Climate data
- Market demand
- ML-based classification from environmental inputs

### 🐛 Crop Disease Detection
- Handles both **image** and **video** inputs
- Identifies disease type through CNN model trained on the **PlantDoc dataset**
- Real-time analysis of video frames (max. 10 frames)

### 👤 User Management
- Registration and login mechanism for farmers
- Safely stores user data in MySQL

---

## 📁 Tech Stack

| Layer | Technology |
|---------------|---------------------------------|
| Frontend | React.js |
| Backend | FastAPI (Python) |
| ML Models | TensorFlow, PyTorch, Scikit-learn |
| Database | MySQL |
| Cloud/Infra | Docker-ready, API-first design |
| Integration | RESTful APIs + CORS |

---

## 📁 Project Structure

project-root/ │ ├── frontend/ # React App (UI) ├── backend/ # FastAPI App (APIs) │ ├── main.py # API entry point │ ├── Registration.py │ ├── Login_page.py │ ├── CropRecommendation.py │ ├── Knowledge_Hub.py │ ├── Disease_Detection.py │ └── DD_from_pic.py └── README.md

yaml
Copy
Edit

---

## ⚙️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/krishkai.git
cd krishkai
2. Run the Backend (FastAPI)
bash
Copy
Edit
cd backend
pip install -r requirements.txt
uvicorn main:app --reload
Verify that MySQL is running and properly configured

3. Run the Frontend (React)
bash
Copy
Edit
cd ./frontend
npm install
npm start

### 🌐 API Endpoints (Backend)

Endpoint Method Description
/login POST User login
/register POST User registration
/recommend-crop POST Crop recommendation engine
/detect-disease/image POST Disease detection from image
/knowledge-hub POST LLM-based query interface

### 🧪 Dataset Used
PlantDoc Dataset – for training the disease detection model

###📌 Acknowledgements
FastAPI & TensorFlow Teams
Hugging Face Community Models
