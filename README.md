🏠 Real Estate House Price Prediction
A full-stack machine learning web application that predicts real estate house prices based on user inputs such as location, square footage, number of bedrooms, and bathrooms. Built using Python, Scikit-learn, Flask, and a responsive HTML/CSS/JavaScript frontend.
📌 Table of Contents
Project Overview
Project Structure
Tech Stack
Dataset
ML Model & Concepts
How to Run Locally
API Endpoints
Screenshots
Author
📖 Project Overview
This project is an end-to-end data science application that:
Builds a machine learning model using Linear Regression on the Bengaluru House Price dataset from Kaggle.
Deploys a Python Flask server that serves the trained model via REST API.
Provides a web interface (HTML/CSS/JavaScript) where users can input house details and get an instant price prediction.
📁 Project Structure
Realestate-House-Price-Prediction/
│
├── model/
│   ├── home_prices_model.ipynb     # Jupyter Notebook for model building
│   ├── banglore_home_prices_model.pickle  # Saved trained model
│   └── columns.json                # List of feature columns used by the model
│
├── server/
│   ├── server.py                   # Flask server entry point
│   ├── util.py                     # Utility functions (load model, predict price)
│   └── artifacts/                  # Folder containing model artifacts
│
├── client/
│   ├── app.html                    # Main frontend HTML page
│   ├── app.css                     # Styling
│   └── app.js                      # JavaScript for API calls and UI logic
│
└── README.md
🛠️ Tech Stack
Layer
Technology
Language
Python 3.x
ML Library
Scikit-learn (sklearn)
Data Handling
Pandas, NumPy
Visualization
Matplotlib
Backend
Python Flask
Frontend
HTML5, CSS3, JavaScript
Notebook
Jupyter Notebook
📊 Dataset
Source: Kaggle – Bengaluru House Price Data
Features used: Location, Total Square Feet, Number of Bathrooms, Number of BHK (Bedrooms)
Target Variable: Price (in Lakhs INR)
🤖 ML Model & Concepts
The model building phase (inside model/home_prices_model.ipynb) covers:
✅ Data loading and exploration
✅ Handling missing values and data cleaning
✅ Feature engineering (e.g., deriving BHK from size column)
✅ Outlier detection and removal
✅ Dimensionality reduction (consolidating rare locations)
✅ One-Hot Encoding for categorical variables (location)
✅ Model training using Linear Regression
✅ Hyperparameter tuning with GridSearchCV
✅ Model evaluation using K-Fold Cross Validation
✅ Saving the model using Python pickle
▶️ How to Run Locally
Prerequisites
Python 3.x installed
pip package manager
A modern web browser
Step 1: Clone the Repository
git clone https://github.com/Pavankumarudu/Realestate-House-Price-Prediction.git
cd Realestate-House-Price-Prediction
Step 2: Install Dependencies
pip install -r server/requirements.txt
If requirements.txt is not present, install manually:
pip install flask scikit-learn numpy pandas
Step 3: Start the Flask Server
cd server
python server.py
The server will start at http://127.0.0.1:5000/
Step 4: Open the Frontend
Open client/app.html directly in your browser or configure an Nginx/Apache server to serve it.
🔌 API Endpoints
Method
Endpoint
Description
GET
/get_location_names
Returns list of available locations
POST
/predict_home_price
Returns predicted price
Sample POST Request – /predict_home_price
{
  "total_sqft": 1000,
  "location": "Indira Nagar",
  "bhk": 2,
  "bath": 2
}
Sample Response
{
  "estimated_price": 85.75
}
🖥️ Screenshots
(Add screenshots of your web app here once deployed)
👨‍💻 Author
Pavan Kumar
📧 Registration No: 222G1A0580
🏫 Anantha Lakshmi Institute of Technology & Sciences
💼 B.Tech – Computer Science & Engineering
🔗 GitHub Profile
📄 License
This project is open-source and available under the MIT License.
⭐ If you found this project helpful, please consider giving it a star on GitHub!🏠 Real Estate House Price Prediction
A full-stack machine learning web application that predicts real estate house prices based on user inputs such as location, square footage, number of bedrooms, and bathrooms. Built using Python, Scikit-learn, Flask, and a responsive HTML/CSS/JavaScript frontend.
📌 Table of Contents
Project Overview
Project Structure
Tech Stack
Dataset
ML Model & Concepts
How to Run Locally
API Endpoints
Screenshots
Author
📖 Project Overview
This project is an end-to-end data science application that:
Builds a machine learning model using Linear Regression on the Bengaluru House Price dataset from Kaggle.
Deploys a Python Flask server that serves the trained model via REST API.
Provides a web interface (HTML/CSS/JavaScript) where users can input house details and get an instant price prediction.
📁 Project Structure
Realestate-House-Price-Prediction/
│
├── model/
│   ├── home_prices_model.ipynb     # Jupyter Notebook for model building
│   ├── banglore_home_prices_model.pickle  # Saved trained model
│   └── columns.json                # List of feature columns used by the model
│
├── server/
│   ├── server.py                   # Flask server entry point
│   ├── util.py                     # Utility functions (load model, predict price)
│   └── artifacts/                  # Folder containing model artifacts
│
├── client/
│   ├── app.html                    # Main frontend HTML page
│   ├── app.css                     # Styling
│   └── app.js                      # JavaScript for API calls and UI logic
│
└── README.md
🛠️ Tech Stack
Layer
Technology
Language
Python 3.x
ML Library
Scikit-learn (sklearn)
Data Handling
Pandas, NumPy
Visualization
Matplotlib
Backend
Python Flask
Frontend
HTML5, CSS3, JavaScript
Notebook
Jupyter Notebook
📊 Dataset
Source: Kaggle – Bengaluru House Price Data
Features used: Location, Total Square Feet, Number of Bathrooms, Number of BHK (Bedrooms)
Target Variable: Price (in Lakhs INR)
🤖 ML Model & Concepts
The model building phase (inside model/home_prices_model.ipynb) covers:
✅ Data loading and exploration
✅ Handling missing values and data cleaning
✅ Feature engineering (e.g., deriving BHK from size column)
✅ Outlier detection and removal
✅ Dimensionality reduction (consolidating rare locations)
✅ One-Hot Encoding for categorical variables (location)
✅ Model training using Linear Regression
✅ Hyperparameter tuning with GridSearchCV
✅ Model evaluation using K-Fold Cross Validation
✅ Saving the model using Python pickle
▶️ How to Run Locally
Prerequisites
Python 3.x installed
pip package manager
A modern web browser
Step 1: Clone the Repository
git clone https://github.com/Pavankumarudu/Realestate-House-Price-Prediction.git
cd Realestate-House-Price-Prediction
Step 2: Install Dependencies
pip install -r server/requirements.txt
If requirements.txt is not present, install manually:
pip install flask scikit-learn numpy pandas
Step 3: Start the Flask Server
cd server
python server.py
The server will start at http://127.0.0.1:5000/
Step 4: Open the Frontend
Open client/app.html directly in your browser or configure an Nginx/Apache server to serve it.
🔌 API Endpoints
Method
Endpoint
Description
GET
/get_location_names
Returns list of available locations
POST
/predict_home_price
Returns predicted price
Sample POST Request – /predict_home_price
{
  "total_sqft": 1000,
  "location": "Indira Nagar",
  "bhk": 2,
  "bath": 2
}
Sample Response
{
  "estimated_price": 85.75
}
🖥️ Screenshots
(Add screenshots of your web app here once deployed)
👨‍💻 Author
Pavan Kumar
📧 Registration No: 222G1A0580
🏫 Anantha Lakshmi Institute of Technology & Sciences
💼 B.Tech – Computer Science & Engineering
🔗 GitHub Profile
📄 License
This project is open-source and available under the MIT License.
⭐ If you found this project helpful, please consider giving it a star on GitHub!
