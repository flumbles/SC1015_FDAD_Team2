# SC1015_FDAD_Team2
1. Koh Huei Shan Winnie
2. Lee Jedidiah
3. Firdaus Khan Bin Feroz Khan
   
# Research Context
 In recent years, there has been an evident increase in Anemia amongst children in Singapore. As seen in figure 1, a study conducted by World Health Organisation(WHO), there has been a substantial increase in Anemia amongst children under 5 years old in Singapore. Hence, to tackle this growing concern, we decided to investigate the factors affecting children Anemia levels in Nigeria, a country where anemia amongst children is prevalent. By doing so, we hope to be able to gain a better understanding of the factors that affect the level of Anemia amongst children and also create a model to predict the Anemia level of children accurately.
 
 ![Anemia Singapore](https://github.com/flumbles/SC1015_FDAD_Team2/assets/128465695/80ab85be-793c-4bfe-8da7-82bb0b061d94)


## Problem Definition/Practical Motivation
1) Understand the important factors that affect the Anemia Level of Children
2) Predict the exact Anemia Level of a child.

# Notebook Details

  We split our original notebook into 2 as it was too big to place into github.
  ## Jupyter Notebook #1 - (EDA1015_first_part.ipynb) Data cleaning and Basic Visualisation
  In this first notebook, we first clean the dataset - clearing rows with NULL child anemia levels, as well as removing variables that are extremely skewed. 
  Then, we started visualising our dataset. We first looked at the distribution of each variable, as well as used some new visualisation methods that we learnt from Plotly. 
  
  ## Jupyter Notebook #2 - (EDA1015_second_part.ipynb) Exploratory analysis
  Here, we looked at the relationships of each variable with Child Anemia Levels. 
  We used different visualisation methods such as the use of bar charts, sunburst charts, violin plots and box plots. 
  Lastly, we made use of the mosiac plot to look at the actual percentages of each Child anemia level against the different variables.
  
  #### Machine Learning

  ## Jupyter Notebook #3 - (RandomForestML.ipynb) Random Forest
  *a. Random Forest*
  
   1) Using all the predictors, build a Random Forest Classifier to predict 'child_anemia_level'
   2) Check the OOB score and Classification accuracy of the model (Obtain HIGH accuracy)
   3) Obtain feature importance
   4) Observed that one predictor to be very significant. Use single decision tree to obseve the predictor
   5) Repeat the Random Forest model without this predicor to observe feature importance once more

         
  *b. Support Vector Machine*

 ## What we have learnt from this project?
   
   *a. New Visualisation Methods*
   
   1) Mosiac Plot -  Offers a perspective to observe correlations between categorical datas similar to assessing correlations between numerical variables
   2) Plotly Exprees - Craft more engaging and interactive visualizations, enhancing data exploration.

      
   *b. Random Forest Model*
   
   1) Establish nonlinear relationships within categorical data
   2) Assess feature importance
      
   *c. Support vector*
   
   1) Recognise signs of overfitting in data 


  ## References
   1) https://www.geeksforgeeks.org/how-to-convert-categorical-variable-to-numeric-in-pandas/
   2) https://saturncloud.io/blog/how-to-convert-categorical-data-to-numerical-data-with-pandas/
   3) https://stackoverflow.com/questions/52404971/get-a-list-of-categories-of-categorical-variable
   4) https://towardsdatascience.com/random-forest-in-python-24d0893d51c0
   5) https://www.datacamp.com/tutorial/random-forests-classifier-python
      
