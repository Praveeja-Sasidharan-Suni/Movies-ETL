# Movies-ETL

#### *ETL pipeline on movie data using Python and postgreSQL*

## Overview
This project consisted on a automated Extraction, Transformation and Load pipeline. This ETL extracted movie data from wikipedia, kaggle, and MovieLens rating to clean it, transform it,
 and merge it using Pandas.Later the clean merged  data will be transformed to a PostgreSQL database.

## Resources
- Data sources:
  - movies_metadata.csv
  - ratings.csv
  - wikipedia_movies.json

- Software:
  - Python
  - PostgreSQL
  - Pandas
  - SQLAlchemy
  - Regular Expressions 

## Results

-Using our knowledge of Python, Pandas, the ETL process, and code refactoring, wrote a function that reads in the three data files and creates three separate DataFrames.

[Wiki_movies_df.PNG](https://github.com/Praveeja-Sasidharan-Suni/Movies-ETL/blob/main/Resources/Wiki_movies_df.PNG?raw=true)
[Kaggle_df.PNG](https://github.com/Praveeja-Sasidharan-Suni/Movies-ETL/blob/main/Resources/Kaggle_df.PNG?raw=true)
[ratings_df.PNG](https://github.com/Praveeja-Sasidharan-Suni/Movies-ETL/blob/main/Resources/ratings_df.PNG?raw=true)

- Using Python, Pandas, the ETL process, and code refactoring, we have extracted and transformed the Wikipedia data so we can merge it with the Kaggle metadata.

 While extracting the IMDb IDs using a regular expression string and dropping duplicates, used a try-except block to catch errors.
[Wiki_movies_df.PNG](https://github.com/Praveeja-Sasidharan-Suni/Movies-ETL/blob/main/Resources/Wiki_movies_df.PNG?raw=true)
[Wiki_column_list.PNG](https://github.com/Praveeja-Sasidharan-Suni/Movies-ETL/blob/main/Resources/Wiki_column_list.PNG?raw=true)

- We merged the Kaggle metadata DataFrame with the Wikipedia movies DataFrame to create the movies_df DataFrame. Finally, we have merged the MovieLens rating data DataFrame 
with the movies_df DataFrame to create the movies_with_ratings_df.

[Movies-with-ratings-df.PNG](https://github.com/Praveeja-Sasidharan-Suni/Movies-ETL/blob/main/Resources/Movies-with-ratings-df.PNG?raw=true)
[movies-df-d3.PNG](https://github.com/Praveeja-Sasidharan-Suni/Movies-ETL/blob/main/Resources/movies-df-d3.PNG?raw=true)

- we have added the movies_df DataFrame and MovieLens rating CSV data to a SQL database.

![movies_query.PNG](https://github.com/Praveeja-Sasidharan-Suni/Movies-ETL/blob/main/Resources/movies_query.PNG?raw=true)
![Movies-data-count.PNG](https://github.com/Praveeja-Sasidharan-Suni/Movies-ETL/blob/main/Resources/Movies-data-count.PNG?raw=true)
![ratings_query.png](https://github.com/Praveeja-Sasidharan-Suni/Movies-ETL/blob/main/Resources/ratings_query.png?raw=true)
![Ratings-data-count.PNG](https://github.com/Praveeja-Sasidharan-Suni/Movies-ETL/blob/main/Resources/Ratings-data-count.PNG?raw=true)
