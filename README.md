# Final Project: Regression Analysis
## Author and Resources

Author: Megan Chastain
Dataset: UCI Insurance Dataset
Jupyter Notebook: 

## 🚀 Project Setup
This project uses uv for dependency management and virtual environment creation. Follow these steps to set up your local development environment.
### Environment Setup
Run the following commands after cloning the repository to ensure all dependencies are installed correctly and the environment is managed by uv:
uv venv
uv python pin 3.12
uv sync --extra dev --extra docs --upgrade
uv run pre-commit install
uv run python --version


Activate Virtual Environment
You must activate the virtual environment before running any code or notebooks.
Windows (PowerShell):
.\.venv\Scripts\activate



### Opening Notebooks
Once the environment is active, run the following command to open the Jupyter interface in your browser:
jupyter notebooks


## ⚙️ Daily Workflow (Git)
Follow these steps for a standard development cycle:
Pull Changes: At the start of each working session, pull any changes from the remote repository:
git pull


Stage Changes: Use git add . to stage all local changes.
Commit Changes: Commit your staged changes with a descriptive message:
git commit -m 'message'


Push Changes: Push your committed changes to the GitHub repository:
git push -u origin main


## 📈 Analysis Outline
This project follows a standard machine learning workflow for building and evaluating a regression model on the UCI Insurance dataset.
1. Introduction and Project Goal
Start the project with a title and a brief introduction outlining the goal of predicting insurance charges.
2. Import and Inspect the Data
Load the dataset and display the first 10 rows to verify successful loading.
Check for missing values and display summary statistics (.info(), .describe()).
3. Data Exploration and Preparation
Explore data patterns, relationships, and distributions using visualizations.
Handle missing values and perform necessary data cleaning (e.g., encoding categorical variables).
Perform feature selection and engineering to prepare data for modeling.
Create new derived features as applicable (e.g., interaction terms, bins).
4. Feature Selection and Justification
Clearly define and justify the chosen features (X) and the target variable (y).
5. Train an Initial Model (Linear Regression)
Split the data into training and test sets using train_test_split (or StratifiedShuffleSplit if needed).
Train the initial model using the Scikit-Learn model.fit() method.
Evaluate performance using standard regression metrics (R2, MAE, RMSE).
6. Improve the Model or Try Alternates (Implement Pipelines)
Implement a robust Scikit-Learn Pipeline for data transformation and modeling (e.g., Imputer → StandardScaler → LinearRegression).
Explore alternative model types or use hyperparameter tuning.
Compare the performance of all tested models across the same set of performance metrics.
7. Final Thoughts & Insights
Summarize the final model's performance and explain the key findings and conclusions derived from the analysis.
