# 🩸 AI-powered Anemia Diagnosis with Explainability Techniques

A complete explainable AI (xAI) project to classify **anemia** using real-world medical data.  
This project combines powerful machine learning with **SHAP**, **LIME**, and **Fuzzy Association Rule Mining** to interpret model predictions clearly and transparently.  

---

## 📊 Dataset Overview

This project uses a dataset from **Kaggle**:

🔗 [Original Dataset - Kaggle: Anemia Dataset](https://www.kaggle.com/datasets/biswaranjanrao/anemia-dataset)

> For demonstration purposes, we selected the **first 70 rows** and removed the `Gender` column to simplify visualization.  
> You can easily switch to the original dataset or use your own modified version.

📁 Dataset file provided:  
`data/anemia_cleaned_70rows.csv`

---

## ⚙️ Project Structure

```bash
.
├── Full_Pipeline.ipynb              # Complete notebook with all steps
├── notebooks/                       # Modular notebooks
│   ├── 01_LIME_Explainer.ipynb
│   ├── 02_SHAP_Explainer.ipynb
│   └── 03_Fuzzy_Association.ipynb
├── data/
│   ├── anemia_cleaned_70rows.csv
│   └── kaggle_dataset_link.txt
├── requirements.txt                 # Required libraries
├── README.md                        # Project documentation
└── LICENSE                          # MIT License


---

## 🔍 Methods Used

### ⚡️ Model
- `XGBoostClassifier`: Trained on clinical features (`Hemoglobin`, `MCV`, `MCH`, `MCHC`)
- Evaluation metrics: `Accuracy`, `Precision`, `Recall`, `F1-Score`

### 🧠 Explainability Techniques

| Tool          | Purpose                               | Output                      |
|---------------|----------------------------------------|-----------------------------|
| **SHAP**      | Global & local feature importance      | Summary plots, waterfall   |
| **LIME**      | Local explanations (per sample)        | Bar explanation plots       |
| **Fuzzy Rule Mining** | Human-readable diagnostic rules | IF-THEN association rules   |

---

## ✨ Example Output

Example SHAP summary plot:  
![SHAP Summary](https://github.com/YourUsername/YourRepo/blob/main/images/shap_summary.png)

Fuzzy rule (sample):
IF {Result_Anemia, MCHC_Medium} THEN {Hemoglobin_Medium}: Confidence = 0.93


---

## 🧪 How to Run

### ✅ 1. Install dependencies

```bash
pip install -r requirements.txt



### ✅ 2.  Run full pipeline

# Jupyter notebook
jupyter notebook Full_Pipeline.ipynb

Or run each explanation method individually from the notebooks/ folder.


---

📦 Dependencies
Main libraries used:

xgboost

shap

lime

scikit-learn

mlxtend

scikit-fuzzy

matplotlib, seaborn, pandas, numpy

📋 Full list in: requirements.txt


---

💡 License
This project is licensed under the MIT License.
See LICENSE for more details.

👨‍💻 Author
Ahmad Paknezhad
M.Sc. Student in Artificial Intelligence in Medicine
📧 Email: a.s.paknezhad.1@gmail.com
🔗 LinkedIn: https://www.linkedin.com/in/ahmad-sourtiji-paknezhad-353842373/

🌟 Contributions
Contributions, suggestions, or issues are welcome!
Feel free to ⭐️ the repository if you find it helpful


