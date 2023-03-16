# QUT and Hastings Deering project

##### Note: N11096837-Final Report.pdf - The report itself.
#####       correlation.ipynb - A file contains code for correlation test.
#####       data dictionary.txt - Data dictionary.
#####       decision_tree.ipynb - This file contains code for a classification model(decision tree).
#####       exploratory_data_analysis.ipynb - This file contains code for exploratory data analysis.
#####       rainfall.ipynb - This file contains code for the visualisation of rainfall data.
#####       random_Forest.ipynb - This file contains code for a classification model(Random Forest).
#####       random_forrest_regressor.ipynb - This file contains code for a simple regression model(Random Forest regressor).
#####       usdollar.ipynb - This file contains code for the visualisation of US dollar Index.


Self reflection:
1. A regression problem is a regression problem, we cannot try to convert it to a classification problem.
2. The importance of exploratory analysis.
3. Depends on the situation, sometimes old method is better than new method.
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
This project was made in IFN703-Advanced Project, which is a unit in the 3rd semester. This is also my first practical project. A construction equipment dealership Hastings Deering provided us a piece of data, and asked us if we can add any external factors such as weather, social economic factor etc. to the data and analyse it, as long as the factor can be related to the data itself. This piece of data belongs to HD's Toowoomba warehouse, it's actually a series of repair transactions of their contractors. In another words, construction contractors buy machines from HD, and left records when they do maintenance and parts replacement in HD's warehouse. The data has 35146 rows and 12 columns including unique identifier, invoice date, postcode, customer market segment, product etc. The timespan of the data is from Dec 2019 to Dec 2021, which overlaped the main period of COVID-19 pandemic. According to the agreement between QUT and HD, I cannot upload the data to this platform.

During the research, my main focus was to find any financial factors that can help to analyse this data. I noticed the house price in Australia wide was skyrocketed especially in Queensland due to COVID-19 pandemic. Therefore, I used Producer Price Index of Queensland, Number of building approvals in Toowoomba, value of building jobs in Toowoomba, Monthly COVID cases in Toowoomba as my external factors. Producer Price Index is the quantified inflation from production side, the reason for house price uprising during the pandemic is because of the interuption of worldwide supply chain, which made the price of commodities and house price go up, thus inflation. Accoding to several housing market report by real state agency, the house price and the activity in real estate market significantly increased in Toowoomba during 2020, therefore I treated PPI as an indicator of house price here. I expected the number of repair transactions would increase due to the increase of real estate activity. Number of building approvals and value of building jobs can also be related to the activity of real estate market. Monthly COVID cases is just a factor for me to check whether or not there was any abnormalities in Toowoomba during the timespan. 

After an initial exploratory analysis, we found there is nothing really special in terms of monthly and weekly scale except holiday when people off the work, which probably cause the number of transactions decreased. My professor said this peice of data is a challenge because the data itself has no significant flutuation. Indeed, the accuaracy of classification was low, a series of indicators of regression also suggest that not a single factors can significantly contribute to the prediction, which means no feature is highly correlated with number of transactions. However, this piece of data let me realise that the practical situation will always be tougher than training, that is also why the exploratory analysis is important because we get to see an approximate full scale of the data in the first step. This experience also made me realise that Data Analytics itself as an advanced technique still has its limit in terms of real world utilisation. Depends on the situation, sometimes some boards will be much intuitive than fency techniques.
