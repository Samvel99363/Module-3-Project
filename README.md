# Module 3 Mini-Project — Data Cleaning & Preparation Case Study  
### Dataset: Employment in India (Messy / Dirty Dataset)

This project is part of the **Machine Learning Data Preparation Workshop (Module 3)**.  
The goal is to independently perform a full end-to-end data preparation pipeline on a messy real-world dataset and produce a fully clean, transformed, and model-ready dataset.

The final notebook includes:  
✅ Exploratory Data Analysis (EDA)  
✅ Missing value handling  
✅ Data cleaning & data type corrections  
✅ Outlier detection and treatment  
✅ Feature engineering  
✅ Data transformation (encoding + scaling)  
✅ Machine Learning model (Linear Regression)

---

## 📁 Project Files

| File | Description |
|------|-------------|
| `module3_employment_project_ENHANCED.ipynb` | **Main Jupyter Notebook** with the entire workflow completed |
| `Messy_Employment_India_Dataset.csv` | Original raw dataset used in the project |
| `README.md` | Documentation and project description |

---

## 📊 Project Overview

### **Objective**
Prepare a dirty Kaggle dataset for a machine learning model that predicts **Income** in the Indian employment sector.

### **Dataset Characteristics**
- Real-world messy dataset
- Contains missing values, inconsistent formatting, mixed data types, and outliers
- ~4,000 rows, ~12 columns
- Contains both numerical and categorical variables

---

## 🔍 Steps Performed

### **1. Exploratory Data Analysis (EDA)**
- `df.info()`, `.describe()`, data type inspection  
- Histograms for numerical variables  
- Bar charts for categorical variables  
- Correlation heatmap  
- Identified missing values and outliers  

---

### **2. Data Cleaning**
- Missing values filled:  
  - Numeric → **Median**  
  - Categorical → **Mode**
- Converted numeric-like strings into numeric values  
- Removed impossible values  
- IQR-based outlier capping  

---

### **3. Feature Engineering**
Created new meaningful features:
- **Experience_Level** → bucketed experience into 4 categories  
- **Income_per_YearExp** → ratio of income vs experience  
- **Income_Age_Interaction** → interaction term capturing demographic effects  

---

### **4. Data Transformation**
- One-hot encoded categorical columns  
- Scaled numerical features using `StandardScaler`  
- Produced final **100% numerical**, model-ready dataset  

---

### **5. Machine Learning Model**
Built a baseline model:
- **Linear Regression**
- Train-test split  
- Evaluated using:  
  - MAE  
  - RMSE  
  - R² Score  
- Extracted model coefficients to understand feature importance  

---

## 🧠 Results & Insights

- The dataset required significant cleaning before modeling.  
- Several engineered features improved model interpretability.  
- Linear Regression provided a good baseline, with potential improvements from tree-based models.

---

## 🚀 How to Run the Notebook

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/<your-repo>.git
