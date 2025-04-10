# 🤖 🧠 AI-Powered Job Portal (MERN Stack + Cloudinary + ML Job Prediction)
Authors and their Github Links: Suma Sanjana-https://github.com/SumaSanjana, Mekala Varun: https://github.com/ShadowwPhoenix

This project introduces an end-to-end **AI-Powered Job Portal**, developed using the **MERN stack** (MongoDB, Express.js, React.js, Node.js) to offer a responsive and full-featured web application for seamless **job posting, user authentication, company management**, and **resume uploads via Cloudinary**. Enhancing traditional job portals, it integrates a **Flask-based Machine Learning microservice** powered by the **XGBoost algorithm**, which predicts job placement outcomes based on inputs like **CGPA, internship experience, communication skill**, and **technical skill rating**, providing real-time insights to users and enabling smarter hiring decisions.
.


## Project Overview

This project leverages the LLaMA 3 model for generating conversational responses. The application provides a user-friendly interface where users can input messages, and the chatbot responds in real-time. The conversation history is stored and displayed, and all interactions are logged for future reference.

## 🚀 Features

- 👤 User & Company Authentication (JWT)
- 📝 Job Posting & Application System
- 🏢 Company Profile Management
- 📦 Resume Upload via Cloudinary
- 🔍 Smart Job Recommendations
- 🤖 ML-based Job Prediction using academic & skill inputs
- 🎯 Role-based Dashboards (User / Recruiter)
- 🧠 Integrated Flask ML model (CGPA, skills → predicted placement)
---
## 📷 Screenshots

### 🏠 Dashboard View

![Dashboard View](Screenshots/Screenshot%202025-02-27%20141114.png)
### 📤 Job Posting Page

![Job listing](Screenshots/Screenshot%202025-02-27%20141300.png)

---

## 🧱 Tech Stack

### 🔧 Backend
- Node.js
- Express.js
- MongoDB (Mongoose)
- JWT for Auth
- Multer for file handling
- Cloudinary API for image/resume storage

### 🎨 Frontend
- React.js
- Vite
- Tailwind CSS
- Redux Toolkit

### 🤖 Machine Learning
- Python (Flask)
- Scikit-learn
- Pandas, NumPy
- Trained ML model: `job_placement_model.pkl`

---

## 🗂️ Project Structure

```bash
AI-Powered-Job-Portal/
│
├── backend/
│   ├── controllers/
│   ├── middlewares/
│   ├── models/
│   ├── routes/
│   ├── utils/
│   ├── index.js
│   └── .env
│
├── frontend/
│   ├── public/
│   └── src/
│       ├── assets/
│       ├── components/
│       ├── hooks/
│       ├── lib/
│       ├── redux/
│       └── utils/
│
├── prediction/
│   ├── app.py
│   ├── job_placement_model.pkl
│   ├── job_placement.ipynb
│   └── collegePlace.csv
│
└── README.md
```

---



## **⚙️ Setup Instructions**

### 📦 Backend Setup
```bash
cd backend
npm install
npm run dev

```
Create a .env file and add

```env
PORT=5000
MONGO_URI=your_mongo_uri
JWT_SECRET=your_secret
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret

```
### 💻 Frontend Setup


```bash
cd frontend
npm install
npm run dev
```


### 🧠 ML Prediction Server

```bash
cd prediction
pip install -r requirements.txt
python app.py

```
---
## 📡 API Endpoints

| Method | Endpoint             | Description                    |
|--------|----------------------|--------------------------------|
| GET    | `/api/jobs`          | Get all job listings           |
| POST   | `/api/job`           | Create a job (company only)    |
| POST   | `/api/apply/:jobId`  | Apply to a job                 |
| POST   | `/api/register`      | Register user or company       |
| POST   | `/predict` (Flask)   | Predict job placement using ML |


---



Feel free to reach out with questions or suggestions.  
G-Mail- varunyadav4868@gmail.com, sanjananvs812@gmail.com
*by Shadow Phoenix*
