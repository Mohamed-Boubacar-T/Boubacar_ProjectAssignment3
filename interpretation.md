# Week 5 interpretation

I used multiple linear regression to estimate dissolved oxygen (DO) from pH, district, and seasonal timing in Kerala (Central Pollution Control Board, n.d.). The model was trained on 2,670 observations and tested on 671 later observations. Its test R² was 0.126, with RMSE of 1.44 mg/L and MAE of 1.13 mg/L, indicating limited predictive ability despite outperforming the mean baseline (Scikit-learn, n.d.-b). For the 37 test readings below 3.05 mg/L, the average predicted DO was 5.46 mg/L, suggesting the model could overlook unusually low oxygen conditions. Uneven station coverage, missing BOD measurements, and the linear model’s assumptions limit the results. I would use this model for preliminary estimates, not pollution warnings, and collect additional measurements before relying on its predictions.

## References
Central Pollution Control Board. (n.d.). *Surface water quality: Manual chemical parameters (CPCB)* [Data set]. National Water Data Portal. https://nwdp.nwic.gov.in/dataset/surface-water-quality-manual-chemical-parameters-cpcb/resource/744b2bd4-7483-4eb1-a59a-5fbe06b62588

Scikit-learn. (n.d.-a). *Getting started*. https://scikit-learn.org/stable/getting_started.html

Scikit-learn. (n.d.-b). *Metrics and scoring: Quantifying the quality of predictions*. https://scikit-learn.org/stable/modules/model_evaluation.html
