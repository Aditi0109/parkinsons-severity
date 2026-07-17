## Prediction of Parkinson's Disease Severity Using Voice Features and Machine Learning

### This project compared seven regression models and three experimental setups for predicting Parkinson's disease severity from voice features.

Among the baseline models, the Random Forest Regressor Chain gave the best accuracy at R squared ~ 0.95, well ahead of any linear approach. 

Running both targets through a chain rather than predicting them independently worked well because motor and total UPDRS are highly correlated.

The lag-augmented model which included patient's previous UPDRS score technically scored higher at 0.998, but that number is misleading, it was mostly predicting that tomorrow's score would look like today's, not learning anything from the voice. 

The voice-only model with per-subject temporal splits is the most honest result in the paper: R squared = 0.895 and MAE = 1.85 UPDRS points with no access to prior clinical scores.
