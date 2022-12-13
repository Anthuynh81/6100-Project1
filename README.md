# Group Project for ITCS 6100
Git Hub Repository for ITCS 6100 Project

## Members
- He Zhao 
- An Huynh

## Communication Plan
We will get together at the library once a week. In the event that we go behind schedule, we have the option of increasing the total amount that we contribute in order to fulfill the target date.

## Business Problem or Opportunity, Domain Knowledge

The distribution of  used automobiles is at the heart of our company's operational challenge. In order to boost sales, we are planning to analyze data pertaining to used cars in order to determine which aspects of electric used cars have the greatest influence on sales. We want to investigate many different characteristics of the car, including as its range, speed, and acceleration, amongst other things, to determine what may be done to enhance sales.

## Dataset 
https://www.kaggle.com/datasets/ananaymital/us-used-cars-dataset

## Research Objectives and Question
1. Which groups of automobiles, in terms of the fuel types they use, have an average horsepower rating that is the highest across the board?

2. In a broad sense, what is the most typical size of the fuel tank that has the most significant amount of mileage on it?

3. Which car manufacturers, in general, have the best and worst ratings for their vehicles' fuel economy?

4. In general, what is the general tendency when it comes to the number of seats in a car versus the price?

# Deliverable 3
-------

#### Analytics, Machine Learning

For the purposes of designing and implementing the relevant insightful visualization graphs, as well as providing responses to the relevant questions that we have been asking from the very beginning stages of this project, we are making use of the Quick Sight Visualization Tool that is available through the AWS Academy.

**[Contents Will Be Posted on a PDF File That Will Be Shared Via Google Drive]**

-------
#### Evaluation and Optimization
https://docs.google.com/forms/d/e/1FAIpQLSf2hgc5hBMB1DMY3r35Twiq0S568WFvBjUZ9W6zCYSqSBxZDw/viewform?usp=sf_link
-------
#### Results

Future Work, Comments - students may want to consider the following questions

##### What was unique about the data?  Did you have to deal with imbalance? What data cleaning did you do? Outlier treatment?  Imputation?

Our data is unique is because cars selling are one of the trending topics in the USA nowadays, especially during this COVID-19 period, where the price of car chips are becoming increasingly high.  

No, we did not deal with imbalance. 

Yes, we have to filter the data, revise, and delete columns and rows in order to make the regarding predictations. 

We didn't treat outliers. 

We revised some rows of the data in order to proceed data analysis and data predications.

##### Did you create any new additional features / variables?

No, wo didnt create any new additional features or variables. 

##### What was the process you used for evaluation?  What was the best result?

Using Sage Maker Canvas to produce evaluations. 

##### Is there Bias in your work? What were the problems you faced? How did you solve them?

Yes. We did sampling by filtering the original dataset into a smaller dataset, which could end up being a bit biased. 

##### What future work would you like to do?

We would want to optimize the sampling dataset to reduce the bias, and use a better methodology on making certain predictations.

##### Instructions for individuals that may want to use your work

For those who want to user our work: 

1. Download our filtered dataset 
2. Run in through Sage Studio Canvas 
3. Creating models using the datas
4. Making predications using different methodolgies 
-------
#### Group members are also required to complete Final Group Project Evaluation (Individual).

# Deliverable 2

## Exploratory Data Analysis
During the data exploration phase, one of our goals was to investigate the data to see what aspects of the information would be helpful in achieving the goals and answering the questions of our research. The data set that we have on used automobiles comprises 67 different features, but the vast majority of these features won't be required in order to move forward with the project. With Sagemaker Data Wrangler, we have access to a tool called Insights On Data and Data Quality, which allows us to perform an analysis on the data and obtain information on each of these characteristics. I've attached a picture below showing the general dataset statistics that were generated regarding our data. It may be found below.

![image](https://user-images.githubusercontent.com/55640125/200463760-2f73c80f-e437-4bed-a4b0-5c639e344be4.png)

We are able to observe that many of these capabilities are not necessary and contribute very little to nothing of value to the overall analytics as a result of using the tool. Features such as bed are examples of features that we do not require. The feature summary reveals that only 0.688% of the rows are legitimate; this is one example of a feature that we do not require. I have added a picture of the findings to this post below.

![image](https://user-images.githubusercontent.com/55640125/200463935-a6bc4989-4ff3-4164-86ec-d16869cc6662.png)

In addition, we are able to observe that some of the characteristics in our tables require some more data cleanup, which consists of changing certain variables in order to provide improved data. This is demonstrated in the figure that follows, which illustrates the engine type feature.

![image](https://user-images.githubusercontent.com/55640125/200464166-bdcce68f-0d83-4cf5-a1db-6dd9e1b7ec1c.png)

It is clear from the image that some of the categories can and should be combined in order to provide a more effective management of issues such as outliers. In general, we are able to observe that in order to get ready for the subsequent stage of the project, a wide variety of elements, both old and new, will need to be eliminated or cleaned up.

## Dashboard
We came to the conclusion that AWS Sagemaker would be the best choice for our project's dashboard. We have included all of the various graphs that were generated in this github, and you can find them in the folder labeled "deliverable 2." The primary visual was derived from the Insight on Data and Data Quality tool, which provided us with comprehensive information on each of the attributes contained inside our table. The dashboard itself has feature summaries, in addition to frequency histograms that display the data. Additional visualizations that highlight the association between the primary characteristics of the data were also generated by our team.

## Data Preparation
We were able to modify our data using Sagemaker Studio by making use of the information that we obtained from Sagemaker Data Wrangler. This allowed us to get ready for the next phase of the project. In order to get the data ready, one of the first things that we did was to take some samples of the data. In spite of the fact that this could result in sample bias, the original data collection contained more than 3 million data points, which was far too many for our particular application. Given the restricted amount of money that we are able to spend and the increased amount of processing time required to handle such a large amount of data, we came to the conclusion that the best way to proceed would be to randomly choose 50,000 rows from the original data set. Following that, we proceeded to tidy up some of the columns on their own. Because many of the rows contained labels for the columns, the data were transformed into strings rather than the more straightforward numerical data. This made it more difficult to deal with the data. We cleaned up the data by employing SageMaker Studio's data flow in order to prepare it for use in the creation of graphs and other types of visualizations. Then, following the data exploration, we were able to locate many different features that either weren't used or are less essential in our overall study, so we used a similar procedure to delete them from the table. This was done after we had discovered these features. Following the completion of all of these procedures, our data ought to be ready for the next phase of the project. I have attached a picture that shows how it appears in SageMaker when you perform the transformations that were mentioned before in this paragraph.
![image](https://user-images.githubusercontent.com/55640125/200463332-1592554d-1c82-4edc-a166-0258bc46194c.png)

