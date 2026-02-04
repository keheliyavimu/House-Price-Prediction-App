![Project Banner](assets/ss.png)


# 🏡 Bangalore House Price Prediction – Full Stack ML Project

A complete end‑to‑end Machine Learning application that predicts house prices in Bangalore using a trained regression model.  
The system integrates a lightweight HTML/JS frontend, a Flask backend API, and a production‑ready ML model.

---

## 🧠 Project Overview

This project estimates house prices based on:

- Location  
- Square footage  
- Number of bedrooms (BHK)  
- Number of bathrooms  

The model was trained on Bangalore housing data and deployed through a Flask API for real‑time predictions.

---

## 🧪 Machine Learning Model

Built using:

- Python  
- Pandas  
- NumPy  
- Scikit‑learn  

Model components inside the `model/` directory:

- **bangalore_house_price_prediction.ipynb** – Data cleaning, feature engineering, model training  
- **model.pkl** – Trained regression model  
- **columns.json** – Feature names used by the model  

---

## 🖥️ Frontend (client/)

A simple, responsive UI built with:

- **app.html** – Main interface  
- **app.css** – Styling  
- **app.js** – Sends user inputs to the backend and displays predictions  

Users enter property details, and the frontend fetches predictions from the Flask server.

---

## 🔧 Backend (server/)

Powered by **Flask**, responsible for serving predictions and model metadata.

Key files:

- **server.py** – Main API server  
- **util.py** – Loads model, processes inputs, returns predictions  
- **artifacts/** – Production model + feature columns  

### API Endpoints

- `GET /get_location_names` – Returns list of available locations  
- `POST /predict_home_price` – Returns predicted house price  

---

## 🚀 How to Run the Project Locally

### 1. Install dependencies
```bash
pip install -r requirements.txt
```

### 2. Start the Flask backend
```bash
python server/server.py
```

### 3. Open the frontend
Open:
```
client/app.html
```
