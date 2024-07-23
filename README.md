<div align="center">
  <h1 align="center">Training Regression Models with the Communities and Crime Dataset to Predict Violent Crime Using both Human Understanding and Machine Learning Techniques</h1>
</div>
</br> 

<div align="center"> 
  <h2 align="center"> Katherine Wickett, Student Number: 501280122 </h2>
  <h3 align="center"> Supervisor: Professor Tamer Abdou </h3>  
</div>
</br> 

<h1 alighn="left">Study Replication</h1>

My first step was to recreate the Ahishakiye et al. study as it was presented. The code for that replication can be found here: <a href="https://github.com/kwickett/CIND820/blob/main/Study_Replication.ipynb">replication</a>

<h1 align="left"> Preprocessing and Initializing Models </h1>
</br>
In this stage of the project I worked the complete dataset, dealing with missing data, as well as reducing dimensionality through two techniques of feature selection: 

- Stepwise Feature Selection 
- VIF Feature Elimination

I also created datasets which divided my target feature into different numbers of classes. This created four datasets to train models on: 


1. Stepwise selected features with 5 classes in target attribute
2. Stepwise selected features with 3 classes in target attribute
3. VIF selected features with 5 classes in target attribute
4. VIF selected features with 3 classes in target attribute

Pre-procesing code can be found here: <a href="https://github.com/kwickett/CIND820/blob/main/Preprocessing_and_Initialization.ipynb">pre-processing</a> 
</br>
<h1 alighn="left"> Testing Decision Tree, Logistic Regression, and K Nearest Neighbors Regression Models </h1>
</br>
In this stage of the project I tested my four datasets using decision tree, logistic regression, and knn nearest neighbors models. Each model was evaluated based on f1 score
and Matthews Correlation Coefficient to determine how Precision and Recall metrics were performing. Stability was evaluated by two types of cross-validation and efficiency 
was evaluated by processing time. 
</br>
</br>
Model testing code can be found here for both stepwise selected features datasets: <a href= "https://github.com/kwickett/CIND820/blob/main/Stepwise%20Features/stepwise_features.ipynb">stepwise</a>
</br>
</br>
Model testing code can be found here for both VIF selected features datasets: <a href="https://github.com/kwickett/CIND820/blob/main/VIF%20Features/vif_features.ipynb">vif</a>
</br>
</br>
<h1 align="left"> Grouping Features and Training with Most Effective Model </h1>

Features were separated into groups based on their real-world relationship to each other. The most effective model, which I determined to be the K Nearest Neighbors 
Model trained on a target attribute with 3 classes, was then trained on all groups to evaluate their indiviudal importance to the target attribute. 

Group Initialization Code can be found here: <a href="https://github.com/kwickett/CIND820/blob/main/Grouped%20Features/Groups_Initializing_Models.ipynb">initializing groups</a>

Group Training Code can be found here: <a href="https://github.com/kwickett/CIND820/blob/main/Grouped%20Features/Groups_Model_Testing.ipynb">training groups</a>

<h1 align="left"> Initial Results </h1>

Inital Results including f1 scores, MCC scores, processing time, and ranking of the models can be found here for initial models: <a href="https://github.com/kwickett/CIND820/blob/main/Results/Regression%20Model%20Results%20.docx">results</a>
</br>
</br>
and here for the grouped models: <a href="https://github.com/kwickett/CIND820/blob/main/Results/Grouped%20Model%20Results%20(1).docx">results</a>

