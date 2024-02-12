# Tanzania_waterFall_Predictions

![pumping](https://thumbs.dreamstime.com/z/young-african-boy-drinking-water-community-borehole-hand-pump-young-african-boy-drinking-water-community-172697689.jpg?w=992)

# Overview

Tanzania is the largest country in East Africa with a population of approximately 59 million. However, the country faces challenges in providing clean water to its large population and about 47% of the population lack access to clean drinking water. Many existing water points need repairs or have failed completely. The purpose of the project is to build a classifier for two potential audiences;
 -The Government of Tanzania who might be interested in identifying patterns in non-functional wells and understand  factors influencing their failure. This knowledge can be used to improve how new wells are built to ensure their longevity and functionality.
 -NGOs-Identifying non-functional and in-need-of-repair wells to optimize resource allocation and maximize their impact in providing clean water access.

# Objective

The goal is to build a classifier using data points like pump type, installation date, pump status etc to predict the functionality of water pumps found throughout the country.

# Data Understanding

Data was obtained from the Taarifa waterpoints dashboard which aggregates data from the Tanzania Ministry of Water. The data collected contains features related to water pumps such as geographic location, water quality, organizations that build and manage them and population among others. The target feature is 'status group'with three possible values of functional, non-functional and functional-need-repairs.

![Age vs functionality](https://github.com/JohnNkakuyia/Tanzania_waterFall_Predictions/blob/main/images/age_wel.jpg)


# Modeling

Three models were run on the data; XGBoost, LinearSVC and RandomForest.
![logistic regression](https://github.com/JohnNkakuyia/Tanzania_waterFall_Predictions/blob/main/images/logistics_con.jpg)
![svm](https://github.com/JohnNkakuyia/Tanzania_waterFall_Predictions/blob/main/images/svm_con.jpg)
# Evaluation
![best model](https://github.com/JohnNkakuyia/Tanzania_waterFall_Predictions/blob/main/images/model_output.jpg)

From the perfomance evaluation XgBoost have highest accuracy.and also using
other perfomance evaluation precision value is high for XgBoost .so we choose XgBoost is the best model
# Conclusion

Groundwater is very important to maintain the functionality of the wells.Almost, the entire water supply to the wells is dependent on groundwater. Hence, we would look into different methods such as rainwater harvesting and soil conservation which would also help sustain more water in the lakes.

We see that when we make payment based on bucket or monthly payment, the wells are maintained better. So payment is an important factor.

Definitely, age of the wells is an important factor to predict the functionality of the wells. The newer the wells are, more water they have or better is their condition.

We can see that having a public meeting helps in functioning of the wells. More than 50% wells are functional when there is a public meeting held for the same. Thus, Public meeting is an important factor for the functioning of wells.

Further send out designated people to inspect the pumps detected by the model and assess what needs to be done.

Future Work
Need to examine the missing values or Zero values of Population and gps. Also, try binning the highly cardinal columns. Most static head values were 0. Need to examine those too.
