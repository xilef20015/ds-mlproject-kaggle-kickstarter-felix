# Kickstarter Campaign Success Prediction

## Project Overview
This project develops machine learning models to predict the success of Kickstarter campaigns. It utilizes a logistic regression model as a baseline and an advanced RandomForest model to improve prediction accuracy. The data used includes various features related to the campaigns such as category, country, and amount pledged.

## Installation
To run this project, you need to have Python installed along with the following libraries:
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

You can install these packages using pip:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```
## Model Details

### Baseline Model
- **Model Type**: Logistic Regression
- **Performance Metrics**:
  - **Accuracy**: 87.6%
  - **Precision and Recall**: Detailed analysis for both successful and not successful campaigns shows the model's ability to identify true positives and true negatives effectively.

### Improved Model
- **Model Type**: RandomForest Classifier
- **Configuration**: The model was optimized using GridSearchCV with parameters for:
  - `n_estimators`: [50, 100, 200]
  - `max_depth`: [None, 10, 20, 30]
  - `min_samples_split`: [2, 5, 10]
- **Performance Metrics**:
  - **Accuracy**: 99.3%
  - **Precision and Recall**: The model demonstrates nearly perfect scores, highlighting its effectiveness in classifying both successful and not successful campaigns.

## Results

The RandomForest model significantly outperforms the baseline logistic regression model, achieving a 99.3% accuracy rate with nearly perfect precision and recall scores. This indicates a substantial improvement in identifying successful campaigns, underscoring the effectiveness of more complex ensemble methods over simpler models for this type of data.

The success of the RandomForest model in this context suggests that it is well-suited for handling the complexities and nuances of Kickstarter campaign data, which may involve intricate patterns not easily captured by simpler models like logistic regression.

