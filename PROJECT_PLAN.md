# Project Plan: Vancouver Business Heritage Proximity Predictor

A machine learning project to predict whether a Vancouver business is located near a heritage site.

## Task 1: Data Collection and Acquisition

- Obtain Vancouver business license dataset from City of Vancouver Open Data Portal
- Obtain heritage sites dataset (heritage buildings, landmarks, heritage conservation areas)
- Collect geographic coordinates (latitude/longitude) for both datasets
- Document data sources, licensing, and any access limitations

## Task 2: Data Preprocessing and Feature Engineering

- Clean and standardize business data (handle missing values, normalize addresses)
- Clean and standardize heritage site data
- Geocode any addresses missing coordinates
- Calculate distance-based features (distance to nearest heritage site, count of heritage sites within radius)
- Create the target variable: binary label indicating "near heritage site" (define threshold, e.g., within 500m)
- Merge datasets and create final feature matrix

## Task 3: Exploratory Data Analysis

- Analyze distribution of businesses across Vancouver neighborhoods
- Map heritage site locations and business density
- Visualize relationship between business types and heritage proximity
- Identify potential predictive features (business type, neighborhood, year established)
- Check for class imbalance in the target variable

## Task 4: Model Development and Training

- Split data into training, validation, and test sets
- Establish baseline model (e.g., logistic regression)
- Train and compare multiple classifiers (Random Forest, XGBoost, Neural Network)
- Perform hyperparameter tuning using cross-validation
- Evaluate models using appropriate metrics (accuracy, precision, recall, F1, AUC-ROC)
- Address class imbalance if present (SMOTE, class weights, or threshold adjustment)

## Task 5: Model Evaluation and Documentation

- Evaluate final model on held-out test set
- Analyze feature importance and model interpretability
- Create visualizations of model predictions on Vancouver map
- Document methodology, results, and limitations
- Prepare reproducible pipeline (scripts, requirements.txt, README)
