# NASA CMAPSS Jet Engine RUL Prediction (FD001)  

## Project Overview:  
NASA is seeking data professionals to analyze simulated jet engine data to predict the number of remaining operational cycles before an engine reaches failure. This project focuses on the FD001 dataset, aiming to understand when failure may occur to save lives and reduce economic costs.  
*** 
### Methodology:  

To obtain a model with the highest predictive power, the following steps were taken:

* Model Selection: The XGBoost regressor was chosen for its ability to handle complex, non-linear sensor data.

* Feature Engineering: Analysis focused on three critical sensors (s_7, s_8, s_11) to guide the prediction of Remaining Useful Life (RUL).

* Hyperparameter Tuning: A GridSearch was implemented to tune the model to its best possible capabilities.

* Data Analysis: The training set was used to establish a RUL column, focusing attention on the most useful information regarding engine degradation.
*** 
### Modeling Results:  

* The final optimized model achieved a Root Mean Squared Error (RMSE) of 20.72.  

* This indicates that the model’s predictions are, on average, within approximately 20.72 cycles of the actual observed failure values.  

* The model effectively predicts the timeframe in which an engine is likely to fail.  

As shown in the performance visualization, points closer to the red line represent higher prediction accuracy.  
<img width="812" height="496" alt="Data Visualization" src="https://github.com/user-attachments/assets/e4a95d3a-01e0-4f4e-845b-58f30566e887" />  
*** 
### Impact and Recommendations:  

* Maintenance Planning: These results can be used to determine when to perform critical maintenance checks or replace engines entirely.  

* Safety and Economics: Accurate RUL prediction allows for proactive interventions that save lives and prevent the high costs associated with unscheduled engine failure.  

* Operational Awareness: Users should account for the margin of error, as the model provides a highly informed timeframe for failure rather than a perfect single-point prediction.  
