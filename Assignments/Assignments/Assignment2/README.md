# Assignment 2 – Exploratory Data Analysis (EDA) Workflow

## Overview
This assignment focused on performing a full exploratory data analysis (EDA) on a dataset by examining its structure, understanding its variables, and analyzing relationships across categorical and numerical features. The goal was to apply a systematic approach to univariate, bivariate, and multivariate analysis to better understand the data before modeling.


## Data Inspection and Structure
The analysis began by loading the dataset and reviewing its basic structure:

- Displayed the number of rows and columns  
- Viewed the first and last few records  
- Examined the dataset’s shape  
- Split features into **categorical** and **numerical** groups  
- Verified that the dataset contained **no null values** (all cells populated)

Although no missing values were present, the dataset still required deeper inspection to identify inconsistencies, outliers, or unusual patterns.


## Univariate Analysis
Univariate analysis was performed separately for categorical and numerical features.

### **Categorical Features**
- Category distributions were plotted to understand frequency patterns  
- Rare categories with very small counts were grouped together or flagged for exclusion  
- Repeated visualizations helped identify which categories were meaningful and which added noise  

### **Numerical Features**
- Numerical variables were plotted individually  
- Some numerical features behaved more like discrete categories  
- Outliers were identified but not immediately removed until their impact was better understood  
- Each numerical feature was analyzed until all variables were explored

This phase helped establish a baseline understanding of the dataset’s composition.


## Bivariate Analysis
Next, the analysis explored relationships between pairs of variables.

### **Categorical vs. Categorical**
- Cross‑tabulations and visual comparisons were used  
- Some variable pairs showed strong relationships  
- Others showed little to no interaction  

### **Numerical vs. Numerical**
- Scatterplots and correlation checks were used  
- Certain numerical features demonstrated meaningful influence on each other  
- Others were independent and contributed little to shared variance  

This step helped identify which variables might be useful predictors or redundant.


## Multivariate Analysis
The final stage involved examining how **multiple variables interact simultaneously**.

- Correlation heatmaps were generated to visualize relationships across all features  
- High‑correlation pairs were identified  
- Weak or irrelevant relationships were also noted  
- Multiple graph types were used to provide different perspectives on the data  

This multivariate approach offered a more intuitive and visual understanding of the dataset compared to traditional spreadsheet‑based analysis. The graphical output made it far easier to interpret patterns than manually reviewing numerical correlation tables.


## Key Takeaways
- The dataset was complete but required careful inspection to understand category distributions and outliers  
- Univariate analysis provided foundational insight into each variable  
- Bivariate analysis revealed which variables influenced each other  
- Multivariate analysis highlighted
