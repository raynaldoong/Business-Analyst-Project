# Introduction

This project is aimed to evaluate the success probability of future startup based on 100k+ historic startup data via Python. This project includes:
1. Explatory data analysis
2. Data cleaning 
3. Data Transformation (Pandas + Numpy)
4. Data Visualization (Matplotlib + Syborn)
5. Data Analysis 
6. Machine Learning Model (Logistic Regression + XGBoost)

# Findings
From the analysis section we can see that certain industries, especially the technology-led industries are populated with more startups and more startups receive funding as compared to start ups in less technologically advanced sectors before 2013. We also saw that the majority of successful companies were completing more milestones than their
counterparts although their variability was higher. Adittionally, we understood that the country with most startups is the US and in other economicly strong countries.
From the ML models we confirmed our analysis that technological companies effect the probability of success as well as the assumption made from the analysis that funding rounds are negatively correlated to success. Although the Logistic Regression algorithm was not a good solution to the problem, the XGBoost algorithm shows promising results
that need to be explored further and create a commercializatble tool for VC funds to assess incoming stratup's success.

# Limitation
We removed the majority of our data - ‘operating’ startups in the cleaning stage which leads to the possibility of our data being skewed as we are excluding potentially successful startups. Operating might not necessarily mean that they are not successful, but might mean that founders have a different vision for the path of their business and might
still want operating control over the business. We could have ommitted this limitation by exploring the dataset further given more time.
The founding and closing dates have been removed due to missing values. These columns and other date columns could have provided insight about the years of operating the start up and we could have achieved it through reducing the dataframe further to less than 10 thousand values. The limitation could be ommited by gathering more data and
time to explore.
We decided to not explore the rest of the date attributes (like first and last funding rounds) as some company might get a funding round in a short period of time compared to the inital funding round due to it being easier to get rounds if someone has already invested. This is a limitation to our project because we could ave gained additional insight
about a company's performance. This limitation could be ommited by feature engineering the date variables and performing futher analysis in the future.

# File
1. MSIN0413_2021_Group_M2.ipynb = Jupyter Notebook file for the project
2. VC Startup BA.pdf = PDF Version of Notebook
3. Cleaned_Data.csv = Data used for analysis (after cleaning)
4. Obtained Data = https://www.kaggle.com/justinas/startup-investments?select=offices.csv
