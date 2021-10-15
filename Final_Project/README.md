# The Homelessness Crisis in the United States 

**Abstract:**

Today the United States is experiencing an extensive homelessness crisis. Homelessness has been increasing nationwide since 2016. Currently, roughly 570,000 individuals experience homelessness on a given day. Proper planning and resource allocation is a difficult process to forecast and is extremely important in reducing the number of individuals experiencing homelessness. The objective of this analysis is to collect a broad range of socioeconomic data for each state within the United States over a 14 year period. The goal is to create a time series model that can predict the number of homelessness individuals in the years to come. With the ability to predict these population sizes better planning and resource allocation can take place. A tableau dashboard was created to consolidate all of the socioeconomic data in one location. This dashboard gives the user the ability to monitor these features over time and make comparisons between states. Some of these initial findings showed that Massachusetts has had a decline in their homeless population since 2018, going against the nationwide trend. One factor hypothesized to be playing a role is the public welfare spend per capita. Massachusetts has had a steady increase in their welfare spend year over year, whereas other more impacted states have had a stagnate or decreasing welfare spend.

**Design:**
In 2020, roughly 570,000 individuals experience homelessness on a given day. There is a great need to understand how one becomes homeless and what factors play into and increase the homeless population. 

**Impact hypothesis:**
We hypothesize that predicting and understanding the future size of the homeless population by state will give the ability to better allocate resources. With this data NGOs can target states that are predicted to have an increasing homeless population and send more aid. 

**Primary Impact:** Predict which states will have an increasing population of homeless individuals.

**Secondary Impact:**
Prevent the growth of homeless populations through the use of the prediction data by allocating resources more effectively and with greater accuracy. 

**Suggested Solution Path:**
Create a time series analysis from available homeless statistics to determine which states are in the greatest need of assistance.

**Other Possible Solution Path:**
Create a categorical model that defines what attributes lead to homelessness to try to reduce the number of people becoming homeless in the first place.

**Measures of Success:**

Technical: High model accuracy is imperative. If the model under predicts what the true homeless population will be in future years, resources can’t be taken from that state prematurely. This could ultimately make the problem worse in that state.

Non-technical: The true homelessness size is roughly the same as the predicted size for the first few years. As time progresses the goal is to see these numbers trending downwards, meaning that resources are being utilized and are working.

**Data:** The socioeconomic data for the analysis was collected from many different government websites including, but not limited to the U.S. Bureau of Labor Statistics, the U.S. Department of Housing and Urban Development, the Bureau of Economic Analysis, and Census.gov. The main target variable for this data set was the homeless data. The homeless data was available over a 14 year period from 2007 to 2020 and aggregated by state. All other data collected follow the format of the target data. 

**Algorithms:**

**Cleaning and EDA:**
Python, Google Sheets, were used for data analysis. The initial step was creating a pairplot of the features to see if there were any obvious trends in the data. Much of the data was not on scales that were comparable because states vary so differently in population size. In excel, vauls like number of homeless people and tax revenue were normalized by population to make values comparable.

**Aggregation:**
Data was then aggregated into pivot tables. To draw more meaningful conclusions two states were compared, Washington and Massachusetts. Using pivot tables, homelessness data and public welfare spending data was pulled out for each state and each year. Comparing homelessness data showed that from 2018 to 2020 Massachusetts had a decline in their homeless population, going against the nationwide trend. Washington followed that trend. One factor that could play a role in this is the state's public welfare spending per capita. Massachusetts has had a steadily increasing public welfare spend, whereas Washington’s had been going up and down. 

**Visualization:**
The Tableau dashboards can be accessed [here](https://10ay.online.tableau.com/t/stephenblount/views/HomelessnessAnalysis/Dashboard1/6e14483c-d66f-40b8-97dc-1ce2e4e47007/b71f12f0-affa-463b-8336-7919fb6be8aa?:display_count=n&:showVizHome=n&:origin=viz_share_link ) & [here](https://10ay.online.tableau.com/t/stephenblount/views/HomelessnessAnalysis/BarDashboard?:showAppBanner=false&:display_count=n&:showVizHome=n&:origin=viz_share_link). The charts presented on the dashboard show the total percentage of each state that is homeless over time and the percentage by which the homeless population increases or decreases over time. Additionally, the first chart contains useful socioeconomic data within the details.






