# Partial-Correlation-with-Bootstrapping-on-R
This project conducts a detailed Partial Correlation Analysis on a dataset concerning the empathy, mental health, and burnout of medical students in Switzerland. It focuses on key variables like year of study, CESD (Center for Epidemiologic Studies Depression scale), STAI_T (State-Trait Anxiety Inventory scale), and self-reported health status. The analysis is performed using R programming.

**Objectives** <br>
To analyze the correlation between CESD and STAI_T for B.MED and M.MED students. <br>
To understand the impact of controlling for 'HEALTH' on the correlation between CESD and STAI_T. <br>
To employ non-parametric tests due to the non-normal distribution of the data. <br>

**Data** <br>
The dataset includes 20 variables and 886 observations, providing comprehensive information on the mental health status of medical students.

**Methods** <br>
Data Normality Check: Utilized Shapiro-Wilk normality test.<br>
Data Transformation: Explored log, sqrt, and reciprocal transformations.<br>
Correlation Analysis: Spearman rank-order correlation is used due to the non-normal distribution of data.<br>
Bootstrapping: Applied to account for the non-normality of the data.<br>

**Installation** <br>
Clone the Repository:
gh repo clone bhupeshdod/Partial-Correlation-with-Bootstrapping-on-R

Install R and RStudio:
Ensure you have R and RStudio installed on your machine.

Required R Packages:
The following R packages are required to run the scripts:

ggplot2,
dplyr,
tidyr,
psych

**Install them using R command:**
install.packages(c("ggplot2", "dplyr", "tidyr", "psych"))

**Results** <br>

The conclusion of the analysis report on the mental health and burnout of medical students in Switzerland can be summarized as follows:

Strong Positive Correlation: There is a strong and positive correlation between the CESD (Center for Epidemiologic Studies Depression scale) and STAI_T (State-Trait Anxiety Inventory scale) scores for both B.MED (year 1-3) and M.MED (year 4-6) students. This indicates that higher levels of depression are associated with higher levels of anxiety among these students.

Bootstrapping Results: The bootstrapping approach, used due to the non-normal distribution of data, confirmed the strong correlation but with slight differences in the correlation strength between B.MED and M.MED students.

Partial Correlation Controlled by Health: When controlling for the self-reported health status (HEALTH), there remains a significant positive correlation between CESD and STAI_T for both B.MED and M.MED students, though the correlation slightly decreases.

Negative Correlation with Health: There is a small-to-medium negative correlation between HEALTH and CESD, as well as between HEALTH and STAI_T for B.MED students, indicating that lower self-reported health status is associated with higher depression and anxiety. For M.MED students, this negative correlation is smaller and not statistically significant for STAI_T.

Other Influential Factors: The report suggests that there are other factors besides HEALTH influencing CESD and STAI_T, especially in M.MED students.

![image](https://github.com/bhupeshdod/Partial-Correlation-with-Bootstrapping-on-R/assets/141383468/3025134a-18b3-44d2-80b8-c9aff8cb3edf)

![image](https://github.com/bhupeshdod/Partial-Correlation-with-Bootstrapping-on-R/assets/141383468/3413923c-75c6-4b14-ba49-8c5ede5a125a)

