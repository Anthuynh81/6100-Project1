# Group Project for ITCS 6100
Git Hub Repository for ITCS 6100 Project

## Members
- An Huynh
- He Zhao 

## Communication Plan
Meet once a week at the libary. If we get behind, we can increase the amount we meet in order to hit the deadline.

## Business Problem or Opportunity, Domain Knowledge

Our Business Problem relates to the sale of electric cars. In order to increase sales, we want to look at electric car data in order to see what features of electric cars have the biggest impact on sales. We want to look at many different aspects of the car from range, battery capacity, speed, acceleration, etc to see what can be done to increase sales.

## Dataset 
https://www.kaggle.com/datasets/ananaymital/us-used-cars-dataset

## Research Objectives and Question
1. Which car model is the most affordable to buy while still having the best overall fuel efficiency? 

2. What type of relationship does the price have with the miles per gallon? 

3. Given that different cities have varying average fuel efficiencies, which city has the highest and lowest average fuel efficiencies? And which automaker is popular in those cities? Exist any relationships at all? 

4. Is there often a relationship of any type between the top speed, the acceleration, and the cost of the vehicle?
This is the questions i come up with for our group proj

# Deliverable 2

## Exploratory Data Analysis
For data exporation, we wanted to look into the data to see what was going to be useful in answering our research objectives and questions. Our data set on used cars has 67 different features and most of these features won't be necessary in moving forward with the project. Using Sagemaker Data Wrangler, we can use their Insights On Data and Data Quality tool to be able to analyze the data and get information on each of these features. Below I've attached an image of the general dataset statistics generated about our data.
![image](https://user-images.githubusercontent.com/55640125/200463760-2f73c80f-e437-4bed-a4b0-5c639e344be4.png)

From the tool, we are able to see that many of these features are unnecessary and provide little to no value to the overal analytics. Some example of features we don't need are features like bed, which in the feature summary shows that only 0.688% of the rows are valid. Below I've attached an image of the results.

![image](https://user-images.githubusercontent.com/55640125/200463935-a6bc4989-4ff3-4164-86ec-d16869cc6662.png)

Additionally, we are able to see that some features in our tables need some additional data cleanup in which different values can be changed to create better data. This can be seen in the graphic below showing the engine_type feature.

![image](https://user-images.githubusercontent.com/55640125/200464166-bdcce68f-0d83-4cf5-a1db-6dd9e1b7ec1c.png)

In the graphic, we can see that some of the categories can and should be consolidated to help better handle things like outliers. Overall, we are able to see that a lot of different features need to be removed or cleaned up in order to prepare for the next part of the project. 

## Dashboard
For our dashboard for the project, we decided used AWS sagemaker, Attached in the deliverable 2 folder in this github, we have the different graphs that were generated. The main visual comes from the Ingiths on Data and Data Quality tool which gave us indepth information on each of the features within our table. The dashboard istelf has feature summaries as well as frequency histograms of the data.

## Data Preparation
Using the data we gained from Sagemaker Data Wrangler, we are able to use Sagemaker Studio to transform our data to prepare for the next step in the project. One of the first things that we did in order to prep the data is to sample the data. Although this might create sampling bias, the original data set had over 3 million data points which is too much in our use case. With out limited amount of money that we can spend and the increased processing time to process so much data, we decided to random sample 50,000 rows from the orginal data set. Then, we went ahead and cleaned up some of the columns itself. Many of the columns had labels within the rows which made the data become strings instead of the numerical data which is easier to work with. Using the data flow from SageMaker Studio, we cleaned the data so we could use it to create graphs and other visuals. Then, after the data exploration, we were able to find many different features that weren't used or are less important in our overall analysis so we used a similar process to remove them from the table. After all of these steps, our data should be prepared for the next step in the project. Below, I have attached an image of what it looks like in SageMaker to do the transformation said earlier.
![image](https://user-images.githubusercontent.com/55640125/200463332-1592554d-1c82-4edc-a166-0258bc46194c.png)

