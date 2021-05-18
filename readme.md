# Table of Contents

  - [Business Understandingn](#Business-Understanding)  
  - [Data Understanding](#Data-Understanding)
  - [Prepare Data](#Prepare-Data)
  - [Data Modeling](#Data-Modeling)
  - [Results](#Results)
  - [Deployment](#Deployment)
  - [Installation](#Installation)
  - [File Descriptions](#File-Descriptions)

# Business Understanding

Data science was predicted as the [most promising job of the 21st century](https://hbr.org/2012/10/data-scientist-the-sexiest-job-of-the-21st-century). As such it is supposed to attract a lot of professionals trying to change their careers. For those, it can be important to know upfront what are the key requirements to work as a data scientist, and what can help you to be data scientist of success. In this article we will tackle some of those points. More specifically we will try to understand the following points:

  1. If data science is a trending job. How is evolving the share of data scientists along the years.
  2. What distinguishes data scientists from other developers. What are the technological competencies and educational differences from those subpopulations.
  3. How these differences in technolofical and educational characteristics reflects into salary.
  

# Data Understanding

To answer those questions we will be using data from the [Stack Overflow Survey](https://insights.stackoverflow.com/survey/2020). This is one of the largest worldwide survey involving primarily, people who codes. It is already a stablished and tradition initiative in the area that is running for almost a decade. In the year of 2020, the survey involved nearly 65,000 respondents.

The survey include a great set of questions. Of interest for this project are the questions regarding the developer types that best describe the respondents, technologies that they have worked with, compensation levels, educational level and declared undergraduate major.

With the exception of the compensation levels, all the other used variables are of categorical type. The compensation used for the analysis is the one that was already standardized by converting all the values to annual dollars.
# Prepare Data

To fit a linear model, we selected from our data only the developers declared to be data scientists, and removed observation with missing information in the compensation levels variable. All the categorical variables were one-hot encoded. Missing information on those dummies generated variables was 0 inputed (representing the absense of the feature). To improve the linear association of our selected independent variables we took the log of our compensation values. 

# Data Modeling

Along the project we used descriptive analysis to answer the first and second questions. The third question was answered by a multiple linear regression model using ordinary least squares. We used dummies generated from the selected technological and educational categorical variables as our independent variable, and the log of the compensations levels as our dependent variable. With the aid of variance inflation factor we removed one of the dummies features in order to reduce multicolinearity. 

# Results

Even though we could not confirm that data science is still a proeminant profession, we could identify some important aspects regarding their technological and educational features. First, they are not like other developers, they usually have a higher educational level and use some technologies more specific to machine learning and big data. Even though most data scientists uses Python for their work, this language is not important for determining their compensation levels. In this sense, working with Python function more as a requirement than a competitive advantage in labour markets. Getting a doctoral, professional or master degree is what is really important for professional to achieve higher compensation levels.

# Deployment

The main findings of this project are presented in my Medium article [Path to Data Science](https://leonardo-fmr.medium.com/path-to-data-science-84dad09404ab)


# Installation

Even though it was used the pipenv library for environment configuration, all the packages used are available in the default installation of the Anaconda distribution of Python. The code should run without issues using Python 3. For a more detailed descrition of the envirement the requirements.txt and Pipfile are available in the project.

# File Descriptions

  - **01 - DataScienceEvol.ipynb**: analysis of the evolution of the share of data scientists in the population of developers. 
  - **02 - DataScienceEnemployment.ipynb**: complementary to the first notebook a comparsion between unemployment rates between data scienctists and all the other developers.
  - **03 - DataScienceTechEdu.ipynb**: a comparison between data scientists and other developers educational and technological features.
  - **04 - SalaryPrediction.ipynb**: a multiple linear model with all the technological and educational categorical variables being used to predict compensation levels.