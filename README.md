# Metal Trading – Lead–Lag Networks

This project investigates dynamic **lead–lag** relationships among key metal trading and financial assets (gold, silver, FX pairs, interest‐rate indices, etc.) using advanced time‐series and machine‐learning techniques.

## What We Do

1. **Data Collection & Preprocessing**  
   - Fetch historical data (Yahoo Finance) for:  
     - Metals: Gold, Silver  
     - FX & Indices: EUR/USD, JPY/USD, Dollar Index  
     - Long‐term rates: 10‑year US Treasury, 10‑year Euro Bund  
   - Clean data, handle missing values, and align time series.

2. **Exploratory Analysis (EDA)**  
   - Plot each series and compute correlation matrices (instantaneous & lagged).  
   - Examine similarity structures and seasonality.

3. **Lead–Lag via DTW**  
   - Compute Dynamic Time Warping distances for all asset pairs.  
   - Determine typical lead/lag offsets (who leads, who follows).

4. **Model Tuning & Validation**  
   - Optimize hyperparameters (Optuna) and perform cross‐validation.  
   - Evaluate performance with MSE, MAE, RMSE and the Wasserstein distance.

5. **Entropy Transfer Graph**  
   - Convert DTW results into a similarity/entropy matrix.  
   - Build and visualize a directed network showing information flow between assets.

6. **Conclusions & Insights**  
   - Identify leading and lagging assets.  
   - Provide actionable trading and risk‐management recommendations.

