
# ❤️ Heart Disease Prediction

This project predicts whether a person is likely to have **heart disease** ...
(# ❤️ Heart Disease Prediction

This project predicts whether a person is likely to have **heart disease** based on medical attributes.  
The model outputs a simple result:  
- ✅ **Has Heart Disease**  
- ❌ **Does Not Have Heart Disease**

---

## 📊 Dataset
- File: `heart.csv` (from UCI Heart Disease dataset)  
- Features include:
  - Age
  - Sex
  - Chest Pain Type (cp)
  - Resting Blood Pressure (trestbps)
  - Serum Cholesterol (chol)
  - Fasting Blood Sugar (fbs)
  - Resting ECG (restecg)
  - Max Heart Rate (thalach)
  - Exercise-Induced Angina (exang)
  - Oldpeak
  - Slope
  - Number of Major Vessels (ca)
  - Thalassemia (thal)  
- **Target column**: `1 = has disease`, `0 = no disease`

---

## ⚙️ How It Works
1. Load dataset  
2. Split into training & testing sets  
3. Train **Logistic Regression model**  
4. Evaluate with accuracy and confusion matrix  
5. Predict disease outcome for new patient data  

---

## 🚀 Run the Project in Google Colab
1. Upload `heart.csv`  
2. Open and run `heart_disease.ipynb`  
3. Example prediction:  

```python
# Example new patient data
# Format: [age, sex, cp, trestbps, chol, fbs, restecg, thalach, exang, oldpeak, slope, ca, thal]
new_person = [[52, 1, 0, 125, 212, 0, 1, 168, 0, 1.0, 2, 2, 3]]
prediction = model.predict(new_person)

if prediction[0] == 1:
    print("✅ Person has heart disease")
else:
    print("❌ Person does not have heart disease")
)
