# Data Scientist

## Professional Summary
Data Science student with a Bachelor’s degree in Statistics and Economics and hands-on experience in meta-analysis
from an internship at the European Institute of Oncology (IEO). Strong background in data analysis, statistical modeling,
and machine learning. Initially passionate about machine learning, I thought I had found my path—until I discovered
deep learning and computer vision, which completely shifted my perspective. Now deeply driven to explore the frontiers
of AI, with a keen interest in applying data-driven solutions to real-world challenges.

## Education
- MSc in Data Science, University of the Studies of Milan-Bicocca Oct 2024 – Ongoing
- BSc in Statistics and Economics, University of the Studies of Milan-Bicocca Oct 2021 – Sept 2024

## Work Experience
European Institute of Oncology (IEO), Researcher Intern Milan, MI Mar 2024 – Aug 2024
• Worked on multiple biostatistical projects, developing data analysis skills and domain knowledge in medical research
• Contributed to a meta-analysis, which became the foundation of my BSc thesis
DOI: 10.17605/OSF.IO/3T6FK 2
• Assisted in data cleaning, exploratory analysis, and results interpretation in a collaborative research environment

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

### Analysis of Tactical Evolution and Player Roles in the NBA (1997–2023)

This project presents a statistical analysis of the tactical evolution in the NBA and the redefinition of player roles over 25 seasons, from 1997 to 2023. The study investigates the transition from rigid traditional positions (Point Guard, Shooting Guard, Small Forward, Power Forward, Center) toward a more fluid and flexible model, often described as "roleless basketball."
The main goal is to evaluate the declining distinctiveness of traditional roles and validate JJ Redick’s theory, which proposes three functional categories: Ball Handler, Off-Ball Player, and Big. The dataset includes per-game stats (e.g., shooting, passing, rebounding), advanced metrics (e.g., Usage Rate, Net Rating), and physical attributes (height, weight).
A classification analysis using EDDA shows a rising misclassification error rate for traditional roles—from ~24% in 1997–2002 to ~40% in 2018–2023—demonstrating how statistical boundaries between positions have blurred. Meanwhile, cluster analysis on recent seasons (2019–2023) supports the 3-role model. Ball Handlers show high assist rates and usage; Off-Ball Players are efficient perimeter shooters; Bigs lead in rebounds, blocks, and size.
Findings confirm that the modern NBA emphasizes skill, versatility, and three-point shooting, shifting away from rigid positional structures. This supports the use of model-based approaches to understand role evolution in sports analytics.
(All the statistical analisys were performed using R.)


