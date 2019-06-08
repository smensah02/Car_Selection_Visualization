# Car_Selection_Visualization
 
<div align="center">
  <img src=" "><br>
</div>
 
## Data Analysis for Buying a Company Car
### Problem Statement
Select a vehicle based on the company’s criteria and comparing it to personal criteria. The vehicle choices given by manager include Ford Escape, Honda CRV, Hyundai Santa Fe, or Toyota Rav 4. 2018 Basic models of all vehicles where used in this analysis. 2018 was chosen because 2019 did not as robust information as 2018 had for the criteria.

The criteria used for this analysis are state below:
Criteria 1 (Company Criteria):
Safety features – weighted at 10
Maintenance cost – weighted at 5
Price point – weighted at 7

Criteria 2 (Personal Criteria):
Insurance
Fuel Economy
Resale Value

### DATA SCRAPE
Edmunds.com provided data on safety, price point for basic models for each vehicle type and fuel economy while your mechanic provided data for maintenance cost.
Kelley Blue Book provided data for resale value and data for insurance was got from nerdwallett and quote inspector.

A total of 4 safety features were retrieved from edmunds website and they include average of Barrier crash ratings, Rollover rating, Risk of Rollover and IIHS Rating. The Risk of Rollover (RoR) was measured in percentage and the higher the percentage, the higher the risk. A contrast to the crash ratings. As a result, weights of (1:4) were assigned to the RoR with 1 being the highest risk and 4 being the lowest. The outcome was then divided by a 100% since the RoR was given in initially percentage. The resulting value was then added to the crash rating to form a combine overall risk. IIHS Rating and actual Rollover rating were not used since it was the same for all 4 vehicles and will have no effect on the overall risk.
DATA CONFIGURATION
Data collected was further cleaned and separated based on criteria 1 and 2 respectively. Weights were already assigned to features in criteria 1. Weights were also assigned to each variable in the criteria and analyzed for comparison.
To fuel economy, a weight of 10 was assigned because it seemed like the most important being that fuel will used on a regular basis regardless of the type of vehicle chosen. Also, this cost of fuel varies depending on season of year and economic conditions. It is important to have a car that has a high mile per gallon (mpg). For this reason, it was weighed the highest of the personal criteria, especially since the manager did not indicate that cost of fuel would be company or personal funded. Less out of pocket is better regardless. 
A weight of 7 was assigned to resale value, since the company may want to upgrade the vehicle at some point down the line. Having a higher trade in value helps to company save money on investment especially being that cars usually depreciate.
Finally, a weight of 5 was assigned to insurance, primarily because, it is a fixed rate usually for the year and based on driving record the cost may reduce. It doesn’t play as high as important compared to the others but still important of enough to be considered when choosing a vehicle. 
In addition to weighing the features, the data was normalized to a 100% for the purpose of scaling which helps to enhance visualization.

### DATA PRESENTATION
 Clean combined data was imported into Tableau for further analysis and visualization. 
Three different visualizations for criteria 1 was created showing:
1.	Maintenance cost comparison among the 4 selected cars
2.	Price point comparison 
3.	Safety features comparison

Three visualizations were also created for criteria 2 showing:
1.	Insurance cost comparison among the 4 cars selected
2.	Fuel Economy comparison
3.	Resale value comparison

A Dashboard showing all relevant charts was created to on the tableau storyboard.
Vehicle Selection

Weight 10 Features
Based on the outcome from the analysis, the features that weigh the most - 10 (Safety features and fuel economy), Honda ranks the safest, followed by Hyundai, Ford and the least Toyota. 
In comparison to their fuel economy, Honda also ranked highest, followed by Toyota, then Ford, and Hyundai the least in fuel economy as shown in figure 1. 
We see here that the safest car is also the best in terms of fuel economy and the lest safest is the second best in fuel economy. Although, the difference in value of the safety measures between each car is very close, that little difference could determine life or death. Whereas, there is a wide disparity in the values for the mpg especially between the least, Hyundai and the others. 
Honda is the best choice based on the two highest weighed features ranking the highest in both safety and fuel economy.

 
Figure 1 (Features with weight of 10)

Weight 7 Features
Features with weight of 7(price point and resale value), Hyundai is the most expensive with a gap of about 25% more in price value compared to the other 3 cars. Toyota ranks 2nd most expensive, Honda 3rd and least expensive is Ford. With the last 3 within about a 1% difference of each other in price point. 
For the resale value, Honda tops with the best in resale value and ford the least, also with about 20% gap from the other 3 cars shown in figure 2

 
Figure 2 (Features with weight of 7)

Although Hyundai has the second-best resale value, it has the highest price point with a huge gap compare to the others. This huge price difference cannot be made in the resale value because the disparity in resale price is insignificantly small. Similarly, Ford has the lowest resale value with a huge gap from the others. This difference can also not be made up for in the purchase price point even though it has the best price point because the disparity between Ford and the other two cheaper cars is also very small. 
This leaves us with Toyota and Honda. Of the two, Honda has the both the best price point and resale value. Again, in this weight category, Honda wins.


Weight 5 Features
Maintenance cost and Insurance are weighed 5. They play a role in the consideration of choosing a car but not as high an importance as the other criteria. Regardless, based on the results shown in figure 3, Ford has the most maintenance with Toyota having the least while Toyota has the highest insurance cost and Hyundai the least. Again, can we make up for the expense in insurance with what we save in maintenance cost? Yes, over time we would be saving way more in maintenance cost. So, Toyota wins this category with Honda being the 2nd best for both features. Although Hyundai is the best in insurance savings, it is considerable high in maintenance cost and do not believe the cost in higher maintenance can be made in the insurance savings. Also, this savings can be lost based on the driving incidents/record just as well the maintenance cost could go even higher depending on road conditions and how often the car is driven. Based on this, the race falls between Toyota and Honda, with Toyota being the best in this category due to its low maintenance cost. 

 

Figure 3 (Features with weight of 5)



### VEHICLE SELECTION
Of the 4 vehicle choices given (Ford Escape, Honda CR-V, Hyundai Santa Fe, or Toyota RAV 4) in the 2018 models, Honda CR-V is the vehicle of choice to purchase as a company vehicle. The following findings influenced this decision:
1.	Honda CR-V is the safest vehicle of the 4 selections given.
2.	Honda CR-V was the best in fuel economy.
3.	Honda CR-V had the best price point.
4.	Honda CR-V had the best resale value.
5.	Although Toyota RAV4 has the best Maintenance value, Honda comes 2nd best. However, maintenance cost weighs the least in the criteria 1. 
6.	Hyundai Santa Fe has the best insurance savings, Honda CR-V is the 2nd best, yet this feature weighs the least in criteria 2.
7.	Honda CR-V is the best to invest in as shown in figure 4.
8.	More consideration is given to 1-4 above (figure 5) because they weigh much more than 5 and 6. Despite this, Honda-CR-V consistently places higher than most of the other vehicle choices given.

 
Figure 4(Purchase Price Vs. Resale Value)

 

Figure 5(Features with weight 10 and 7)


#### Additional visualizations can be found on car visualization pdf file.
#### Sources can be found in the Car_Visualization_Report.
