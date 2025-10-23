# -flash-drought-prediction-1
This project aims to predict flash droughts by analyzing key environmental parameters such as rainfall, soil moisture, and temperature, obtained from Google Earth Engine (GEE).
Machine Learning models like XGBoost and LSTM are used to detect early drought onset patterns from time-series data.

🧠 Workflow Overview
Data Collection:
Retrieved rainfall, soil moisture, and temperature data from Google Earth Engine (GEE).
Exported to CSV for model training.
Preprocessing:
Cleaned missing values using mean imputation.
Created time-series sequences for temporal modeling.
Modeling:
XGBoost: baseline model for feature importance and quick prediction.
LSTM: deep learning model for sequential drought prediction (achieved ~92% validation accuracy).
Evaluation:
Compared performance on accuracy, F1-score, and confusion matrix.

📊 Dataset
Due to GitHub file size limits, the full dataset (≈626 MB) is stored externally.
You can download it from the link below:
📂 https://drive.google.com/file/d/1CrZuh4Ws3wuYRxS037qXs75Tt6sIsn5h/view?usp=drive_link

Results:
| Model   | Accuracy | Validation Accuracy |
| ------- | -------- | ------------------- |
| XGBoost | 99.8%    | 99.8%               |
| LSTM    | 91–92%   | 92%                 |

📚 Tools & Technologies
Google Earth Engine (GEE)
Python, Pandas, NumPy, Scikit-learn, TensorFlow/Keras, XGBoost
Matplotlib, Seaborn
Jupyter Notebook
