# Ames Machine Learning Project
This project explores the modeling capabilities of sklearn to create an accessible (but less accurate) model and a more accurate (but less accessible)
model using the Ames housing dataset from Kaggle. These models, respectively, are a multiple linear regression model and a gradient boosting model. 
The repo is organized as follows:

"Ames_HousePrice.csv" is the original downloaded dataset.  

## EDA and Impute Missing Data  
  ### EDA.ipynb  
  I. Setup and EDA  
  II. Missing Values - first pass, formalized in the next file in this folder.  
  III. Feature Engineering- first pass, formalized in the next file in this folder.
  IV. Multicollinearity  
  V. SLR and MLR first pass  
  VI. MLR Continued- One Numerical/One Categorical
  VII. Explore Target Transformation  
  ### Impute Missing Data- Export.ipynb
  I. Exploratory SLR  
  II. Impute Missing Data  
  III. Feature Engineering  
  IV. Missing Data Imputed + Feature Engineering Done: Export as 'ames.csv'  
      'ames.csv' copied into 'Modeling' directory.  

## Modeling  
  ### SLR and MLR.ipynb  
  I. SLR with Train-Test Split  
  II. SLR with Cross-Validation  
  Multiple Linear Regression  
  III. Sequential Feature Selection  
  IV. MLR continued  
  V. Build 'Notebook Model'- Extract coefficients  
  VI. "Notebook" Multiple Linear Regression Model  
  VII. MLR Model Closer Look: StatsModels, VIF, Residuals  
     Export scores to 'master_scores_MLR.csv'
    
  ### PLR- Lasso, Ridge, ElasticNet.ipynb  
  I. Setup  
  II. Set up Pipelines  
  III. Run PLR's  
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
    Export scores to 'master_scores_PLR.csv'
  
  ### Tree Based and SVR.ipynb- both require similar encodings, so they are include together here.  
  I. Setup  
  II. Set up Encoding/RF Pipeline  
  III. Run RF Pipeline  
  IV. Tuning Hyperparameters  
  V. Tune Pipeline/Report Importances and Residuals  
  VI. Repeat Process with GradientBoostingRegressor  
  VII. Tune Hyperparameters  
  VIII. Tune Pipeline/Report Importances and Residuals  
  IX. Repeat Process with SVR  
  X. Summarize Findings  
    Export scores to 'master_scores_Tree_and_SVR.csv'  
