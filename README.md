
# Stock Price Prediction using LSTM

This project builds a deep learning model using **LSTM (Long Short-Term Memory)** to predict stock prices based on historical data. The model is trained on Coca-Cola Company (KO) stock prices from 2012 to 2020 using Yahoo Finance data, with preprocessing and sequence modeling for time series forecasting.

---

## 📊 Dataset

- **Source:** Yahoo Finance via `yfinance`
- **Stock Symbol:** KO (Coca-Cola Company)
- **Date Range:** 2012–2020
- **Target:** Predict `Close` price for next day
- **Features Used:** Only `Close` price (can be extended)

---

## 🚀 Project Highlights

- Downloaded historical stock prices using `yfinance`
- Visualized trends with Matplotlib
- Preprocessed and scaled data with `MinMaxScaler`
- Built sequences of 60 time steps to capture temporal dependencies
- Trained a two-layer LSTM model with dropout and dense layers
- Compared predicted vs. actual prices using plots
- Measured accuracy based on a thresholded prediction difference

---

## 🧠 Model Architecture

- LSTM (64 units, return sequences)
- Dropout (0.2)
- LSTM (64 units, final layer)
- Dropout (0.2)
- Dense (32 units, ReLU)
- Dense (1 unit, final output)

---

## 🔍 Results

- Model trained on 80% of data; tested on the remaining 20%
- Accuracy metric: % of predictions within ±5% of actual price
- **Final Accuracy:** ~`87%` 

---

## 📈 Visualization

- Plots include:
  - Full closing price history
  - Train/Validation split
  - Actual vs. Predicted price overlay
- Sample Output:

![LSTM prediction graph placeholder](https://github.com/ShwetWasnik/Stock-Price-Prediction/raw/main/graph.png)

---

## 🛠️ Tech Stack

- **Languages:** Python
- **Libraries:**  
  - Pandas, NumPy, Matplotlib  
  - Scikit-learn  
  - TensorFlow/Keras  
  - yfinance

---

## 📁 Files Included

- `resumeStock.ipynb` — Main notebook
- `README.md` — Project overview

---

## 📌 Author

**Shwetang Wasnik**  
📫 [vishveshgupta191@gmail.com](mailto:vishveshgupta191@gmail.com)  
