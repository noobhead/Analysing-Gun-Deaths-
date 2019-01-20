# Analysing-Gun-Deaths

This project explores the trends(if any) that exists in the Gun Deaths in US from 2012 to 2014 and try to find patterns in the demographics of the victims. We will explore the gun deaths on the time of occurence using the datetime module. Analysing if the gun deaths vary on the basis of race and gender. However, my analysis only gives us the total number of gun deaths by race in the US. Unless we know the proportion of each race in the US, we won't be able to meaningfully compare those numbers. What we really want to get is a rate of gun deaths per 100000 people of each race. In order to do this, we'll need to read in data about what percentage of the US population falls into each racial category. For this we'll use the census data to help and answer above question.


# About the Dataset

The dataset came from [FiveThirtyEight](https://fivethirtyeight.com/), and can be found [here](https://github.com/fivethirtyeight/guns-data). The dataset is stored in the **guns.csv file**. It contains information on gun deaths in the US from 2012 to 2014. Each row in the dataset represents a single fatality. The columns contain demographic and other information about the victim.

The csv file has following attributes:

-- this is an identifier column, which contains the row number. It's common in CSV files to include a unique identifier for each row, but we can ignore it in this analysis.

year -- the year in which the fatality occurred.

month -- the month in which the fatality occurred.

intent -- the intent of the perpetrator of the crime. This can be Suicide, Accidental, NA, Homicide, or Undetermined

police -- whether a police officer was involved with the shooting. Either 0 (false) or 1 (true)

sex -- the gender of the victim. Either M or F.

age -- the age of the victim

race -- the race of the victim. Either Asian/Pacific Islander, Native American/Native Alaskan, Black, Hispanic, or White

place -- where the shooting occurred. Has several categories, which you're encouraged to explore on your own.

education -- educational status of the victim. Can be one of the following:

1 -- Less than High School
2 -- Graduated from High School or equivalent
3 -- Some College
4 -- At least graduated from College
5 -- Not available

The census data contains information on the total population of the US, as well as the total population of each racial group in the US. The data is stored in the **census.csv file**, and only consists of two rows:

- the first row is a header row
- the second row consists of population counts
