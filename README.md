# CarsRUS-MechaCar-Challenge-15
## Linear Regression to Predict MPG
Pr(>|t|) is the probabilty that each coefficient contributes a random amount of varience to the linear model. According to the results of the linear regression analysis, vehicle length, and ground clearence appear to provide a random amount of varience to linear model. The interecept is also statistically significant indicating that one of the significant features may need scaling or transforming to help improve the predictive model or there are other variables that can help explain the variability.

Since the p-value of our analysis is less than our significance value of 0.05, this indicates that we should reject the null hypothesis, and indicates that the slope of our linear model is not zero.

This linear model has an R-squared >0.7 which indicates a strong correlation.  This means that the linear model does predict the mpg of MechaCar prototypes effectively.

## Summary Statistics on Suspension Coils
Based on the total summary, the variance is under 100 lbs/sqinch and therefore meets the manufacturing tolerance requirements. However wheng grouped by lot, Lot 3 exceeds the manufacturing tolerance requirements of 100lbs/sqinch with a variance of 170lbs/sqinch.

## T-Tests on Suspension Coils

The T-test of the summary suspension coil data has a p-value greater than our significance value of 0.05 which suggests that we should accept the null hypothesis and that there is sufficient evidence to suggest that there is not a difference compared to the mean assuming the mean is 1500lbs/sqinch.  The actual mean is 1498.78 which could bias the results. Out of the three lots, lot 2 and 3 exceed our p-value cutoff of 0.05, suggesting that there is no statistically significant difference from the mean, however lot 3 has a p-value of 0.04168 which is below our significance cutoff and therefore means in this instance we should reject the null hypothesis, and conclude that lot 3 is statistically different from the mean of the population if the mean of the population is 1500 lbs/sqinch.

## Study Design: MechaCar vs Competition

Since MechaCar sounds cool and is therefore imagined as a high performance vehicle, we are going to be measuring lap times to determine the performance of the MechaCar against the competition.  In order to measure the performance of the MechaCar, we are going to measure lap times around the Nurburgring test track in Germany against similarly priced high performance sports cars with a precision of one one thousandths of a second. The start time will begin when the tip of the front bumper crosses the start line, and end when the tip of the rear bumper crosses the finish line. 20 consecutive laps will be performed by each car with the same driver and the results analyzed.  This test will examine the sum of several performance features at once including power, handling, breaking and endurance.

H0: The average lap time of the MechaCar is statistically not faster around the Nurburgring test track than other cars in its price catagory.
HA: The average lap time of the MechaCar is statistically different (higher/lower) around the Nurburgring test track than other cars in its price catagory.

Information we will need are going to be: The Nurburgring lap times of each car in each run, and the retail cost of each vehicle.

Once all the data is collected, we will summarize the information.  First we need perform an R-test for normality to determine if we should use the mean or median lap times for our analysis. Once we find our measure of normal tendancy, we can normalize the lap times of the car against the mean or median price of each car.  After that we can perform another T-Test against the normalized lap times to determine if the racing performance of the MechaCar is statistically higher than the other cars in its price category normalized against the mean or median cost.  This will give us the performance/value metric that hopefully the MechaCar will stand out in.
