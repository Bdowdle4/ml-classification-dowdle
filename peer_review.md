# Applied Machine Learning Midterm Project - Nick Elias
**Author:** Brittany Dowdle  
**Date:** April 2, 2025

[Clickable Link to Notebook](https://github.com/NickElias01/midterm-applied-ml-nickelias/blob/main/mushrooms.ipynb)

****

### Clarity & Organization
The notebook is well-structured, following a clear progression from data loading to preprocessing, modeling, and evaluation. Clearly labeled sections make it easy to follow, with reflections after each major step. The introduction provides context, explaining the dataset and the importance of classification in this case. The only thing I would suggest is more visualizations. While textual analysis is clear, adding more visual aids would enhance interpretability.

### Feature Selection & Justification
The categorical features are properly encoded, ensuring that the model can interpret them. The feature selection is well-reasoned by choosing attributes with strong predictive power. The feature analysis done in section 2.3 provided justification for his selection. It doesn't seem like any unnecessary features are included. Identifying “perfect predictors” is a great approach, as it acknowledges features that may lead to overfitting. 

### Model Performance & Comparisons
While both Random Forest and Decision Tree models performed flawlessly, this outcome is likely due to the dataset’s inherent separability rather than model superiority. Further validation, such as testing with reduced features is recommended to confirm robustness beyond this specific dataset. Testing different hyperparameters could help determine whether the perfect accuracy is due to feature choice or model settings.

### Reflection Quality
Each reflection summarizes the outcomes and discusses the implications for model validation and the importance of cross-validation when confronted with unexpectedly perfect results. This level of detail shows that Nick critically evaluated the model performance and questioned whether the perfect accuracy was a sign of issues with the model. My favorite part of the reflections was pointing out that zero false negatives (no poisonous mushrooms were misclassified as edible) was critical for safety.