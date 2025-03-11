# Supervised Learning 
## Project 1 (DataCamp) | Sowing Success: How Machine Learning Helps Farmers Select the Best Crops

![Unbenannt](https://github.com/user-attachments/assets/d3f6f2ca-471b-4f84-ac8f-51b95377d17a)

### Overview

In this project, a farmer has provided a dataset (`soil_measures.csv`) containing essential soil measurements:
- **N**: Nitrogen content ratio
- **P**: Phosphorous content ratio
- **K**: Potassium content ratio
- **pH**: pH value of the soil
- **crop**: The optimal crop for the field (target variable)

Our objective is to build multi-class classification models to predict the best crop for a field based on these soil measurements and to identify the single most important predictive feature.

### Project Details

- **Dataset:** `soil_measures.csv`
- **Target Variable:** `crop`
- **Features:** `N`, `P`, `K`, `pH`
- **Methodology:**
  - Perform exploratory data analysis (EDA) to ensure data quality.
  - Evaluate the predictive power of each soil measurement individually using both a simple train-test split and k-fold cross-validation.
  - Use metrics such as accuracy, precision (macro), recall (macro), and F1 scores (macro and weighted) to assess feature performance.
  - Visualize the results to compare how each feature performs.

### Code Structure

- `sowing_success.ipynb`: Contains the main code for loading data, evaluating each feature with both simple and cross-validation approaches, and visualizing the results.

## Key Findings

- **Single Feature Performance:**  
  Evaluation indicates that Potassium (K) is the strongest predictor among the individual soil measurements. However, even the best single feature achieves a mean accuracy of approximately 29%, suggesting that no single measurement is sufficient for robust prediction.

- **Next Steps:**  
  To improve predictive performance, a model that incorporates all soil features should be developed.
