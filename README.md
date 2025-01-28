# IMPACT-OF-ENVIRONMENTAL-ROAD-INFRASTRUCTURAL-FACTORS-AND-AIR-QUALITY-ON-ACCIDENT-SEVERITY-IN-THE-UK
Triangulation of Data Source from Road Safety Data and AURN Air Quality Data.

# GUIDE ON HOW TO USE THE STEP BY STEP EDA

Load all the required modules as stated in the first cell, Any other module needed will be loaded along the way, although it is not the standard practice.

## Dataset for this work can be found on 

Download the Raw Air Quality Data   [AURN File](https://drive.google.com/file/d/1rN1EhmChTP3GoJ0EMXYmfcEruqsBCK9-/view?usp=sharing) here.

Download the Raw Collision 2018 - 2023    [Collision folder](https://drive.google.com/file/d/1rN1EhmChTP3GoJ0EMXYmfcEruqsBCK9-/view?usp=sharing) here.

Download the Raw Vehicle 2018 - 2023    [Vehicle folder](https://drive.google.com/drive/folders/1daF59ltjKtuaNAy2y4veYMBQVLWcPJWX?usp=sharing) here.

Download the Data Dictionary for Decoding Collision & Vehicle Data   [Road Safety Data Guide](https://docs.google.com/spreadsheets/d/1EOdWBPqk_NxFVa3_27CdD0cprfatvfqu/edit?usp=sharing&ouid=102542169710904108713&rtpof=true&sd=true) here.


Download the Final Merged File [Accident & Air Quality](https://docs.google.com/spreadsheets/d/1EOdWBPqk_NxFVa3_27CdD0cprfatvfqu/edit?usp=sharing&ouid=102542169710904108713&rtpof=true&sd=true) here.

# ABSTRACT
The purpose of this study is to consolidate previous research and provide insights to individuals or stakeholders working towards creating a safer and more sustainable transport system i.e. reducing the menace caused by road traffic accidents in the UK.
Adopting data source triangulation methodology, this study analysed the impact of environmental, road infrastructural factors and air quality on accident severity from 2018 – 2023 by following the CRISP-DM methodology, using a similar approach to a study conducted in Taiwan in 2022, this study uses ordinal logistic regression and the other research uses binary logistic regression, Furthermore, this study applied random forest machine learning algorithm to predict accident severity based on factors suggested from the best model during inferential analysis.
Ideal environmental conditions and road infrastructural factors recorded the highest number of accidents and casualties on all levels of accident severity, except for darkness–unlit lighting conditions, which resulted in more accidents. Furthermore, a correlation between sulphur dioxide and accident occurrence was noticed for all the years in this study, ozone correlates with the occurrence of accidents in some specific years too. The machine learning model predicted the occurrence of accident severity with 79.5% accuracy based on the factors from the inferential analysis. 
Using tableau visualisation and ordinal logistic regression model, this study helps shed more insight into the impact of environmental, road infrastructural factors and air quality on accident severity. Further studies are needed to examine the specific impact of sulphur dioxide on road users by triangulating the National Health Service data with the accident and air quality merged data to help develop preventive measures and create appropriate awareness for road users. 


## Dashboard
  ![Tableau dashboard A](/images/Dashboard_1a.png)
  ![Tableau dashboard B](/images/Dashboard_1b.png)

# INSIGHTS
More attention should be placed on ROAD B, more road safety measures should be put in place.
Junction controlled by authorized person is less likely to cause an accident, compared to use of stop sign and other things. Deploying more authorized people to Junctions could help to prevent the occurrence of accident more.
If road planners or urban and rural planners can devise a better road layout that does not include T-junctions or if the existing T-junctions could be modified to some other type of Junction, this could also help to reduce accident occurrence on the UK road.
Driving during darkness unlit is more of the driver’s responsibility, because the government is trying their best to light up all roads and streets. So in situation of unlit condition in darkness, the driver should not assume and follow the required road safety precautions. More awareness about this be done.
According to inferential analysis model, driver within the age band of 25-35 are less likely to get involved in accident compared to all other age bracket. The government could develop an automated road safety precaution article that is sent out like once every two months to anyone within other age band and once every quarter to people with the 25-35 age band. 
With the emergence of self-driving cars, training their algorithms with a data that is imbalanced and predicting a specific severity level before taking decision, could later lead to unforeseen disaster, and road traffic accident data is one of the potential dataset that could be used or already been used in training self-driving cars models, some biases due to imbalanced day could cost a lot. Although some studies suggested the use of SMOTE (Synthetic Minority Oversampling Technique) during machine learning. Which helps to generate synthetic examples of the Minority Class. The outcome of smote application to machine learning algorithm is an increased in RECALL (the overall model gets better) at the expense of Lower precision. Meaning more addition of the minority class prediction will be introduced and since it is synthetic in nature, part of the introduced class will be correct (helping to increase recall), and some of them will be wrong, which leads to (reduction in prediction) (Joos, 2022).

## Trend line of SO2 Sub-Index and All Accident in 2021 in the UK
![Tableau dashboard A](/images/Trendline_So2_Accidents.png)

# RESEARCH OUTCOMES
The finding from this study shows that there is an association between air pollutants (Sulphur dioxide and ozone ), bad lighting condition, first road class B, junction not controlled by an authorized person, junctions that are T-shaped, driver trying to overtake others,  and accident severity of all level. Good and perfect weather conditions records more accident than when it is raining or foggy, there is likelihood of accident severity of all level happening on dry road surface compared to wet and snow road surface.  
Drivers within the age-band of 25-35 are less likely to get involved in accident, Females are also less likely to get involved in an accident. Electric vehicle is less likely to lead accident.
The algorithm used for prediction works best for predicting slight accident severity, performs poorly for others, which is based on imbalanced nature of the dataset.
Unit increase in Air quality Index  could increase  accident severity by 0.36% while 
Unit increase in Sulphur dioxide could increase accident severity by 0.75%


# RECOMMENDATION
Enforce stronger emissions standards and air quality laws to lower pollution levels of sulphur dioxide and enhance air quality in metropolitan areas, especially area with high traffic congestions and encouragement of electric cars adoption.
Modifications of existing T-junctions to other type of junctions.
Deployment of more authorized personnel to control junction traffic.

# CONCLUSION
In conclusion, this study has provided a detailed analysis of impact of environmental, road infrastructural and air quality (pollutants) on accident severity. Using statistical analysis (where the null hypothesis was rejected for all the models), visualization with tableau and a comprehensive review of previous literature, the study has been able to point out the negative effect of sulphur dioxide, poor lighting condition in the darkness, and other road infrastructure like not having an authorized person at a junction, T-junction menace, class B first road type on accident severity and shows they contribute significantly to increase in accident at all severity level. It also went further to look into the age group with less likelihood of having accident (25-35) and the gender by that is less likely to get involved in accident (female).
The missing values and meaningless values could help to see some other hidden factors leading to accident but due to the volume of the data generated and with the help of artificial Intelligence algorithms it can be argued as not important. Nevertheless, considering the effect of bias on data analytics, this study would suggest that more attention should be paid to capturing of data accurately during accident and air quality measurement, over reliability on artificial intelligence could lead to missing out of small information that could help in reducing accident to the lowest level
Additionally, the study shows that road users tend not to be too careful when every conditions and circumstance seems to be okay. And this has resulted in more accident happening under ideal and perfect condition, which is more of a psychological effect. 
Based on the result from the Machine Learning Algorithm, this study believes that using ordinal logistic regression model is a better way of making inference on accident severity along all the level, rather than separating them and trying to predict the individual accident severity separately based on the data available that is imbalanced in nature. Accident is a menace, as stated in the literature review, whether slight, serious or fatal. Accident should be seen as accident and tackled together. 
More awareness should be given to the people and road users, about the pollutant observed in this study. Mitigating the effects of pollutants with planting of more trees initiative should be encouraged, reduction of vehicles that are not electric should be aided with government policies and as suggested by this study more authorized person should be placed at junctions, automated bi-monthly or quarterly article should be sent to all road user about road safety precautions.
According to the popular Data Analytics saying “CORRELATION DOES NOT EQUAL CAUSATION”. For future research, taking a deeper look into the specific effect of SO2 on road accident by combining road accident data, air quality data and National Health Service (NHS) data could give a deeper insight into effect of road users’ exposure to a very small amount of SO2 (even other pollutants) and occurrence of accident. Most of the previous studies have focused more on NO2 and PM2.5. Ozone is another pollutant that shows high correlation with road traffic accidents in the UK in some specific year. 
Further research into this area is needed, by Exploring the Effect of Green Infrastructure to Mitigate the Impact of SO2 on Road Accidents and Road Users could help give more precautionary advice to the people, road users and give them the appropriate awareness. Another area that can be researched more is adoption of the latest Large Language Models (LLM) like GPT-4-Omini /Deepseek (Multimodal Models) as an intelligent system in vehicles. The Large Language Models will be trained to detect driver’s behaviour and communicate with drivers their potential of being exposed to any pollutants that can lead to accident.
Finally, this project has added to the general understanding on the complex relationship between environmental, road infrastructural factors, air quality and accident severity, and has reveal some valuable insights for urban planners, transportation authority, policymakers on how to develop effective and strategical road safety precautions. For better awareness the research above should be considered and supported by the appropriate agencies.



## Contributing

The RAW DATA are gotten from 

[GOV.UK](https://www.data.gov.uk/dataset/cb7ae6f0-4be6-4935-9277-47e5ce24a11f/road-safety-data) AND

[KAGGLE](https://www.kaggle.com/datasets/airqualityanthony/uk-defra-aurn-air-quality-data-2015-2023)
