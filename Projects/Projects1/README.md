# Midterm Project: Data Storytelling – An End-to-End Machine Learning Investigation

## Overview
This project represents a complete machine learning investigation from data loading through model evaluation. The goal was not only to write code, but to become a *data storyteller*—to explore a dataset, uncover meaningful patterns, and communicate insights clearly. The assignment required applying concepts from Modules 1–10, including EDA, data preparation, feature engineering, modeling, and interpretation.

The project followed a structured workflow using the Titanic dataset, guiding the analysis through univariate, bivariate, and multivariate exploration before building and evaluating predictive models.


## Part 1: Dataset Selection and Initial Exploration
The Titanic dataset was selected and successfully loaded. Initial inspection included:

- Viewing the first and last rows  
- Checking dataset shape (891 rows × 12 columns)  
- Reviewing column descriptions  
- Splitting features into categorical and numerical groups  
- Confirming that all cells were populated (though not necessarily clean)

A gender distribution check revealed 577 males and 314 females.


## Part 2: Exploratory Data Analysis (EDA)

### **Univariate Analysis**
The dataset was explored feature by feature:

- Categorical variables were visualized to understand distribution and identify rare categories.
- Numerical variables were plotted, noting outliers and non-continuous values.
- Age groups were created using bins to better understand survival patterns.

### **Bivariate Analysis**
Relationships between pairs of variables were examined:

- **Sex vs. Survival** showed that women survived at much higher rates than men.
- **Passenger Class vs. Survival** revealed that first- and second-class passengers had significantly better outcomes.
- **Age vs. Class** and other combinations were visualized to understand deeper patterns.

### **Multivariate Analysis**
A correlation heatmap was generated to explore interactions across multiple variables. Key findings included:

- Strong negative correlation between being male and survival  
- Moderate correlation between passenger class and survival  
- Visualizations provided a far more intuitive understanding than raw numeric tables

### **Key EDA Insights**
- Women and children had the highest survival rates.
- Third-class passengers—especially men—had the lowest survival rates.
- Some personal assumptions (e.g., first-class men surviving at higher rates) were challenged by the data.


## Part 3: Data Preparation & Feature Engineering

### **Handling Missing Values**
- **Age** was imputed using the **median**, chosen because it is less sensitive to outliers.
- **Embarked** was filled using the **mode**.
- One-hot encoding was applied to the `Embarked` column using `pd.get_dummies()`.

### **Encoding Categorical Features**
- `Sex` was encoded using a binary map (`female = 0`, `male = 1`).
- One-hot encoding avoided multicollinearity and allowed the model to treat embarkation ports independently.


## Part 4: Modeling

### **Model 1: Logistic Regression (Baseline)**
- Achieved **81.01% accuracy**.
- Served as the baseline for comparison.

### **Model 2: Random Forest Classifier**
- Achieved **80.45% accuracy**.
- Although slightly lower in this dataset, Random Forests are generally more robust and capable of capturing complex patterns.

### **Model Comparison**
Both models performed similarly—likely due to the simplicity and size of the dataset. In more complex datasets, Random Forests typically outperform linear models.


## Part 5: Evaluation & Reflection

### **Classification Report (Random Forest)**
- Precision (class 1): **0.79**  
- Recall (class 1): **0.74**

**Interpretation:**
- Precision of 0.79 means that when the model predicted survival, it was correct 79% of the time.
- Recall of 0.74 means the model correctly identified 74% of actual survivors.

### **Confusion Matrix**

