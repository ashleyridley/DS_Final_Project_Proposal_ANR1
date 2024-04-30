# DS_Final_Project_Proposal: Customer bankruptcy prediction analysis (paper)
Traditional bankruptcy prediction models typically focus on predicting the event of bankruptcy itself, and do not consider the socio-economic consequences of their prediction. Therefore, I will use machine-learning to conduct a prediction analysis to predict and consider different costs caused by bankruptcy. The datatset was found on Kaggle and collected from the Taiwan Economic Journal. The dataset contains 6,819 instances, which is highly imbalanced. I will use Random Forest, Decision Tree's and KNN since these algortihmn's strengths relies on its ability to handle complex datasets. 

# DS_EDA_ANR.pdf: Churn EDA analysis (paper)
Previously, I was going to use predictive analysis to make a prediction model regarding company bankruptcy that would accurately predict whether a company can go bankrupt or not. Unfortunately, the data from the model was very imbalanced with only 3% of the instances being bankruptcies. This new dataset contains 10,000 entires and 12 columns as well as categorical and numerical variables. There are no missng values from the data. I used numerical summarization, and the correlation matrix to give a better representation of the relationship between each column.

# DS_EDA_ANR.ipynb
- dropped customer_id column because its not needed for interpretation
- printed the categorical and numerical columns
- made a histograms for the gender and age columns
- made the gender column binary using str.replace()
- made a histplot for credit score, age and tenure by the distribution of churn
- made a heatmap using the correlation matrix
- made a pairplot to show the relationship between numerical features and churn status

# DS_EDA_ANR.twb
This is a visual model using tableau to display histograms using averages. This was not a good model for visualization for the data, since i coudnt display the categorical data. The numerical data was a little easier to display but i had to use the averages which defeated the purpose. These models were not good enough to use, so i will be switching the visualizations to python.

# DS_Preliminary_model_ANR.ipynb
For the churn preliminary model,the origianl correlation matrix did not make sense, since there were categorical variables that were not needed for the actual anaylsis. Using the new df2 for the correlation matrix i made 2 heatmaps, one for the categorical variables and the other for the numerical variables. Then i disaplayed the value counts for the categorical variables country, gender, churn, active_member, product_number and credit_score, as well as their bar charts.
- instead of using str.replace() i used one hot coding for the gender and country column
- then used df.sample() to make sure the program is running
- made a heatmap for df2 for the categorical variables, which showed there was little to no correlation between these variables at all
- made another heatmap for the numerical variables, which showed a higher percentage of correlation between the variables
- made scatterplots to show correlations between specific variables such as credit_score and age
- used Decision Tree and KKN for the classifier algorithms and displayed a heatmap with the accuracy

  # DS_Poster_ANR.pptx (celebration of student research)
  This poster will be used at the student celebration of research. It has the abstract and introduction of the project  as well as materials and methods used and results. The aim of this project is to identify patterns and factors that contribute to customer churn, which can enable banks to manage customer relationships and ultimately drive business growth and profitability. This project will display majority of the research used throughout the preliminary notebooks in python. I will display some of the classification reports, heatmaps and bar charts for better visualization.
  - showed the heatmap for both numerical and categorical variables to show howi determined which variables i will need to use
  - showed the confusion matrix for decision trees as well as the accuracy of the matrix itself
  - will show the accuracy scores of both models for comparision
  - will need to clean up the results section and show how to read a classification report along with precision, recall and f1-score

# Ds_Preliminary_Model_ANR1.ipynb (final project)
This notebook continues the process of the previous notebooks with the custome churn prediction model. For this final notebook, I have added the Random Forest algorithm along with a plot that shows how the number of decision trees affect the model score. I have also incorporated the classification report, and the heatmap as well as its accuracy. 
- I have added a bar chart for all 3 algorithms to show their accuracy score for comparision
- in conclusion the slight imbalance of the gender column affected the accuracy of the model
- random forest had the highest accuracy with an 84%, decision trees 80%, and KKN with 74%
- for future work i will use SMOTE to oversample the data to make the data balanced

# DS_Final_Project_Slide_Deck_ANR (final presentation)
This powerpoint contains information from the final project including the final results after using the random forest algorithm. All three models were proven successful with an accuracy of 75% and above.
For the final preliminary model,I have further cleaned the data using one hot coding for the gender and country columns as well as adding the Random Forest algorithm. I have also added heatmaps for both numerical and categorical data, as well as the heatmap accuracy. Finally, i made a bar chart to show the accuracy scores of each algorithm. 
