# MechaCar_Statistical_Analysis
## Introduction
This analysis aimed at utilizing R programming. This was done by using statistical tests to analyze data from AutoRUs motor vehicle company. The aim of the data analyses was to help improve the overall efficiency of their manufacturing process.
![image](https://user-images.githubusercontent.com/89704371/178796608-a7a63108-0221-45a9-8682-a93efecbbc7f.png)

### Deliverables
* Deliverable 1
* Deliverable 2
* Deliverable 3
* Deliverable 4

## Deliverable 1
### Linear Regression to Predict MPG
linear regression is a statistical model that is used to predict a continuous dependent variable based on one or more independent variables fitted to the equation of a line. Multiple linear regression builds a linear regression model with two or more independent variables In this deliverable we chose to use the multiple linear regression beacuse we had a multiple number of avriables as our input. It is useful in quantifying the variablility of two correlated variables.

### Hypothesis
H0 : The slope of the linear model is zero, or m = 0

Ha : The slope of the linear model is not zero, or m ≠ 0

To perform the linear regression, we utilized the lm() function and passed in all our six variables(vehicle_length, vehicle_weight, spoiler_angle, ground_clearance, AWD, and mpg) .

Below snapshot short displays the results
 
![image](https://user-images.githubusercontent.com/89704371/178800500-9f12d60f-2649-4a83-a30c-e2b413081839.png)

#### Output Analysis
1. The p-value of our linear regression analysis isp-Value: 5.35e-11, which is much smaller than our assumed significance level of 0.05%. Therefore, we can state that there is sufficient evidence to reject our null hypothesis, which means that the slope of our linear model is not zero.
2. The r-squared value for this out put model is 0.7149 which can be translated as to say that approx, over 70 % of all our mpg predictions many be determined suing the current model.
3. A close observation of the output indicates that the **vehicle length**, and **vehicle ground clearance** are statistically likely to provide non-random amounts of variance to the model. That is to say, the vehicle length and vehicle ground clearance have a significant impact on miles per gallon on the MechaCar prototype. Conversely, the vehicle weight, spoiler angle, and All Wheel Drive (AWD) have p-Values that indicate a random amount of variance with the dataset. This model does predict mpg .


## Deliverable 2
### Summary Statistics on Suspension Coils
The weight capacities of multiple suspension coils were tested to determine if the manufacturing process is consistent across production lots. The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch.  Below snapshot displays tahe results of the analysis.

#### total_summary
![image](https://user-images.githubusercontent.com/89704371/178804045-f6a3e394-f6ee-4a6a-b948-90fa03c81004.png)


#### lot summary
![image](https://user-images.githubusercontent.com/89704371/178803864-9960f943-8ba6-46ac-96ce-f205eb7de197.png)

#### Output analysis

Based on the variance of the suspension coils in the total summary, the suspension coils overall meet the MechaCar design specifications. However, the lot summary shows that while manufacturing Lots 1 and 2 meet the design specifications and have variances under 100 PSI, Lot 3 does not meet the design specifications as its variance is much over the 100 PSI limit.

## Deliverable 3
### T-Tests on Suspension Coils
Perform t-tests to determine if all manufacturing lots and each lot individually are statistically different from the population mean of 1,500 pounds per square inch.

t-test is used to compare the mean of one dataset to another under a few assumptions.
There are two main forms of the t-test that we use: the one-sample t-test and the two-sample t-test. The one-sample t-test is used to determine whether there is a statistical difference between the means of a sample dataset and a hypothesized, potential population dataset. In other words, a one-sample t-test is used to test the following hypotheses:

H0 : There is no statistical difference between the observed sample mean and its presumed population mean.
Ha : There is a statistical difference between the observed sample mean and its presumed population mean.

The following snapshot represents the output of the analysis

![image](https://user-images.githubusercontent.com/89704371/178810597-a01d5bdb-874c-41ac-8fba-144ea52279c8.png)
 
### analysis of the output
If p-value is lower than the significance level, you would have sufficient evidence to reject the null hypothesis and state that the two means are statistically different.
Assuming our significance level was the common 0.05 percent, our p-value is below our significance level. Therefore, we do not have sufficient evidence to reject the null hypothesis, and we would state that the two means are statistically similar.

#### Lot 1
The results of the t-test to test if the PSI mean for Lot1 is statistically different from the population mean of 1,500 pounds per square inch show that, at a 95% confidence level, the two means are not statistically different. The p-value of  1.568e-11 shows that the mean for Lot1 is exactly the same same as the population mean of 1500 PSI.

![image](https://user-images.githubusercontent.com/89704371/178812328-5fac6f38-2eaf-41e0-b4d0-20b8926dc07c.png)


#### Lot 2 
The results of the t-test to test if the PSI mean for Lot2 is statistically different from the population mean of 1,500 pounds per square inch show that, at a 95% confidence level, the two means are not statistically different. Because the p-value of 0.0005911 is higher than the critical value of 0.05, the null hypothesis can be accepted in that there is no difference between the means of the PSI for the population and Lot2. The means within the 95% confidence range are between 1499.423 and 1500.977 PSI.

![image](https://user-images.githubusercontent.com/89704371/178812409-6fc40e01-5f10-4ea4-a4a3-6837bdf29fdc.png)


#### Lot 3
The results of the t-test to test if the PSI mean for Lot3 is statistically different from the population mean of 1,500 pounds per square inch show that, at a 95% confidence level, the two means are statistically different. Because the p-value of 0.1589 is lower than the critical value of 0.05, the null hypothesis should be rejected in that there is a difference between the means of the PSI for the population and Lot3 and the true mean is not equal to 1500. The means within the 95% confidence range are between 1492.431 and 1499.849 PSI.

![image](https://user-images.githubusercontent.com/89704371/178812457-56653f60-254c-4335-a8a7-cc8e05bba37a.png)

## Deliverable 4
### Study Design: MechaCar vs Competition

This study would involve collecting data on MechaCar and its comparable models across several different manufacturers over the last 3 years.

What are the competitions' comparable models,
Which cars will MechaCar be competing with head-to-head? which cars will be included in the study?
Which factors will look at the study to determine the relevant to selling price?

The statistical study design has the following:

A metric to be tested  
A null hypothesis or an alternative hypothesis 
A statistical test is   to test the hypothesis
#### Relevant metrics

Safety Feature Rating: Independent Variable 
Current Price (Selling): Dependent Variable
Drive Package : Independent Variable
Engine (Electric, Hybrid, Gasoline / Conventional): Independent Variable
Resale Value: Independent Variable

Hypothesis: Null and Alternative
After determining which factors are key for the MechaCar's genre:

Null Hypothesis (Ho): MechaCar is priced correctly based on its performance of key factors for its genre.
Alternative Hypothesis (Ha): MechaCar is NOT priced correctly based on performance of key factors for its genre.
Statistical Tests
A multiple linear regression would be used to determine the factors that have the highest correlation/predictability with the list selling price (dependent variable); which combination has the greatest impact on price (it may be all of them!)
