# Ames Machine Learning Project:
This project uses the Ames housing dataset to predict real estate prices. My goal was to thoroughly explore the modeling capabilities of sklearn and to 
create two models, one that was highly interpretable (but less accurate), and one that was highly accurate (but less interpretable). The results are a multiple
linear regression model, and a gradient boosting model. The files are organized as follows:
"Ames Real Estate Data.csv" and "Ames_HousePrice.csv" are two versions of the original dataset.

### 1. EDA.ipynb
  I. Examine columns individually, assess types of variables, basic descriptive statistics, and get an idea of missing values.  
  II. Rough draft of examining missing data for visualization purposes. The exact imputed dataset used in the modeling process is contained in "2. Impute Missing Data- Export.ipynb".  
  III. Rough draft of Feature Engineering- formalized in second notebook.  
  IV. Assess for multicollinearity  
  V. SLR and MLR first pass: Assess R2 from simple linear regression on all variables- no splits, just for basic idea of relationships.  
  VI. MLR Continued- One Numerical/One Categorical- Visualize columns with top R2, one categorical one numerical. Combine into linear regression and report R^2.  
  VII. Explore Target Transformation  

### 2. Impute Missing Data- Export.ipynb
  I. Exploratory SLR  
  II. Impute Missing Data  
  III. Feature Engineering  
  IV. Missing Data Imputed + Feature Engineering Done: Export as 'ames.csv'  

### 3. SLR and MLR.ipynb  
  I. SLR with Train-test Split  
  II. SLR with 5-fold Cross-Validation  
  III. Multiple Linear Regression: Sequential Feature Selector  
  IV. MLR continued: Experimentation  
  V. Build "Notebook Model"- Extract Coefficients  
  VI. "Notebook Model"  
  VII. MLR Model Closer Look: StatsModels, VIF, Residuals  
      Export model results as 'master_scores_MLR.csv'  

### 4. PLR- Lasso, Ridge, ElasticNet.ipynb  
  I. Setup  
  II. Set up Pipelines  
  III. Run Untuned PLR's  
  IV. Tuning: Lasso  
  V. Tuning: Lasso Results  
  VI. Tuning: Ridge  
  VII. Tuning: Ridge Results  
  VIII. Tuning: ElasticNet  
  IX. Tuning: ElasticNet Results  
  X. Summary of Tuning Improvements  
  XI. Lasso- Coefficients Closer Look- General  
  XII. Lasso- Coefficients Closer Look- Specific Values/Feature Importances/Residuals  
  XIII. Ridge- Coefficients Closer Look- Specific Values/Feature Importances/Residuals  
    Export model results as 'master_scores_PLR.csv'  

### 5. Tree-Based and SVR.ipynb- These models require similar encoding, so they are grouped together in this notebook.  
  I. Setup  
  II. Set up Encoding/RF Pipeline  
  III. Run untuned RF Pipeline  
  IV. Tuning: RF  
  V. RF: Report Importances/Residuals  
  VI. GradientBoostingRegressor- repeat Process  
  VII. Tuning: GBR  
  VIII. GBR: Report Importances/Residuals  
  IX. SVR and Tuning  
  X. Summarize Findings  
    Export model results as 'master_score_Tree_and_SVR.csv'  

