# Hotel-booking-analysis
For this EDA Project, I have used Hotel booking dataset.
This data set contains booking information for a city hotel and a resort hotel, and includes information
such as when the booking was made, length of stay, the number of adults, children, and/or babies, and
the number of available parking spaces, among other things.

# Abstract

Hotel booking dataset describes two datasets with hotel demand data. One of the hotel is a resort hotel and the other is a city hotel. Both datasets share the same structure, with 31 variables describing the 119390 observations represents a hotel booking. This dataset contain booking information such as when the booking was made, length of stay, the number of adults, children and/or babies, and the number of available parking space, among other things. 
Our EDA can help us to explore and analyse the data to discover important factors that govern the bookings of a hotel.
We will use different EDA concepts using Python and their packages, Matplotlib and seaborn to come up with various graphs and charts by using the dataset and get to some conclusion for our problem statement. 

# Problem statement

We need to explore and analyze the data to discover important factors that govern the bookings of a
Hotel.

# Introduction

Hotel industry is a very volatile industry and the bookings depend on variety of factors such as type of hotels, seasonality, days of week and many more. This makes analyzing the patterns available in the past data more important to help the hotels plan better. Using the historical data, hotels can perform various campaigns to boost the business. We will be using the data available to analyze the factors affecting the hotel bookings. These factors can be used for reporting the trends and predict the future bookings.

# Packages Required

To do the EDA of the dataset, we required following packages firstly imported to the notebook. This will help us to do code and get a clear picture of the data.
The packages are:

1. Numpy
2. Pandas
3. Matplotlib
4. Seaborn

# Steps Involved for EDA:

**1. Loading the dataset:**

After importing required packages to the notebook, we need to read the csv file i.e., Hotel booking dataset file to the notebook. We can do this with the help of pandas by using pd.read_csv.

**2.Studying the raw data:**

Before cleaning the data or studying the data, we should first study the raw data and try to understand the pattern of data.By looking at the head of the dataset, we can get some insight of the data like what are the columns available. Most importantly which columns are useful to us for EDA. The shape of the dataset will give us a vibe of how much of data we are playing with.
Also we can check the value_counts of each column and check what all things are there in each column and how it is distributed.

**3. Dealing with NaN Values:**

There are 119390 and 32 columns in the dataset, which is huge. So there is high chance that there must be some NaN values. We need to deal with it as it may affect our end results drastically and we don’t want that.
After inspecting the Nan Values of Dataset, we have quite a lot of NaN values in company and agent (Agent- 16340, Company- 112593). But as per our analysis, these 2 has very less impact.
So we can decide to remove those columns. The reason why we can't remove rows with NaN value is because that will mean we are removing 112593 rows out of 119390 rows which is absolutely not a good idea. So removing columns will be a better idea since those 2 attributes (agents and companies) are unimportant.
We also have one more column with NaN Values i.e., country column with 488 NaN values. 488 rows out of 119390 is negligible hence just removed.

**Some more methods used:**

1. As there were only 2 types of hotels, we used a pie chart and looked at the distribution of the hotels. We can use bar chart also.

2.For numerical variables, we used describe method to understand the distribution of number in terms of five number summary.

3. When we want numerical values distribution by using graph, its better to use bar plot to get a clarity of the distribution.

4.To see the price distribution, we used lineplot to see the variation of the price in a interval of time.

5.We should always check atleast the head and tail of the dataset just to get a raw idea of the data.

# Limitations

1. The data for 2015 and 2017 is for different months.

2. The definition of new customers is not very well described. A new customer this year will be existing next year, or they can be existing customer from the 2nd booking. A deeper analysis in required based on definition

3. The weekday vs weekend analysis can be further drilled for the type of bookings

# Insights from Data analysis

1. Majority of the hotels booked are city hotel. Definitely need to spend the most targeting fund on those hotel.

2. We also realise that the high rate of cancellations can be due high no deposit policies.

3. We should also target months between May to August. Those are peak months due to the summer period.

4. Majority of the guests are from Western Europe. We should spend a significant amount of our budget on those area.

5. Given that we do not have repeated guests, we should target our advertisement on guests to increase returning guests.







