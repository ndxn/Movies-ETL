# Movies Extract-Transform-Load

This program allows users to insert the filenames of data sources with varying parameters from particular sources with specified file types to enter the file names and have the data extracted, transformed with no small level of data cleaning, and extracted to a postgresQL database. While the function provided is robust enough to deal with variations in data, some assumptions are made. These are outlined below.

## Assumptions
1. The IMDB movie data is the most important for this analysis, hence the ```try-except``` block has been included therein.
2. There are not detrimental data types in columns when the ```lamda``` fuctions are searching for and converting lists
3. That data that requires parsing, namely the data pertaining to box office revenues and the movie budget, is contained to those data sets and to values pertainint to money.\
    3a. That no years of data include an inordinate number of indie flix or those which had awful box office results (I think this means 2020 is out!).
4. If data from other decades is included, that the data columns are consistent
5. That users will update parameters based on date ranges or will define variables to be passed into the function in order to define the tranformation within the function 
6. (A small one) That the same file types for the data across other analyses are used. This is kind of a gimme but it's super important or else the program won't work.
7. (And really big) For the grading, it's assumed there won't be any issues with the pgAdmin username/password combination or the network information.