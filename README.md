🏡 Bangalore House Price Prediction – Full Stack ML Project
A complete end‑to‑end Machine Learning project that predicts house prices in Bangalore using a trained regression model.
This project includes:

A frontend client (HTML/CSS/JS)

A Flask backend server

A trained ML model (pickle)

Supporting utilities and artifacts

The goal is to provide a simple web interface where users can input property details and receive an estimated price instantly.

📁 Project Structure

BHP/
│
├── client/
│   ├── app.html
│   ├── app.js
│   ├── app.css
│
├── server/
│   ├── server.py
│   ├── util.py
│   ├── artifacts/
│   │   ├── model.pkl
│   │   ├── columns.json
│   └── __pycache__/   (ignored)
│
├── model/
│   ├── bangalore_house_price_prediction.ipynb
│   ├── model.pkl
│   ├── columns.json
│
├── .idea/              (ignored)
└── README.md
🧠 Project Overview
This project predicts house prices based on:

Location

Square footage

Number of bedrooms (BHK)

Number of bathrooms

The model was trained using a dataset of Bangalore house prices and deployed using a Flask API.

🧪 Machine Learning Model
The model is built using:

Python

Pandas

NumPy

Scikit‑learn

Inside the model/ folder:

bangalore_house_price_prediction.ipynb → Jupyter notebook for data cleaning, feature engineering, model training

model.pkl → Trained regression model

columns.json → List of input features used by the model

🖥️ Frontend (client/)
The frontend is a simple, clean UI built with:

app.html → Main webpage

app.css → Styling

app.js → Sends user inputs to the backend API and displays predictions

Users enter property details, and the page fetches predictions from the Flask server.

🔧 Backend (server/)
The backend is powered by Flask.

server.py → Main API server

util.py → Loads the model, processes inputs, and returns predictions

artifacts/ → Contains the production model and feature columns

API endpoints include:

/predict_home_price → Returns predicted price

/get_location_names → Returns list of locations

🚀 How to Run the Project Locally
1. Install dependencies
Code
pip install -r requirements.txt
2. Start the Flask server
Code
python server/server.py
3. Open the frontend
Open client/app.html in your browser.

📦 Requirements
Typical dependencies include:

Flask

NumPy

Pandas

Scikit‑learn

(You can generate a requirements.txt using pip freeze > requirements.txt.)

🧹 Ignored Files
The following are excluded using .gitignore:

__pycache__/

.idea/

*.pyc

*.ipynb_checkpoints

These are not needed in version control.

⭐ Features
Clean UI for user input

Real‑time price prediction

Fully trained ML model

Modular backend architecture

Easy to deploy on EC2, Render, or Railway

📌 Future Improvements
Add location dropdown from backend

Add model retraining pipeline

Deploy as a live web app

Add Docker support
