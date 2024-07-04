### Project Overview: Predicting Production Line Issues at ChocoDelight Factory

**Objective:**
The primary goal of this project is to predict potential production issues in the ChocoDelight Factory's chocolate production line, understand the variables leading to these problems, and quantify savings in rework time and costs using causal inference. The findings will be displayed in an interactive dashboard for easy interpretation and decision-making.

### Data Preprocessing

1. **Handle Missing Values:**
   - Identify and impute or remove missing values to ensure dataset completeness.
2. **Rectify Outliers or Anomalies:**
   - Detect and treat outliers to avoid skewed analysis and model predictions.
3. **Standardize/Normalize Measurements:**
   - Standardize/normalize numerical measurements to ensure uniform scale across all features.

### Exploratory Data Analysis (EDA)

1. **Distribution Analysis:**
   - Analyze the distribution of measurements for each station to understand the central tendencies and variances.
2. **Pattern Identification:**
   - Identify patterns and trends in the "not okay" instances to understand common failure points.
3. **Correlation Analysis:**
   - Determine correlations between different stations to identify interdependencies and potential cascading effects of failures.

### Feature Importance Analysis

1. **Feature Selection:**
   - Use techniques such as recursive feature elimination or permutation importance to determine the most influential features.
2. **Visualization:**
   - Visualize the relative importance of top features to understand their impact on the production line's performance.

### Predictive Modeling

1. **Model Development:**
   - Develop a machine learning model to predict "not okay" situations using the identified features.
2. **Model Assessment:**
   - Assess model performance using metrics like accuracy, precision, recall, and F1-score.
3. **Model Refinement:**
   - Refine the model for optimal performance, focusing on explainability to ensure the results are interpretable by stakeholders.

### Causal Inference

1. **Rework Data Analysis:**
   - Analyze the ‘rework_data’ to understand the relationship between production issues and rework time and costs.
2. **Scenario Simulation:**
   - Simulate various scenarios to determine how changes in key features can lead to savings in rework time and costs.
   - Example: Analyze the impact of improving the Cocoa_Roasting_Level on reducing rework costs and time.

### Dashboard Development

1. **Interactive Dashboard:**
   - Design an interactive dashboard using PowerBI
