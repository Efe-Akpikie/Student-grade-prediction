Final Grade Prediction Using Regression

This project predicts students' final grades (`G3`) based on academic, personal, and social features. Using machine learning regression models, we aim to understand the factors that influence academic performance in Portuguese secondary schools.

🔗 [Kaggle Dataset](https://www.kaggle.com/datasets/dipam7/student-grade-prediction)

## Objective

Predict the final grade (`G3`) of students using features such as:
- G1: First period grade
- G2: Second period grade
- Personal, family, and academic background

## Key Findings

### Positively Correlated with Final Grade (`G3`)
| Feature         | Correlation | Interpretation                            |
|----------------|-------------|-------------------------------------------|
| G2             | **0.95**     | Strongest predictor – second period grade |
| School Support | 0.75         | Extra academic support helps              |
| Sex (Female)   | 0.29         | Female students performed better on avg   |
| famrel         | 0.28         | Good family relationships boost grades    |
| G1             | 0.10         | First period grade has some predictive power |

### Negatively Correlated with Final Grade (`G3`)
| Feature     | Correlation | Interpretation                              |
|-------------|-------------|---------------------------------------------|
| activities  | **-0.58**    | Extracurriculars linked to lower grades     |
| romantic    | -0.40        | Students in relationships performed worse   |
| failures    | -0.38        | More past failures = lower final grade      |
| nursery     | -0.26        | Nursery attendance showed weak negative corr|
| internet    | -0.23        | Home internet access had a small negative corr |

## Languages/Libraries Used

- Python 3
- Jupyter Notebook
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn (for regression models)

## Citation

> P. Cortez and A. Silva. Using Data Mining to Predict Secondary School Student Performance. FUBUTEC 2008, Porto, Portugal.

