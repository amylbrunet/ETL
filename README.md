# ETL project

![eTL_img.jpeg](https://github.com/amylbrunet/ETL_Project/blob/main/ETL_img.jpeg)

### Extract
Our team wanted to continue our research and analysis on the factors that influence student achievement. In our search, we found three datasets from the years 2013, 2015, and 2017 on poverty rates and median house income in each of the 50 states across varying age groups. We decided to use the three datasets we found for this project in conjunction with one of our data sets from our last project, which encompasses average math and reading scores for students in each of the 50 states over a span of several years.

### Transform
The first step was to clean and transform the new datasets we procured on the poverty rates and median household income data in the United States. After the initial cleaning and formatting in excel, we loaded the three csv files into pandas to create data frames and tables to load into our database. 
We created three new data frames in pandas in order to give each attribute its own table in the database with a primary key. We created a year tableholds the years, a subject table holds math and reading,and a table for the grade level includes 4th and 8th grade.
The final step of transforming the data was to merge each of the aforementioned tables together with the average test score data and with a state table that we created in excel before loading into pandas.
Through this transformation, we were able to create six different tables to be loaded into our PostgreSQL database.

### Load
We loaded the data into our PostgreSQL database through pandas and SQLAlchemy. We loaded six different tables into our database including a state table, a year table, a subject table, a grade table, an average score table with corresponding keys, and an income and poverty rate table also with corresponding state and year keys.

Through this project, we were hoping to learn more about the factors that impact student achievement in the United States. In our first project we looked at funding and discovered that it does not have much of an impact, so we concluded that we would need to do more research on other factors that could be influencing student test scores. By looking at poverty rates and median household income, we hoped to find more evidence either for or against our hypotheses. Although this project does not require any analysis, we plan to investigate this topic further in the future and utilize the database we created to help inform future projects.
