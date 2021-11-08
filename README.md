# CIND820
repository for capstone project

For Literature Review, Data Description, and Approach
  - Data collection, data prep/cleaning, data pre-processing and descriptive data analysis (n-grams and class overlap)
  - This code can be found: CIND820 - code for descriptive analysis.ipynb

Initial Results and the Code
For this portion I took the pre-processed data from provious file and altered to include category id and type classes. This was to further differentiate and be able to add dictionary items with category ids. Next I looked at the distribution (based on the workbook focus classes), and retrieved the dataset shape. I split the data into the test and train sets, with 25% of the data for testing and 75% for testing. Defined function for 5 times cross validation, on 4 models: Linear, Random Forest, Multinomial Naive Bayes, and Logistic Regression. Found the mean accuracy and the deviation, plotted visually in the form of a boxplot. Then I created confusion matrices for all four models to compare. After was able to find samples of the content of falsely predicted classes, this was to see how many were incorrectly predicted and to view any patterns in the content (if present). Lastly, ran a classification report to retrieve the precision, recall and F score of the model to figure out if it is good.

  - CIND820 - Test/Train + NB and RF.ipynb : this file contains the sentiment models for 4 classes (good, good + helpful, bad, bad + helpful)
  - CIND820 - Test/Train/ helpful v. non-helpful reviews.ipynb : this file has same sentiment models analysis to distinguish between two classes - helpful v non helpful
  - CIND820 - Good subset helpful v. non-helpful reviews.ipynb : this file has same sentiment models analysis but only applied to the good reviews to distinguish between two classes (helpful v non helpful). This was done to see if the removing bad review types would improve accuracy.
  - CIND820 - Test/Train/ Good & bad reviews.ipynb :  this file has same sentiment models analysis to distinguish between two classes - good vs bad

The reason for the split in the workbooks is to see how results compare between the two types of classes: bad/good and helpful/nonhelpful. I was able to see that the helpfulness level was a weak point for the sentiment models to predict.
