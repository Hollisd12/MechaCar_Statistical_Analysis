# MechaCar_Statistical_Analysis

Perform a statistical analysis of automobile performance using R

## Linear Regression to Predict MPG

![call1](https://user-images.githubusercontent.com/112137694/213603083-cfa51d1e-8131-4ee9-9530-caf9b70713c9.png)
![call2-values](https://user-images.githubusercontent.com/112137694/213603096-71a36410-787c-423e-b29b-0be80dcb3f62.png)

- Vehicle Length and Ground Clearance show a non-random amount of variance on the MPG of the MechaCar
- The slope of the linear model is not considered to be zero. The p-value of the linear model is lower than an extrememe level of significance. This provides sufficient statistical evidence that the null hypotheses is not true. The relationship between our variables and miles per gallon is subject to more than random chance.
- The r-squared value is .7149 indicating that there is a 71.48% chance that any future data points will fit this model. The linear model does predict the MechaCar prototypes effectively. There is most likely still unconsidered factors but the model is relatively effective.

## Summary Statistics on Suspension Coils

**Total Summary**

![total_summary](https://user-images.githubusercontent.com/112137694/213603167-1c963c6a-fa3e-4613-bf1a-a30a4fdbb37d.png)

**Lot Summary**

![lot_summary](https://user-images.githubusercontent.com/112137694/213603175-7611ae96-a6ba-42d5-9db9-17e094cf71d3.png)

- The specs for the MechaCoil suspension coils dictate that the variance of the suspension coils must not exceed 100 psi. Based on the Total Summary, the overall variance is below 100 psi and therefore meets the specifications. However, the lot summary stats shows that the variance for Lot 3 is well over the acceptable threshold (170.29)

## T-Tests on Suspension Coils

**Suspension Coils cumulative T-Test**

![sum_t_test](https://user-images.githubusercontent.com/112137694/213603255-2bcc616c-192f-497b-af19-42da219cc9b2.png)

**Lot 1 T-Test**

![lot1_t_test](https://user-images.githubusercontent.com/112137694/213603298-7170403a-213a-41b7-bcf3-daadd33360a5.png)

**Lot 2 T-Test**

![lot2-t-test](https://user-images.githubusercontent.com/112137694/213603313-53ae553b-7528-4132-9ab0-f3acf96d487d.png)

**Lot 3 T-Test**

![lot3-t-test](https://user-images.githubusercontent.com/112137694/213603329-be1b0ab7-583d-46b5-8fc0-eadac86d0904.png)

- T-Tests of Lot 3 show that the suspension coils are slightly statistically different from the population mean. The p-value (0.0417) is low enough to reject the null hypothesis. Further analysis of this lot might be necessary or it might need to be discarded.

## Study Design: MechaCar vs Competition

There are many reasons and factors that consumers consider before purchasing a car. With ridesharing on the rise, the app convenience, relatively affordable prices, and availability of these rideshares, affordablility and effectiveness need to be considered when manufactoring and marketing a car. Consumers are likely to look for an affordable and easy to maintain mode of transportation.

**Metric to test:**

- maintenance costs
- cost of vehicle

**Null and Alternate Hypothesis:**

H0: MechaCars prototypes' average maintenance costs is similar to competitor vehicles in the same class. Ha: MechaCar prototypes' average maintenance costs is statistically above or below that of competitor vehicles.

**Statistical Test to Use**

Two sample T-Test

**Data Needed**

Gather maintenace cost data from all MechaCar prototypes as well as from major competitor vehicles Use simple linear regression to test the hypothesis
