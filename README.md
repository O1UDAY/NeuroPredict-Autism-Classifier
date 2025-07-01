Autism Prediction Using Machine Learning
Overview
This project demonstrates a machine learning pipeline for predicting Autism Spectrum Disorder (ASD) using structured survey data. As a student passionate about the intersection of healthcare and data science, I designed this notebook to showcase both my technical skills and my commitment to building impactful, real-world solutions. The project follows best practices in data preprocessing, model selection, and evaluation, using Python and popular data science libraries.

Problem Statement
Early detection of ASD is crucial for timely intervention and support. The goal of this project is to build a robust classifier that can predict the likelihood of ASD based on responses to a set of behavioral and demographic questions.

Dataset
Source: Survey data with 800 samples and 22 features, including behavioral scores (A1–A10), age, gender, ethnicity, medical history (jaundice, autism), country, and more.

Target: Class/ASD (1 = ASD, 0 = Non-ASD)

Class Distribution: The dataset is imbalanced, with more non-ASD cases than ASD cases.

Project Workflow
1. Data Exploration & Preprocessing
Loaded and inspected the data for missing values and inconsistencies.

Label encoding was applied to categorical features for compatibility with machine learning models.

Used SMOTE (Synthetic Minority Over-sampling Technique) to address class imbalance and ensure fair model training.

2. Feature Selection
Explored feature distributions and correlations to understand which attributes are most predictive.

3. Model Building & Tuning
Implemented several classifiers:

Decision Tree

Random Forest

XGBoost (Extreme Gradient Boosting)

Performed hyperparameter tuning with RandomizedSearchCV for XGBoost to optimize model performance.

4. Evaluation
Used accuracy score, confusion matrix, and classification report (precision, recall, F1-score) to evaluate models.

Cross-validation ensured the results are generalizable and not overfitted to the training data.

5. Model Saving
The best-performing model was serialized using pickle for easy deployment or further use.

Results
XGBoost emerged as the top performer after hyperparameter tuning, balancing both precision and recall for ASD detection.

The model is robust to imbalanced classes thanks to SMOTE and careful validation.

Why This Project Matters
Human Impact: Early ASD detection can change lives. This project is a step toward accessible, data-driven screening tools.

Technical Breadth: The notebook demonstrates proficiency in data wrangling, visualization, model selection, and validation.

Industry Relevance: The workflow mirrors real-world data science practices, from problem framing to model deployment.

How to Run
Clone the repository and ensure you have Python 3.x installed.

Install dependencies:

bash
pip install -r requirements.txt
Run the Jupyter notebook:

bash
jupyter notebook Autism_Preidiction_using_machine_Learning-2.ipynb
The notebook is annotated for clarity, so you can follow each step from data loading to final prediction.
