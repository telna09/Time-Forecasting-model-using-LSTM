# ✈️ Air Passengers Time Series Forecasting using LSTM

This project implements a deep learning model using **Long Short-Term Memory (LSTM)** networks to forecast monthly international airline passenger counts based on historical data from **1949 to 1960**. It includes end-to-end processing: loading, training, evaluation, and **future forecasting for the next 24 months**.

---

## 📊 Dataset

- **Source**: [Airline Passengers Dataset](https://raw.githubusercontent.com/jbrownlee/Datasets/master/airline-passengers.csv)
- **Description**: Monthly totals of international airline passengers from 1949 to 1960.
- **Features**:
  - `Month`: Date (YYYY-MM)
  - `Passengers`: Number of passengers in that month

---

## 🧠 Model Architecture

- **Type**: LSTM (Long Short-Term Memory) Neural Network
- **Framework**: TensorFlow / Keras
- **Layers**:
  - LSTM layer with 50 units (return sequences)
  - Dropout (20%)
  - Second LSTM layer
  - Dropout (20%)
  - Dense output layer
- **Loss Function**: Mean Squared Error (MSE)
- **Optimizer**: Adam

---

## 🔄 Workflow

1. **Load & visualize** the dataset
2. **Normalize** values using MinMaxScaler
3. **Create sequences** of 12 months to predict the next month
4. **Train/test split** (80/20)
5. **Build and train** the LSTM model
6. **Evaluate** performance with MSE
7. **Forecast** 24 months into the future using recursive prediction
8. **Plot** and optionally **export** forecast results

---

## 📈 Results

- Plots include:
  - Model loss over epochs
  - Historical vs Forecasted passenger trends (1961–1962)
- Forecast is based on the model's ability to learn from the temporal trends in the original 1949–1960 data.

---

## 🚀 How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name

## Install dependencies

pip install -r requirements.txt

## Launch Jupyter Notebook

jupyter notebook Deep_learning_Timeseries_Forecasting_model_using_LSTM.ipynb


## 🛠️ Requirements

- Python 3.7+

- TensorFlow

- Keras

- Numpy

- Pandas

- Scikit-learn

- Matplotlib

## Install all with:
pip install numpy pandas matplotlib scikit-learn tensorflow

## 📁 Files
Deep_learning_Timeseries_Forecasting_model_using_LSTM.ipynb – Main notebook with full workflow

future_air_passengers_forecast.csv (optional) – Output file with future predictions

README.md – Project documentation

## 📌 To-Do
 Add hyperparameter tuning

 Evaluate using RMSE/MAE

 Add multivariate time series support (e.g., including economic factors)
