# Tanzania_waterFall_Predictions

![pumping](https://thumbs.dreamstime.com/z/young-african-boy-drinking-water-community-borehole-hand-pump-young-african-boy-drinking-water-community-172697689.jpg?w=992)

# Overview

Tanzania is the largest country in East Africa with a population of approximately 59 million. However, the country faces challenges in providing clean water to its large population and about 47% of the population lacks access to clean drinking water. Many existing water points need repairs or have failed. The purpose of the project is to build a classifier for two potential audiences;
 -The Government of Tanzania might be interested in identifying patterns in non-functional wells and understanding  factors influencing their failure. This knowledge can be used to improve how new wells are built to ensure their longevity and functionality.
 -Identifying non-functional and in-need-of-repair wells to optimize resource allocation and maximize their impact in providing clean water access.

# Objective
Tanzania faces difficulties in providing clean water to its population of over 57 million due to issues with existing water points. Some wells need repairs, while others have failed altogether. To address this, an analysis is conducted to understand factors affecting well functionality, such as water source, age of wells, and the impact of public meetings. Additionally, the analysis aims to determine the best mode of payment for wells maintenance and utilize classification methods to identify the most effective strategies for improving well functionality. This analysis is intended to support the Government Ministry of Water and NGOs in their efforts to ensure access to clean water for Tanzanian communities.

# Data Understanding

Data was obtained from the Taarifa waterpoints dashboard which aggregates data from the Tanzania Ministry of Water. The data collected contains features related to water pumps such as geographic location, water quality, organizations that build and manage them, and population among others. The target feature is a 'status group with three possible values functional, non-functional, and functional-need-repairs.

![Age vs functionality](https://github.com/JohnNkakuyia/Tanzania_waterFall_Predictions/blob/main/images/age_wel.jpg)


# Modeling

Three models were run on the data; XGBoost, LinearSVC, and RandomForest.
![logistic regression](https://github.com/JohnNkakuyia/Tanzania_waterFall_Predictions/blob/main/images/logistics_con.jpg)
![svm](https://github.com/JohnNkakuyia/Tanzania_waterFall_Predictions/blob/main/images/svm_con.jpg)
# Evaluation
![best model](https://github.com/JohnNkakuyia/Tanzania_waterFall_Predictions/blob/main/images/model_output.jpg)

From the performance evaluation, XgBoost has the highest accuracy and also using
other performance evaluation precision value is high for XgBoost so we choose XgBoost as the best model
# Conclusion

Groundwater is very important to maintain the functionality of the wells. Almost, the entire water supply to the wells is dependent on groundwater. Hence, we would look into different methods such as rainwater harvesting and soil conservation which would also help sustain more water in the lakes.

We see that when we make payments based on bucket or monthly payments, the wells are maintained better. So payment is an important factor.

The age of the wells is an important factor in predicting the functionality of the wells. The newer the wells are, the more water they have or the better their condition.

We can see that having a public meeting helps in the functioning of the wells. More than 50% of wells are functional when there is a public meeting held for the same. Thus, Public meeting is an important factor for the functioning of wells.

Further, send out designated people to inspect the pumps detected by the model and assess what needs to be done.

Future Work
Need to examine the missing values or Zero values of Population and GPS. Also, try binning the highly cardinal columns. Most static head values were 0. Need to examine those too.
