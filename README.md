# Nigeria-COVID-19-Data-Analysis-Using-Python

Data Scientist Microdegree Capstone Project- Ustacky 

This project is a detailed analysis of datasets correlated to Covid 19 in Nigeria.
Here i was able to collect data, clean, process,and analyse it to get insights on the Outbreak of the Covid 19 and its effects in Nigeria.

This major steps can be Compunded in just 3

# 1) Data Collection.

First step was clearly to fork and clone the data sets from Ustacky github as advised. I did web scrapping on the Ncdc site which involved using the pandas read .html(url) function to extract data from the site.

Budget data set,covid 19 external data set,Real gdp was also extracted using pandas read .csv format.

#Budget data set contained prior and revised budget of Nigeria segmented in states.
#Covid 19 external data set contains population density,overall vunerability index and many more.
#Real gpd contains quartely(Q1-Q4) GDP of nigeria from 2014 to 2020

I also collected data for John Hopkins Repository which contained daily confirmed,recovered and death cases across 275 countries of the world. i used pandas read .html(url) format to extract the data.

A total of 7 datasets was considered and used for analysis in this project.

# 2) Data Cleaning and Preparation.
All data set was check for or explored for basic information using basic functions like df.head() to preview dataset, df.info() to see information on the dataset, df.isnull() to check for empty or null columns and rows and df.duplicated() to check for duplicate values

Particularly on the data we extracted from Ncdc website we had quite alot of duplicated values which sumed up the rows to be 54 instead of 37. I used the df.duplicates() to drop the duplicated row across all colums.
I also renamed the column headers or name on the Ncdc dataset using df.rename()

i was also able to extract daily recovered,confirmed,death cases from John Hopkins Repository for only Nigeria.

# Data Analysis
From Ncdc dataset, a total visualization of 3 Barplot was done to derive insights from our data considering top 10 states with Confirmed, Recovered and Death cases Respectively.

Using the John Hopkins data and line plot i was able to get daily infectious rate and many more.

I also merged my Ncdc data set and Covid 19 external data set using pandas merge function pd.merge() to be able to compare Confirmed Cases and the overall community vulnerability index, Relationship between Recovered cases and Death Cases and Confirmed Cases against Population to get joint insights from the data.

# Insights
1) The 23rd day  January 2021 recorded the maximum infection as regards to days.
With regards to the Confirmed cases Lagos, Fct, Rivers, Kaduna, Oyo, Pleatue, Edo and Ogun State had the highest 2)Confirmed cases. This clearly means that there was high rate of infection in the aformentioned states. 
2) Lagos,Fct,Rivers, Kaduna, Plateau, Oyo has the most discharged cases as seen in our barplot for discharged cases to this effect these states were able to manage the disease to a height.
3) Lagos, Edo and Oyo lost had the maximum deaths count as recorded across all states
4) Population density for all the confirmed cases is hovering around 0.0 to 1.0
5) Majority of the confirmed cases across all population density were below 10,000 aside from few as seen from the graph
6) Lagos states has the highest population and Confirmed cases of Covid 19
7) Ondo and Akwa Ibom has the Highest Confirmed cases 
8) Fct has a small Population with a very high Confirmed case.
9) There was a great decline in Nigeria's GDP as seen in Quarter 2 of 2020 which was exactly when Covid 19 hit Nigeria, it was noted that there was reduction in employment rate which directly let to increase in unemployment rate.

# Conclusion

The novel coronavirus spread so rapidly that it has changed the rhythm of the globe. Whether from the perspective of a single country Nigeria or multilateral levels, the solidity of international relations has been put under test. The most obvious consequences include economic recession, a crisis of global governance, trade protectionism and increasing isolationist sentiment. People-to-people, cultural and travel exchanges have all been restricted. Nigeria  felt this on high side particularly in 2020 and this impacted negatively on both the population and economy as well. The ignorance and population in some state led to increase in those states.

Finally this project has widened my horizon on knowledge of covid 19 and its impact in states and Countries at large. It has also helped me to understand better ways of using Google and its platforms to research on methods and solutions to problems.



