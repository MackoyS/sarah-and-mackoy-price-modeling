# Every Door Real Estate - Educating Clients About Sale Price and Pre-Approval Process
This repository was created to help educate home buyers understand sales price and the attributes that most contribute to its variance. The data used is from 2014-2015 for houses sold in King County, Washington. The original stakeholder goal for our hypothetical client, Every Door Real Estate, was to come up with a model to help analyze what attributes most impact the sales price of a home. This way they could help their clients prioritize the features most important to them, so that they could understand what impact those features had on the sales price of the home. Through our analysis, Specs Consulting was able to come up with several features that Every Door agents can talk over with their clients.

# Bottom Line Up Front
The team’s statistical analysis discovered several attributes that agents and home buyers need to keep in mind as they start their home search.
 1. Construction Grade
 2. Square Footage
 3. If the property is located in Seattle proper
 4. If the property is on a waterfront
 5. Square footage of the 15 closest homes

## Business Understanding
The business problem at hand is that Every Door Real Estate (our stakeholder) is wanting to help better prepare their clients for the home buying process. Part of that process involves getting pre-approved for a home loan through a lender. Many of Every Door’s agents would like to provide their clients with a model that shows how property attributes affect sales price. That way clients can better understand how much their pre-approval needs to be for their dream home. 

## The Notebooks
The technical lead on this project operated out of the main branch, while their teammate primarily assisted through paired programming and EDA of the documentation. The main files for this data set can be found in SpecsProject.ipynb

## Data Cleaning
The data set kc_house_data.csv is the sole data set used for Specs Consulting’s statistical analysis. This data set provided excellent information including: price, square footage, zip code, waterfront, and several other important attributes to know when purchasing a home. After the data set was cleaned and had the outliers removed, the team was able to start their model analysis.

# Model Analysis
## EDA
For our initial Data Analysis, the team decided to look at certain series and look at them to see if they had any relationship to price. Some of the attributes we looked at were construction grade, if the property was on the waterfront or not, and square footage of the home.

![graph1](./images/graph1.png)

![graph2](./images/graph2.png)

![graph3](./images/graph3.png)

## Baseline
The team's baseline model is based off of the mean of our cleaned data set, which was a property sales price of ~$489,000. This essentially gives us the bare minimum number when it comes to telling home buyers what to expect when purchasing a home. The team then moved on to a simple model to start adding in specific home attributes.

![graph4](./images/dummy_model.png)

## Simple
For the simple model, the team used construction grade and square footage of the home. This model showed that ~44% of sales price variance is caused by these two attributes.

![graph5](./images/model_6.png)

## Best Multiple
For our best model we went to the attributes for the construction grade, square footage of the home, if it was on the waterfront, square footage of the 15 closest homes, square footage of the home above the basement, and a feature stating if the home is in the city or not. This model showed that ~52% of sales price variance is caused by these attributes.

![graph6](./images/model_best.png)

# Conclusions
For the agents of Every Door, it is important that they help educate their clients by explaining to them how certain attributes will affect their potential home purchase. The main values to keep an eye on are the construction grade, the square footage, if it’s on the waterfront, the comparable properties in the area, and if it is in the city or not. Equipped with this knowledge, home buyers can better prepare themselves for their home buying journey.

## Future Investigations
During our exploration of the King County data set, the team became interested in other potential insights, but as they were outside of the scope of this project, the team created a list so that they could potentially dive into them in the future. Three of those insights are: Incorporating household income into our model to help create a predictive model for pre-approvals, localizing the model down to the neighborhood level, analyzing the relationship between remodeling and sales price over the last 10 years.

## For More Information
Please review our full analysis in our [our Jupyter Notebook](./SpecsProject.ipynb) or our [presentation](./presentation.pdf).
For any additional questions, please contact **Sarah Jack | sajack2000@gmail.com, Mackoy Staloch | mackoy.staloch@gmail.com**

## Repository Structure
```
├── README.md                        <- The top-level README for reviewers of this project
├── SpecsProject.ipynb               <- Narrative documentation of analysis in Jupyter notebook
├── presentation.pdf                 <- PDF version of project presentation
├── data                             <- Both sourced externally and generated from code
└── images                           <- Both sourced externally and generated from code
```
