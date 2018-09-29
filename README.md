# Quartic.ai
EDA and model building for random data set

1)  Briefly describe the conceptual approach you chose! What are the trade-offs?
Ans) The data set given was little complex, so little care had to taken while studying it. 
Let me begin by giving a quick summary of the data set.
No. of Rows : 596000
No. of Columns: 58
The structure of the data set clearly shows us that all the variables are of integer type. 
After checking each column separately and carefully I found that there are lot of NA values in the data. Some of the columns 
(num18, cat6. Cat8) contains more than 1 Lakh NA values. So, it was wise to drop these columns.
Proper care had to be taken to impute the other missing values.
I imputed some columns by inserting the mean value of that columns. Some values were simple removed as they could pollute the data.
The next step was to convert the “cat and target” variables into categorical values.
The id column was dropped as was not suitable for our model building.
After following the above steps, the data was clean and fit to proceed.

2) What's the model performance? What is the complexity? Where are the bottlenecks?
Now the data that we have does not specify the column names. So, it was very difficult to perform EDA.
Since we do not know if the variables have certain relationship between them, it was wise to choose Decision Tree as our model.
The performance of the model: - 
As per confusion matrix, our model is 96.35 accurate.

3) If you had more time, what improvements would you make, and in what order of priority?
If given more time, I would once again do the data analysis to find some pattern. Would have k-fold cross validation and 
perform random forest modelling as well to see the difference between decision tree and random forest.
