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

  ## Exploratory Data Analysis / Visualisation 
  We split our original notebook for Exploratory Data Analysis into 2 as it was too big to place into github.
  ### Jupyter Notebook #1 - (EDA1015_first_part.ipynb) Data cleaning and Basic Visualisation
  In this first notebook, we first clean the dataset - clearing rows with NULL child anemia levels, as well as removing variables that are extremely skewed. 
  Then, we started visualising our dataset. We first looked at the distribution of each variable, as well as used some new visualisation methods that we learnt from Plotly. 
  
  #### Jupyter Notebook #2 - (EDA1015_second_part.ipynb) Exploratory analysis
  Here, we looked at the relationships of each variable with Child Anemia Levels. 
  We used different visualisation methods such as the use of bar charts, sunburst charts, violin plots and box plots. 
  Lastly, we made use of the mosiac plot to look at the actual percentages of each Child anemia level against the different variables.
  
  ## Machine Learning

  ### Jupyter Notebook #3 - (RandomForestML.ipynb) Random Forest
  *a. Random Forest*
  
   1) Using all the predictors, build a Random Forest Classifier to predict 'child_anemia_level'
   2) Check the OOB score and Classification accuracy of the model (Obtain HIGH accuracy)
   3) Obtain feature importance
   4) Observed that one predictor to be very significant. Use single decision tree to obseve the predictor
   5) Repeat the Random Forest model without this predicor to observe feature importance once more

  (Might want to insert reason why SVM was split into 2?)
  ### Jupyter Notebook #4 - (SVM_testmodel.ipynb) SVM Test Model Pt.1
  *b. Support Vector Machine*
  
  For the support vector machine, we created 2 different models. The first one was using our cleaned data set that we generated from the model. However, with the insights provided by our random forest tree, we wanted to enahnce our project. This led to us developing a second model where we used the top 3 predictors from our random forest tree as our predictors for child anemia. For easy readibility, we decided to seperate the jupyter notebooks, with one for each model. 

### Jupyter Notebook #4 - (SVM_testmodel.ipynb) SVM Test Model Pt.1
  In this model, we used our entire clean dataset as predictors, less child anemia level 
  1) Using all the predictors, we first decided the most suitable kernel. In this case, it was the linear kernel
  2) We trained our model, using 80-20 splits and calculated the accuracies
  3) Our model performed very well, which led us to test for overfitting
  4) Through different test, our model was not overfiited

With this knowledge, we went on to develop our next model, to see which model is more accurate

  ### Jupyter Notebook #5 - (SVM_testmodel2.ipynb) SVM Test Model Pt.2
  In this model, we used the top 3 predictors from our random forest tree. We repeated steps 1 to 4 as per Jupyter Notebook 4. Unsurprisingly, this model performed better than our first, with perfect scores in terms of precision,recall and f1 scores. With this information, it was evident that this model was better than our initial model. Hence, this led to us using this model to make predictions. 

Using this model, we were able to input values and our machine was able to accurately predict the child's anemia level. Moreover, we repeated this for various input values and it gave us accurate results across all the different inputs. 

![image](https://github.com/flumbles/SC1015_FDAD_Team2/assets/162455199/b500b3fb-d660-452e-af13-1d72a184c1db)
![image](https://github.com/flumbles/SC1015_FDAD_Team2/assets/162455199/0f4b8cf9-4d2c-4751-8e67-34b1d0d7c2b5)



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
      
