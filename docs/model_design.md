# 🤖 Model Design  
## Flight Delay Prediction

---

## 1. Problem Type
Binary classification:  
**Target:** delay_15 = 1 if arrival_delay >= 15 minutes, else 0

---

## 2. Feature Engineering Plan

### Time Features
- hour  
- weekday  
- month  
- season  
- weekend indicator  
- peak hour indicator  

### Route Features
- origin  
- destination  
- airport distance (optional)

### Airport Features
- number of runways  
- runway utilization  
- traffic volume  

### Airline Features
- historical delay rate  
- cancellation rate  

---

## 3. Baseline Model
- Logistic Regression

## 4. Advanced Models
- Random Forest  
- Gradient Boosting  
- XGBoost  

---

## 5. Evaluation Metrics
- Accuracy  
- Precision / Recall  
- F1-score  
- ROC–AUC  
- SHAP values for explainability  

---

## 6. Data Splitting
- Train: 70%  
- Validation: 15%  
- Test: 15%

---

## 7. Risks & Considerations
- Class imbalance  
- Missing time values  
- Airport code inconsistencies  
- Seasonal variability  
