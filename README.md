# Financial_Market_Movements_Prediction_System
The project focuses on predicting NASDAQ stock prices using both machine learning and deep learning techniques. To predict stock prices and other financial indicators using different models.
(NASDAQ Stock Price Prediction - Quant Researcher Assessment)

This repository contains the solution to the Quant Researcher Assessment focused on predicting NASDAQ stock prices using deep learning models.

 ## Project Overview

**Goal: Predict closing prices using historical stock data**

**Models Trained:**

      Linear Regression (baseline)

      Random Forest

      LSTM

      GRU (best performer)

      CNN-LSTM

 **Key Results**

   *Model*     ,    *RMSE*

    Random Forest , 0.00035
    LSTM , 0.2246
    GRU , 0.1519
    CNN-LSTM , 0.2469

GRU achieved the best performance with the lowest RMSE.

 ## Setup Instructions

   **Clone the repository:**
 
    git clone https://github.com/ranugi/Financial_Market_Movements_Prediction_System.git
    cd Financial_Market_Movements_Prediction_System

   **Create a virtual environment:**
   
    python -m venv venv
    source venv/bin/activate   # on Unix/macOS
    venv\Scripts\activate      # on Windows

   **Install dependencies:**
   
    pip install -r requirements.txt
    

 ## How to Run   

   **Load the Trained Model**

    from tensorflow.keras.models import load_model
    model = load_model("models/trained_model.h5")
    model.summary()

   **To test a prediction, run:**

    import numpy as np
    sample_input = np.random.rand(1, 60, 5)
    model.predict(sample_input)
   
