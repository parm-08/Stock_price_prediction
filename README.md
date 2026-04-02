# 📈 Stock Price Prediction using LSTM

## 📌 Overview
This project predicts stock prices using a deep learning model called Long Short-Term Memory (LSTM). It analyzes historical stock data to learn patterns and forecast future prices.

---

## 🚀 Features
- Time-series forecasting using LSTM  
- Data preprocessing and normalization  
- Sequence creation (60-day window)  
- Model training and prediction  
- Visualization of actual vs predicted prices  

---

## 🛠️ Technologies Used
- Python  
- NumPy  
- Pandas  
- Matplotlib  
- Scikit-learn  
- TensorFlow / Keras  

---

## 📂 Project Workflow

### 1. Data Collection
- Load historical stock data (CSV file)  
- Includes Date, Open, Close, Volume  

### 2. Data Preprocessing
- Select "Close" price  
- Set Date as index  
- Normalize data using MinMaxScaler  

### 3. Train-Test Split
- Split dataset into training and validation  

### 4. Sequence Creation
- Use past 60 days to predict next value  
- Create input-output pairs  

### 5. Model Building
- Sequential model  
- 2 LSTM layers (150 units each)  
- 1 Dense output layer  

### 6. Model Compilation
- Loss: Mean Squared Error  
- Optimizer: Adam  

### 7. Model Training
- Train using epochs and batch size  

### 8. Prediction
- Prepare test sequences  
- Reshape into 3D format  
- Generate predictions  

### 9. Inverse Scaling
- Convert predictions back to original values  

### 10. Visualization
- Plot:
  - Training data  
  - Actual prices  
  - Predicted prices  

---

## 📊 Output
Graph comparing actual vs predicted stock prices.

---

## ▶️ How to Run

```bash
pip install numpy pandas matplotlib scikit-learn tensorflow
