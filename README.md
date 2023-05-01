# deep-learning-challenge
# Model improvement record/analysis is in "Learning and testing result.PDF"
# All testing models as h5 files

#                                                                                  Analytics Report
# Overview of the analysis
<!-- This analysis is a tool that can help Alphabet Soup to select the applicants for funding with the best chance of success in their ventures.
Data had been devided into training and testing purpouse so that model can be produced to predict success chance. -->

# Data Preprocessing
# Target(s) for the model: 
<!-- Column IS_SUCCESSFUL is the target and it had been defined by this code: y = categorical_data["IS_SUCCESSFUL"].values -->
# Features for the model
<!-- All other columns are the features and it had been defined by this code: X = categorical_data.drop(["IS_SUCCESSFUL"],1).values  -->
# Variable(s) should be removed:
<!-- There are some variable should be removed from the input data because they are neither targets nor features.
Drop the non-beneficial ID columns, 'EIN' Only
code: application_drop=application_df.drop(["EIN"], axis=1) -->

# Model detail i.e. How many neurons, layers, and activation functions did you select for your neural network model, and why?
<!-- 
Main activation function used is the rectified linear unit (ReLU) function as it is ideal for modelling positive, nonlinear 
input data for classification or regression. The ReLU function is always a good 
starting point, but not all data are positive, especially when normalised. 
Learning structure as below: 
   Layer1 150
   Layer2 80
   Layer3 55
   Epochs 60-->

# Outcome i.e. were you able to achieve the target model performance? 
<!-- AlphabetSoupCharity: ~72% is reasonable outcome for this analysis -->
<!-- AlphabetSoupCharity_Optimisation: 77% is reasonable outcome for this analysis -->

# Improving performance i.e. What steps did you take in your attempts to increase model performance?
Summary: Summarise the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.
<!-- There are few steps which been used to improving the performance in AlphabetSoupCharity_Optimisation
1. Drop less columns which only "EIN" dropped 
application_drop=application_df.drop(["EIN"], axis=1)
application_drop
2. Increasing neurons to different layers
   Layer1 150
   Layer2 80
   Layer3 55
3. Add one more layer
4. Increase epochs to 60 -->