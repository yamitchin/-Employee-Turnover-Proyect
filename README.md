# Employee Turnover Risk Prediction

## Overview
End-to-end ML pipeline to predict which employees are most likely to leave a company, quantify the financial impact of attrition, and generate individual risk scores to help HR prioritise retention actions.

**Model:** Decision Tree Classifier · **AUC: 0.716** · **176 high-risk employees identified**

---

## Business Impact
- **16.1% attrition rate** across 1,470 employees
- **$2,719,005** total financial exposure from past turnover
- **Sales Representatives** identified as highest-risk role: 39.8% attrition rate
- Reducing turnover by 30% would save **$815,701/year**

---

## Key Findings
- Employees who work overtime are significantly more likely to leave
- Single employees show higher attrition rates than married employees
- Low salary combined with high overtime is the strongest attrition signal
- Top 5 predictive features: `horas_extra`, `estado_civil`, `nivel_laboral`, `salario_mes`, `anos_compania`

---

## Tech Stack
- **Language:** Python 3 (Google Colab)
- **Libraries:** Pandas, NumPy, Matplotlib, Scikit-learn
- **Model:** DecisionTreeClassifier (max_depth=4)
- **Encoding:** OneHotEncoder
- **Evaluation:** ROC-AUC Score
- **Visualisation:** Tableau Public

---

## Dataset
- **Source:** IBM HR Analytics Employee Attrition dataset
- **Size:** 1,470 employees × 31 original variables → 27 after cleaning
- **Target:** `abandono` (Yes/No) — 16.1% positive class

---

## Next Steps
- [ ] Upgrade to Random Forest + SMOTE (target AUC 0.85+)
- [ ] Add SHAP values for individual prediction explainability
- [ ] Translate Tableau dashboard to English

---

## Author
**Yamit Chinchilla** — Data Analyst & Data Scientist  
[LinkedIn](https://www.linkedin.com/in/yamit-chinchilla5456067b/) · [Portfolio](https://www.notion.so/5b0890e2c52382d3b18a819018199713)
