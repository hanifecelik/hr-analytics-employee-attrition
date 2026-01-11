# HR Analytics: Employee Attrition Prediction

Machine Learning project predicting employee churn for TechSolutions using Logistic Regression

## Quick Links

- **Live Notebook (Kaggle)**: https://www.kaggle.com/code/hanifeelik/hr-analytics-employee-attrition-prediction/notebook
- **LinkedIn**: https://www.linkedin.com/in/hanifecelik/

## Project Overview

**Business Problem**: TechSolutions is losing talented employees to competitors. HR needs to predict at-risk employees for proactive retention.

**Solution**: Binary classification model using Logistic Regression

**Dataset**: [IBM HR Analytics Attrition Dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset) (1,470 employees, 35 features)

## Results

| Metric | Score |
|--------|-------|
| Accuracy | 87.4% |
| Precision | 71.2% |
| Recall | 65.8% |
| F1-Score | 0.684 |
| ROC-AUC | 0.851 |

## Key Findings

1. **Overtime** is the strongest predictor of attrition
2. Younger employees (20-35) at higher risk
3. Sales department needs targeted retention
4. Low income + poor work-life balance = critical factors

## Feature Engineering

Created 5 new features:
- `career_stability`: TotalWorkingYears / Age
- `low_salary_hike`: Flag for raises < 15%
- `work_life_risk`: Low balance + Overtime combination
- `undervalued`: Low rating + Below-median income
- `travel_risk`: Frequent travel + Long commute

## Business Impact

- **Expected turnover reduction**: 30-40%
- **Annual savings**: $360K-$480K
- **ROI**: 3-4x on retention programs

## Technologies

- Python 3.10+
- scikit-learn (Logistic Regression)
- pandas, numpy
- matplotlib, seaborn

## Project Structure
```
├── notebooks/
│   └── HR_Analytics_Kaggle.ipynb
├── README.md
└── LICENSE
```

## How to Use

### Option 1: View on Kaggle (Recommended)
Click the **Live Notebook** link above - code runs automatically!

### Option 2: Local Setup
```bash
git clone https://github.com/KULLANICI-ADINIZ/hr-analytics-employee-attrition.git
cd hr-analytics-employee-attrition
pip install pandas numpy scikit-learn matplotlib seaborn
# Download dataset from Kaggle link above
```

## AI Tools Disclosure

This project utilized AI assistance for:
- Feature engineering brainstorming (ChatGPT)
- Code optimization (GitHub Copilot)
- Documentation enhancement

All strategic decisions, data analysis, and business insights are human-driven.

## Author

**Hanife Çelik**
- LinkedIn: https://www.linkedin.com/in/hanifecelik/
- Kaggle: https://www.kaggle.com/hanifeelik
- Email: hnfcelik34@gmail.com

## License

MIT License - Free to use for learning and portfolio purposes

## Acknowledgments

- Dataset: IBM HR Analytics (Kaggle)
- Bootcamp: Ecodation Makine Öğrenmesi Bootcamp
- Mentor: Deniz Alkan
