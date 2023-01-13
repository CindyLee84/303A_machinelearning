303 Machine Learning
International Medical University HIA122 - Health Data Analytics (303) Group A Group Project
The dataset is available for public and was created by Dr. William H. Wolberg, physician at the University of Wisconsin Hospital at Madison, Wisconsin, USA. It was donated by Olvi Mangasarian on July 15th,1992. To create the dataset, Dr. Wolberg used fluid samples, taken from patients with solid breast masses and an easy-to use graphical computer program called Xcyt, which is capable of perform the analysis of cytological features based on a digital scan.
There is total 7 files in the data folder discovered from https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/. These includes:
•	breast-cancer-wisconsin-data
•	breast-cancer-wisconsin-names
•	unformatted data
•	wdbc.data
•	wdbc.names
•	wpbc.data
•	wpbc.names
Wdbc.data, wpbc.data and breast-cancer-wisconsin-data are files that without attributes or names and only contain datasets, while breast-cancer-wisconsin-names, wdbc.names and wpbc.names files are files that describes how is the database is obtained, list of attributes, class distributions, references of the study, results, and relevant information about the study. The attributes should be included in the datasets to provide clearer and meaningful database for performing data and statistical analysis.
Summary of the WBCD dataset:
Attribute	                       Domain
Sample code number	             ID number
Clump Thickness    	              1–10 (numeric)
Uniformity of Cell Size	          1–10 (numeric)
Uniformity of Cell Shape	        1–10 (numeric)
Marginal Adhesion	                1–10 (numeric)
Single Epithelial Cell Size	      1–10 (numeric)
Bare Nuclei	                      1–10 (numeric)
Bland Chromatin	                  1–10 (numeric)
Normal Nucleoli	                  1–10 (numeric)
Mitoses	                          1–10 (numeric)
Class	                            2 for Benign & 4 for Malignant
Class Distribution	              Benign:                458(65.5%) 
                                  Malignant:             241(34.5%)
Total Number of All Instances	    699
Number of Missing Values	        16

Pre-processing method
Method 1
#imputer = SimpleImputer(strategy='mean')
    #imputer.fit(X)
    #Xtrans = imputer.transform(X)
Method 2
# Imputing with MICE

Out of 7 files, we decided to choose breast-cancer-wisconsin-data to perform Machine Learning data analysis. The breast-cancer-wisconsin-names file listed 11 attributes matches with the dataset in breast-cancer-wisconsin-data file. The objective of the project is to investigate the accuracy of ML classifiers employed in the dataset. There are seven ML classification methods we focused in this study: Random Forest, Naive Bayes, Decision Tree, Logistic Regression, k-nearest Neighbour, support Vector Machine and Deep Learning neural network.
