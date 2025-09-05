## Predicting Wine Quality:  A Comparison of Linear Regression Techniques on a Multicollinear and Outlier-Affected Dataset
[![DOI](https://img.shields.io/badge/DOI-10.13140%2FRG.2.2.16657.13926-blue)](https://doi.org/10.13140/RG.2.2.16657.13926)

[![Open In Colab](https://img.shields.io/badge/Colab-Open%20In%20Colab-blue?logo=googlecolab)](https://colab.research.google.com/drive/155YRm4swD98EgS-pEEcDidi7c-C1gCED)
---

### Abstract
This project explores the application of various linear regression techniques for predictingwine quality, which has a very important role, particularly in the wine industry for shaping upthe preferences of consumers, influencing the pricing related strategies and guiding decisionmaking in production, using a dataset characterised by multicollinearity and a significantpresence of outliers. The dataset comprises 32 wine samples, each evaluated across 10physicochemical attributes - including pH, total sulphur dioxide, anthocyanin concentrationand colour density - with quality scores assigned on a 0-20 scale. An extensive ExploratoryData Analysis (EDA) revealed distributional skewness, strong inter-variable correlations, anda high incidence of outliers. The initial application of Ordinary Least Squares (OLS)regression exposed limitations due to multicollinearity, as confirmed through elevatedVariance Inflation Factors (VIFs). Stepwise regression (both-way) improved modelparsimony, but heteroscedasticity and sensitivity to outliers persisted. To address these, robustregression approaches were adopted, including Huber’s M-estimator and the MM-estimator.Comparative analysis using metrics such as Adjusted R² and Root Mean Square Error(RMSE) demonstrated the MM-estimator’s superior resilience to data irregularities.Ultimately, the MM-estimator emerged as the most reliable and interpretable model, offeringa robust framework for data-driven wine quality assessment and decision-making inviticulture. This project thus underscores the importance of robust techniques in real-worlddata environments and presents a generalisable modelling framework to support objectivewine quality assessment in the wine industry. 

### Keywords
 Wine quality rating;
 Exploratory Data Analysis;
 Ordinary Least Squares;
 Stepwise Regression;
 Robust Regression

### Repository Structure
- `analysis.ipynb` → Clean notebook aligned with the project report  
- `explorations.ipynb` → Additional experiments, alternative methods, and sampling tests  
- `dataset/data.csv` → Dataset used in the study  
- `dataset/data_description.md` → Description of dataset variables  
- `project_report.pdf` → Full project report (sample paper)  
- `project_presentation.pdf` → Summary presentation slides  
- `requirements.txt` → R package dependencies  
- `README.md` → This file  

### Conclusion 
In this project, we explored the challenge of predicting wine quality using a small,multicollinear, and outlier-affected dataset. Starting with Ordinary Least Squares (OLS)regression as a baseline, we uncovered limitations stemming from multicollinearity andsensitivity to outliers, which compromised the stability and interpretability of the model.Through stepwise selection, we improved model parsimony, but residual diagnostics revealedpersistent issues such as heteroscedasticity.To overcome these challenges, we turned to robust regression techniques, particularlyHuber’s M-estimator and the MM-estimator. Among the approaches compared, theMM-estimator emerged as the most effective method, achieving the best trade-off betweenpredictive accuracy and resistance to data irregularities as demonstrated by the lowest RMSEand a relatively high Adjusted R². This robust method proved especially valuable in handlingsmall-sample data with violations of key linear regression assumptions.The findings underscore the importance of choosing adaptive and assumption-resilientmodels in practical data science applications. Particularly in domains like oenology, wherequality assessment can benefit from more objective, data-driven methods, such approachesoffer a reliable framework for supporting decision-making and quality control.While the dataset size and lack of metadata presented certain limitations, the modellingpipeline developed in this study can serve as a generalisable blueprint for future studies inwine quality assessment or similar regression problems involving complex real-world data.Further research could explore advanced regularisation techniques like Robust RidgeRegression, expand the dataset for improved statistical power and improve generalisabilitywithout sacrificing interpretability. 

### Citation

If you use this project, please cite:

Roy, S. (2025). Predicting Wine Quality: A Comparison of Linear Regression Techniques on a Multicollinear and Outlier-Affected Dataset. ResearchGate. DOI: 10.13140/RG.2.2.16657.13926

### License

This repository is licensed under the **Creative Commons Attribution 4.0 International License (CC BY 4.0)**.  
You are free to use, modify, and distribute this work for academic, research, or commercial purposes, with proper attribution.  
See the LICENSE file for details. [Read more here](https://creativecommons.org/licenses/by/4.0/).  
