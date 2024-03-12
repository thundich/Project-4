# Project-4

Tamara Hundich

03/12/2024

Michigan State University edX Data Analytics Bootcamp 

# Introduction 
The main objective for this group project was find a dataset and use our machine learning skills to analyze, solve, or visualize a problem of our choice. I originally chose to predict the sales price of the home based on the dataset that was found on Redfin. However, while prepping the data for linear regression, the sales price of the home was not constant. The sales price varied and was not able to be determined. After determining the sales price was not constant, I decided to change to a more categorical approach and whether the dataset could predict the correct property type.  

# Installation 
The following applications were required to be installed for this Project: 
- PG Admin 4/Postgres, Pandas, Python, sklearn, tensorflow, distutils. 

# Configuration 
The orignal dataset was created by importing the data into Postgres SQL. An ERD table has been provided showing the relationship, with the query tables. After placing in Postgres SQL to create an updated CSV table, Python was used to created 3 different models to determine which model would be the most succesful in determining the property type: clustering, linear regression, and neural network. 

# Data Resources/References: 
https://www.redfin.com/news/data-center/

# Analysis 
There were a total of 35,424 records in this dataset. Of this dataset, 1,417 had null values which needed to be removed. These null values were removed using Python. With 5 variables for the property type: multi-family, condo, townhouse, all residential, and single family resident. The closest analysis results was from the linear regression model. However, even with this model creation, the required results of 75 accuracy was not met. The highest accuracy rating was at 50% accuracy. The neural network model was then created. Even after multiple attempts of dropping columns, adding an additional layer, and even changing the activations, the maximum accuracy was 20%. Once the accuracy came back, I created the Kmeans clustering model. The Kmeans cluster model showed that before transformation, those that were in cluster 0 had the highest median sale price based on the property type. Based on the models created, it was determined that the dataset that was found was not able to produce desirable results. 

# Future Exploration 
If more time had been permitted, would have done more research to see if a different dataset would have achieved a better outcome. Overall, the best result came from linear regression model as with 5 variables to determine the property type, the result came back at 50%. 