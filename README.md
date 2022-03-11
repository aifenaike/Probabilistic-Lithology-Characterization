# Probabilistic-Lithology-Characterization-ML

Accurate characterization of the lithology is essential to optimize all drilling parameters and to minimize the drilling cost. Various methods have been used previously for predicting lithology using well log data. However, the use of drilling data for lithology predicting received only a little attention. Here, I have developed a Random Forest model to determine the probability of the existence of certain lithofacies as a function of drilling data (i.e. depth (D), Rotation per minute at drill bit  (BIT_RPM), Pump total stroke rate (STRATESUM), Surface Torque Average (TORQUE), Depth averaged rotation per minute (ROP_AVG), Pump pressure (PUMP),  weight on bit (WOB), Effective circulating density on bit (ECDBIT), Total gas content (TOTGAS), and Mud flow out (FLOWOUT)).


## Objectives

The objective of this work is to use machine learing in automating the classification of lithology. This project integrates Random Forests for formation lithology identification and comprehensively evaluated the performance of the proposed classifier based on the metrics of  the area under the receiver operating characteristic curve (AUC). The developed model can help petroleum engineers to determine reservoir lithology and optimize drilling parameters. i.e This will serve as a decision support system for the experts in the field.

## Dataset
The data used in this project is from the open database for the Volve oil field in Stavanger at the southern end of the Norwegian sector in the North Sea. It includes drilling sample data with known lithology facies class (Mudstone, Claystone, Dolomite, Marl and Sandstone). 

## Results
- The model's ability to estimate the certainty of the lithology belonging to a specific class of lithologies is measured using two metrics.
  - One-vs-Rest AUC
  - One-vs-One AUC
- One-vs-One involves splitting the multi-class dataset into multiple binary classification problems. A binary classifier is then trained on each binary classification problem and predictions are made using the model that is the most confident.
- Like one-vs-rest, one-vs-one splits a multi-class classification dataset into binary classification problems. Unlike one-vs-rest that splits it into one binary dataset for each class, the one-vs-one approach splits the dataset into one dataset for each class versus every other class
- The final test 0VR accuracy of the model is 99.37%
- The final test OVO accuracy of the model is 97.52%


This attempt to predict lithology from drilling data is just the beginning of more exciting opportunities to create more robust predictive models with more data.
