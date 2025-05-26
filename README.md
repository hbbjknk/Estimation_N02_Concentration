# Estimating Ground-Level NO₂ in Lombardy and Veneto: A Machine Learning Approach with Explainable AI(XAI) Insights
## Objectives
  - To estimate ground-level NO₂ concentrations in the target regions using advanced machine learning models.
  - To apply Explainable AI (XAI) techniques for interpreting and understanding the internal workings of the predictive models.
## Dataset
  - `ID_Zindi`, `Date`, `ID` (Station ID)
  - `LAT`, `LON` (Geolocation)
  - `Precipitation`, `LST` (Land Surface Temp)
  - `AAI` (Aerosol Absorbing Index)
  - `CloudFraction`, `NO2_total`, `NO2_strat`, `NO2_trop`
  - `TropopausePressure`
  - `GT_NO2` (Ground Truth NO₂ concentration)
## Methods & Tools
  - **Languages & Libraries**: Python, Pandas, NumPy, Scikit-learn, XGBoost, Seaborn, Matplotlib
  - **Techniques**:
   - Data Cleaning & Preprocessing
   - Feature Engineering & Correlation Analysis
   - Model Training & Hyperparameter Tuning
   - Evaluation Metrics: RMSE, MAE
## Machine Learning Models Used
  - Linear Regression
  - Spline Regression
  - Decision Tree Regressor
  - Random Forest Regressor
  - Gradient Boosting
  - XGBoost Regressor
  - Long Short Term Memory
  - LightGBM
  - CatBoost
  - Ensemble(Catboost and LightGBM)
## Results
  - Best model: `Ensemble Model`
  - RMSE: 6.9300
  - MAE: 4.6535 µg/m³
  - Visualizations: Heat Map, Beeswarm Plot, Bar Plot for SHAP values
## Conclusion
This project demonstrates the effectiveness of machine learning techniques in estimating ground-level NO₂ concentrations using satellite-derived data and environmental variables. By leveraging features such as tropospheric NO₂, land surface temperature, precipitation, cloud cover, and other atmospheric indicators, the models achieved reliable predictive performance. Furthermore, the integration of Explainable AI methods provided valuable insights into the contribution and influence of each feature, enhancing the interpretability and transparency of the models. These insights are crucial for environmental scientists and policymakers to make informed decisions. The results suggest that satellite data, when combined with robust machine learning and interpretability techniques, can serve as a cost-effective and scalable solution to monitor air pollution levels in regions with limited ground monitoring infrastructure. This work contributes to ongoing efforts in air quality management, offering a framework that can be extended to other pollutants and geographical areas.
