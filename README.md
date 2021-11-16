![Wine_Enthusiast_Review_Analysis(1)](https://user-images.githubusercontent.com/74638365/140579630-811933db-7604-4b2f-96f7-1784da484da2.png)

![GitHub last commit](https://img.shields.io/github/last-commit/bklee095/Py-WineReviewAnalysis)

# 2017 Wine Enthusiast Review Analysis

## Dataset
[Data source URL](https://www.kaggle.com/zynicide/wine-reviews?select=winemag-data_first150k.csv)

This dataset is a compile of a total of ~150,000 rows of wine reviews from the world renowned multi-channel wine marketer, the Wine Enthusiast Companies. Well known for their Wine Enthusiast Magazine, the Wine Enthusiast provides introduction to the wine industry and the lastest trends, along with numerous ratings and reviews. While anything that involves flavors and their respective ratings are bound to be highly subjective, these types of publishments are commonly accepted to be good guideline and reference for the consumers.

This dataset consists of a total of 11 columns on the wines, including the country of origin, the state/province of origin, the region of harvest, the name of the winery, the vineyard within the winery, the grape varietal, the purchasing price, the point ratings, and the review (description).

<br/><br/>

## Data Cleaning

![carbon(1)](https://user-images.githubusercontent.com/74638365/140630174-eb5eec8f-c9f1-491b-9e94-2c2fc2085017.png)

['num' 'points' 'price']

['country' 'description' 'designation' 'province' 'region_1' 'region_2'
 'variety' 'winery']
 
 ![carbon(2)](https://user-images.githubusercontent.com/74638365/140630214-86d760b1-ba82-43fa-b99d-ab6f219eaa3c.png) 
 
![Capture](https://user-images.githubusercontent.com/74638365/140663740-72f4b591-7624-46fe-8cef-9383469b8361.PNG)

_*Missing value plot for each column_

 Remove attribute "region_2" as most of it is missing values and it isn't important for this analysis

<br/><br/>
![carbon(3)](https://user-images.githubusercontent.com/74638365/141885973-1c4b1a84-5156-4840-b643-b8bca18c2137.png)
![Capture1](https://user-images.githubusercontent.com/74638365/141885988-0e08f842-1090-44f5-bf3b-c585f5858b73.PNG)

_*Histogram and boxplots of points and prices of the wine_

There are too many outliers in the price range as examples listed below (namely some Grand Cru): 

![Capture2](https://user-images.githubusercontent.com/74638365/141886367-3b37afed-179e-42cc-9e1f-85d121ff4e6f.PNG)

Remove outliers ($400+ per bottle) in price range, removing 154 data entries
![Capture3](https://user-images.githubusercontent.com/74638365/141886545-6b8c6093-145f-4621-bc47-f487cabc1f7b.PNG)

_*Histograms and boxplots of points and prices of the wine after removing the outliers_

<br/>
No duplicate records detected in the dataset

<br/><br/>

## Exploratory Data Analysis
![carbon(4)](https://user-images.githubusercontent.com/74638365/141888210-67532586-1ea7-4ac1-b144-0f9528c46585.png)

![Capture4](https://user-images.githubusercontent.com/74638365/141888194-a7bd3fd1-d6dc-4def-8235-79f2b1194bb5.PNG)

_Points vs Price scatter plot with trend line_

<br/>
Correlation coefficient between points and price

Pearson's R = 0.5190, P-value ~= 0.0

<br/><br/>
![carbon(5)](https://user-images.githubusercontent.com/74638365/141888625-22894b01-56df-484f-832f-b9ab4a92a403.png)


Star Rating | Points
----|----
1 star | 80 ~ 84 points
2 star | 85 ~ 89 points
3 star | 90 ~ 94 points
4 star | 95 ~ 99 points
5 star | 100 points
<br/>

![carbon(6)](https://user-images.githubusercontent.com/74638365/141888947-bfe4a1b1-9947-48c5-8a85-ddcd3efd2624.png)

![Capture5](https://user-images.githubusercontent.com/74638365/141888968-655b9f4b-8db6-43c9-a105-ccf015934b41.PNG)

_* Amount of wines per star rating_

<br/>

![carbon(7)](https://user-images.githubusercontent.com/74638365/141888960-a6882927-d3fa-479d-9ffc-6ff4a65afe86.png)
![Capture6](https://user-images.githubusercontent.com/74638365/141888973-70a3afe3-343b-4221-bc4f-0ef13d612c64.PNG)

_* Average price per star rating_
