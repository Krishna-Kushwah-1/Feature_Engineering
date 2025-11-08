# 🧠 Feature Engineering on IBM HR Analytics Attrition Dataset

Colab Notebook: https://colab.research.google.com/drive/1A5CQMQNBNpQTVuzXzp-qhJMFrLewcu0f?usp=sharing

***

## 📘 Overview
This project showcases feature engineering techniques applied to the **IBM HR Analytics Employee Attrition Dataset**. The primary goal is to clean and transform HR data, making it suitable for predictive modeling—specifically, to forecast whether an employee will leave the company (attrition: Yes/No).

***

## 🧾 Dataset

- **Source:** [Kaggle – IBM HR Analytics Employee Attrition Dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)
- **Records:** 1,470 employees
- **Features:** 35 columns including Age, Gender, JobRole, OverTime, MonthlyIncome, and Attrition

***

## ⚙️ Feature Engineering Steps

1. **Data Cleaning**
   - Checked for missing or duplicate entries (none found).
   - Converted object columns to categorical types for efficiency.

2. **Encoding**
   - Applied label encoding to categorical variables (e.g., Gender, OverTime, Department).

3. **Scaling**
   - Standardized numeric columns using `StandardScaler` to balance feature contributions.

4. **Feature Extraction**
   - Utilized PCA to reduce dimensionality and identify principal components explaining ~90% of variance.

5. **Feature Selection**
   - Examined correlation heatmap and used Random Forest feature importance to identify and retain key predictors.

***

## 🔍 Observations

- Resulting dataset is clean, uniform, and fully numeric.
- Most impactful features for attrition prediction: **OverTime**, **MonthlyIncome**, and **YearsAtCompany**.
- PCA revealed that much of the dataset’s information can be represented in fewer dimensions.

***

## ⚖️ Ethical Discussion

- **Bias risk:** Features like Gender and MaritalStatus can introduce discrimination.
- **Mitigation:** These features were excluded from model training.
- **Best practices recommended:** Perform bias audits and utilize explainability tools (e.g., SHAP, LIME) to ensure transparent, fair predictions.

***

## 🏁 Conclusion

The feature engineering process successfully converted raw HR data into a model-ready and ethically sound format, underscoring the importance of thorough preprocessing and bias awareness in HR analytics projects.

***

**Author:** Krishna Kushwah  
**Institute:** MIT Academy of Engineering, Pune  
**Faculty:** Anita Shingade
