# Data Scientist

### Education
- B.S., Statistics and Economics | The University of Milan Bicocca (_September 2024_)
### Work Experience
**Internship in the Department of Experimental Oncology at the European Institute of Oncology (_March 2024-August 2024_)**
- I performed all the statistical analyses regarding a meta-analysis

## Projects

### Sex-Related Differences in Toxicities caused by Treatment of Advanced Melanoma Patients
[Publication](https://osf.io/3t6fk/)

This project presents a systematic review and meta-analysis aimed at investigating sex-based differences in the manifestation of adverse events (AEs) caused by modern treatments for advanced melanoma, specifically immunotherapy and targeted therapy. These therapies have transformed the prognosis of melanoma patients, yet they are frequently associated with toxicities that can impact treatment adherence and quality of life. Prior studies suggested that female patients may be at higher risk of AEs under cytotoxic therapies. The primary objective of this meta-analysis is to determine whether sex significantly influences the occurrence of side effects from immunotherapy and targeted therapy, thereby allowing clinicians to optimize treatment strategies and enhance patient quality of life.
A comprehensive literature search was conducted using databases such as PubMed and Embase, including all independent studies published up to April 2024 that reported sex-specific toxicity data in patients with melanoma as the primary disease. Data extraction focused on obtaining sufficient information to estimate Odds Ratios (ORs) with 95% Confidence Intervals (CIs), or raw data on male and female patients with or without AEs. Due to limited availability of general AE data, the analysis focused on specific categories such as dermatologic, thyroid-related, and grade III–IV AEs.
Statistical analysis was performed using random-effects models to calculate summary odds ratios (sORs) and corresponding CIs. Study heterogeneity was assessed using the I² statistic, and publication bias was evaluated via Egger’s and Begg’s tests. Sensitivity analyses, including leave-one-out methods, were used to explore the sources of heterogeneity.

Key findings revealed significant sex-related differences in treatment toxicity:
- Female patients exhibited a higher risk of developing thyroid-related adverse events.
- Women were also more likely to experience dermatologic and grade III–IV toxicities.
- Specifically, for dermatologic AEs, the sOR was 1.31 (95% CI [1.06–1.61]), indicating a significantly greater risk for females.
- Heterogeneity was not significant for thyroid AEs (I² = 29.39%), and moderate for dermatologic AEs.
- No significant evidence of publication bias was found for the analyzed AE categories.

This study contributes to the growing body of evidence on sex-specific responses to advanced melanoma therapies. It is one of the first to systematically examine modern treatments through this lens and confirms that female sex is associated with a higher likelihood of certain adverse events. These results emphasize the relevance of statistical and machine learning models in biomedical research and support the inclusion of sex-based considerations in clinical decision-making and future studies.
Limitations include the retrospective nature of the analysis and the limited ability to extract general AE data from many studies, which constrained the analysis to specific toxicity categories.
 (All the statistical analisys were performed using R.)

### Heart Failure Analysis

This project focuses on the early detection of heart failure risk using machine learning models applied to the Heart Failure Dataset, which contains 918 observations and 12 clinical features collected from five different sources.
The data preprocessing phase included the handling of missing values (notably imputing Cholesterol using the CART method after comparative analysis), standardization of numerical variables, and the creation of balanced training, validation, and test sets. Due to multimodal distributions, models assuming conditional normality such as LDA and QDA were excluded from evaluation.
Several classification models were tested, including Logistic Regression, K-Nearest Neighbors (K-NN), MDA, and Classification Trees. Model selection was based primarily on Sensitivity (ability to detect patients at risk) and Accuracy. Logistic Regression and K-NN demonstrated the best validation performance.
In the testing phase, Logistic Regression with stepwise feature selection achieved superior results, avoiding the overfitting issues observed with K-NN. With the default threshold of 0.5, the model reached 88.5% Accuracy and 91.1% Sensitivity. After optimizing the decision threshold to 0.35, performance further improved to 90.7% Accuracy and 96.0% Sensitivity.
The most influential predictors in the final model included: male sex, high fasting blood sugar (FastingBS1), exercise-induced angina, ST segment slope (Flat and Up), age, and Oldpeak. Interestingly, asymptomatic patients showed a higher risk compared to those presenting various types of chest pain.
In conclusion, the logistic regression model with stepwise selection and optimized threshold proved to be the most effective and interpretable solution for predicting heart failure risk, confirming the value of machine learning in biomedical data analysis. 
(All the statistical analisys were performed using R.)

### Loan Approval Prediction with Machine Learning on Imbalanced Data

This project explores the use of Machine Learning techniques to automate and improve the loan approval process, with a particular focus on addressing the challenge of imbalanced datasets. The main goal is to build a reliable predictive model capable of assessing the likelihood of loan repayment.
The dataset used contains 252,000 loan applications, including detailed demographic, financial, employment, and property-related features. Key variables include income, age, work experience, marital status, home and vehicle ownership, profession, city, state, and employment/residence duration. The target variable is binary (Risk_Flag), where 1 indicates a high-risk applicant and 0 indicates a low-risk applicant.
The project followed a standard machine learning pipeline. During data preprocessing, missing values and outliers were addressed, new features were engineered (e.g., Income-to-Age ratio, Employment and Residential Stability), and numerical features were standardized. Categorical variables such as marital status, profession, and property ownership were encoded numerically. Feature selection was performed using correlation analysis to eliminate redundant or irrelevant features.
To manage the class imbalance issue, both oversampling (SMOTE) and undersampling techniques were applied to the training data. Several classification models were evaluated, including Logistic Regression, Decision Trees, Random Forests, Naive Bayes, Neural Networks, and XGBoost. Model evaluation was conducted using a 70/30 hold-out split and metrics such as Accuracy, Precision, Recall, F1-score, and AUC (Area Under the ROC Curve).
The best results were achieved using an ensemble model that combined two Decision Trees: one trained with undersampling and the other with SMOTE. This approach allowed for the aggregation of predictions to improve accuracy and robustness. The ensemble model achieved strong performance on the test set, with 89% Accuracy, 53% Precision, 90% Recall, an F1-score of 0.67, and an AUC of 0.89. This confirms the model’s ability to handle imbalanced data effectively while maintaining strong generalization.
In conclusion, the ensemble approach based on Decision Trees and dual sampling techniques outperformed individual models in predicting loan repayment. It highlights the potential of ensemble methods for robust predictions in real-world applications involving imbalanced data, such as credit risk assessment, fraud detection, and customer churn prediction.
One major limitation of the project was the lack of sufficient computational resources, which restricted experimentation with more complex models and advanced validation techniques such as stratified k-fold cross-validation. Future improvements could include the use of cloud-based infrastructure or distributed computing to overcome these constraints.
(All the statistical analisys were performed using KNIME.)

### Analysis of Tactical Evolution and Player Roles in the NBA (1997–2023)

This project presents a statistical analysis of the tactical evolution in the NBA and the redefinition of player roles over 25 seasons, from 1997 to 2023. The study investigates the transition from rigid traditional positions (Point Guard, Shooting Guard, Small Forward, Power Forward, Center) toward a more fluid and flexible model, often described as "roleless basketball."
The main goal is to evaluate the declining distinctiveness of traditional roles and validate JJ Redick’s theory, which proposes three functional categories: Ball Handler, Off-Ball Player, and Big. The dataset includes per-game stats (e.g., shooting, passing, rebounding), advanced metrics (e.g., Usage Rate, Net Rating), and physical attributes (height, weight).
A classification analysis using EDDA shows a rising misclassification error rate for traditional roles—from ~24% in 1997–2002 to ~40% in 2018–2023—demonstrating how statistical boundaries between positions have blurred. Meanwhile, cluster analysis on recent seasons (2019–2023) supports the 3-role model. Ball Handlers show high assist rates and usage; Off-Ball Players are efficient perimeter shooters; Bigs lead in rebounds, blocks, and size.
Findings confirm that the modern NBA emphasizes skill, versatility, and three-point shooting, shifting away from rigid positional structures. This supports the use of model-based approaches to understand role evolution in sports analytics.


