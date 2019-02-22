# Dataset Exploration with Ford GoBike System Data
## by Xi Zhou


## Data source :
Ford GoBike System Data : https://www.fordgobike.com/system-data This data set includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area .

## Features :
Trip Duration (seconds) , Start Time and Date , End Time and Date , Start Station ID , Start Station Name , Start Station Latitude , Start Station Longitude , End Station ID , End Station Name, End Station Latitude , End Station Longitude , Bike ID , User Type (Subscriber or Customer – “Subscriber” = Member or “Customer” = Casual) , Member Year of Birth, Member Gender

## Questions to be answered:
How long does the average trip take?
Is the trip duration affected by weather( months/seasons)
Does the above depend on if a user is a subscriber or customer?

## Summary of findings :
Since the trip duration has a close relationship with bike share company's revenue, I tried to find out what are the key factors affect trip duration. It turns out that Weather does not have a big effect on the trip duration but user type does have an impact on trip duration. According the analysis, I found subscribers tend to rend the bikes for longer trips ( generally above 300 minutes ). One possible way to increase revenue is to attract more potential customers and convert more exiting customers to subscribers.

## References:
* https://stackoverflow.com/questions/26942476/reading-csv-zipped-files-in-python    read in files in a zip file
* pandas datetimeindex docs: https://pandas.pydata.org/pandas-docs/stable/generated/pandas.DatetimeIndex.html
* https://github.com/Alicelibinguo/Python-Explore-BikeShare-Data/blob/master/Bike_Share_Analysis%20.ipynb   (helpful)
* https://www.google.com/search?rlz=1C1SQJL_enUS762US762&q=bike+share+analysis+ipynb&sa=X&ved=2ahUKEwjmo7PcrLXgAhXprFQKHVJrBnAQ1QIoBXoECAUQBg
* https://github.com/NickZward/Nanodegree-Data-Analyst/blob/master/Project%205/exploration.ipynb      ( helpful)
* https://github.com/seby-sbirna/Data-Analyst-Nanodegree-Project-Portfolio/blob/master/Project%205%20-    %20Communicate%20Data%20Findings/README.md
