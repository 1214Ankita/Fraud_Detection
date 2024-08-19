# Fraud_Detection

### Objective: 
Build a fraud detection model using a RandomForestClassifier to classify transactions as fraudulent or legitimate.

### Steps:
#### Loading Data
    Load a CSV dataset containing transaction records.
    
#### Basic Analysis
    Display dataset dimensions, basic statistics, and correlation matrix.
    Visualize the distribution of fraud and non-fraud transactions.

#### Preprocessing
    Handle multicollinearity by combining and dropping highly correlated features.
    Create new features based on existing ones, e.g., actual_amt_orig and actual_amt_dest.
    Encode categorical variables and drop zero variance and irrelevant features.
    Visualize the distribution of transaction types and receiver/payer types.

#### Model Building
    Prepare the dataset for modeling by separating features and target variable (isFraud).
    Split the data into training and testing sets.
    Train a RandomForestClassifier with balanced class weights and entropy criterion.
    
#### Evaluation
    Predict fraud labels on the test set, adjusting predictions for transactions above a certain amount.
    Evaluate model performance using classification report, confusion matrix, and ROC curve.

### Model Insights:
The RandomForestClassifier is tuned to handle class imbalance and predict fraudulent transactions effectively.
Additional adjustments include handling high-value transactions explicitly to ensure accurate fraud detection.
