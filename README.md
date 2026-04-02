#Stock Price Prediction using LSTM
📌 Overview

This project predicts stock prices using a deep learning model called Long Short-Term Memory (LSTM). It analyzes historical stock data to learn patterns and forecast future prices. The model is trained on past data and evaluated by comparing predicted values with actual stock prices.

🚀 Features
Time-series forecasting using LSTM
Data preprocessing and normalization
Sequence creation (60-day window)
Model training and prediction
Visualization of actual vs predicted prices

🛠️ Technologies Used
Python
NumPy
Pandas
Matplotlib
Scikit-learn
TensorFlow / Keras

📂 Project Workflow
1️⃣ Data Collection
Historical stock data is loaded (CSV file)
Contains columns like Date, Open, Close, Volume, etc.
2️⃣ Data Preprocessing
Selected relevant column (e.g., Close price)
Converted Date column to index
Normalized data using MinMaxScaler (0 to 1 range)
3️⃣ Train-Test Split
Dataset divided into:
Training data
Validation (testing) data
4️⃣ Creating Sequences
Used past 60 days data to predict next value
Prepared input-output pairs for model training
5️⃣ Building LSTM Model
Created Sequential model
Added:
2 LSTM layers (150 units each)
1 Dense output layer
6️⃣ Model Compilation
Loss function: Mean Squared Error
Optimizer: Adam
7️⃣ Model Training
Trained model on training dataset
Used multiple epochs and batch size
8️⃣ Prediction
Prepared test data sequences
Reshaped data into 3D format (samples, time_steps, features)
Generated predictions
9️⃣ Inverse Scaling
Converted predicted values back to original scale
🔟 Visualization
Plotted graph comparing:
Training data
Actual prices
Predicted prices

📊 Output
<img width="1326" height="683" alt="image" src="https://github.com/user-attachments/assets/8c251268-7a23-44a8-82a5-7e2ff5debee9" />


📎 How to Run
# Install dependencies
pip install numpy pandas matplotlib scikit-learn tensorflow

# Run the notebook or Python script
💡 Future Improvements
Add multiple features (Open, Volume, etc.)
Improve accuracy using hyperparameter tuning
Deploy using Streamlit for interactive UI
Add real-time stock datas.
