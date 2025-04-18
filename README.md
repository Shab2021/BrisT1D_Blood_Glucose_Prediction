# BrisT1D_Blood_Glucose_Prediction
 Forecast blood glucose levels one hour ahead using the previous six hours of participant data.  
https://www.kaggle.com/competitions/brist1d/overview

Среда для разработки:  
Python 3.12.9  
scikit-learn 1.6.1  
pandas 2.2.3  
numpy 2.2.4  

*BrisT1D_Blood_Glucose_Prediction-hour_shuffle.ipynb*:  
Данные берутся за последний час, используются все признаки, в датафрейме index_col='id', 'time' преобразуется в 'hour' и 'minute', в activities NaN заменены на категорию 'No activity'.  Используется алгоритм HistGradientBoostingRegressor с поддержкой пропущенных значений (NaN) и категориальных данных. 
