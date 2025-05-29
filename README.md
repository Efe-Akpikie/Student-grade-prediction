# 🎓 Final Grade Prediction Using Regression

This project predicts students' final grades (`G3`) based on academic, personal, and social features. Using machine learning regression models, we aim to understand the factors that influence academic performance in Portuguese secondary schools.

🔗 [Kaggle Dataset](https://www.kaggle.com/datasets/dipam7/student-grade-prediction)

## 📌 Objective

Predict the final grade (`G3`) of students using features such as:
- G1: First period grade
- G2: Second period grade
- Personal, family, and academic background

## 📂 Dataset Overview

- **Source**: UCI / Kaggle Student Performance Dataset
- **Features**: 30
- **Target Variable**: `G3` (Final Grade)

### Sample Features:
- `sex`, `age`, `studytime`, `failures`, `schoolsup`, `famrel`, `activities`, `romantic`
- `G1`, `G2` (grades from earlier periods)

## 🔍 Key Findings

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

## 📊 Technologies Used

- Python 3
- Jupyter Notebook
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn (for regression models)

## 🚀 Getting Started

1. **Clone the repo**:
   ```bash
   git clone https://github.com/yourusername/student-grade-prediction.git
   cd student-grade-prediction
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Download dataset**:
   Download the CSV file from [Kaggle](https://www.kaggle.com/datasets/dipam7/student-grade-prediction) and place it in the `data/` folder.

4. **Run the notebook**:
   Open `Student_Grade_Prediction.ipynb` in Jupyter and run through the cells.

## 📈 Model Performance

- Several regression models were explored.
- Feature importance and correlation analysis were conducted.
- Final evaluation metrics (MAE, RMSE, R²) are detailed in the notebook.

## 📚 Citation

> P. Cortez and A. Silva. Using Data Mining to Predict Secondary School Student Performance. FUBUTEC 2008, Porto, Portugal.

## 📝 License

This project is licensed under the MIT License.
