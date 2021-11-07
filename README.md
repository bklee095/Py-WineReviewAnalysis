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
 
 Remove attribute "region_2" as most of it is missing values and it isn't important for this analysis
 
 
![Capture](https://user-images.githubusercontent.com/74638365/140663740-72f4b591-7624-46fe-8cef-9383469b8361.PNG)

![carbon(3)](https://user-images.githubusercontent.com/74638365/140663797-400781fb-f371-4e87-afdf-da947202bff9.png)
![Capture1](https://user-images.githubusercontent.com/74638365/140663914-37dfc3ff-a034-42fa-8967-8d026f43d043.PNG)

_histogram and boxplots of points and prices of the wine_

Spotting multiple outliers in the price range

![Capture2](https://user-images.githubusercontent.com/74638365/140663884-0ca305d6-f812-44e5-affa-c9e0df5f7717.PNG)

_Points vs Price scatterplot_
