# House-Price-Prediction-using-Machine-Learning-in-Python

We all have experienced a time when we have to look up for a new house to buy. But then the journey begins with a lot of frauds, negotiating deals, researching the local areas and so on.

House Price Prediction using Machine Learning
So to deal with this kind of issues Today we will be preparing a MACHINE LEARNING Based model, trained on the House Price Prediction Dataset. 


<h2>The dataset contains 13 features :</h2>

1	Id	To count the records.

2	MSSubClass	 Identifies the type of dwelling involved in the sale.

3	MSZoning	Identifies the general zoning classification of the sale.

4	LotArea	 Lot size in square feet.

5	LotConfig	Configuration of the lot

6	BldgType	Type of dwelling

7	OverallCond	Rates the overall condition of the house

8	YearBuilt	Original construction year

9	YearRemodAdd	Remodel date (same as construction date if no remodeling or additions).

10	Exterior1st	Exterior covering on house

11	BsmtFinSF2	Type 2 finished square feet.

12	TotalBsmtSF	Total square feet of basement area

13	SalePrice	To be predicted


<h2>Importing Libraries and Dataset</h2>

Here we are using 

Pandas – To load the Dataframe

Matplotlib – To visualize the data features i.e. barplot

Seaborn – To see the correlation between features using heatmap




<h2>Data Preprocessing</h2>

Now, we categorize the features depending on their datatype (int, float, object) and then calculate the number of them.


<h2>Exploratory Data Analysis</h2>

EDA refers to the deep analysis of data so as to discover different patterns and spot anomalies. Before making inferences from data it is essential to examine all your variables.


<h2>Data Cleaning</h2>

Data Cleaning is the way to improvise the data or remove incorrect, corrupted or irrelevant data.

As in our dataset, there are some columns that are not important and irrelevant for the model training. So, we can drop that column before training. There are 2 approaches to dealing with empty/null values

We can easily delete the column/row (if the feature or record is not much important).


<h2>OneHotEncoder – For Label categorical features</h2>

One hot Encoding is the best way to convert categorical data into binary vectors. This maps the values to integer values. By using OneHotEncoder, we can easily convert object data into int. So for that, firstly we have to collect all the features which have the object datatype.
Filling the empty slots with mean/mode/0/NA/etc. (depending on the dataset requirement)


<h2>Splitting Dataset into Training and Testing</h2>
X and Y splitting (i.e. Y is the SalePrice column and the rest of the other columns are X)

<h2>Model and Accuracy</h2>
As we have to train the model to determine the continuous values, so we will be using these regression models.

SVM-Support Vector Machine

Random Forest Regressor

Linear Regressor

And To calculate loss we will be using the mean_absolute_percentage_error module. It can easily be imported by using sklearn library. 

The formula for Mean Absolute Error : 

![image](https://user-images.githubusercontent.com/81943886/218579993-1e77f531-3767-4fe6-b160-0c2288f6d6d7.png)



<h2>Conclusion</h2>
Clearly, SVM model is giving better accuracy as the mean absolute error is the least among all the other regressor models i.e. 0.18 approx. To get much better results ensemble learning techniques like Bagging and Boosting can also be used.
