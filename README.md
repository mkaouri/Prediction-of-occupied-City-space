# The biggest problem of a city in year 2400

## Introduction

Al-Khiyam, the beautiful city in south of Lebanon. Recently, the city is growing rapidly, especially in new homes, commercial buildings and public places such as service facilities, gardens and streets.
 I had a curiosity to know when the area of the city would be completely occupied by buildings and public places. Accordingly, I thought of searching the GIS maps of the Google Earth application, hoping to find historical maps of Al-Khiyam city for use in statistical prediction. While researching Google Earth, I found that there are historical maps of that city from 2004 to 2017. Accordingly, the most accurate maps to choose from are the maps 2004, 2008, 2010, 2013 and 2016. These maps were used in the prediction to obtain accurate results for the year in which the area of the city is fully occupied. Based on the statistical prediction, Al-Khiyam city will be fully occupied by buildings and public places in 2400. Yes, it is still too early, but is not it the biggest problem for future generations?

## Historical GIS maps of Al-Khiyam City from Google Earth

Below screenshots of Al-Khiyam city historical GIS maps from Google Earth for years 2004, 2008, 2010, 2013, and 2016 respectively. (Figures 1-5)

### Al-Khiyam City map of year 2004

![Alt text](/images/2004.jpg?raw=true "Al-Khiyam City map of year 2004") 
Figure 1. Shows the GIS map of Al-Khiyam city, south of Lebanon, of year 2004 from Google Earth.

### Al-Khiyam City map of year 2008

![Alt text](/images/2008.jpg?raw=true "Al-Khiyam City map of year 2008") 
Figure 2. Shows the GIS map of Al-Khiyam city, south of Lebanon, of year 2008 from Google Earth.

### Al-Khiyam City map of year 2010

![Alt text](/images/2010.jpg?raw=true "Al-Khiyam City map of year 2010") 
Figure 3. Shows the GIS map of Al-Khiyam city, south of Lebanon, of year 2010 from Google Earth.

### Al-Khiyam City map of year 2013

![Alt text](/images/2013.jpg?raw=true "Al-Khiyam City map of year 2013")
Figure 4. Shows the GIS map of Al-Khiyam city, south of Lebanon, of year 2013 from Google Earth.

### Al-Khiyam City map of year 2016

![Alt text](/images/2016.jpg?raw=true "Al-Khiyam City map of year 2016")
Figure 5. Shows the GIS map of Al-Khiyam city, south of Lebanon, of year 2016 from Google Earth.

## Converting the GIS maps into readable data

Now, to make the maps readable by the prediction analysis model, I had to convert it into black and white using a graphic designer tool. The black color is the area without buildings and public places and the white color is the area with buildings and public places. I only used in my analysis the border of Al-Khiyam Mountain from Al-Dardara Lake, west, to the east of the Mountain, excluding the area of the agriculture (Figure 6). 

![Alt text](/images/2016.png?raw=true "Al-Khiyam city border")
Figure 6. Shows Al-Khiyam city border that is considered in the prediction analysis.

Below are the converted screenshots of the maps by considering only the specified border. (Figures 7-11)

### Converted map into black and white of Al-Khiyam City border for year 2004

![Alt text](/images/2004b.jpg?raw=true "Converted map into black and white of Al-Khiyam City border for year 2004")
Figure 7. Shows the converted map into black and white of Al-Khiyam City border for year 2004.

### Converted map into black and white of Al-Khiyam City border for year 2008

![Alt text](/images/2008b.jpg?raw=true "Converted map into black and white of Al-Khiyam City border for year 2008")
Figure 8. Shows the converted map into black and white of Al-Khiyam City border for year 2008.

### Converted map into black and white of Al-Khiyam City border for year 2010

![Alt text](/images/2010b.jpg?raw=true "Converted map into black and white of Al-Khiyam City border for year 2010")
Figure 9. Shows the converted map into black and white of Al-Khiyam City border for year 2010.

### Converted map into black and white of Al-Khiyam City border for year 2013

![Alt text](/images/2013b.jpg?raw=true "Converted map into black and white of Al-Khiyam City border for year 2013")
Figure 10. Shows the converted map into black and white of Al-Khiyam City border for year 2013.

### Converted map into black and white of Al-Khiyam City border for year 2016

![Alt text](/images/2016b.jpg?raw=true "Converted map into black and white of Al-Khiyam City border for year 2016")
Figure 11. Shows the converted map into black and white of Al-Khiyam City border for year 2016.

Below chart shows the average growth of the occupied spaces of Al-Khiyam city from year 2004 to 2016. (Figure 12)
Average Growth of Occupied Spaces in Al-Khiyam City
Figure 12. Shows the average growth of the occupied spaces of Al-Khiyam city from year 2004 to 2016.

## Creating a virtual map of fully occupied spaces for prediction

I used the above average growth binary values of black and white as an input into my prediction model of linear regression algorithm to train and test its prediction accuracy and make sure it’s working properly before predicting the year of fully occupied space. The recorded accuracy score is equal to: 90.6% which is a good score to start the prediction process.
To predict our big problem year, I had to create a demonstration of virtual city of Al-Khiyam in future as an approximate fully occupied spaces. As shown in the below screenshot. (Figure 13)

![Alt text](/images/khiyam_full.png?raw=true "Virtual city map of Al-Khiyam in future")
Figure 13. Shows the virtual city map of Al-Khiyam in future as an approximate fully occupied spaces.

So, I converted the above virtual map of fully occupied city spaces into black and white (Figure 14) to feed it into the prediction model.

![Alt text](/images/prediction_features.jpg?raw=true "Converted virtual city map of Al-Khiyam of fully occupied spaces")
Figure 13. Shows the converted virtual city of Al-Khiyam of fully occupied spaces into black and white.

## Predicting the big problem

As mentioned before, I used the Linear Regression algorithm to build a prediction model to predict the future year where the city will be fully occupied with buildings.
I have trained the prediction model with binary data of the converted GIS Maps of black and white for years 2004, 2008, 2010, 2013, and 2016 and tested the model with sample existing data to get accuracy of 90.6%, then used that model to predict the unknown year using the average binary data of the virtual GIS map of fully occupied spaces.
The result of the prediction model on the above converted virtual map is approximately equal to 2400.





