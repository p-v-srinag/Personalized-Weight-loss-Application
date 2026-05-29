# Personalized Health & Weight Loss App (Hybrid ML Framework)

[![IEEE Publication](https://img.shields.io/badge/IEEE-Published_Paper-blue.svg)](https://ieeexplore.ieee.org/document/11497296)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![React](https://img.shields.io/badge/React-Vite-blue.svg)](https://vitejs.dev/)

## 📌 Overview
This repository contains the full-stack application code for the research paper: **"A Hybrid Machine Learning Framework for Personalized Weight Loss through Protein Intake Pattern Analysis"** (Published in IEEE).

The application leverages a hybrid machine learning pipeline—combining Hierarchical Clustering and Multilayer Perceptrons (MLP)—to analyze user dietary habits and protein intake. It generates highly personalized, data-driven weight loss and health recommendations through a modern, responsive web interface.

## ✨ Key Features
* **Hybrid ML Pipeline:** Utilizes a custom `hcmlp_model.keras` and hierarchical clustering (`hc_cluster_model.pkl`) to analyze complex dietary data.
* **Proxy Discriminator:** Implements an advanced discriminator network (`proxy_discriminator.keras`) to refine intake pattern analysis.
* **Food Logging & Dashboard:** A React-based interface allowing users to log daily food intake, visualize metrics on a dashboard, and receive personalized feedback.
* **Secure Backend API:** Robust Python backend handling authentication, database queries, and seamless ML model integration.

## 🛠️ Tech Stack
* **Machine Learning:** Python, Keras/TensorFlow, Scikit-Learn, Pandas
* **Backend:** Python, SQLAlchemy
* **Frontend:** React.js, Vite, Tailwind CSS, PostCSS
* **Authentication:** JWT / Secure Session Handling

## 📂 Project Structure
```text
WEIGHTLOSS_APP/
│
├── backend/
│   ├── deployment_artifacts/
│   │   ├── cluster_encoder.pkl
│   │   ├── food_database.csv
│   │   ├── hc_cluster_model.pkl
│   │   ├── hcmlp_model.keras
│   │   ├── minmax_scaler.pkl
│   │   └── proxy_discriminator.keras
│   ├── auth_utils.py
│   ├── database.py
│   ├── main.py
│   ├── ml_model.py
│   ├── requirements.txt
│   └── schemas.py
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   └── Navbar.jsx
│   │   ├── pages/
│   │   │   ├── About.jsx
│   │   │   ├── Dashboard.jsx
│   │   │   ├── Home.jsx
│   │   │   ├── LogFood.jsx
│   │   │   ├── Login.jsx
│   │   │   └── Register.jsx
│   │   ├── App.jsx
│   │   ├── index.css
│   │   └── main.jsx
│   ├── index.html
│   ├── package-lock.json
│   ├── package.json
│   ├── postcss.config.js
│   ├── tailwind.config.js
│   └── vite.config.js
│
└── .gitignore
```

## 🚀 Local Installation & Setup

To run this project locally, you need to start both the backend server and the frontend development server.

### 1. Clone the repository
```bash
git clone [https://github.com/p-v-srinag/WEIGHTLOSS_APP.git](https://github.com/p-v-srinag/WEIGHTLOSS_APP.git)
cd WEIGHTLOSS_APP
```

### 2. Backend Setup
Open a terminal, navigate to the backend directory, set up the environment, and run the server:
```bash
cd backend
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python main.py
```
*(Note for Windows users: use `venv\Scripts\activate` instead of `source venv/bin/activate`)*

### 3. Frontend Setup
Open a new, separate terminal window, navigate to the frontend directory, and start the development server:
```bash
cd frontend
npm install
npm run dev
```
*The frontend should now be running locally, typically on `http://localhost:5173`.*

## 📄 Citation
If you find this project or the associated research useful, please cite the IEEE paper:
> **P. V. S. Nag, et al.,** *"A Hybrid Machine Learning Framework for Personalized Weight Loss through Protein Intake Pattern Analysis,"* IEEE Xplore, 2026. [DOI/Link: 11497296](https://ieeexplore.ieee.org/document/11497296)

## 👨‍💻 My Self
**P Venkata Sri Nag** [LinkedIn](https://www.linkedin.com/in/p-v-srinag) | [GitHub](https://github.com/p-v-srinag)
