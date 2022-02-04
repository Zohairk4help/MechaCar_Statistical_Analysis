# MechaCar_Statistical_Analysis
Module15


## *Written Summary-deliverable 1:* 

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



***the p-value of our over all mult regression analysis is 5.35 x 10-11, which is much greater than our assumed significance level of 0.05%.
Despite the number of significant variables, the multiple linear regression model has the regression score of 0.7149 in our multiple linear regression model while the p-value remained significant.***

<figure>
  <img src="PNG files\dliv1-summary.PNG" width="450" height="250">
  <figcaption>Picture 1: Deliverable 1's summary of Multi Linear Regression.</figcaption>
</figure>


<figure>
  <img src="PNG files\graphs_combined.png" width="450" height="250">
  <figcaption>Picture 2: Combined graphs for a X-variables Vs mpg.</figcaption>
</figure>

Picture 2 depicts all the x-variables have some positive correlation with the y-axis(mpg) except the x-variables(AWD and Spoiler_angle). 

## *Written Summary-deliverable 2: Summary Statistics on Suspension Coils* 

Situation :::  The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?


According to the picture 4's total summary PSI table, MechCar suspension coils' variance is under 100 pounds per square inch. On the other hand, the picture 3's Lot summary table shows the different scenario by showing only Lot 3 has the unwanted variance, which is way greater than the required MechCar suspension coils' variance. 

Hence, it could be said that the lot 3 from the lot summary table is not satisfying the design specifications. However, as a whole manufacturing unit by combining all Lots, they are satisfactorily meeting the car's design. 

<figure>
  <img src="PNG files\lot_summary_table.PNG" width="450" height="250">
  <figcaption>Picture 3: Lot summary table.</figcaption>
</figure>

<figure>
  <img src="PNG files\totsummarysusPSItable.PNG" width="450" height="250">
  <figcaption>Picture 4: Total summary PSI table.</figcaption>
</figure>


## *Written Summary-deliverable 3:T-Tests on Suspension Coils*

---> As the p-value is 0.06%, the value is above than the significance level. Hence, it can be concluded that the there is no enough evidence to reject the null hypothesis. Our H<sub>0</sub>  is: PSI across all manufacturing lots is statistically different from the population mean of 1,500 pounds per square inch.

<figure>
  <img src="PNG files\ttestvspopmean.PNG" width="450" height="250">
  <figcaption>Picture 5: T-test Vs population Mean of all the lots' PSI.</figcaption>
</figure>



---> As the p-values for the individual lots' numbers (1 and 2) are greater than 0.05%, it can be concluded that the there is no enough evidence to reject the null hypothesis. The T-tests values for lot 1 is 1 and that of lot 2 is 0.61. Our H<sub>0</sub>  is: PSI across all manufacturing lots is statistically different from the population mean of 1,500 pounds per square inch.

<figure>
  <img src="PNG files\var1_2ttests.PNG" width="450" height="250">
  <figcaption>Picture 6: T-test Vs population Mean of the lots(1 & 2) PSI.</figcaption>
</figure>

On the other hand, the p-value for the individual lot number 3 is 0.04, which is lesser than 0.05%, it can be concluded that there is enough evidence to reject the null hypothesis. Our H<sub>0</sub>  is: PSI across all manufacturing lots is statistically different from the population mean of 1,500 pounds per square inch.
<figure>
  <img src="PNG files\var3ttest.PNG" width="450" height="250">
  <figcaption>Picture 7: T-test Vs population Mean of the lot 3's PSI.</figcaption>
</figure>

## *Written Summary-deliverable 4:Design a Study Comparing the MechaCar to the Competition.*

#### Study Design: MechaCar vs Competition:

---> Most of the Customers, who are financially tight but still need a vehicle, see the following metrics before the purchase of the vehicle:
1. Re-used vehicles' cost.
2. City and highway fuel efficiency.
3. Maintenance cost. 
4. Vehicle history.

---> H<sub>0</sub>: There are affordable used cars that have a good highway and city fuel efficiency, reasonable maintenance costs and no severly bad vehicle history for needy customers to be satisfied with their purchase. 

---> H<sub>a</sub>:There are no affordable used cars that have all the enlisted vehicular metrics for needy customers to buy. 

---> Possible statistical tests: 
1. chi-squared test as the customers' satisfaction can be a dependent variable.
2. multiple linear regression: to see the relationship between the enlisted metrics Vs 
the satisfaction of the needy customers. 

---> Possible data to be analysed could be both categorical and continous. 
