# Stainless Steel Jewellery Buyback Analytics
## MSc Data Analytics Dissertation - Statistical Analysis Code

**Author:** Urmila Ramesh Koli  
**Student ID:** Q1093614  
**Institution:** Berlin School of Business & Innovation / University for the Creative Arts  
**Program:** MSc Data Analytics  
**Year:** 2025-2026  

---

## 📊 Project Overview

This repository contains Python code for statistical analysis and machine learning 
models supporting the dissertation:

**"Leveraging Data Analytics for Sustainable Stainless Steel Jewellery Buyback 
Programs in Indian Retail Markets"**

### Research Objectives:
1. Develop predictive models for buyback participation (>80% accuracy)
2. Validate optimal pricing thresholds through statistical analysis
3. Implement SQL database for 100% material traceability
4. Create interactive Tableau dashboards for stakeholder visualization
5. Quantify consumer preferences through structured survey research (N=69)
6. Demonstrate circular economy framework feasibility

---

## 🔬 Methodology

### Data Sources:
- **Primary Data:** Online survey (N=69 respondents, November-December 2024)
- **Secondary Data:** Transaction database (313 records, 2019-2024)

### Statistical Methods:
- Chi-square tests for independence (α = .05)
- One-sample t-tests (comparison to neutral midpoint)
- Independent samples t-tests (group comparisons)
- Pearson correlation analysis
- Random Forest classification (scikit-learn)
- Scipy.optimize pricing algorithms

### Key Findings:
- ✅ Random Forest model: **82.8% accuracy** (exceeds 80% benchmark)
- ✅ Optimal premium: **10%** (statistically validated, p < .001)
- ✅ Sustainability consciousness predicts buyback: **r = .284, p = .018**
- ✅ Gender-neutral market: **p = .604** (no significant difference)

---

## 📁 Repository Structure

---

## 🚀 Quick Start

### Requirements:
- Python 3.11+
- Libraries: pandas, numpy, scipy, scikit-learn, matplotlib, seaborn

### Installation:
```bash
# Clone repository
git clone https://github.com/Urmilakoli/dissertation-stainless-steel-analytics.git

# Install dependencies
pip install -r requirements.txt

# Run analysis
Python
```

---

## 📈 Analysis Scripts

### 1. Data Preparation (`01_data_preparation.py`)
- Cleans survey data (N=69)
- Handles missing values
- Encodes categorical variables
- Creates derived features

**Output:** `data/survey_data_cleaned.csv`

---

### 2. Chi-Square Tests (`02_chi_square_tests.py`)
- **Test 1:** Sustainability Importance × Premium Willingness
  - χ²(12, N=69) = 31.58, p = .002, Cramér's V = .389
- **Test 2:** Gender × Sustainable Purchase Behavior
  - χ²(3, N=69) = 0.187, p = .980 (no significant difference)
- **Test 3:** Age × Stainless Steel Interest
  - χ²(9, N=69) = 3.42, p = .945 (no significant difference)

**Output:** `results/tables/chi_square_results.csv`

---

### 3. T-Tests (`03_t_tests.py`)
- **One-Sample:** Materials vs neutral midpoint (3.0)
  - Stainless Steel: t(68) = -1.63, p = .108 (ambivalent)
  - Recycled Precious Metals: t(68) = 2.86, p = .006 (positive)
- **Independent:** Gender comparisons
  - t(67) = -0.52, p = .604 (no difference)

**Output:** `results/tables/ttest_results.csv`

---

### 4. Correlation Analysis (`04_correlations.py`)
- Sustainability × SS Interest: r(67) = .284, p = .018, R² = .081
- Premium × Buyback: r(67) = .412, p < .001, R² = .170
- Correlation matrix (6 materials)

**Output:** 
- `results/tables/correlation_results.csv`
- `results/figures/correlation_scatter.png`

---

### 5. Random Forest Model (`05_random_forest.py`)
- **Accuracy:** 82.8% (test set)
- **Precision:** 0.80
- **Recall:** 0.84
- **F1-Score:** 0.82
- **AUC-ROC:** 0.87
- **Cross-validation:** 83.7% ± 2.1% (5-fold)

**Top Predictors:**
1. Sustainability Importance (Gini = 0.342)
2. Premium Willingness (Gini = 0.278)
3. Purchase Value (Gini = 0.156)

**Output:** 
- `results/tables/random_forest_performance.csv`
- `results/figures/feature_importance.png`

---

### 6. Pricing Optimization (`06_pricing_optimization.py`)
- **Algorithm:** scipy.optimize.minimize_scalar
- **Optimal Premium:** 10.2%
- **Expected Participation:** 40.6%
- **Projected Profit:** ₹104,521 annually

**Output:** 
- `results/tables/pricing_sensitivity_analysis.csv`
- `results/figures/pricing_optimization_curve.png`

---

### 7. Visualizations (`07_visualizations.py`)
- Demographic distributions
- Material preference charts
- Scatter plots with regression lines
- Feature importance bar charts

**Output:** All figures in `results/figures/`

---

## 📊 Key Results Summary

| Analysis | Key Finding | Statistical Evidence |
|----------|-------------|---------------------|
| **Predictive Model** | 82.8% accuracy | Exceeds 80% benchmark (Kumar et al., 2024) |
| **Optimal Pricing** | 10% premium | χ²(4)=18.67, p<.001; 40.6% acceptance |
| **Material Interest** | RPM > SS > Bio | t-tests, p<.05 for RPM, p>.05 for SS |
| **Gender Effect** | No difference | t(67)=-0.52, p=.604, d=-0.13 |
| **Sustainability Link** | Positive correlation | r=.284, p=.018, R²=.081 |

---

🔗 Related Resources

- **Dissertation PDF:** [Link when available]
- **Tableau Dashboard:** [Public link when deployed]
- **SQL Database Schema:** See `documentation/database_schema.md`
- **Survey Instrument:** See `documentation/survey_questionnaire.pdf`

---

## 📝 Citation

If you use this code or methodology, please cite:Koli, U. R. (2026). Leveraging Data Analytics for Sustainable Stainless Steel
Jewellery Buyback Programs in Indian Retail Markets. MSc Dissertation,
Berlin School of Business & Innovation / University for the Creative Arts.
---

## 📄 License

This project is licensed under the MIT License - see LICENSE file for details.

**MIT License Summary:**
- ✅ Free to use, modify, and distribute
- ✅ Must include original license and copyright notice
- ✅ No warranty provided

---

## 🤝 Contributing

This is academic research code. While contributions are not expected, feedback 
and suggestions are welcome via Issues tab.

---

## 📧 Contact

**Urmila Ramesh Koli**  
- **Email:Q1093614@students.berlinsbi.com**
- **LinkedIn:** Q1093614@students.berlinsbi.com 
- **University:** Berlin School of Business & Innovation  

---

## ⚠️ Data Privacy Notice

Survey data has been anonymized to protect participant privacy:
- No personally identifiable information (PII) included
- Aggregate statistics only
- Compliant with GDPR and university ethics guidelines

Raw data available upon reasonable request with appropriate ethics approval.

---

## 🙏 Acknowledgments

- **Supervisor:** Dr. Anuj, Berlin School of Business & Innovation
- **Python Libraries:** pandas, scipy, scikit-learn, matplotlib, seaborn
- **Inspiration:** Circular economy literature (Kirchherr et al., 2017)

---

**Last Updated:** January 31, 2026  
**Status:** ✅ Complete - Dissertation submitted
