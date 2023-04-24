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
Drop the non-beneficial ID columns, 'EIN' and 'NAME'.
code: application_drop=application_df.drop(["EIN","NAME"], axis=1) -->

# Model detail i.e. How many neurons, layers, and activation functions did you select for your neural network model, and why?
<!-- There are 4 method had been selected to neural network model.
All detail information of these 4 models are in Learning and testing analysis is in "Learning and testing result.PDF"
Main activation function used is the rectified linear unit (ReLU) function as it is ideal for modelling positive, nonlinear 
input data for classification or regression. The ReLU function is always a good 
starting point, but not all data are positive, especially when normalised. -->

# Outcome i.e. were you able to achieve the target model performance? 
<!-- ~72% is reasonable outcome for this analysis -->

# Improving performance i.e. What steps did you take in your attempts to increase model performance?
Summary: Summarise the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.
<!-- All detail information of improvement is in the "Learning and testing result.PDF"
Model recommend is the second model 3 layers with 20 neurons each layer and activation function is ReLU as this model prodced highest accuracy. -->