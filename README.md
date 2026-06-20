# House-Price-Predictor-Machine-Learning-model-using-LR.
California House Price Prediction 🏡📉An end-to-end machine learning project that predicts median house values in California using a Random Forest Regressor pipeline. This project focuses on data preprocessing, feature engineering, and model evaluation following the NeuralNine implementation framework.

🚀 Project OverviewPredicting housing prices is a classic regression problem. Using the California Housing dataset, this project builds a complete data science workflow in a Jupyter Notebook to clean data, engineer spatial metrics, handle distribution skews, and deploy an ensemble learning model.

📊 Dataset FeaturesThe model utilizes the following structural attributes of California blocks:longitude / latitude (Geographic positioning)housing_median_age (Median age of houses in the block)total_rooms / total_bedrooms (Aggregated structural sizes)population / households (Demographic metrics)median_income (Median income for households in tens of thousands of USD)ocean_proximity (Categorical proximity to the coast)Target Variable: median_house_value 

🛠️ Key Pipeline StepsData Cleaning: Handled missing data points within the bedroom features.Exploratory Data Analysis (EDA): Visualized feature distributions and cross-correlations using seaborn heatmaps.Feature Engineering:Applied log1p transformations to fix highly skewed demographic data.Encoded categorical ocean_proximity values via One-Hot Encoding.Derived high-utility metrics: bedroom_ratio and household_rooms.Data Isolation: Implemented a clean pipeline architecture to apply training transformations to the test set independently, strictly preventing data leakage.Model Training: Fitted a RandomForestRegressor and evaluated performance using R-squared statistics.

💻 Tech Stack & LibrariesLanguage: Python 3Environment: Jupyter NotebookLibraries: pandas, numpy, matplotlib, seaborn, scikit-learn

📈 Key FindingsPrimary Drivers: median_income and coastal geographical proximity (INLAND vs NEAR OCEAN) maintain the strongest predictive weights.Feature Scaling: Log transformations on population data significantly reduced noise and improved prediction accuracy across sparse structural subsets.
