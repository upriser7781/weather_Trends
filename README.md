Exploring weather Trends

### Aim: 
To analyze local and global temperature data and compare the temperature trends of local to overall global temperature trends. 
### Process: 
#### 1.	Extracting data:
  •	SQL query was used to extract data from the temperature database, than the results were downloaded in CSV files. At first, data about global temperature by year was to be extracted. The following Query was used to extract the global data:
        
        SELECT * FROM global_data; 
 
   •	Then, I exported the temperature data for the world as well to find out the nearest city to me in the database. The following Query was used to extract the city level data:
        
        SELECT * FROM city_list;
 
  •	At last, the data about the average temperature for the city nearest to me was extracted from the city_data database, by using following Query:
  
        SELECT * FROM city_data
        WHERE city = 'Delhi' AND country = 'India';
 The above Query gives the list of yearly average temperature of the city ‘Delhi’ from country ‘India’.
#### 2.	Analyzing the CSV file:
I used MS Excel for extracting the data from the downloaded CSV files. At first I took the data of the city nearest to me, i.e. Delhi from year 2004 to 2013. I calculated the moving average in order to smooth out lines, making the temperature trends more observable. 

###### Moving average: 
The moving average is used to smooth the irregularities for the clear observations of the temperature trends. In the city level data, average temperature was used to calculate the moving average. From the list of average temperature (CITY  AVG  T), we found out the average of first 3 year, that is from 2004 to 2006. The following formula was used in the formula bar, =AVERAGE(D2:D4)  in E4 cell. Now you can use Copy + Paste, Ctrl + D, or click and drag the formula down to the next cell. If you look at the new formula, you'll see that now it calculates the average sales for the second through fifth year. Rest of the average was calculated similarly. Then we plotted the line chart using the year at x-axis and city average at the y-axis, as shown below.

<img width="459" alt="image 1" src="https://user-images.githubusercontent.com/57844178/81323363-1efb8080-904a-11ea-8fc1-a82898a395e4.png">

Same was done with global level data. The following picture shows the global level line chart was plotted similarly, by taking the year at x-axis and global average at the y-axis, as shown below.

<img width="308" alt="image 2" src="https://user-images.githubusercontent.com/57844178/81323414-320e5080-904a-11ea-91fc-018731318f5e.png">

#### 3.	Making the observations:
Now the city’s temperature with the global temperature is compared. The moving average is used to plot the comparison graph.

<img width="335" alt="image 3" src="https://user-images.githubusercontent.com/57844178/81323449-42bec680-904a-11ea-959c-c09549745c10.png">

-	By observing the charts it shows the temperature is moderate during the 10 years span. It is going up just by 1 or 2 degrees and then again coming down in same manner. Both globally as well as in local city.
- During initial year (2004) the temperature is raises by 0.38 degrees globally and again coming down in 2005 by 0.17 degrees.
- The city nearest to me, i.e. Delhi is hotter on average compared to the global average.
- Delhi is in moderate type of climate during the span of 10 years, i.e. from 2004 to 2013.
- The change of climate between the globe and Delhi city is slightly on average, and both of them are usual and face a very small change in both ways. 

#### 4.	Conclusion: 
The report suggest that in a span of 10 years, the global temperature as well as the local temperature is facing a slight change in both ways due to the change in climate.


(The data of 2004 to 2013 is used i.e. analysis of span of 10 years)

- NAME: Ishita Singh
- DATE: 07/05/06
- COUNTRY: India
