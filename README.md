cogs 108 final project for airbnb

# COGS 108 - Project Proposal

## Important

Make sure all group members (3-5 people) are listed in the group members section.

ONE, and only one, member of your group should upload this notebook to TritonED.

Each member of the group will receive the same grade on this assignment.

Keep the file name the same: submit the file 'ProjectProposal.ipynb'


## Overview

Read the project description and detailed instructions for this assignment in the 'ProjectOutline' document.

Group Members: Fill in the Student IDs of each group member here

Replace the lines below to list each persons full student ID. Add lines as needed for your group size, and make sure each ID is listed on a separate line.

A12906520

A14871746

A12829502

A11907392

A11198334

## Research Question

Is there a trend of pricing and satisfaction in respect to time?

## Hypothesis

As San Diego has a lot of beaches and is associated with warm climates, we predict higher pricings over Summer and lower over Winter. In addition, because people expect more over time, we predict a trend of decreasing overall satisfaction
Dataset(s)

Dataset Name: Airbnb san diego data

Link to the dataset: http://tomslee.net/airbnb-data-collection-get-the-data
        http://insideairbnb.com/get-the-data.html 
        
Number of observations: 152,368

The dataset contains information about Airbnbs in san diego from 2014 to 2017 including price, number of rooms, accommodations, neighborhood, room type, reviews, and overall satisfaction. 

The first dataset is more likely to give host based viewpoints while the second gives a little information as to the client perspective.

## Background and Prior Work

Why is this question of interest, what background information led you to your hypothesis, and why is this important?

Find some relevant prior work, and reference those sources. Even if you think you have a totally novel question, find the most similar prior work that you can and discuss how it relates to your project.

References can be research publications, but they need not be. Blogs, github repositories, company websites, etc., are all viable references if they are relevant to your project.

We chose this topic because we were interested in seeing how people give higher ratings to more expensive Airbnbs since typically, more expensive Airbnbs are nicer and thus people will give higher ratings. We were also inspired by the Uber wait time example provided in class, describing how the time clients were inclined to wait decreased by a minute each year. The example provides a sense that a customer’s expectations can change over time. We would like to see if such an effect is present for Airbnb since like Uber, it has many competitors has a very similar type of client host relationship.
The first reference provides data on predicting the most optimal price for Airbnb listings in New york. Furthermore, it relates to our research since we are focusing on how much people are willing to pay for an Airbnb with respect to ratings and time. The second reference provides data on Airbnbs in Boston. More specifically, it gives insight about prices in comparison to seasons and also an analysis utilizing Airbnb reviews.

### References:

1) https://github.com/samuelklam/airbnb-pricing-prediction 

2) https://github.com/ruchigupta19/Boston-Airbnb-data-analysis 

3)https://www.ftc.gov/system/files/documents/public_comments/2015/06/01912-96334.pdf This reference provides insight to the idea of customers changing over time due to competition. What happens between Uber, Lyft, and taxis, may be happening to Airbnb, TripKey, and hotels/motels.

## Proposed Methods

What methods will you use to analyze your data?

How 'clean' is the data? To the extent that it requires cleaning, how will you do so?

How will you analyze the data? Be as specific as you can. Briefly mention any pre-processing steps that are required for your methods (for example, checking data distributions and performing any transformations that may be required). Include a brief outline of how you will apply your chosen method(s).

What do you plan to report? Briefly mention any key visualizations you plan to create, and/or the kind of results you will be able to report that address your question (this could be, for example, the outcome of some statistical test(s), prediction error on a model, a model fit parameter, etc.).

Include a list of packages you expect to use for you project. If you plan to use packages we have not used in class, add a very brief description about them (a few words is sufficient).

Create graphs on price vs ratings

### Data Cleaning

The data is clean and organized into relevant columns. There are some unnecessary data that does not relate to our topic. Thus, we dropped columns to clean our data of useless info that we won't use in our research

### Data Analysis 

We will clean up our data and remove any missing values and read through our data to ensure that the encoding is correct. We will merge data tables and evaluate a popularity based on review rate and satisfaction score. We will then visualize our data by creating a graph that will measure rating and price over 2014-2017 in San Diego. If data is still too obscure, we may continuously separate data based on time and compare resulting graphs by their linear prediction models. We could possibly use scattermap if it is appropriate for comparing between time periods.

### What to report 

We will report any graphs we construct such as price vs. ratings. We will also include results of statistical tests and model fit parameters on whether satisfaction decreases over time. 

### Packages 

A) pandas will be used to process and analyze our data. 

B) Numpy will be used to clean up our data and get rid of the NAN values. 

C) matplotlib - we will use matplotlib to create graphs measuring the rating and price of the Airbnb from 2014-2017.
Ethics and Privacy

Briefly acknowledge and address any potential issues of ethics and privacy for the proposed project. In particular:
Do you have permission to use this data, for this purpose?

Are there privacy concerns regarding your datasets that you need to deal with, and/or terms of use that you need to comply with?

Are there potential biases in your dataset(s), in terms of who it composes, and how it was collected, that may be problematic in terms of it allowing for equitable analysis? (For example, does your data exclude particular populations, or is it likely to reflect particular human biases in a way that could be a problem?)

Are there any other issues related to your topic area, data, and/or analyses that are potentially problematic in terms of data privacy and equitable impact?

How will you handle any issues you identify?

We have permission to use this data since it is a public dataset and can be used for research projects

There are privacy concerns about our dataset since it contains longitude and latitude on each Airbnb, room id, and host id. However, the longitude and latitude are not accurate and can not really determine the exact location of the Airbnb.
 
 There may be potential biases since it gathers information about Airbnbs in certain neighborhoods of San Diego. The dataset could only contain a number of Airbnbs in specific neighborhoods instead of the entirety of Airbnbs in San Diego.

There are no other issues related to our topic that can be problematic in terms of data privacy

We will not use data that will violate any privacy concerns.

## Discussion

If our analyses and hypotheses are correct, we’ll be able to determine the relationship between pricing and satisfaction over the past few years in San Diego. Our data will predict when Airbnb prices in San Diego are cheaper at the expense of lower satisfaction levels, and vice versa. In addition, if certain overall trends discovered show negative impact for Airbnb, our data may provide evidence for a need of call to action. If our method doesn’t produce the results we were expecting, we will re-examine how we dealt with our dataset and the tools we used from python libraries to reach our conclusion. If we are confident in our data and our hypotheses are wrong, then we will conclude there is no relationship between pricing and ratings with respect to time. 

A potential issue with our data is the inconsistency in the dates. Some years like 2014 will have less data than other years like 2016, meaning we will be missing some data from some months in some years. Overall, we believe it will not have a big impact on our results because we still have over 150,000 observations to process. Even though we are missing some months from other years, we still thousands of data to observe. We also lack the data to interpret actual purchases to locations. We only have data based on the location’s information and how popular it is based on customer review. Further data is needed to investigate actual popularity and rental rates. Hence, this project is by no means an full interpretation of the client side of Airbnb.
