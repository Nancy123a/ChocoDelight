### Overview and Problem Definition

ChocoDelight Factory, a leading chocolate bar manufacturer, aims to predict and prevent production line inefficiencies using data science to enhance operational efficiency, reduce costs, and maintain product quality.

### Data Columns Overview

- **Quality Metrics**: Cocoa_Roasting_Level, Texture_Smoothness, Sweetness_Level, Cocoa_Source_Check, Chocolate_Glossiness
- **Ingredient Metrics**: Sugar_Granularity, Milk_Solid_Percentage, Nuts_Inclusion_Rate, Flavor_Infusion
- **Packaging Metrics**: Seal_Integrity, Box_Dimensions, Label_Readability, Nutritional_Info_Accuracy
- **Testing Metrics**: Shelf_Life_Test, Barcode_Scan_Success

### Key Insights

1. **Cocoa_Roasting_Level & Sugar_Granularity**: Significant variability in Cocoa_Roasting_Level; consistent Sugar_Granularity.
2. **Consistent Metrics**: Symmetrical distributions in Cocoa_Source_Check, Sweetness_Level, and Texture_Smoothness.
3. **Milk_Solid_Percentage & Nuts_Inclusion_Rate**: Significant deviations in Milk_Solid_Percentage; consistent Nuts_Inclusion_Rate.
4. **Nutritional_Info_Accuracy**: High variability and longest whisker length.
5. **Box Dimension & Label Readability**: Larger deviations in Box Dimension and readability issues.

### Feature Importance and Model Optimization

- **PCA Findings**: 
  - PC1: Trade-off between sugar granularity, flavor infusion, and texture smoothness.
  - PC2: Contrasts milk solid percentage and shelf life with roasting levels.
  - PC4: Highlights nuts inclusion and box dimensions with label readability issues.

- **Logistic Regression**: 
  - PC4 has the highest positive coefficient, indicating strong influence on "not okay" status.

- **Handling Imbalanced Data**: 
  - Used SMOTE and Optuna for optimization.
  - **Cross-validation (4 folds)**:
    - Average Precision (Not Okay): 0.52
    - Average Recall (Not Okay): 0.53
    - Average F1-Score (Not Okay): 0.52

### Conclusion

Cross-validation outperformed Optuna optimization for predicting "Not Okay" status, making it the preferred model. Advanced data science techniques effectively predict and mitigate production issues, enhancing ChocoDelight Factory's efficiency and product quality.
