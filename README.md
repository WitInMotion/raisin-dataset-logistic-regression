# Raisin Variety Classification 🍇

This project is part of **TechCrush AI BootCamp - Assignment 4**.  
The goal is to build a machine learning model that classifies raisin varieties (Kecimen or Besni) using the **Raisin Dataset**.

---

##  Dataset
- **File**: `Raisin_Dataset.xlsx`
- **Features**: Measurements of raisin shape and size (Area, Perimeter, Convex Area, etc.)
- **Target**: `Class` (Kecimen = 0, Besni = 1)

---

##  Methodology
1. Load dataset with **pandas** in Google Colab.
2. Encode target labels (`Kecimen`, `Besni`) into numeric values.
3. Split data into **80% train / 20% test** (stratified).
4. Build a pipeline with:
   - **StandardScaler** (feature scaling)
   - **Logistic Regression**
5. Perform **5-fold Cross Validation** on training set.
6. Evaluate performance on the test set.

---

##  Results
- **Cross-validation accuracy (train)**: ~0.88  
- **Test set accuracy**: **0.89 (88.9%)** ✅  
- Performance exceeds the required **81% minimum accuracy**.

**Classification Report (Test Set):**
          precision    recall  f1-score   support
       0       0.94      0.83      0.88        90
       1       0.85      0.94      0.89        90

accuracy                           0.89       180
macro avg 0.89 0.89 0.89 180
weighted avg 0.89 0.89 0.89 180

##  Requirements
- Python 3.8+
- pandas  
- numpy  
- scikit-learn  
- matplotlib  
- seaborn  
- openpyxl  

---

##  How to Run
1. Open the notebook `Raisin_Classification.ipynb` in **Google Colab** or Jupyter.  
2. Upload the dataset (`Raisin_Dataset.xlsx`).  
3. Run all cells.  
4. View model performance and confusion matrix.

---

Habiba Musa 
TechCrush AI BootCamp Participant  
