# Lab 1
This folder contains my Lab 1 notebook and documentation.
# ✅ **Lab 1 – Machine Learning Workflow & Types of Learning**

## **Overview**
This lab introduced the complete end‑to‑end machine learning workflow using the Wine Classification dataset. I explored the three major types of machine learning (supervised, unsupervised, and reinforcement learning) and applied the supervised learning process to build and evaluate classification models. The lab walked through data exploration, preprocessing, model training, evaluation, and interpretation.

## **Objectives**
By completing this lab, I learned how to:

- Distinguish between **supervised**, **unsupervised**, and **reinforcement learning**
- Understand the **full ML workflow** from data → model → evaluation → insights
- Load and explore real datasets using pandas and scikit‑learn
- Perform **exploratory data analysis (EDA)** and visualize patterns
- Split data into training/testing sets
- Train and compare multiple classification models
- Interpret model performance using accuracy, classification reports, and confusion matrices
- Experiment with different feature selections to improve accuracy
- Understand how ML handles different **data types** (numerical, categorical, text, boolean)


## **Dataset Used**
**Wine Classification Dataset** from scikit‑learn  
- **178 samples**  
- **13 numerical features**  
- **3 wine classes**  
- No missing values  
- Ideal for practicing supervised classification  

## **What I Did in This Lab**

### ✅ **1. Reviewed Types of Machine Learning**
- **Supervised learning:** classification & regression  
- **Unsupervised learning:** clustering & dimensionality reduction  
- **Reinforcement learning:** agent learns through rewards  

### ✅ **2. Set Up the ML Environment**
Imported essential libraries:
- pandas, numpy, matplotlib, seaborn  
- scikit‑learn models & utilities  
- warnings suppression for cleaner output  

### ✅ **3. Loaded and Explored the Dataset**
- Converted the Wine dataset into a pandas DataFrame  
- Inspected shape, features, class distribution  
- Verified no missing values  
- Added readable class names  

### ✅ **4. Performed Exploratory Data Analysis (EDA)**
- Visualized class distribution  
- Generated correlation heatmaps  
- Identified relationships between features  

### ✅ **5. Followed the 6‑Step ML Workflow**
1. **Data Preparation** – selected features  
2. **Data Splitting** – 80% train / 20% test  
3. **Model Training** – Logistic Regression & Decision Tree  
4. **Model Evaluation** – accuracy, classification report  
5. **Model Interpretation** – confusion matrix  
6. **Insights** – compared model performance  

### ✅ **6. Compared Models**
- **Logistic Regression:** 88.9% accuracy  
- **Decision Tree:** 83.3% accuracy  
- **Best Model:** Logistic Regression  

### ✅ **7. Experimented With New Features**
I selected:
```
['alcohol', 'hue', 'proline']
```
This improved accuracy to **97.2%**, outperforming the original model.

### ✅ **8. Completed Concept Assessments**
- Identified ML types for real‑world scenarios  
- Scored 5/5 on the conceptual quiz  


## **Key Learnings**
- The ML workflow is structured and repeatable  
- Feature selection can dramatically improve model performance  
- EDA is essential for understanding data before modeling  
- Confusion matrices provide deeper insight than accuracy alone  
- Different data types require different preprocessing techniques  


## **Challenges I Faced**
- Choosing the right subset of features for improved accuracy  
- Interpreting correlations and understanding which features matter  
- Understanding how model depth affects Decision Tree performance  


## **Reflection**
**Best performing model:** Logistic Regression  
**Why it performed best:**  
It generalized better across all classes and handled the selected numerical features more effectively than the Decision Tree, which was more sensitive to depth and potential overfitting.

**Next steps to improve performance:**  
- Try scaling features  
- Test additional algorithms (Random Forest, SVM, KNN)  
- Use all 13 features with feature engineering  
- Tune hyperparameters  


## **Files Included**
- `Lab_3_Mary_Ann_Mastri_Module_03_Lab_Exercise.ipynb` 
- `README.md` (this file)

---

## **Summary**
This lab provided a complete walkthrough of the machine learning workflow, from understanding ML types to building and evaluating classification models. It strengthened my understanding of supervised learning and gave me hands‑on experience with real data, model comparison, and performance interpretation.
