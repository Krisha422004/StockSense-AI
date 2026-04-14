A sophisticated 8th-semester B.Tech Major Project featuring a Flask-based web application for real-time market analysis, LSTM-driven price forecasting, and comprehensive administrative oversight.

## 🚀 Overview
 AI stock predictor bridges the gap between traditional technical analysis and modern Deep Learning. By utilizing Long Short-Term Memory (LSTM) networks, the system identifies non-linear patterns in historical stock data to provide actionable financial recommendations.

## ✨ Key Features

### 🧠 AI & Analytics
- **LSTM Deep Learning:** High-accuracy 5-day price forecasting for top-tier stocks.
- **Technical Fallback:** Hybrid prediction engine using Simple Moving Averages (SMA) and Volatility modeling for non-trained tickers.
- **Interactive Visuals:** Real-time historical price charts and training convergence (Loss) plots.

### 👤 User Experience
- **Personalized Dashboard:** Track recent prediction history and global market indices (NIFTY 50, SENSEX).
- **Profile Management:** Securely update personal details and encrypted passwords.
- **Stock Comparison:** Side-by-side performance analysis of two different symbols.

### 🛡️ Admin & Security
- **System Telemetry:** Real-time monitoring of CPU, RAM, and Storage health during AI training.
- **Audit Logs:** Immutable tracking of all administrative actions with **CSV Export** capability.
- **User Management:** Full CRUD system with secure Bcrypt password hashing.

## 🛠️ Tech Stack
- **Backend:** Python (Flask)
- **Database:** MySQL (via XAMPP/SQLAlchemy)
- **Frontend:** HTML5, Tailwind CSS, Jinja2, Chart.js
- **Machine Learning:** TensorFlow, Keras, Scikit-learn
- **Data APIs:** Yahoo Finance (yfinance), Finnhub API

## ⚙️ Installation & Setup
w
### 1. Prerequisites
- Python 3.9+
- XAMPP (For MySQL)
- A stable internet connection (for real-time API data)

### 2. Environment Configuration
Create a `.env` file in the root directory:
```text
FLASK_SECRET=your_dev_key_123
FINNHUB_API_KEY=your_api_key_here

### 3. Database Setup
Start Apache and MySQL in XAMPP.
Go to http://localhost/phpmyadmin.
Create a new database named stock_db.

    The application uses SQLAlchemy to automatically generate tables on first run.

### 4. Install dependencies
pip install -r requirements.txt

### 5. AI Model Training : To generate the initial LSTM models for the top 10 stocks:
python train_top_10.py

### 6. run the application
python app.py


###Project Structure

├── app.py              # Main Flask server & Routes
├── train_top_10.py     # LSTM Training Pipeline
├── services/           # API Logic & External Integrations
├── models/             # Saved .h5 models and .pkl scalers
├── templates/          # Jinja2 HTML Templates
├── static/             
│   ├── plots/          # Generated Training Loss Charts
│   └── assets/         # CSS & JS files
└── requirements.txt    # Python Dependencies