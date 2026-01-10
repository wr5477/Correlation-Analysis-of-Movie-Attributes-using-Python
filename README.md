# 🎬 Movie Correlation Project

## 📌 Project Overview
This project explores the relationships between various movie attributes—such as budget, gross earnings, ratings, runtime, and categorical features—to identify which factors are most strongly correlated with a movie’s financial success.

The analysis focuses on data cleaning, preprocessing, encoding categorical variables, and correlation analysis using Python.

---

## 📊 Dataset
- **Source:** Kaggle  
- **Link:** https://www.kaggle.com/datasets/danielgrijalvas/movies  

The dataset contains information on thousands of movies, including:
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
Key preprocessing steps include:
- Removing rows with missing critical values
- Standardizing the `released` column by removing country information and converting mixed date formats into datetime objects
- Converting numeric columns such as `votes` and `runtime` from floats to integers
- Creating a corrected release year (`Year_correct`) from the release date
- Identifying inconsistencies between the original `year` column and parsed release year
- Encoding categorical variables using category codes for correlation analysis

---

## 📈 Correlation Analysis
- Pearson correlation was applied to numeric features
- Categorical variables were encoded to enable exploratory correlation analysis
- A correlation matrix and visualizations were used to identify strong relationships between variables

**Key Insight:**  
Movies with higher budgets tend to generate higher gross earnings, showing the strongest positive correlation in the dataset.

---

## 📚 Reference
This project was inspired by the following YouTube course, with independent implementation and customization:

- **YouTube Course:**  
  https://www.youtube.com/watch?v=iPYVYBtUTyE&list=PLUaB-1hjhk8H48Pj32z4GZgGWyylqv85f&index=4
