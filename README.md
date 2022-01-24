# MechaCar_Statistical_Analysis
Module15


Written Summary-deliverable 1: 
In your README, create a subheading, ## Linear Regression to Predict MPG, and write a short summary using a screenshot of the output from the linear regression, and address the following questions:

*Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?*  Vehicle weight, Spoiler_angle and AWD are the variables that provide non-random amount of variance to the linear model. These variables have significant impact on mpg. This is all concluded by seeing the summary output, Pr(>|t|) values for each variables. where p-values are not lesser than 0.05. 

*Is the slope of the linear model considered to be zero? Why or why not?* Keeping the most impactful variables--(Vehicle weight, Spoiler_angle and AWD)--in mind, it is concluded that when the intercepts of the significant variables are statistically significant, it means that the intercept provide random amount of variance to the linear model. In other words, these highly impactful are not going to produce zero slope. 


*Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?* Speaking of the remaining variables (ground_clearance and vehicle_length) are not statisfically significant to produce non random variance and thus their slopes are considered zero. This is because these variables may need scaling and/or transforming to improve the predictive power of the model. Hence, depending upon the Mechacar_mpg_table-dataset, there might be a need to change the dataset's  independent variable/s and/or transform them to re-evaluate the co-efficients and significance. Thus the dataset might be effective only for the independent variables: Vehicle weight, Spoiler_angle and AWD.



|Variables      | P-values |intercept|
|:---------------|:------|:----------|
|*vehicle_weight:| 0.0776|1.245e-03|  
|*spoiler_angle: | 0.3069|6.877e-02|
|*AWD          : | 0.1852|-3.411   |
|ground_clearance: | 5.21x10^-8|6.877e-02|
|vehicle_length        : | 2.60e-12|6.267e+00|



***the p-value of our over all mult regression analysis is 5.35 x 10-11, which is much smaller than our assumed significance level of 0.05%.
Despite the number of significant variables, the multiple linear regression model outperformed the simple linear regression. According to the summary output, the r-squared value has increased from 0.50 in the simple linear regression model to 0.71 in our multiple linear regression model while the p-value remained significant.***

