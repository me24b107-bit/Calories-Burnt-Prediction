# Calories Burnt Prediction Using Machine Learning

## Overview

This project predicts the number of calories burned during physical activity using machine learning techniques. The model leverages physiological and workout-related features such as age, gender, height, weight, exercise duration, heart rate, and body temperature to estimate calorie expenditure.

The objective was to compare multiple regression algorithms and identify the model that provides the most accurate calorie predictions.

---

## Dataset

The dataset contains **15,000 fitness activity records** with the following features:

| Feature | Description |
|----------|-------------|
| User_ID | Unique user identifier |
| Gender | Male/Female |
| Age | Age of the user |
| Height | Height (cm) |
| Weight | Weight (kg) |
| Duration | Exercise duration (minutes) |
| Heart_Rate | Heart rate during exercise |
| Body_Temp | Body temperature during exercise |
| Calories | Calories burned (Target Variable) |

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- XGBoost

---

## Project Workflow

### Data Exploration

- Analyzed feature distributions
- Studied relationships between physiological variables
- Visualized feature correlations and trends

### Data Preprocessing

- Handled categorical features
- Removed unnecessary columns
- Prepared training and validation datasets
- Performed feature selection and encoding

### Model Development

The following regression models were trained and evaluated:

- Linear Regression
- Ridge Regression
- Lasso Regression
- Random Forest Regressor
- XGBoost Regressor

### Model Evaluation

Models were compared using Mean Absolute Error (MAE) on both training and validation datasets.

---

## Exploratory Data Analysis

### Height vs Weight Relationship

A strong positive relationship was observed between height and weight, indicating consistent physical characteristics across the dataset.

### Calories Burned Analysis

Exercise duration showed the strongest relationship with calories burned, making it one of the most influential predictive features.

### Feature Distribution Analysis

Distributions of:

- Height
- Weight
- Duration
- Heart Rate
- Body Temperature
- Calories Burned

were analyzed to understand data spread and potential outliers.

### Correlation Analysis

A correlation heatmap was generated to identify relationships among features and determine their impact on calorie expenditure.

---

## Model Performance

| Model | Training Error | Validation Error |
|---------|---------|---------|
| Linear Regression | 17.89 | 18.01 |
| Ridge Regression | 17.89 | 18.01 |
| Lasso Regression | 17.92 | 18.00 |
| Random Forest Regressor | 4.00 | 10.45 |
| XGBoost Regressor | 7.89 | 10.12 |

### Best Model

**XGBoost Regressor**

- Training Error: **7.89**
- Validation Error: **10.12**

XGBoost achieved the lowest validation error and demonstrated the best generalization performance among all evaluated models.

---

## Results

- Built a calorie prediction system using **15,000 fitness activity records**.
- Evaluated five machine learning regression models.
- Identified exercise duration, body temperature, and heart rate as major predictors of calorie expenditure.
- Achieved a minimum validation error of **10.12 calories** using XGBoost.

---

## Project Structure

```text
Calories-Burnt-Prediction/
│
├── Calories_Burnt.csv
├── Calories_Burnt.py
├── README.md
│
├── images/
│   ├── height_weight.png
│   ├── feature_relationships.png
│   ├── distributions.png
│   └── correlation_heatmap.png
│
└── requirements.txt
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/Calories-Burnt-Prediction.git

cd Calories-Burnt-Prediction
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Usage

Run the project using:

```bash
python Calories_Burnt.py
```

The script will:

1. Load and preprocess the dataset.
2. Perform exploratory data analysis.
3. Train multiple regression models.
4. Compare model performance.
5. Display visualizations and evaluation metrics.

---

## Applications

- Fitness Tracking Systems
- Health Analytics Platforms
- Workout Recommendation Systems
- Personal Health Monitoring
- Sports Performance Analysis

---

## Future Improvements

- Hyperparameter tuning for XGBoost.
- Feature engineering using derived fitness metrics.
- Deployment as a Streamlit web application.
- Integration with wearable fitness devices.
- Real-time calorie expenditure prediction.

---

## Author

Sathwik Gorrela

B.Tech Mechanical Engineering  
Indian Institute of Technology Madras
