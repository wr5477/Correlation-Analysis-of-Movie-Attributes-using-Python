# 🎬 Correlation Analysis of Movie Attributes using Python
<img width="1800" height="400" alt="image" src="https://github.com/user-attachments/assets/beba8f13-b6be-4e87-a18a-06ae1c71c604" />


## 📌 Project Overview
This project explores the relationships between various movie attributes—such as budget, gross revenue, ratings, runtime, and release year—to identify which factors are most strongly associated with a movie’s financial success.

The analysis focuses on **data cleaning, preprocessing, categorical encoding, and correlation analysis** using Python, with an emphasis on understanding how different features interact rather than building predictive models.

---

## 📊 Dataset
**Source:** Kaggle  
https://www.kaggle.com/datasets/danielgrijalvas/movies

**Dataset includes**
- Movie title, genre, director, writer, and main actors  
- Release year and release date  
- Budget and gross revenue  
- Ratings, votes, runtime, and production company  

---

## 🎯 Objectives
- Clean and standardize raw movie data  
- Handle missing values and inconsistent date formats  
- Convert categorical variables into numeric representations  
- Analyze correlations between numeric features  
- Identify which factors are most associated with gross earnings  

---

## 🛠️ Tools & Libraries
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Jupyter Notebook  

---

## 🧹 Data Cleaning & Preprocessing
Before analysis, several preprocessing steps were performed to ensure data consistency and reliability:

- Removed rows with missing critical values (e.g., budget, gross revenue)  
- Standardized the `released` column by removing country information and converting mixed date formats into datetime objects  
- Converted numeric columns such as `votes` and `runtime` from floats to integers  
- Created a corrected release year (`Year_correct`) from the parsed release date  
- Identified inconsistencies between the original `year` column and the corrected release year  
- Encoded categorical variables using category codes to enable correlation analysis  

These steps ensured that both numeric and categorical features could be meaningfully compared.

---

## 📈 Exploratory & Correlation Analysis

### Budget vs. Gross Revenue
The scatter plot below shows the relationship between movie budgets and gross earnings, along with a fitted trend line.

<img width="1002" height="695" alt="image" src="https://github.com/user-attachments/assets/c31e2da7-1719-4958-88cc-f6d0597d0073" />


A clear positive trend is observed, indicating that movies with higher budgets tend to generate higher gross revenue, although variance increases significantly at higher budget levels.

---

### Correlation Matrix (Numeric Features)
A Pearson correlation matrix was used to examine relationships among key numeric variables.

<img width="917" height="703" alt="image" src="https://github.com/user-attachments/assets/501ce0f7-8caf-40b3-813e-6a5d1b8076af" />


Key observations:
- **Budget and gross revenue** show a strong positive correlation  
- **Votes** are highly correlated with gross revenue, suggesting audience reach plays an important role  
- Ratings have a weaker direct relationship with revenue compared to budget and votes  

---

### Correlation Including Encoded Categorical Features
Categorical variables were encoded to explore broader relationships across all features.

<img width="1000" height="774" alt="image" src="https://github.com/user-attachments/assets/e1cb4344-bde8-4877-9d57-9bd4139adc05" />


While correlations involving encoded categorical variables should be interpreted cautiously, this step provides exploratory insight into how production-related attributes may relate to financial performance.

---

## 🎯 Key Insight
Among all examined features, **budget shows the strongest positive correlation with gross revenue**, indicating that higher production investment is closely associated with higher box office returns.  
Audience engagement (measured by votes) also plays a significant role in revenue outcomes.

---

## 📚 Reference
This project was inspired by a Python-based data analysis tutorial and was independently implemented with customized preprocessing, analysis logic, and visualizations.

YouTube Reference:  
https://www.youtube.com/watch?v=iPYVYBtUTyE&list=PLUaB-1hjhk8H48Pj32z4GZgGWyylqv85f&index=4
