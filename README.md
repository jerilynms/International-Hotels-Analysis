# International Hotels Analysis
This project pertains to a database of 25 international hotels, their customer reviews, and reviewer demographics.

While examining the database in excel, I looked for consistent naming conventions in the variable titles, and if any of the values varied 
from each other within columns. I could not find any inconsistencies. I used SQLite's column reordering function to pinpoint any nulls and could not find any either. 
Of the 25 hotels, all are 5 star accommodations and located in a distinct city and country.
The reviews are dated from 2020 to 2025. 

The Hotel Reviewer Demographics Dashboard aims to give insights into the users who are leaving hotel reviews. The dashboard reveals that families tend to leave the highest reviews and that most reviewers tend to be from the United States or Western Europe. The age group that leaves higher reviews varies by hotel. There are also filters for those who are interested in specific hotels or time frames. These insights could inform what groups of travelers to target if hotels were hoping to increase their reviews scores or the number of reviews. 

The analysis I performed in SQLite first created a report of all 25 hotels and their average overall review score. Then I focused on finding the best and worst hotels in the database for each year of data. The Golden Oasis in Dubai was the highest rated from 2020 to 2023 while Canal House Grand in Amsterdam took the highest score from 2024 to 2025. The Savannah House in Lagos was consistently the lowest rated. Then I focused on what the different review scores revealed about each hotel and the user demographics of their reviewers. Lastly, I calculated a rate of returning customers based on repeated reviewers. While writing this last query, my rate calculation kept returning zero. I knew my calculation was correct, so I decided to utilize ChatGPT to find out why. ChatGPT pointed out that one reason could be the data types. I converted one of the variables being used into a decimal type instead of integers and suddenly my rate was returning the correct value. ChatGPT helped remind me that my data types in a formula will affect the result of that calculation.  

Please take a look at the SQLite Analysis file for more detailed insights and the queries. 

Data obtained from Kaggle: https://www.kaggle.com/datasets/alperenmyung/international-hotel-booking-analytics?resource=download
