# Benchmarking Classification Algorithms: A Marketing Use Case

**Overview**  
In this project, we benchmark the performance of four popular classification algorithms:  
- **K-Nearest Neighbors (KNN)**  
- **Logistic Regression**  
- **Decision Trees**  
- **Support Vector Machines (SVM)**

The evaluation is conducted using a dataset derived from **telephone marketing campaigns for bank products**.  
Our comparison focuses on key metrics such as:
- **Training Time**
- **Training Accuracy**
- **Testing Accuracy**

---

## Dataset

The dataset is sourced from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/bank+marketing), collected by a Portuguese banking institution. It consists of results from 17 different direct marketing campaigns.

Further details can be found in the accompanying paper: `CRISP-DM-BANK.pdf`.

---

## Project Workflow

1. **Data Preprocessing**
2. **Exploratory Data Analysis**
3. **Model Training & Evaluation**
4. **Comparison of Classifiers**

Link to the notebook: https://github.com/amiteshks/comparing_classifiers/blob/main/comparing-classifiers.ipynb

---

## Conclusion and Summary
### Conclusion

All four classifiers—**K-Nearest Neighbors (KNN)**, **Logistic Regression**, **Decision Trees**, and **Support Vector Machine (SVM)**—achieved perfect training accuracy, indicating that each model fit the training data exceptionally well. However, differences in test accuracy and training time reveal key trade-offs:

## Model Comparison Results

| Model Name              | Train Time (s) | Train Accuracy | Test Accuracy |
|------------------------|----------------|----------------|---------------|
| KNN                    | 12.19          | 1.00           | 0.9001        |
| Logistic Regression    | 2.23           | 1.00           | 0.9094        |
| Decision Trees         | 2.72           | 1.00           | 0.9129        |
| Support Vector Machine | 1016.92        | 1.00           | 0.8990        |


- **Decision Trees** delivered the **highest test accuracy (91.29%)** with a **relatively low training time (2.72 seconds)**, making it the most balanced and efficient model in this comparison.
- **Logistic Regression** followed closely with **90.94% test accuracy** and the **fastest training time (2.23 seconds)**, offering excellent performance with minimal computational cost.
- **KNN**, while also quick to train, had a slightly lower test accuracy (**90.01%**), suggesting it may be more sensitive to data complexity.
- **Support Vector Machine (SVM)** had the **longest training time (over 1000 seconds)** and the **lowest test accuracy (89.90%)**, indicating it is less efficient and may be overfitting or less suited to this dataset.

---

### Summary

**Decision Trees** and **Logistic Regression** stand out as the most effective classifiers for this task, offering a strong balance between accuracy and computational efficiency.

