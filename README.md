# Predicting Elevated Systolic Blood Pressure Using Machine Learning

## Project Overview

This project explores the use of Python and machine learning to classify individuals according to whether their systolic blood pressure (SBP) is elevated based on a defined threshold.

The project was completed as part of my data analysis and machine learning learning journey. It involved exploring a health-related dataset, preparing the data, training classification models, and evaluating their performance.

The primary objective was to understand how different machine learning algorithms perform on a classification problem and how evaluation metrics can help reveal the strengths and limitations of each model.

## Project Objectives

- Explore and understand the structure and characteristics of the dataset.
- Identify missing values, distributions, potential outliers, and relationships between variables.
- Prepare the data for machine learning.
- Train and compare multiple classification algorithms.
- Evaluate model performance using appropriate classification metrics.
- Interpret the results and identify limitations, particularly in the presence of imbalanced classes.

## Tools and Technologies

- **Python** — programming and analysis
- **Pandas** — data manipulation and analysis
- **NumPy** — numerical operations
- **Matplotlib and Seaborn** — data visualization
- **Scikit-learn** — preprocessing, model training, cross-validation, and evaluation
- **Jupyter Notebook** — interactive development and documentation

## Project Workflow

### 1. Exploratory Data Analysis (EDA)

I explored the dataset to understand its structure, variable distributions, missing values, and relationships between features.

The exploratory analysis included:
- Summary statistics and data inspection
- Histograms to examine distributions
- Boxplots to investigate potential outliers
- Correlation analysis
- Pairplots to explore relationships between selected variables
- A missing-value heatmap

### 2. Data Preparation

The data preparation stage included examining missing values and using median imputation for missing numerical values.

The data was then prepared for model training, including splitting it into training and testing sets. Feature scaling was applied where appropriate for algorithms that are sensitive to differences in feature scales.

### 3. Machine Learning Models

Four classification algorithms were trained and evaluated:

- Logistic Regression
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)
- Random Forest Classifier

### 4. Model Evaluation

The models were assessed using several evaluation methods and metrics:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Specificity
- Five-fold cross-validation
- ROC curve comparison

These metrics were used to examine model performance from different perspectives rather than relying on accuracy alone.

## Key Findings

The dataset contained 4,999 observations, with 250 positive cases for the target classification, representing approximately 5% of the observations.

The Random Forest model achieved a test ROC-AUC of approximately **0.806**, while its mean ROC-AUC across five-fold cross-validation was approximately **0.780**.

However, the models showed very low recall for the positive class, with Random Forest identifying only around 4% of the positive cases in the test evaluation.

This highlights an important lesson: **high accuracy does not necessarily mean a model performs well at identifying the cases we care about.**

Because the classes were imbalanced, accuracy alone was insufficient to assess model usefulness. Recall, precision, F1-score, ROC-AUC, and the confusion matrix are important for understanding the model's limitations.

## Skills Demonstrated

Through this project, I practised:

- Exploratory data analysis
- Data cleaning and missing-value treatment
- Data visualization and correlation analysis
- Feature preparation and scaling
- Classification model development
- Model comparison and evaluation
- Cross-validation
- Interpreting machine learning results
- Communicating findings and acknowledging analytical limitations

## Limitations and Responsible Use

This project is educational and demonstrates a machine learning workflow. It is **not a clinically validated diagnostic or prediction tool**.

The low recall for positive cases indicates that the evaluated models missed many positive observations. Further investigation, appropriate validation, and careful consideration of class imbalance would be necessary before considering any practical application.

The classification threshold used in this project should also not be interpreted as a universal clinical definition of hypertension.

The dataset is not included in this repository. Access to the data and permission to share it must be confirmed before it is distributed.

## Repository Contents

- `MEDIACREST FINAL PROJECT.ipynb` — Jupyter Notebook containing the analysis, visualizations, model training, and evaluation.

Additional project files may be added as the repository develops.

## Conclusion

This project strengthened my understanding of the machine learning workflow, from exploratory data analysis and data preparation to model evaluation and interpretation.

One of my key takeaways was the importance of selecting evaluation metrics that reflect the actual problem being solved. In imbalanced classification, a model's ability to identify positive cases can be more informative than accuracy alone.

I look forward to continuing to develop my skills in Python, data analysis, and machine learning through practical projects.

---

**Project type:** Educational Data Analysis and Machine Learning

**Focus:** Health-related classification, exploratory data analysis, and model evaluation
