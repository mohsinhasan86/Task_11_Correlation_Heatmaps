# Task 11 – Correlation & Heatmaps

## 📊 Project Overview

This project is part of the **PlaceMux Phase 1 – Data Analyst Industry Immersion Program**.

The objective of Task 11 is to quantify and visualize relationships between numeric variables in a retail sales dataset using **correlation analysis and a heatmap**.

## 🎯 Objective

* Calculate the correlation matrix for key numeric variables.
* Visualize correlations using a heatmap.
* Identify the strongest relationships between variables.
* Distinguish correlation from causation.
* Identify potential multicollinearity that may affect modelling.
* Summarize the relationships that are useful for business and analytical decisions.

## 🛠️ Tools & Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Google Colab

## 📁 Dataset

The analysis uses the cleaned retail sales dataset developed during the previous tasks of the PlaceMux Phase 1 project.

## 🔍 Numeric Variables Analyzed

The correlation analysis includes:

* Quantity
* Unit Price
* Discount %
* Gross Sales
* Discount Amount
* Net Sales

## 📈 Key Findings

### 1. Gross Sales and Net Sales

Correlation: **0.991**

There is an extremely strong positive relationship between Gross Sales and Net Sales. These variables contain very similar linear information.

### 2. Unit Price and Gross Sales

Correlation: **0.680**

A moderately strong positive relationship exists between unit price and gross sales.

### 3. Unit Price and Net Sales

Correlation: **0.673**

Unit price also shows a moderately strong positive relationship with net sales.

### 4. Discount % and Discount Amount

Correlation: **0.629**

A moderate positive relationship exists between discount percentage and the resulting discount amount.

### 5. Quantity and Gross Sales

Correlation: **0.624**

Quantity has a moderate positive relationship with gross sales.

### 6. Quantity and Net Sales

Correlation: **0.620**

Quantity also shows a moderate positive relationship with net sales.

### 7. Discount % and Net Sales

Correlation: **-0.246**

A weak-to-moderate negative relationship was observed between discount percentage and net sales.

### 8. Quantity and Unit Price

Correlation: **-0.030**

There is almost no linear relationship between quantity and unit price in this dataset.

## ⚠️ Modelling Consideration

The correlation of **0.991 between Gross Sales and Net Sales** indicates potential multicollinearity if both variables are used together as independent predictors in a model.

Correlation should not automatically be interpreted as causation. The relationships identified in this analysis describe statistical association, not proof that one variable causes another.

## 📊 Output

The main visual output of this task is:

**`Task_11_Correlation_Heatmap.png`**

The heatmap provides a visual representation of the strength and direction of correlations among the numeric variables.

## ✅ Conclusion

The correlation analysis highlights several meaningful relationships in the retail sales dataset. Gross Sales and Net Sales show an exceptionally strong relationship, while Unit Price and Quantity demonstrate moderate positive associations with sales measures. Discount Percentage has a negative relationship with Net Sales and a positive relationship with Discount Amount.

The analysis also identifies potential multicollinearity between Gross Sales and Net Sales, which should be considered when developing predictive models.

Overall, the heatmap provides a concise view of how the key numeric variables move together and helps identify relationships that deserve further investigation.
