📊 Titanic Dataset – Exploratory Data Analysis (EDA)

This repository contains Task 5: Exploratory Data Analysis (EDA) performed on the classic Titanic Survival Dataset.
The goal of this task was to explore the data visually and statistically, extract insights, identify trends, and understand the factors that influenced passenger survival.

📌 Task Objective

Extract insights using visual and statistical exploration.
This includes understanding data structure, identifying patterns, trends, anomalies, relationships between variables, and summarizing key findings.

🛠 Tools Used

Python

Pandas (data cleaning, manipulation)

Matplotlib (visualizations)

Seaborn (advanced visualizations)

📂 Deliverables

Jupyter Notebook containing full EDA code

PDF Report with all graphs, visuals, and observations

README.md (this file)

📘 Dataset

Titanic Dataset (train.csv)
Contains 891 passenger records with survival information.

Key columns include:

PassengerId, Survived, Pclass, Name, Sex, Age

SibSp, Parch, Ticket, Fare, Cabin, Embarked

📊 EDA Process

The analysis followed the suggested mini-guide:

✔ 1. Dataset Exploration

.info()

.describe()

.value_counts()

Missing values analysis

✔ 2. Visual Exploration

Histograms

Boxplots

Scatter plots

Correlation heatmap

Pairplot

Survival rate analysis (Sex, Pclass, AgeGroup)

✔ 3. Writing Observations

For every plot and table, clear observations were documented.

✔ 4. Final Summary

Key insights and conclusions were compiled from all visuals.

📈 Detailed Outcomes & Observations

Below are the clean and structured insights extracted from all images/plots in the EDA report.

🔹 Column Information & Missing Data

Age → 177 missing values

Cabin → 687 missing values (majority)

Embarked → 2 missing

All other columns are complete.

➡️ Cabin is too incomplete to use without heavy imputation.
➡️ Age requires reasonable imputation.

🔹 Summary Statistics

Survival rate: 38%

Most passengers in 3rd class

Average age: ~30 years

Fare highly skewed (max = 512)

Most traveled alone (SibSp & Parch mostly 0)

➡️ The dataset has strong social/economic diversity.

🔹 Categorical Distributions
Sex

Male ≈ 577

Female ≈ 314
➡️ Almost twice as many men.

Pclass

Most passengers are 3rd class, then 1st, then 2nd.
➡️ Titanic was heavily populated by lower-class passengers.

Embarked

Southampton (S) → Most

Cherbourg (C)

Queenstown (Q)
➡️ Southampton was the primary departure point.

Survived

549 died

342 survived
➡️ Survival was not evenly distributed.

🔹 Age Distribution (Histogram)

Mostly 20–40 years old

Few children and seniors

Some infants (<1 year)

➡️ Young adults dominated the passenger list.

🔹 Fare Distribution (Histogram)

Right-skewed

Most fares < 50

Some extreme high values (~500)

➡️ Huge economic inequality among passengers.

🔹 Age by Pclass (Boxplot)

1st class passengers tend to be older

3rd class passengers younger

➡️ Wealthier people were generally older.

🔹 Fare by Pclass (Boxplot)

Strong fare difference by class

Large outliers in 1st class

Very low fares in 3rd class

➡️ Ticket price reflects socioeconomic status.

🔹 Age vs Fare (Survived vs Died)

Survivors cluster around higher fares

Children have noticeable survival advantage

Overall overlap indicates multiple factors influence survival

➡️ Fare and Age alone do not fully predict survival.

🔹 Correlation Heatmap

Pclass ↔ Fare → strong negative

Survived ↔ Fare → weak–moderate positive

Survived ↔ Pclass → negative

SibSp ↔ Parch → small positive correlation

➡️ Class and Fare are the most informative numeric features.

🔹 Pairplot

Fare shows strong skewness

Age fairly normally distributed

Pclass shows distinct clusters

Survival relates slightly to Fare and Pclass

➡️ Dataset is not linearly separable—requires multi-feature modeling.

🔹 Survival Rate by Sex

Female ≈ 75% survival rate

Male ≈ 20% survival rate

➡️ Strongest predictor of survival.

🔹 Survival Rate by Pclass

1st Class → ~62%

2nd Class → ~47%

3rd Class → ~24%

➡️ Wealth significantly increased survival.

🔹 Survival Rate by Age Group

Highest survival: Children (0–12)

Lowest survival: Elderly (60+)

➡️ “Women and children first” rule is strongly visible.

📌 Final Summary
1. Key Predictors of Survival

Sex (female > male)

Pclass (1st > 2nd > 3rd)

Fare (higher fare → better survival)

Children had priority

2. Data Quality Notes

Cabin unusable due to extreme missingness

Age requires imputation

Fare requires transformation (skewed)

3. Dataset Patterns

Mostly young adults

Mostly males

Mostly 3rd class

Mostly traveling alone

4. Visual Trends

Clear socioeconomic impact on survival

Multiple factors needed to model survival—no single variable is enough

📁 Project Structure
📦 Titanic_EDA
 ┣ 📜 Titanic_EDA.ipynb
 ┣ 📜 titanic_eda_report.pdf
 ┣ 📜 train.csv
 ┗ 📜 README.md

▶ How to Run the Notebook

Install required libraries:

pip install pandas matplotlib seaborn


Open Jupyter Notebook:

jupyter notebook


Run the file:

Titanic_EDA.ipynb

✔ Outcome

Through this EDA, I gained hands-on experience with:

Data exploration

Visualization techniques

Identifying trends and anomalies

Understanding survival patterns

Summarizing insights from statistical and visual analysis

This Repository is created as beginer for learning purpose only!
