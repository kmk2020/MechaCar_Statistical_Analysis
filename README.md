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

