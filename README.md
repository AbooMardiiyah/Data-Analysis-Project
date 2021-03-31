NB: This is a template to make documentation process easy. You can remove the `To-Do` notes in your final commit

# Project Title Here

Analyze Supermarket Data Across the Country - Company XYZ
Company XYZ owns a supermarket chain across the country. Each major branch located in 3 cities across the country recorded sales information for 3 months, to help the company understand sales trends and determine its growth, as the rise of supermarkets competition is seen.

You will apply learnings to analyse the dataset in the data folder, and the description of each feature can be found in this link:https://docs.google.com/document/d/1Sv-DlynHpOBAs5qKokn5MtbzqZcumTSlSI4-wQ0kf0w/edit?usp=sharing

# Project Steps
Step 1 - Loading the Dataset
The datasets are loaded using the `glob()` function and combined together using the `pd.concat()` method and finally read as a single dataframe using the `pd.read_csv()` method.


Step 2 - Data Exploration
Importing the necccesary packages/tools

numpy for carrying out numerical computations,pandas for making a dataframe object
seaborn and matplotlib for visualizations

To check a portion of the dataframe, the `.head()` function is used which returns the first 5 observations of the dataframe. The .`info()` gives us the information about the dataframe such as datatype of each feature, checking if feature contains a missing or null value,the dimension of the dataframe,in this case the dataframe has 17 features.

Observations

Minimun and maximum ratings is 4 and 10 respectively from the result shown when the `.describe()` method is used on the dataframe
Tax and gross income look statistically alike

Step 3 - Dealing with DateTime Features
The Date and Time features were converted to their appropriate feature using the `pd.to_datetime()` method and feature extraction is carried out from the dates and time features such as Month,Day,Hour etc.

Step 4 - Unique Values in Columns
unique() and nunique() methods show the distinct entities and the number of disctinct entities in a particular column respectively. The branch column has 3 unique values, city has 3, customer type has 2, gender has 2, product line has 6, payment has 3

Step 5 - Aggregration with GroupBy
With Groupby we can group columns by using some Aggregate functions such as the `Count()`,`Sum()`,`Min()`,`Max()` etc.
Porthacourt has the total highest gross income followed by Lagos and then finally Abuja

Step 6 - Data Visualization
Visualizations were made using the matplotlib library and seaborn to visualize the results in a graph whch makes more sense.

# Insights
below are some of the insights deduced from the analysis made:

*  The City with the total highest gross income is Portharcourt

* The most used Payment method for Abuja,Lagos and Portharcourt are Epay,Epay and Cash method respectively

* The highest product line sold is Fashion accesories while the least is health and beauty

* Branch B(Abuja) has the lowest Rating

*  Fashion accessories has the highest Unit price followed by Food and beverages
 
*   Home and lifestyle has the highest demand in Branch A, health and beauty has the highest demand in Branch B and finally for Branch C, the product line with the highest demand is Food and Beverages

*   The varying difference in demand in various branches indicates differences in general taste and preference of the people in that region

*   There's obviously no relationship between Quantity and Unit price


# Future Work

The future Profit(total gross income) can be predicted using the past data from the company


# Standout Section
*   in all 3 branches, each customer type seem to have a slight difference in the overall contribution to the cash flow.Breaking them down into the payment types for each customer type,one can see the payment type that is more predominant for all 3 branches.

* The payment type predominant for the Normal customers is the Epay while the Customers with the Membership type used Card method as the highest mode of payment


# Executive Summary.

The insights deduced from each visualizations and Analysis(Univariate and bi-variate) are explained in the comment section in the notebook.

To-Do - Include your Executive Summary document in your repository.
