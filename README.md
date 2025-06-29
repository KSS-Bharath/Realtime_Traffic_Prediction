#Real-Time Traffic Prediction Using LSTM

This project predicts hourly traffic flow at a junction using a Long Short-Term Memory (LSTM) neural network. It simulates real-time traffic data and provides next-hour vehicle count forecasts based on live input.

#Project Highlights:
Time series forecasting using LSTM,
Real-time simulation of traffic input,
Live prediction with next-hour forecasts,
Trained on historical traffic data (Kaggle dataset),
Built with Python, TensorFlow, Pandas, NumPy.

#Project Structure
traffic_prediction_project/
├── traffic # Traffic dataset
├── model.py # Model training and saving
├── stream_sim.py # Simulates real-time traffic input
├── real_time_predict.py # Predicts traffic from streamed data
└── README.md # Project documentation

# Dataset
**Source**: [Kaggle Traffic Prediction Dataset](https://www.kaggle.com/datasets/fedesoriano/traffic-prediction-dataset)**Description**: Hourly vehicle counts at 4 junctions in Hyderabad, India.
**Used Features**: `DateTime`, `Junction`, `Vehicles`

# Model
Input: Last 24 hourly vehicle counts
Output: Forecast for next hour
Model: LSTM with 64 units → Dense(1)
Loss: Mean Squared Error (MSE)
Epochs: 50
Framework: TensorFlow/Keras
