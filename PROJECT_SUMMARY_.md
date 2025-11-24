# Project Summary: Regression Analysis


## Problem Definition (Front Matter)

- Project Title: Regression
- Author/Alias: Megan Chastain
- Brief description of the business or analytical problem: Health data can be used to plan for future potential costs and predict how high or low costs could be.
- What decision or action the model is intended to support: The model is inteded to predict the cost of potential healthcare.
- Who would use this model: Insurance companies, hospitals, and researchers can use the model.


## 1. Target Variable

- Target variable name: Charges



## 2. Feature Review

- List of available features: age, bmi, smoker, children, region, sex, charges
- Any restricted or disallowed features: No
- Possible sources of target leakage: Based on the edited dataset, no.
- Example of potential leakage in this scenario: Actual insurance pay out effects actual charges.


## 3. Evaluation Metrics

- Primary metric chosen: I used R2, MAE, RSME
- Why this metric is appropriate: These metrics tell me if the model works with the data or if the data needs to be transformed.
- Brief discussion of these metrics: R2 describes overall model fit, closer to 1 the better the fit. MAE describes how close the predicted values are to the actual values, the lower the number the better. 




## 4. Data Splitting and Validation

- Method used (train/test split or cross-validation): Stratified split on log transfored charges feature to handle skewness
- Rationale for chosen method: The target feature is skewed
- Is time order relevant (yes/no): no
- If yes, how time-based splitting was handled:
- Possible leakage risks across splits (duplicates, identifiers, out-of-order events): Dupliccates are a risk.
- How these risks were mitigated: train_test_split handles this.


## 5. Real-World Impact

- Primary users or decision-makers for this model: Insurance companies, healthcare researchers.
- Action triggered by a positive prediction: Coverage of healthcare
- Consequences of false positives: Lack of coverage
- Consequences of false negatives: Lack of coverage
- Potential impact on people, decisions, or systems: Insureance companies can build plans that charge more because someone has a higher risk of garnering high healthcare costs.
- Any ethical concerns or additional safeguards: Denial of insurance coverage or plans that are too expensive for people with higher heatlh risks.


## 6. Final Notes

- Key limitations: Data is still skewed.
- Future improvements: Changing charges to be binary to test with different classifiers.
- Any open questions or assumptions: No
