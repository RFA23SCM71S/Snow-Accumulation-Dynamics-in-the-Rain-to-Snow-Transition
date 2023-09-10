# Snow-Accumulation-Dynamics-in-the-Rain-to-Snow-Transition

## Problem Statement

This project aims to analyze a comprehensive hydrometeorological dataset spanning from the water year 2004 to 2014, focusing on the rain-to-snow transition zone in southwestern Idaho's Johnston Draw (JD) watershed. The primary objective is to identify the key factors influencing snow accumulation in this region, with implications for hydrological and biological processes. The study involves preprocessing and merging multiple datasets, exploring correlations among hydrometeorological variables, and applying regression models to investigate the influence of these factors on snow depth. This research has broader implications for understanding and managing water resources, flood control, power generation, and agriculture in climatically sensitive regions undergoing changes in rain-to-snow transitions due to climate change.

## EDA
- Bivariate visualizations revealed peak snow accumulation during specific months and a general trend of increasing snow depth over the years in the Johnston Draw (JD) watershed.
- An inverse correlation between snow depth and soil temperature was observed, indicating that higher soil temperatures were associated with lower snow depth.
- Correlation analysis showed high correlations among certain soil temperature and moisture features, suggesting the need for feature reduction to prevent overfitting in predictive modeling.
- Principal Component Analysis (PCA) was used to reduce dimensionality, with a focus on the top 20 most relevant features.
- Outliers were detected using Tukey's method and addressed through Winsorization to minimize their impact.
- Multiple linear regression, ridge regression, and lasso regression models were developed and evaluated under different conditions, showing that most features were relevant in explaining snow depth variations.
- Ridge and lasso regression successfully shrunk coefficients, while all features remained influential in predicting snow depth.

## Conclusion
1. The importance of retaining most features for accurate snow depth prediction.
2. Multiple linear regression highlighted the significance of various factors in explaining snow conditions, with positive correlations to RH, ppt_a, and perc_snow, and negative correlations to T_a, T_d, and e_a.
3. Ridge regression exhibited lower performance.
4. Soil Temperatures (T_g) and Soil Moistures (s_m) appeared orthogonal to snow depth.
Despite data gaps, our study provided valuable insights, expanding beyond initial plans to incorporate additional tasks as our understanding grew.
