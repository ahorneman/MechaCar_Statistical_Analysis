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
The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

When looking at all manufacturing lots collectively, the variance of 62.29356 meets the 100 pounds per square inch specification. 
##### Total Summary table:
![Capture2](https://user-images.githubusercontent.com/113067853/217107120-9111cf6c-b759-46f4-88a3-1a94fb1631e6.PNG)

When we go deeper and look at individual lots, Lots 1 and 2 pass the 100 pound requirement with variances of .9795918 and .4693878 respectively. 
However, Lot 3 shows 170.2861224 variance, which far exceeds the specification. 
Lot Summary Table:
![image](https://user-images.githubusercontent.com/114044192/215367990-3e9020d1-05a6-4ffe-a159-cde231f00daa.png)

T-Test for all Lots:
![Capture3](https://user-images.githubusercontent.com/113067853/217107220-0a88ef72-4e83-4cea-8746-47aa546baa05.PNG)

The sample mean for all lots is 1498.78. 
The p-value is 0.06 which is higher than 0.05. 
The data supports not rejecting the null hypothesis.
As a whole,the population meets the 1500 psi specification. 

T-Test for Lot 1
![Capture4](https://user-images.githubusercontent.com/113067853/217107276-0604ec99-6010-4c19-8867-9c10e3101179.PNG)

The sample mean for Lot 1 is 1500. 
The p-value is 1 which is higher than 0.05. 
The data supports not rejecting the null hypothesis.
There is no statistical difference between sample mean and population mean. 

T-Test for Lot 2
![Capture5](https://user-images.githubusercontent.com/113067853/217107325-6b2d4548-0cf4-46de-9d6c-86bd17a71d9c.PNG)

The sample mean for Lot 2 is 1500.02. 
The p-value is 0.61 which is higher than 0.05. 
The data supports not rejecting the null hypothesis.
There is no statistical difference between sample mean and population mean. 

T-Test for Lot 3
![Capture6](https://user-images.githubusercontent.com/113067853/217107363-5ceed2b9-ba71-495b-b950-2be5f3dadf5f.PNG)

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

##### Hypothesis:
 - Null Hypothesis:
   MechaCar is comparable and competitive to similar models from other manufacturers. 
 - Alternative Hypothesis
   MechaCar is NOT comparable and competitive to similar models from other manufacturers. 
   
##### Statistical Tests
Multiple Linear regession and T tests should be used to determine identified factors as they correlate to customer satisfaction. 

This would allow us to focus on the factors that highly correlate to customer satisfaction and review possible ways to improve overall
customer satisfaction with the MechaCar.
