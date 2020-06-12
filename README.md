# UK-road-accidents

Using a dataset availabe from Kaggle, I provide an analysis of road accidents in the United Kingdom over the time period 2005-2015.
For about 1.7 million accidents, the data contains information about the severity of each accident as well as about the circumstances
under which the accident occurred, for instance: What were the weather conditions at the scene of the accident? Did the accident happen on an express road or at a junction? What was the speed limit? At what time and on which day did the accident occur? How many vehicles were involved? And so on.

The first part of the project explores how the frequency and severity of accidents change depending on the time of the day
and the day of the week. It becomes apparent that during time periods when the overall number of accidents is below average,
those accidents which do happen tend to be more serious.

Another part of the project is to prepocess data by taking steps such as: Removing accidents for which too much relevant information is missing, removing accidents where some information is implausible (such as a speed limit of zero), and exclude some exceptional events (crashes involving more than 5 cars). Also, some potential sources of collinearity between different variables are removed: For instance, information on weather conditions and road conditions capture similar information (If it rains, then the road is wet). 

The third part of the project tests how good some well-known classifiers can do at predicting whether an accident is "serious" or "slight." One important feature of this classification problem is its class imbalance: About 85% of all accidents in the dataset are "slight," while only 15% belong to the "serious" class. A logistic regression and a k-Nearest Neighbors classifier as well as a Random Forest are used to perform classification. The accuracy of the different classifiers is compared and evaluated using a confusion matrix and metrics derived from it, such as the "naive" accuracy, precision and recall, and Cohen's kappa. 
