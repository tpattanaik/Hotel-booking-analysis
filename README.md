# Hotel-booking-analysis
For this EDA Project, I have used Hotel booking dataset.
This data set contains booking information for a city hotel and a resort hotel, and includes information
such as when the booking was made, length of stay, the number of adults, children, and/or babies, and
the number of available parking spaces, among other things.
**Problem statement**

We need to explore and analyze the data to discover important factors that govern the bookings of a
Hotel.

**Introduction**

Hotel industry is a very volatile industry and the bookings depend on variety of factors such as type of hotels, seasonality, days of week and many more. This makes analyzing the patterns available in the past data more important to help the hotels plan better. Using the historical data, hotels can perform various campaigns to boost the business. We will be using the data available to analyze the factors affecting the hotel bookings. These factors can be used for reporting the trends and predict the future bookings.

**Packages Required**

To do the EDA of the dataset, we required following packages firstly imported to the notebook. This will help us to do code and get a clear picture of the data.
The packages are:

1. Numpy
2. Pandas
3. Matplotlib
4. Seaborn

# Steps Involved for EDA:

**1. Loading the dataset:

After importing required packages to the notebook, we need to read the csv file i.e., Hotel booking dataset file to the notebook. We can do this with the help of pandas by using pd.read_csv.

**2.Studying the raw data:

Before cleaning the data or studying the data, we should first study the raw data and try to understand the pattern of data.By looking at the head of the dataset, we can get some insight of the data like what are the columns available. Most importantly which columns are useful to us for EDA. The shape of the dataset will give us a vibe of how much of data we are playing with.
Also we can check the value_counts of each column and check what all things are there in each column and how it is distributed.

**3. Dealing with NaN Values:

There are 119390 and 32 columns in the dataset, which is huge. So there is high chance that there must be some NaN values. We need to deal with it as it may affect our end results drastically and we don’t want that.
After inspecting the Nan Values of Dataset, we have quite a lot of NaN values in company and agent (Agent- 16340, Company- 112593). But as per our analysis, these 2 has very less impact.
So we can decide to remove those columns. The reason why we can't remove rows with NaN value is because that will mean we are removing 112593 rows out of 119390 rows which is absolutely not a good idea. So removing columns will be a better idea since those 2 attributes (agents and companies) are unimportant.
We also have one more column with NaN Values i.e., country column with 488 NaN values. 488 rows out of 119390 is negligible hence just removed.




