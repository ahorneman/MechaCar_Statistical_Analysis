# MechaCar_Statistical_Analysis

## Overview of Project
AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on us and the data analytics team to review the production data for insights that may help the manufacturing team.

### Linear Regression to Predict MPG
#### Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
Vehicle length and vehicle ground clearance display a non random amount of variance to mpg. 
The vehicle length and vehicle ground clearance have a significant impact on miles per gallon on the MechaCar prototype.

#### Is the slope of the linear model considered to be zero? Why or why not?
The p-value is 5.35e-11 which is much smaller than .05%. Therfore, we reject the null hypothesis, indicating the slope of this linear model is not zero. 

#### Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
The r-squared value is 0.7149, This shows that approximately 71% of mpg predictions will be accurate. 
Therefore, the model does predict mpg of MechaCar prototypes effectively.

![Capture1](https://user-images.githubusercontent.com/113067853/217106946-97180161-e163-4908-8b69-42c80ca25946.PNG)

### Summary Statistics on Suspension Coils
The MechaCar Suspension_Coil.csv dataset contains the results from multiple production lots. In this dataset, the weight capacities of multiple suspension coils were tested to determine if the manufacturing process is consistent across production lots. 
Summary statistics table to show:
- The suspension coil’s PSI continuous variable across all manufacturing lots.
- The following PSI metrics for each lot: mean, median, variance, and standard deviation.

#### The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

When looking at all manufacturing lots collectively, the variance of 62.29356 meets the 100 pounds per square inch specification. 
##### Total Summary table:
![image](https://user-images.githubusercontent.com/114044192/215367956-0734675a-21c3-4aff-8a54-110c87396a89.png)

When we go deeper and look at individual lots, Lots 1 and 2 pass the 100 pound requirement with variances of .9795918 and .4693878 respectively. 
However, Lot 3 shows 170.2861224 variance, which far exceeds the specification. 
##### Lot Summary Table:
![image](https://user-images.githubusercontent.com/114044192/215367990-3e9020d1-05a6-4ffe-a159-cde231f00daa.png)


### T-Tests on Suspension Coils
T-tests were ran to determine if all manufacturing lots and each lot individually are statistically different from 
the population mean of 1,500 pounds per square inch.

##### T-Test for all Lots:
![image](https://user-images.githubusercontent.com/114044192/215369025-ff555e7c-ef4c-4a3e-8289-f880a9567614.png)

The sample mean for all lots is 1498.78. 
The p-value is 0.06 which is higher than 0.05. 
The data supports not rejecting the null hypothesis.
As a whole,the population meets the 1500 psi specification. 

##### T-Test for Lot 1
![image](https://user-images.githubusercontent.com/114044192/215369146-7ecc4138-b916-4945-8856-af99f3563cde.png)
The sample mean for Lot 1 is 1500. 
The p-value is 1 which is higher than 0.05. 
The data supports not rejecting the null hypothesis.
There is no statistical difference between sample mean and population mean. 

##### T-Test for Lot 2
![image](https://user-images.githubusercontent.com/114044192/215369171-8a9940b4-9ad0-4819-90e5-e56c27590276.png)
The sample mean for Lot 2 is 1500.02. 
The p-value is 0.61 which is higher than 0.05. 
The data supports not rejecting the null hypothesis.
There is no statistical difference between sample mean and population mean. 

##### T-Test for Lot 3
![image](https://user-images.githubusercontent.com/114044192/215369203-6c2a5a27-ff4e-4ca6-8ad0-ef9ca3438150.png)
The sample mean for Lot 3 is 1496.14. 
The p-value is 0.04 which is lower than 0.05. 
The data supports rejecting the null hypothesis.

#### Summary of testing
Clearly, there is something occuring in Lot 3 that is causing multiple failures to meet specifications. The processes and checks need to be reviewed 
to determine what is causing system failures. 

### Study Design: MechaCar vs Competition
A statistical study to compare performance of the MechaCar vehicles against performance of vehicles from other manufacturers will include:
- A metric to be tested is mentioned
- A null hypothesis or an alternative hypothesis is described
- A statistical test is described to test the hypothesis

#### Proposed Study:
We would need to collect data for MechCar and its comparable models from different manufacturers for 2 years time to determine which, if any factors correlate to customer satisfaction. 

##### Hypothesis:
 - Null Hypothesis:
   MechaCar is comparable and competitive to similar models from other manufacturers. 
 - Alternative Hypothesis
   MechaCar is NOT comparable and competitive to similar models from other manufacturers. 
   
##### Statistical Tests
Multiple Linear regession and T tests should be used to determine identified factors as they correlate to customer satisfaction. 

This would allow us to focus on the factors that highly correlate to customer satisfaction and review possible ways to improve overall
customer satisfaction with the MechaCar.
   
##### Questons to consider:
1. What are the manufacturers that produce comparable models?
  - 1a. What manufacturers target the same market and are to be included in study?
2. Which car(s) from identified manufacturers should be included?
3. What data points do we want to compare across the population?
  - 3a. Suggested comparison data include:
     - Vehicle Cost
     - Vehicle Weight
     - Vehicle Engine Size
     - Vehicle Engine Type
     - Vehicle MPG
     - Vehicle Safety Rating
     - Vehicle Customer Satisfaction Rating
