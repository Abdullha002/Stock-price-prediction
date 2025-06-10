# 📈 Stock Price Prediction Web App

This project is a web application that predicts stock prices using LSTM (Long Short-Term Memory) deep learning model. The app is built using **Streamlit** for the user interface and **Keras/TensorFlow** for the model backend.

---

## 🚀 Features

- Predict future stock prices using historical data
- Interactive UI to input any stock symbol (e.g., `GOOG`, `AAPL`)
- Visualization of:
  - Moving Averages (MA50, MA100, MA200)
  - Original vs Predicted Prices
- Download historical stock data from Yahoo Finance

---

## 🧠 Tech Stack Used

- Python
- Pandas, NumPy, Matplotlib
- Scikit-learn (MinMaxScaler)
- Keras (LSTM, Dense, Dropout)
- Streamlit
- yFinance

---

## 📁 Folder Structure

```
📦 Stock-Prediction-Streamlit/
│
├── app.py                      # Streamlit Web App
├── stock_prediction.ipynb     # Model training and evaluation notebook
├── Stock Predictions Model.keras  # Saved LSTM model
├── README.md
```

---

## ⚙️ Installation & Setup

1. **Clone the Repository**
```bash
git clone https://github.com/your-username/stock-price-prediction.git
cd stock-price-prediction
```

2. **Create Virtual Environment**
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install Required Libraries**
```bash
pip install -r requirements.txt
```

> Or manually install:
```bash
pip install numpy pandas matplotlib yfinance scikit-learn keras tensorflow streamlit
```

4. **Run the App**
```bash
streamlit run app.py
```

---

## 🧪 How It Works

- The `.ipynb` notebook trains a deep LSTM model on stock data fetched from Yahoo Finance.
- The model is saved and loaded in the `app.py` script.
- Users can input any stock ticker symbol (e.g., `GOOG`) to see data and predictions.
- Visual comparisons are shown between original prices and predicted values.

---

## 📌 Notes

- Make sure the path to `Stock Predictions Model.keras` in `app.py` is correct.
- Streamlit UI automatically refreshes when you update the input stock symbol.
- The prediction is based only on past price trends (no news or external factors considered).

---
