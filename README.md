# California Housing Price Estimation – Full-Stack ML Application

## Project Overview

Developed and deployed a full-stack **Machine Learning application** to predict **median housing values in California**.

This project covers the complete ML lifecycle:

- Exploratory Data Analysis (EDA)    
- Model Selection & Optimization  
- Web-based inference  

## Technical Implementation

### Data Analysis & Feature Analysis

- Analyzed **20,640 instances** from the **1990 U.S. Census dataset**
- Conducted correlation analysis on key features:
  - `MedInc` (Median Income)
  - `HouseAge`
  - `Latitude`
  - `Longitude`
- Evaluated feature impact on the target variable:
  - `MedianHouseValue`

### Model Selection & Optimization

Benchmarked multiple regression algorithms using **Scikit-Learn**:

- AdaBoostM2
- XGBoost
- Random Forest Regressor  
- LightGBM Regressor  

**Best Model: LightGBM**

- Achieved an **R² Score of 0.866**
- Demonstrated better generalization and predictive accuracy

### Inference Pipeline

- Serialized trained model and scalers using **Pickle**
- Ensured consistent feature transformation during real-time inference
- Built a **Flask-based REST API** to:
  - Accept `POST` requests
  - Process district-level housing data
  - Return predicted median values

## Web Integration

- Developed a responsive frontend interface
- Integrated frontend with Flask backend

Users can:
1. Input district-level data
2. Submit for evaluation
3. Receive instant housing price predictions

## Key Technical Stack

### Machine Learning
- Python
- LightGBM
- Scikit-Learn
- Pandas
- NumPy

### Backend & API
- Flask
- Pickle (Model Serialization)

### Frontend
- HTML5
- CSS

## Performance Metrics

| Metric | Value |
|--------|--------|
| **Best Model** | LightGBM Regressor |
| **Evaluation Metric** | R² |
| **Score Achieved** | **0.866** |

## Outcome

A production-ready, end-to-end Machine Learning system capable of:

- Performing real-time inference
- Maintaining feature consistency
- Delivering high-accuracy predictions
