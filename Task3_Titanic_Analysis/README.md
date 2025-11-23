# 🚢 Titanic Dataset – Exploratory Data Analysis (EDA)

This project is part of the **Oasis Infobyte Data Science Internship – Task 3**, where I performed Exploratory Data Analysis (EDA) on the Titanic dataset.  
The objective is to explore survival patterns and understand how different factors influenced passenger survival.

---

## 📌 Objectives
- Load and explore the dataset  
- Identify missing values  
- Perform univariate and bivariate analysis  
- Visualize survival trends  
- Generate insights for future predictive modeling  

---

## 📂 Dataset Used
**titanic_dataset.csv**

Important columns:
- Survived  
- Pclass  
- Sex  
- Age  
- SibSp  
- Parch  
- Fare  
- Embarked  

---

## 🛠️ Steps Performed (EDA)

### ✔ 1. Data Understanding
```python
df.head()
df.info()
df.describe()
df.isnull().sum()
✔ 2. Handling Missing Values
Checked missing Age & Embarked values

Next step: fill or drop based on the model need

✔ 3. Visualizations
📊 Survival Count
python
Copy code
sns.countplot(x='Survived', data=df)
👨‍🦰/👩 Survival by Gender
python
Copy code
sns.countplot(x='Sex', hue='Survived', data=df)
🎟 Survival by Passenger Class
python
Copy code
sns.countplot(x='Pclass', hue='Survived', data=df)
🔥 Correlation Heatmap (Numeric Data Only)
python
Copy code
numeric_df = df.select_dtypes(include=['int64','float64'])
sns.heatmap(numeric_df.corr(), annot=True, cmap='coolwarm')
📊 Key Insights
Female passengers survived significantly more

1st class passengers had the highest survival rate

Fare amount shows positive correlation with survival

Age has weak correlation with survival

Several columns contain missing values which need preprocessing

🧰 Technologies Used
Python

Pandas

NumPy

Matplotlib

Seaborn

Jupyter Notebook / Google Colab

📁 Files Included
Task3_Titanic_EDA.ipynb

titanic_dataset.csv

README.md

⭐ Conclusion
This Titanic EDA gives a strong foundation for upcoming steps like:

Data Preprocessing

Feature Engineering

Predictive Modeling (Logistic Regression, KNN, Decision Trees, etc.)
