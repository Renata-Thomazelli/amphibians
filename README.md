

![Static Badge](https://img.shields.io/badge/STATUS-FINISHED-brightGREEN)


# Amphibians
Machine Learning MultiLabel Classification Problem

This project deals with a multilabel classification problem. The objective is to predict the presence of amphibian species near water reservoirs based on features obtained from GIS systems and satellite images. To achieve this, libraries such as math, pandas, numpy, matplotlib, seaborn, sklearn and skmultilearn problem were used.
Font: font: https://archive.ics.uci.edu/dataset/528/amphibians


The notebook has these topics:
# 1. The Problem Definition 
# 2. Importing and Analysing the data
##    2.1 - Exploring the data
###      2.1.1 checking the shape
###      2.1.2 Verifing the columns names
###      2.1.3 Checking the type of columns
###	 2.1.4 checking the memory usage
###	 2.1.5 Verifing if there is NAN values
###	 2.1.6 Analysing the values of each varible
####		2.1.6.1 TR
####		2.1.6.2 SR  
####		2.1.6.3 NR
####		2.1.6.4 OR 
####		2.1.6.5 RR and BR
####		2.1.6.6 SUR1
####		2.1.6.7 SUR2
####		2.1.6.8 SUR3
####		2.1.6.9 CR
####		2.2.6.10 - Identify the target Labels 
##    2.2 - Data Analysing
###	2.2.1 - Building function to new columns
####		2.2.1.2 - functions to or, rr and br columns
####		2.2.1.3 - adding new columns
###	2.2.2 - Analysing the Type of Amphibians Labels
####		2.2.2.1 - Checking the quantity of each label
####		2.2.2.2 - Building the labels quantities visualization
###	2.2.3 - Analysing OR Label by Type of Amphibian
####		2.2.3.1 - Building the dataframe to analise the OR Label by Type of Amphibian
#####		2.2.3.1.1 - Selecting Varibles to df
#####		2.2.3.1.2 - Grouping by or label
####		2.2.3.2 - Building the visualization by "OR labels" and "Type of Amphibian"
###	2.2.4 - Analysing RR and BR varibles by Type of Amphibian
####		2.2.4.1 - Building the dataframe to analise the RR and BR varibles by Type of Amphibian
#####		2.2.4.1.1 - Selecting Varibles to df
#####		2.2.4.1.2 - Stack the types of Amphibians
#####		2.2.4.1.3 - Grouping by Amphibians RR and BR varibles
#####		2.2.4.1.4 - Reindex by new order of Amphibians type 
#####		2.2.4.1.5 - Reindex the order by minimum distances from water reservior to roads 
#####		2.2.4.1.6 - Reindex the order by minimum distances to builds 
#####		2.2.4.1.7 - Checking the values of df for Minimum distances from water reservior to roads
#####		2.2.4.1.8 - Adding the new column "type_amphibian" to df	
####		2.2.4.2 - Building the visualization by RR and BR varibles by Type of Amphibian
#####		2.2.4.2.1 - Renaming the amphibians_class column
#####		2.2.4.2.2 - Checking the types of columns
#####		2.2.4.2.3 - Changing the varible types or RR and BR varibles
#####		2.2.4.2.4 - Building the Relplot chart type Scatterplot
###	2.2.5 - Analysing NR varible by Type of Amphibian
#####		2.2.5.1 - Building the dataframe to analise the NR varible by Type of Amphibian
#####		2.2.5.1.1 - Selecting Varibles to df
#####		2.2.5.1.2 - Grouping by NR varible
#####		2.2.5.1.3 - Stack the types of Amphibians
#####		2.2.5.1.4 - Replacing 0 for NAN values
#####		2.2.5.1.5 - Identify the unique values
###	2.2.6 - Analysing NR and SR varibles by Type of Amphibian
####		2.2.6.1 - Building the dataframe to analise the NR and SR varible by Type of Amphibian
####		2.2.6.2 - Building the Relplot visualization by NR and SR varibles by Type of Amphibian
####		2.2.6.3 - Building the Relplot visualization by NR and SR varibles by Type of Amphibian with NR less then 100000
####		2.2.6.4 - Building the Relplot visualization by NR and SR varibles by Type of Amphibian with NR less then 20000
###	2.2.7 - Analysing TR varible by Type of Amphibian
####		2.2.7.1 - Building the dataframe to analise the NR varible by Type of Amphibian
#####		2.2.7.1.1 - Stack the types of Amphibians
#####		2.2.7.1.2 - Replacing 0 for NAN values
#####		2.2.7.1.3 - Including Type Amphibian column
#####		2.2.7.2 - Building the Countplot visualization by TR varible by Type of Amphibian
# 3. Preprocessing
##    3.1 - Mitiganting class imbalance problem necessity
##    3.2 - Feature Engineering
###	3.2.1 - Variable Transformation
#####		3.2.1.1 - Transforming the datatype to numerical ones.	
###	3.2.2 - Categorical Encoding
#####		3.2.2.1 - Analysing the Categoric types
#####		3.2.2.2 - Transforming with get_dummies
#####		3.2.2.3 - Having the new Dataframe to work with Machine Learning
#####		3.2.2.4 - Revising objecs types
# 4. Building the Model
##    4.1 - Spliting the dataset into features and targets
##    4.2 - Creating an Instance of MultiLabelBinarizer Class
##    4.3 - Dividing the df into training and test
##    4.4 - Random Forest Classifier
###        4.4.1 - Training
###	4.4.2 - Checking the Metrics
###	4.4.3 - Building a function to plot ROC Curve
###	4.4.4 - Plotting ROC Curves
