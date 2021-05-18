# Table of Contents

  - [Installation](#Installation)  
  - [Project Motivation](#Project-Motivation)
  - [File Descriptions](#File-Descriptions)
  - [Results](#Results)

# Installation

Even though it was used the pipenv library for environment configuration, all the packages used are available in the default installation of the Anaconda distribution of Python. The code should run without issues using Python 3. For a more detailed descrition of the envirement the requirements.txt and Pipfile are available in the project.

# Project Motivation

For this project, I was interested in using Stack Overflow Survey data from various years to better understand:

  1. If data science is a trending job. How is evolving the share of data scientists along the years.
  2. What distinguishes data scientists from other developers. What are the technological competencies and educational differences from those subpopulations.
  3. How these differences in technolofical and educational characteristics reflects into salary.
  
I belive that answering those question might be important for those, like me, are planning to make changes in their carrer and ingress in a data science profession.


# File Descriptions

  - **01 - DataScienceEvol.ipynb**: analysis of the evolution of the share of data scientists in the population of developers. 
  - **02 - DataScienceEnemployment.ipynb**: complementary to the first notebook a comparsion between unemployment rates between data scienctists and all the other developers.
  - **03 - DataScienceTechEdu.ipynb**: a comparison between data scientists and other developers educational and technological features.
  - **04 - SalaryPrediction.ipynb**: a multiple linear model with all the technological and educational categorical variables being used to predict compensation levels.

# Results

Even though we could not confirm that data science is still a proeminant profession, we could identify some important aspects regarding their technological and educational features. First, they are not like other developers, they usually have a higher educational level and use some technologies more specific to machine learning and big data. Even though most data scientists uses Python for their work, this language is not important for determining their compensation levels. In this sense, working with Python function more as a requirement than a competitive advantage in labour markets. Getting a doctoral, professional or master degree is what is really important for professional to achieve higher compensation levels.

A more detailed description of the results of this project can be readed in my Medium article [Path to Data Science](https://leonardo-fmr.medium.com/path-to-data-science-84dad09404ab)