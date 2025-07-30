# 🚨 ML Fraud Detector in Large-Scale Transaction Data

## Project Overview

This project aims to detect fraudulent transactions within a financial dataset containing over **6.3 million records**. The workflow involved thorough data analysis, intelligent feature engineering, and the deployment of robust machine learning models—tackling real-world challenges like class imbalance and the significance of transaction outliers.

## Dataset Summary
-**
- **Source File:** `Fraud.xlsx`
- **Download Link:** [Click here to download the dataset](https://drive.google.com/file/d/15qUXu1ztjybd9qDtYrpsvyaluAKBDmQ2/view?usp=sharing)
- **Rows:** 6,300,000+
- **Columns:** 11
- **Fraudulent Cases:** ~8,200 (Rare/Imbalanced)
- **Initial Observations:**
  - No missing or duplicate values—saving data cleaning effort.
  - Outliers in transaction amounts retained, as they could indicate fraudulent behavior.

## Workflow

1. **Data Assessment**
   - Verified dataset integrity: No duplicates or missing values.
   - Outlier detection in transaction amounts (retained for potential fraud insights).

2. **Feature Engineering**
   - Logical feature selection—removing irrelevant columns.
   - Applied one-hot encoding to categorical features (like transaction `type`).
   - Standardized numeric columns for better model training.

3. **Dealing with Class Imbalance**
   - Selected features via RFECV (with Balanced Random Forests) to address imbalance.
   - Used SMOTE (Synthetic Minority Over-sampling Technique) during training to oversample fraud cases.

4. **Modeling & Tuning**
   - Trained three models: Random Forest, Balanced Random Forest, and XGBoost.
   - Performed hyperparameter tuning on a 60,000-row sample and applied the best settings to the full dataset.

5. **Result**
   - Random Forest yielded the best results, balancing high fraud detection with minimal false positives.

## Project Structure

├── Accredian_Assingment.ipynb

├── Fraud.xlsx

├── generated-image.png
 
├── README.md

├── requirements.txt


## Technologies Used

- Python (pandas, numpy, scikit-learn, imbalanced-learn, XGBoost)
- Jupyter Notebook
- Data visualization libraries (e.g., matplotlib, seaborn)

## Getting Started

1. **Clone the repository.**
2. **Install dependencies:**  

pip install -r requirements.txt

3. **Open and run `Accredian_Assingment.ipynb`** for full analysis and results.

## Highlights & Insights

- **Class imbalance** is the main challenge—handled via resampling (SMOTE) and smart feature selection.
- **Outlier retention** helped the model by preserving possible fraud signals.
- **Random Forest** delivered the best fraud detection performance after careful tuning.

## Acknowledgements

Grateful to the contributors and data providers who made this analysis possible!

---

To create the file on your local system:

1. Open a text editor (like Notepad, VS Code, Sublime Text).
2. Paste the above content.
3. Save the file as `README.md` in your project directory.

If you want, I can also help draft a `requirements.txt` or other project files! Just let me know.
. 
