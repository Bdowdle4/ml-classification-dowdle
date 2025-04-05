# Dowdle's Module 4 Midterm Introduction
This project demonstrates a complete workflow for building a classification model using all numeric features. The notebook guides the user through the process from: exploration and data preprocessing, to model training and evaluation, to interpretation of the results. The goal is to accurately classify banknotes as authentic or forged based on their features and to identify the most significant predictors.
[Clickable link to notebook](https://github.com/Bdowdle4/ml-classification-dowdle/blob/main/classification_dowdle.ipynb)

****

## Dataset
[Clickable link to my data file](https://github.com/Bdowdle4/ml-classification-dowdle/blob/main/data/data_banknote_authentication.txt)

The dataset used in this project is the UCI Banknote Authentication Dataset. This dataset contains features extracted from images of banknotes, and it is used to classify the banknotes as genuine or forged. Key aspects of the dataset include:

>Features: The dataset includes features such as wavelet transformed coefficients that characterize the banknotes.
>
>Target Variable: A binary indicator showing whether a banknote is authentic or forged.
>
>Data Source: The dataset is publicly available from the UCI Machine Learning Repository and is widely used for binary classification tasks. [Original Dataset](https://archive.ics.uci.edu/dataset/267/banknote+authentication)

****

### Methodology
The notebook follows a structured approach:

>Data Exploration: Visualizing feature distributions and relationships. Identifying potential outliers and anomalies. Generating summary statistics to understand underlying data patterns.
>
>Data Preprocessing: Cleaning and preparing the dataset. Handling missing values, encoding variables, and scaling numerical features. Splitting the data into training and testing sets for model validation.
>
>Model Building: Testing multiple machine learning algorithms (logistic regression, decision trees, random forests) to determine the best performing classifier. Applying hyperparameter tuning to optimize model performance.
>
>Model Evaluation: Assessing models using metrics such as accuracy, precision, recall, F1-score, and confusion matrices. Comparing model performances to select the most robust approach.

### Feature Importance Analysis:
Determining the significance of each feature in the prediction process. Drawing insights about the predictors that most effect the classification outcome.

### Findings
The key takeaways from the project include:

>Data Insights: The exploration phase revealed interesting patterns within the dataset. Visualizations highlighted the distribution of the features and potential imbalances, providing insights that guided the preprocessing steps.
>
>Model Performance: Among the evaluated models, the best-performing classifier achieved high accuracy, indicating that the chosen features and preprocessing techniques were effective. Detailed metrics provided clarity on each model’s strengths and limitations.
>
>Feature Relevance: Analysis of feature importance underscored that certain wavelet coefficients had a significant impact on the model’s predictions, suggesting that these features are crucial for distinguishing between authentic and forged banknotes.

****

## Summary
Overall the classification approach was a success. The strengths of the best-performing model (Random Forest) are highlighted and the implications of the evaluation metrics are explained. I reviewed the importance of individual features, reinforcing how specific predictors contribute to the model’s ability to differentiate between authentic and forged banknotes. The limitations are acknowledged of the current approach, such as: potential overfitting or areas where additional feature engineering might be beneficial. Some suggestions for improvement are mentioned below.

As a requirement of this project, I also completed a [peer review](https://github.com/Bdowdle4/ml-classification-dowdle/blob/main/peer_review.md) of another classmates project. I chose a classmate that did a different dataset than myself. 

### Future Work:
* Exploring additional feature engineering techniques and advanced preprocessing methods.

* Testing a wider range of machine learning models or ensemble methods.

* Integrating cross-validation strategies for a more robust performance evaluation.

* Expanding the dataset or incorporating new data sources for a broader analysis.

****

## Instructions On How To Set Up Your Virtual Environment and Run Your Notebook Locally
### Virtual Enviornment Set Up (Windows Users)
**Task 1. Create .venv** Run the following command from the project root directory. Use PowerShell (not cmd):

```shell
py -m venv .venv
```

**Accept VS Code Suggestions** If VS Code asks: We noticed a new environment has been created. 
Do you want to select it for the workspace folder? Click Yes. 

**Task 2. Activate** Run the following command from the project root directory. Use Powershell:

```powershell
.venv\Scripts\activate
```

### Run Jupyter Notebook Locally
**Before Starting** Ensure the .venv is activated. If it is already active, you don't need to reactivate it.

**Install the Jupyter Extension for VS Code** Open the Extensions view in VS Code by pressing Ctrl+Shift+X (Windows). Search for "Jupyter" and install the official extension.

**Open the Notebook in VS Code** Open the notebook in VS Code. The file will have a .ipynb extension.

**Task 1. Select Notebook Kernel** Open the project notebook in VS Code. The file will have a .ipynb extension.
- If prompted, select a Python interpreter that corresponds to your .venv.  
- If not prompted, click the kernel selector in the top-right corner of the notebook editor and choose the interpreter associated with your Python Environment / .venv.
- Or:
   - From VS Code Menu, select View / Command Palette... (CTRL SHIFT P)
   - Type: Python: Select Interpreter 
   - Choose your .venv from the list

**Task 2. Start and Run a Jupyter Notebook** Open the project notebook in VS Code. The file will have a .ipynb extension.

1. Execute cells:  
   - Click on a cell and press Shift+Enter to execute it and move to the next cell.  
   - Alternatively, use Ctrl+Enter to execute the current cell without moving.

2. Save your notebook periodically to avoid losing progress. Or make sure the File / Autosave option is on.

**ALWAYS: Fully Execute Notebooks before add-commit-push** Keep your notebooks organized and execute them fully before running git add-commit-push to GitHub.

****

## Repository Checklist

Verify your repository contains:

- [x] Useful .gitignore (that keeps .venv out of GitHub)
- [x] Professional Jupyter Notebook with with proper name, numbered sections and reflections 
- [x] Useful README.md
- [x] Useful requirements.txt
- [x] Dataset, stored in a data folder
- [x] Peer Review (peer_review.md)
