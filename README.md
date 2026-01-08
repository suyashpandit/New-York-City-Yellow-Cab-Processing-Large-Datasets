*This project was originally completed as part of a Data Analytics & AI Bootcamp and later curated for portfolio presentation.*

# New-York-City-Yellow-Cab-Processing-Large-Datasets
NYC Yellow Cab is a big company run by NYC Taxi Cab Commission which handles many cabs and medallions each year. There are millions of trips every month with hundreds of millions of revenue. Raw data is all over the place and too messy. Cleaning and analyzing this data helps NYC stakeholders to see the details of these trips and revenue.

# Introduction:
New York City Yellow Cab is the hallmark of New York City. Anyone who has ever been there or seen NYC in a movie, has clearly seen the yellow taxis that people raise their hand to stop. With the rise of ride sharing companies like Uber and Lyft, NYC Yellow Cab too is not untouched. It has taken a hit. With the trip record dataset of this yellow cab, this project focuses on the January 2025 dataset to draw useful insights and transform a big taxicab dataset into actionable insights for stakeholders.
# Problem Statement:
NYC Yellow Cab is a big company run by NYC Taxi Cab Commission which handles many cabs and medallions each year. There are millions of trips every month with hundreds of millions of revenue. Raw data is all over the place and too messy. Cleaning and analyzing this data helps NYC stakeholders to see the details of these trips and ultimately the revenue in detail.
# Objectives:
Data Acquisition and Preprocessing: Collecting the dataset, cleaning duplicates, handling outliers, missing values, standardizing datetime formats, creating necessary columns if needed.
Data Processing and Analysis: Exploring trip demand patterns by time and location, analyzing fare and revenue distribution across various features.
Storage and Visualization: Storing the cleaned data efficiently and presenting insights using clear visualizations and report.
# Methodology:
Pandas library in python was used to effectively clean and process the dataset. It was also used to save the cleaned dataset in parquet format which handles large file sizes.
Pyspark was also used to visualize the dataset but was not used for the entirety of the analysis.
Matplotlib and Seaborn in python were used for visualizations. 
Optimization of memory usage by saving data in Parquet format instead of CSV.
Removal of unnecessary columns with little impact.
Handling outliers early, reducing dataset size from 3.5 million rows to 3.2 million rows.
Creating simple pandas ETL pipeline.
Storing dataset in s3 for future use possibly with PySpark.
Visualizing dataset with Pyspark.

 # Conclusion
In conclusion, handling the NYC taxi cab dataset was an experience. There were many hurdles along the way especially in being able to work with pyspark. A small attempt was made but Pandas came in handy as it was able to process data with millions of rows too.

Although the dataset did not have any duplicates, it did come with a lot of null values in multiple columns. As these features were important for the analysis that I was planning to do, dropping them was not an option. Hypotheses were made about how to handle them. Data was analysed well before coming to any decision which was a good learning curve.

Interesting aspect was coming across negative values in financial terms, like negative airport surcharge. Although the actual reason will remain a mystery, thinking over it if it was a refund issue or a data entry issue and handling them was challenging.

Although date and time were already in US format, still forcing them to the datetime format as needed was done.

It was amazing to see how unrealistically high and low values are usually present in a dataset. This could be an indication of lack of proper funding to enter the datas, or system issues. Although some of them could have been real but 90893 distances of under zero is clearly not acceptable in a big corporation like NYC taxi commission.

Data was stored in an amazon s3 bucket and ETL pipeline was created to extract from the local storage. Pyspark was not used, thus despite storing the dataset in s3 bucket, only local pipeline was developed.

Temporal analysis was done to identify patterns, trends and relationships. Having been the first project to analyse and visualize trends and patterns over a course of time, it was a good experience was well to learn and make mistakes and debug.

Grouping distances into categories created was a reminder of the basics of creating labels and bins.

This analysis gave an idea into how to optimize taxi numbers during peak hours like evening, making a weekend vs weekday strategy, making system more robust and better for credit card and flexfare transactions, rethinking about surcharges as well.
