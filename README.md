# Household Electricity Consumption Forecasting using LSTM

## Overview
This project uses a Long Short-Term Memory (LSTM) neural network to forecast household electricity consumption from historical power readings.

## Technologies Used
- Python
- Google Colab
- Pandas and NumPy
- Scikit-learn
- TensorFlow / Keras
- Matplotlib

## Dataset
Household Electric Power Consumption dataset.

- Target variable: `Global_active_power`
- Sampling interval: 1 minute
- Records used: 8,640 consecutive valid readings
- Period used: February 1–6, 2007

**Note:** The selected continuous segment contains 8,640 records rather than the original requirement of 10,000. The notebook selects the longest continuous segment of valid minute-level readings.

## Methodology
1. Load and preprocess the dataset.
2. Select consecutive valid minute-level records.
3. Normalize the consumption values using MinMaxScaler.
4. Create sequences using the previous 60 minutes.
5. Train an LSTM model using the Adam optimizer and MSE loss.
6. Evaluate predictions using MAE and RMSE.
7. Plot actual versus predicted consumption.
8. Generate next-minute consumption forecasts.

## Model Architecture
- LSTM layer: 64 units
- Dropout: 0.2
- LSTM layer: 32 units
- Dense layer: 16 units with ReLU activation
- Output layer: 1 unit

## Evaluation
The notebook reports Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE). Actual results should be taken from the executed notebook.

## How to Run
1. Open the notebook in Google Colab.
2. Upload the dataset CSV file.
3. Run the cells in order.
4. Review the evaluation metrics, prediction table, and forecast graph.

## Project Status
Completed prototype for household electricity consumption forecasting.
