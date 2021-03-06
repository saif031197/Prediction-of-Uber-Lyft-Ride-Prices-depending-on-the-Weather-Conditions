# Team Name: Data Scouts
### Team Members:
 
|Name     | 
|---------|
|[Sai Harika Paluri](https://github.com/harikapaluri)| 
|[Nikhil Kumar Mutyala](https://github.com/NikhilKumarMutyala) |    
|[Sree Divya Keerthi Paravasthu Siddanthi](https://github.com/SreeDivyaKeerthiPS) |    
|[Ravi Theja Goalla](https://github.com/wgaca007) |    
 
#  Project Title: Prediction of Uber Lyft Ride Prices depending on the Weather Conditions

## Project Description:
Uber and Lyft's ride prices are not constant like public transport. They are greatly affected by the demand and supply of rides at a given time. So what exactly drives this demand? The first guess would be the time of the day; times around 9 am and 5 pm should see the highest surges on account of people commuting to work/home. Another guess would be the weather; rain/snow should cause more people to take rides.

The data is approx. for a week of Nov '18 ( I actually have included data collected while I was testing the 'querying' application so might have data spread out over more than a week. I didn't consider this as a time-series problem so did not worry about regular interval. The chosen interval was to query as much as data possible without unnecessary redundancy. So data can go from end week of Nov to few in Dec)
The Cab ride data covers various types of cabs for Uber & Lyft and their price for the given location. You can also find if there was any surge in the price during that time. Weather data contains weather attributes like temperature, rain, cloud, etc for all the locations taken into consideration.
## Data:
The dataset contains 10 features along with the price for 693071 observations. Later we add few more derived features to this dataset.<br>
The description for the 10 features is given below:<br>

<img src="https://github.com/NikhilKumarMutyala/Prediction-of-Uber-Lyft-Ride-Prices-depending-on-the-Weather-Conditions/blob/master/DATA.PNG" width="450">

The date is in timestamp format. So we change that timestamp into date format, the date attribute is added to the dataset and timestamp attribute is removed. 



## CRISP-DM Process:
Cross-industry standard process for data mining, known as CRISP-DM, is an open standard process model that describes common approaches used by data mining experts. It is the most widely-used analytics model.

![alt text](https://github.com/NikhilKumarMutyala/Prediction-of-Uber-Lyft-Ride-Prices-depending-on-the-Weather-Conditions/blob/master/crisp%20dm.PNG)
*image credits: [Youtube](https://www.youtube.com/watch?v=CRKn-9gVNBw)*

This model is an idealised sequence of events. In practice many of the tasks can be performed in a different order and it will often be necessary to backtrack to previous tasks and repeat certain actions. The model does not try to capture all possible routes through the data mining process.
CRISP-DM breaks the process of data mining into six major phases:

* Business Understanding
* Data Understanding
* Data Preparation
* Modeling
* Evaluation
* Deployment

 ### Business Understanding
The first thing we must do in any project is to find out exactly what we are trying to accomplish. We must state objectives and requirements. We should translate these goals and restrictions into the formulation of a data mining problem definition. We must start with a clear understanding of
* A problem that you want to address/ Objectives
* The business goals
* Constraints
 Finally, we prepare a preliminary strategy for achieving these objectives.
 
 ### Data Understanding
The second stage of the CRISP-DM process requires us to acquire the data listed in the project resources. This initial collection includes data loading, if this is necessary for data understanding. The data-understanding phase includes four tasks. These are
* Gathering data
* Describing data
* Exploring data
* Verifying data quality

#### Gathering Data
We need to verify that we have acquired the data or at least gained access to the data, tested the data access process, and verified that the data exists. First we need to Outline data requirements, Verify data availability, Define selection criteria.

#### Describing Data
We describe the source and formats of the data, the number of cases, the number and descriptions of the fields, and any other general information that may be important.

#### Exploring Data
We look at the range of values and their distributions. We’ll use simple data manipulation and basic statistical techniques for further checks into the data. Data exploration supports several purposes:
* Get familiar with the data
* Spot signs of data quality problems
* Set the stage for data preparation steps

#### Verifying Data  Quality
Now we have to determine whether it’s good enough to support our goals. We will often have some quality problem to address yet still be able to move forward, but at times the data quality is so poor that it cannot support our plan and we’ll have to look for alternatives. 

### Data Preperation
The data preparation phase includes five tasks. These are
* Selecting data
* Cleaning data
* Constructing data
* Integrating data
* Formatting data

#### Selecting Data
We will decide which portion of the data that we have is actually going to be used for data mining. The deliverable for this task is the rationale for inclusion and exclusion. In it, we’ll explain what data will, and will not, be used for further data-mining work.

#### Cleaning Data
We make changes, perhaps tracking down sources to make specific data corrections, excluding some cases or individual cells (items of data), or replacing some items of data with default values or replacements selected by a more sophisticated modeling technique.

#### Constructing Data
We may need to derive some new fields.

#### Integrating Data
The data may now be in several disparate datasets. We’ll need to merge some or all of those disparate datasets together to get ready for the modeling phase.

#### Formatting Data
The may need to be formatted. Example, the date might be in int or float, we need to convert it into date format.

### Modeling
The modeling phase includes four tasks. These are
* Selecting modeling techniques
* Designing tests
* Building models
* Assessing models

#### Selecting Modeling Techniques
Classification: logistic regression, decision tree, random forest, gradient-boosted tree
Clustering: K-Means Clustering, Mean-Shift Clustering, Density-Based Spatial Clustering of Applications with Noise (DBSCAN)
Neural Network: Recurrent Neural Network(RNN), Convolutional Neural Network(CNN)

#### Designing Tests
Training data is used to fit mathematical forms to the data model, and test data is used during the model-training process to avoid overfitting. We should at least take care that our training and test data are similar and that we avoid introducing any bias into the data.

#### Building Model
Deliverables for this task include three items namely, Parameter settings, Model descriptions, Models.

#### Assessing Models
Deliverables for this task include two reports, Model assessment, Revised parameter settings.

### Evaluation
We evaluate not just the models you create but also the process that we used to create them, and their potential for practical use. The general evaluation metrics we use are Accuracy, Precision, and Recall, F1 Score, Log Loss/Binary Crossentropy, AUC-ROC Curve.

## Conclusion
Finally from the dataset we acheive useful insights based on pre-defined objectives.
