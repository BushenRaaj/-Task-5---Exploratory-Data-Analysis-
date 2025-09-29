# Task-5---Exploratory-Data-Analysis  
# 🔎 Exploratory Data Analysis (Titanic Dataset)

This project is part of the **Data Analyst Internship (Task 5: EDA)**.  
The goal is to practice **exploratory data analysis** using Python libraries to identify **patterns, trends, and anomalies** in a dataset.

---

## 📌 Project Overview

This project focuses on performing **statistical and visual exploration** of the dataset.  
The primary objective is to use **EDA techniques** to summarize key characteristics, detect relationships, and derive actionable insights.  

The dataset used here is the **Titanic Dataset**, which contains details of passengers such as demographics, ticket information, and survival status.  

---

### 🎯 Key Objectives
- Strengthen proficiency in **EDA techniques**.  
- Demonstrate ability to **summarize datasets** with statistical and graphical methods.  
- Explore **relationships and correlations** between variables.  
- Practice interpreting visuals into **meaningful insights**.  

---

### 🛠️ Techniques Applied
- **Data Inspection** → `.head()`, `.info()`, `.describe()`, `.value_counts()`.  
- **Univariate Analysis** → histograms, boxplots for distribution and outlier detection.  
- **Bivariate Analysis** → scatterplots, barplots, and violin plots.  
- **Multivariate Analysis** → `sns.pairplot()`, correlation heatmaps.  
- **Feature Relationships** → survival vs. gender, class, and age groups.  
- **Handling Skewness** → transformations and scaling when required.  

---
<img width="1907" height="740" alt="5 1" src="https://github.com/user-attachments/assets/6adeec00-6900-4aa7-aa0d-2b02e6c21757" />

---
<img width="1919" height="1023" alt="5 2" src="https://github.com/user-attachments/assets/2caf63d5-a1bb-4bab-a7b7-b80d223b2897" />

---
<img width="1919" height="1013" alt="5 3" src="https://github.com/user-attachments/assets/9013b2ad-811d-42bc-85d0-9f69c015cac7" />

---
<img width="1915" height="1019" alt="5 4" src="https://github.com/user-attachments/assets/4a7427eb-ddab-4ec6-9d2f-1f1bb7b95c70" />

---
<img width="1917" height="1017" alt="5 5" src="https://github.com/user-attachments/assets/ce988e1f-c206-4138-bb9c-5fb59447d9b1" />

---
<img width="1917" height="1018" alt="5 6" src="https://github.com/user-attachments/assets/fe4cd33c-576a-40d2-93b2-a4581af18022" />

---
<img width="1915" height="1020" alt="5 7" src="https://github.com/user-attachments/assets/7fb3eec6-02b8-4c29-a885-3cc1801124ff" />

---
<img width="1919" height="1019" alt="5 8" src="https://github.com/user-attachments/assets/098845f6-45d7-445b-9d7d-72d321a0ef09" />

---
<img width="1919" height="1016" alt="5 9" src="https://github.com/user-attachments/assets/d2adfdd4-bc77-41d4-9e45-8bc8b39008e8" />

---
<img width="1919" height="1018" alt="5 10" src="https://github.com/user-attachments/assets/c47f37f7-6e2c-460d-98d6-b25b3b12d6a8" />

---
<img width="1919" height="1013" alt="5 11" src="https://github.com/user-attachments/assets/240b805a-8be4-46ac-8a0a-8ed658b47d19" />

---
<img width="1919" height="1019" alt="5 12" src="https://github.com/user-attachments/assets/9fc1cf48-67a2-460b-b7ae-a35e92c989c4" />

---
<img width="1918" height="1018" alt="5 13" src="https://github.com/user-attachments/assets/b6d525dc-f901-4b58-ab8a-53a780d39ef2" />

---
<img width="1918" height="1010" alt="5 14" src="https://github.com/user-attachments/assets/16e41c9e-5390-457b-933a-b3ae2f8de081" />

---
<img width="1919" height="1017" alt="5 15" src="https://github.com/user-attachments/assets/b5bd117d-70ab-415e-9cc9-a9440d5df7c8" />

---

## 🗂️ Dataset

The dataset used is **Titanic (train.csv)** from [Kaggle Titanic Challenge](https://www.kaggle.com/c/titanic/data).  

Key features include:  
- `PassengerId` → Unique passenger identifier  
- `Survived` → Survival (0 = No, 1 = Yes)  
- `Pclass` → Passenger class (1st, 2nd, 3rd)  
- `Name`, `Sex`, `Age` → Demographics  
- `SibSp`, `Parch` → Family relations aboard  
- `Ticket`, `Fare` → Ticket and fare details  
- `Cabin`, `Embarked` → Boarding details  

📂 Files included:  
- `train.csv` → Titanic dataset  
- `Task-5 - Exploratory-Data-Analysis.ipynb` → Jupyter Notebook with EDA code   
- `README.md` → Project documentation  

---

## ⚙️ Tools
- **Python** (Pandas, NumPy)  
- **Matplotlib & Seaborn** (Data Visualization)  
- **Jupyter Notebook** (Interactive Analysis)  
- **GitHub** (Version control & submission)  

---

## 📂 Repository Structure  

- [Task-5 - Exploratory-Data-Analysis.ipynb](Task-5%20-%20Exploratory-Data-Analysis.ipynb) → Code implementation  
- [train.csv](train.csv) → Titanic dataset  
- [README.md](README.md) → Project details  

---
## 📊 Observations for Each Visual

**1. Correlation Heatmap**  
- Survival is negatively correlated with Pclass (-0.34) → higher class passengers had better survival.  
- Survival is positively correlated with Fare (+0.26) → wealthier passengers survived more.  
- Age shows a weak negative correlation with Survival (-0.08).  
- SibSp and Parch are weakly related to Survival individually.  

**2. Pairplot (Survived, Pclass, Age, Fare)**  
- Survivors cluster more in lower Pclass (1st class) and higher fares.  
- Age distribution overlaps between survivors and non-survivors, but more children are among survivors.  
- Strong separation seen in Fare and Pclass, weaker distinction in Age.  

**3. Histogram – Age**  
- Most passengers were 20–40 years old.  
- Fewer elderly (>60) and fewer very young children (<10).  
- Distribution is slightly right-skewed, concentrated around 20–30.  

**4. Histogram – Fare**  
- Majority of fares are below $50.  
- A few extreme outliers exist above $200, indicating wealthy passengers in 1st class.  
- Distribution is highly skewed to the right.  

**5. Survival by Sex**  
- Females had a much higher survival rate (~74%).  
- Males had very low survival (~19%).  
- Gender was a major determinant in survival outcomes.  

**6. Survival by Pclass**  
- 1st class passengers survived most (~63%), followed by 2nd class (~47%).  
- 3rd class had the lowest survival (~24%).  
- Socioeconomic status (ticket class) strongly influenced survival.  

**7. Boxplot – Age vs Survival**  
- Survivors’ median age is slightly lower than non-survivors.  
- Many children survived, while older passengers had lower survival.  
- Age alone is not a strong predictor but shows trends for children.  

**8. Scatterplot – Age vs Fare (colored by Survival)**  
- Survivors are concentrated at younger ages and higher fares.  
- Non-survivors dominate the cluster of low-fare, middle-aged passengers.  
- Few survivors paid very high fares, typically in 1st class.  

**9. Countplot – Survived**  
- About 62% of passengers did not survive.  
- Only ~38% survived.  
- Shows the overall imbalance between survivors and non-survivors.
---
## 📊 Key Insights & Findings

1. **Survival Rate**
   - Around **38% survived** while **62% did not survive**.

2. **Class Impact**
   - **Higher class passengers (Pclass 1)** had better survival chances.  
   - **Pclass 3** passengers had the lowest survival rate.

3. **Gender Impact**
   - **Females survived at much higher rates** than males (showing the "women and children first" pattern).

4. **Age Distribution**
   - Most passengers were aged between **20–40 years**.  
   - Children had relatively better survival chances compared to adults.

5. **Fare Distribution**
   - Fare is **right-skewed** (majority paid lower fares, few very high fares).  
   - Passengers who paid higher fares (often 1st class) had better survival rates.

6. **Correlation Analysis**
   - **Survival is positively correlated with Fare** and **negatively correlated with Pclass**.  
   - Age showed **weak correlation with survival**, but distribution differed slightly by survival outcome.

---

## 📜 Interview Preparation (EDA Q&A)

### 1️⃣ What is EDA and why is it important?  
EDA (Exploratory Data Analysis) is the process of analyzing datasets using **statistics and visualizations**.  
📌 **Importance**: detect missing values, outliers, correlations, and patterns; ensures clean and reliable data before modeling.  

---

### 2️⃣ Which plots do you use to check correlation?  
- Heatmap → for correlation matrix  
- Pairplot → pairwise variable relationships  
- Scatterplot → two continuous variables  
- Barplot/Boxplot → categorical vs continuous  

---

### 3️⃣ How do you handle skewed data?  
- Transformation → log, square root, Box-Cox  
- Binning → grouping values  
- Scaling → robust/standard scaling  
- Outlier handling → remove/cap extreme values  
- Non-parametric models → if skew remains  

---

### 4️⃣ How to detect multicollinearity?  
- Correlation matrix (|r| > 0.8 = high correlation)  
- Variance Inflation Factor (VIF > 5 or 10 = collinearity)  
- Condition Index / Eigenvalues  

---

### 5️⃣ What are univariate, bivariate, and multivariate analyses?  
- **Univariate** → 1 variable (e.g., histogram of Age)  
- **Bivariate** → 2 variables (e.g., Survival by Gender)  
- **Multivariate** → 3+ variables (e.g., Age, Class & Gender vs Survival)  

---

### 6️⃣ Difference between heatmap and pairplot?  
- Heatmap → correlation strength in matrix form  
- Pairplot → scatterplots for all variable pairs  

---

### 7️⃣ How do you summarize your insights?  
- Highlight **key findings** (e.g., “Females had higher survival rate than males”).  
- Use **visuals with short interpretations**.  
- Relate insights to **business context or problem statement**.  
- End with **actionable insights**.   

---

## 🚀 Outcome
By completing this project, I:  
- Gained **hands-on experience in EDA**.  
- Improved **data visualization and interpretation skills**.  
- Learned to convert **raw data → business insights**.  

---  
