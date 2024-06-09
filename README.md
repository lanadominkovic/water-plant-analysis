## Enhancing Wastewater Treatment: A Machine Learning Approach

### Overview
This project introduces a Random Forest (RF) model aimed at predicting operational costs (OCI) and effluent quality (EQI) in wastewater treatment plants (WWTPs). The model not only excels in predictive accuracy but also provides comprehensive insights into the variables that impact the effectiveness and economic efficiency of WWTPs.

### Key Results
- **Effluent Quality Index (EQI):**
  - **Training R²:** 0.987
  - **Validation R²:** 0.911
  - **Test R²:** 0.915
- **Operational Cost Index (OCI):**
  - **Training R²:** 0.994
  - **Validation R²:** 0.956
  - **Test R²:** 0.957

These results demonstrate the model's strong predictive performance and generalizability, capturing over 90% of the variation in the data.

### Methodology
- **Data Source:** Benchmark simulation model of the WWTP
- **Data Points:** 8736 hourly averaged data points from a year's worth of 15-minute interval data
- **Modeling Approach:** 
  - Time delays ranging from 0 to 15 hours were introduced to account for potential delayed effects on EQI and OCI.
  - The RF model was trained, validated, and tested on randomly split datasets (90% training, 10% testing).

### Interpretability
- **Feature Importance:** Analyzed using SHAP (Shapley Additive Explanations) values to ensure transparency and understand the impact of various input variables.
- **Top Influential Features for EQI:** Wastewater temperature, influent flow rate, influent COD, NH4, TN, TSS, and control variables like Qintr and DO6.
- **Top Influential Features for OCI:** Influents such as flow rate, COD, NH4, TN, TSS, and control variables including Quprimary, Qw, and DO6.

### Conclusion
The model's robust performance in predicting EQI and OCI, coupled with its explainability through SHAP values, makes it a valuable tool for optimizing WWTP operations. This study's novel contributions include plant-wide consideration of operations, composite criteria for both EQI and OCI, and the use of interpretable machine learning models.

### References
- Breiman, L. (2001). "Random Forests," Machine Learning, 45(1), 5-32.
- Lundberg, S. M., & Lee, S. I. (2017). "A Unified Approach to Interpreting Model Predictions," Proceedings of the 31st International Conference on Neural Information Processing Systems.
- Mihály, N.B., et al. (2022). "Data-driven modelling based on artificial neural networks for predicting energy and effluent quality indices and wastewater treatment plant optimization," Optimization and Engineering, 23, 2235–2259.

For a detailed analysis, please refer to the full paper. (TBA when published)


