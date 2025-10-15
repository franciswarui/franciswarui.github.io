---
title: "data wrangling project"
categories: [introduction, task completed, conclusion]
tags:[discovery, structuring, cleaning, errors, validation]
---
## data discovery
First in imported the data as pd to load the Netflix dataset into the kaggle notebook. 
After that I got a quick overview of the dataset to get information about the dataset where it gave 
me the total number of rows and columns, data types and also non-null counts for each and every 
column. 
Then I checked the number of rows and columns where there was a total of 8807 rows and 12 
columns. 
To get the first row of columns headings I printed all column titles in the dataset 
I then printed all datatypes in the columns to know the datatype in each column where 11 of them 
were objects except 1 ‘’release year’’ which was int64 
After that I grouped and counted the null values in each column. I then grouped and counted of 
duplicate rows where there was none.
---
## structuring
I stated by converting the contents of the date added column to date time 
Then I converted the duration into values and units, where there was addition of two columns: 
duration value and duration unit. 
After that, I converted the duration value into numbers that can be used in mathematical operations 
which I then viewed the two columns. 
I found another way for structuring the dataframe where I reordered the columns according to my 
own way.
---
## cleaning
3. cleaning  
I deleted the description column since it was not to be relevant to my work 
After that I imputed director values that were null with values by using the relationship between 
director and cast, whereby I looked for instances where same director and cast names have 
appeared more than 3 times and number they have appeared in same row. I created combined 
director-cast pairs, counted the unique pairs, filtered the frequent pairs that appeared more than 3 
t
 imes. I then filled country null values with director matched to country values and filled with a Not 
Given to all other country fields. 
To the cast column where values were not available I filled them with a ‘not given’ 
I then dropped all rows that had null values
---
## errors
I started by checking whether there was any date added that came before date released where I 
found 14 rows. 
I printed the 14 rows with those two columns 
To correct that error, I replaced those date added to be of the year released on January 1st. 
I sampled the corrected rows and they were well replaced and confirmed no more release year 
inconsistencies.
---
## validation
I removed the dir cast column that I had added 
I then checked whether the date value was in numeric and date added was in date time. 
I then filtered the shows that were added before 2010. 
I got a sample of the first 4 rows. I reset the index and then saved the dataset as csv.
---
## link code to my work:
https://www.kaggle.com/code/franciswaruikamande/francis-warui-cs-da02-25077
---
