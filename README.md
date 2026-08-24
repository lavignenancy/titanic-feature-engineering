## Project Overview
This project delivers a methodical data science pipeline using the Titanic dataset. Instead of relying on generic shortcuts, the workflow focuses on rigorous data cleaning, structured title-based data imputation, manual historical verification, and an evaluation of categorical encoding techniques on a baseline Logistic Regression model.

## Key Technical Features and Accomplishments

### 1. Rigorous Data Cleaning and Structural Auditing
* Data Type Profiling: Conducted thorough missing value diagnostics across categorical and numerical feature blocks to preempt pipeline breaking.
* Title Based Granular Imputation: Avoided damaging data distributions by building targeted name mask filters to compute separate age averages for Master, Mister, and Miss passenger classes.
* Historical Data Verification: Leveraged external historical records from the Mrs. George Nelson Stone Biography Page to manually fix missing entry data with ground truth facts.

### 2. Strategic Feature Engineering
* Dimensionality Selection: Handled high cardinality noise and potential overfit triggers by cleanly removing text tracking identifier fields like PassengerId, Name, and Ticket.
* Comparative Categorical Encoding: Built and evaluated two independent data vectorization methods, comparing Label Encoding against One-Hot Encoding.

### 3. Model Training and Diagnostics
* Baseline Classification: Implemented a binary classification framework using a Scikit-Learn Logistic Regression pipeline scaled to a 500-iteration cap.
* Leakage Discovery: Successfully highlighted a diagnostic baseline optimization opportunity due to perfect dataset split evaluation scores showing an accuracy of 1.0.

## Pipeline Roadmap and Progress Tracker
* Finished initial data integrity profile and audit.
* Finished advanced title-based context imputation.
* Finished baseline vectorization and training pipelines.
* Planned implementation of a cross-validation matrix to address leakage and overfitting.
* Planned deployment of advanced trees and boosting algorithms such as Random Forest and XGBoost.
* Planned feature importance interpretation and visualizations.

## Technologies and Libraries Used
* Languages: Python 3
* Data Core: Pandas, NumPy
* Machine Learning: Scikit-Learn
* Visualization: Matplotlib

## Project Structure
* tested.csv: Raw historical source data
* feature_engineering.ipynb: Interactive analysis pipeline notebook
* README.md: Professional project documentation

## How to Run the Pipeline
1. Clone this repository to your machine.
2. Ensure you have your dependencies installed using pip install pandas numpy scikit-learn matplotlib.
3. Boot up JupyterLab or Jupyter Notebook.
4. Run all cells in feature_engineering.ipynb to recreate the feature transformation stages.
