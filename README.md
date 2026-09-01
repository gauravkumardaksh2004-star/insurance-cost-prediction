# Insurance Cost Prediction 🏥💰

My first end-to-end Machine Learning project! This project explores the classic **Medical Insurance Cost** dataset and builds a regression model to predict individual medical insurance charges based on personal attributes.

## 📊 Dataset

The dataset (`insurance.csv`) contains 1,338 records with the following features:

| Column     | Description                                      |
|------------|---------------------------------------------------|
| `age`      | Age of the primary beneficiary                    |
| `sex`      | Gender (male/female)                               |
| `bmi`      | Body Mass Index                                    |
| `children` | Number of dependents covered by insurance          |
| `smoker`   | Whether the person smokes (yes/no)                 |
| `region`   | Residential region in the US                       |
| `charges`  | Individual medical costs billed by insurance (target)|

## 🔍 Project Workflow

1. **Exploratory Data Analysis (EDA)**
   - Checked shape, data types, and missing values
   - Visualized distributions of numeric columns (age, BMI, children, charges)
   - Explored categorical variables (sex, smoker, region) with count plots
   - Analyzed feature correlations with a heatmap

2. **Data Cleaning**
   - Removed duplicate rows
   - Verified there were no missing values

3. **Feature Engineering & Encoding**
   - Encoded `sex` and `smoker` as binary features (`is_female`, `is_smoker`)
   - One-hot encoded the `region` column
   - Created a new `bmi_category` feature (underweight, normal, overweight, obese) based on standard BMI ranges, then one-hot encoded it
   - Scaled numeric features (`age`, `bmi`, `children`) using `StandardScaler`

4. **Next Steps (Modeling)**
   - Train/test split
   - Train regression models (e.g., Linear Regression, Random Forest, XGBoost)
   - Evaluate performance using metrics like RMSE and R²

## 🛠️ Tech Stack

- Python
- Pandas & NumPy
- Matplotlib & Seaborn (visualization)
- Scikit-learn (preprocessing & modeling)

## 🚀 How to Run

1. Clone this repository
   ```bash
   git clone https://github.com/<your-username>/insurance-cost-prediction.git
   cd insurance-cost-prediction
   ```
2. Install dependencies
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```
3. Open the notebook
   ```bash
   jupyter notebook insurance_cost_prediction.ipynb
   ```

## 📌 Notes

This is a learning project built to practice the fundamentals of the machine learning workflow — from EDA to feature engineering. Contributions, suggestions, and feedback are welcome!

