# Data_Scientist_Starbucks_Capstone

This project is part of my Data Sciene Nanodegree project by Udacity. There is also a respective blog post on [Medium](https://medium.com/@n.van.bracht/boosting-effectiveness-of-promotional-offers-for-starbucks-customers-8f11a86808c0)

## Libraries
The developer needs to import the following libraries to run the analysis:
- numpy 
- pandas 
- matplotlib
- sklearn
- seaborn 
- datetime
- math
- json

## Motivation for project
When looking at different datasets for that project, the Starbucks one caught my attention since I personally often get swamped by promotional offers and I am also wondering which of those are actually effective to whom.

My goal is to implement a recommendation engine that supports the user to customize their promotional offer and maximizes its effectiveness. 

## Dataset
The analysis uses the a dataset provided by Starbucks/Udacity. It includes the following three files.

- **portfolio.json**: containing offer ids and meta data about each offer 
- **profile.json**: demographic data for each customer
- **transcript.json**: records for transactions, offers received, offers viewed, and offers completed

## Result summary
-	An accuracy of 68% of our base model indicates that it is possible to predict the effectiveness of promotional offers with machine learning.
-	Random forest turns out to be applicable for our binary classification task.
-	The results seem to be robust regarding parameter tuning.
-	Only a limited number of features (mainly customer demographic data) seem to be important.

Please check out my [notebook](https://github.com/nikextens/Data_Scientist_Starbucks_Capstone/blob/main/Starbucks_Capstone_notebook.ipynb) for the detailed findings!

My research is not without limitations. The findings here are observational, not the result of a formal study. 
- There are entries with missing data (i.e., NaN values) in the customer demographic data, which I drop as a simplification. I would recommend having a second look whether it makes sense to keep those data points and improve the model by also anticipating incomplete information.
- As we dedicate one part of the result section to feature importance, it also makes sense to not only look at the built-in feature importance but also check Shapley values of the features that sometimes provide additional insights.
- In a next step, I would conduct a proper hypertuning of the parameters. An effective technique to use is GridSearch

## Acknowledgments
I thank Starbucks/Udacity for providing those data!
