# MelbourneHousing-Tableau

INTRODUCTION:
Outline of the domain: Melbourne is currently experiencing a housing bubble. There are many factors which are affecting property prices in Melbourne. 
The problem is to find out when did the prices exactly started to fall down? What are the variables that showed it slowing down? What are the factors affecting the growth rate of houses in Melbourne? Can we predict future growth rate of houses there? Can we find out the Regions and Suburbs best suitable to buy a house in? which is the most expensive area in Melbourne right now?
Title: Melbourne housing market 
Source of the data:  https://www.kaggle.com/anthonypino/melbourne-housing-market
The agencies working with the data: The data was scraped from publicly available results which is posted every week in domain.com.au.
The attribute types of the data: 
The entire dataset is comprised of 21 variables with 9 variables as characters or strings
String variables:
    • Regionname: General regions like East, West, South, North etc.
    • Suburb: Suburbs that fall under a Region
    • Council Area: Governing council for the area
    • Postcode: postcode of an area
    •  Method: Method used to sell a house. S - property sold; SP - property sold prior; PI - property passed in; PN - sold prior not disclosed; SN - sold not disclosed; NB - no bid; VB - vendor bid; W - withdrawn prior to auction; SA - sold after auction; SS - sold after auction price not disclosed. N/A - price or highest bid not available 
    • SellerG: Real Estate agent
    • Address: Address of the house
    • Type: House types. 
h - house,cottage,villa, semi,terrace; 
u - unit, duplex;
t - townhouse; dev site - development site 
    • Date: date of the house sold

Measure Variables:
    • Year
    • Rooms: Number of rooms
    • Bathrooms: number of bathrooms
    • Price: Price in Australian dollars
    • Bedroom2: Scraped number of bedrooms from other sources
    • Distance: Distance from CBD (Central Business District) in kilometres.
    • Car: Number of car spots in a house.
    •  Building Area: Building size in meters
    • Landsize: Land size in meters
    • Lattitude
    • Longtitude

Link between variables:
    • Regionname and Suburb: Number of suburbs which falls under a Region.
    • Regionname and Price: Average price of the house in a Region.
    • Suburb and Price: Average price of the houses in a Suburb and the Region that Suburb falls under.
    • Landsize and Price: Relationship between landsize and price.
    • Rooms and Price: Relationship between number of rooms and price. With the increase of rooms does price increases or not?
    • Car and price: Relationship between car spots and price.
    • Rooms and Car: With the increase in number of rooms, is there any increase in cars.
    • Bathroom and rooms: With the increase in rooms, is there any increase in the bathrooms.
    • Landsize and rooms: With the increase in landsize, is there any increase in the number of rooms.
    • Landsize and buildingarea: Relationship between landsize and building area.
    • Distance and Suburbs: Suburbs which has the nearest distance from CBD.
    • Date and price: Months in which price are highest and lowest.
    • Date and sale: Months when the demand is maximum.

OBJECTIVE:
Melbourne housing market has cooled off. By performing this exploratory data analysis various factors can be analyzed through which we can find out the reason affecting the sales.
    • When did the pricing started to fall down?
    • Variables that showed it slowing down.
    • Regions where the houses were sold the most.
    • Prices were more in those regions or less?
    • Suburbs with the highest sales.
    • Region, where more houses are sold are away from CBD or closer in distance and what are the prices there? More or less?
    • Top 10 suburbs most popular among buyers.
    • Price of the houses in those suburbs, are they expensive or not?
    • Type of the houses which are being sold the most.
    • Price of those types.
    • Future predictions that in upcoming years price will increase or not?
    • Which regions will see the growth again in upcoming years?
    • What type of houses will that be? “h”, “t” or “u”?
    • Will the land size increase with the price or decrease?
    • What is the relation between building area and land size now?
    • Does the number of rooms increase with the land size?
    • Is there any relation between number of rooms, land size and car spots?

The information retrieved from these data can be used by Property dealers, customers planning to buy a house, builders, sellers and estate agents.
1) Builders can analyse the type of property most of the people prefer to buy by looking at the statistics and accordingly plan to construct a house.
2) The area most popular among people where houses can be built.
3) number of bedrooms people are preferring to buy.
4) Customers can make predictions on the prices of the house in future and purchase a house accordingly if they are planning to make an investment.  
5) Both buyers and sellers can see from the predictions generated, the Regions and Suburbs where there will be hike in the future or not?
6) Customers planning to buy a house, can see from the data, which type of house has seen the most hike in past.
7) Builders can check the period in the year when the demand is highest, and they can accordingly make maximise their sale at that time of the year.

Data preparation:
Before applying the dataset for house price prediction, it needs to be pre- processed and cleaned. The original dataset downloaded from Kaggle consists of 34,857 records and 21 attributes.
Attributes like “Landsize” and “Buildingarea” consisted of data too small to exist. First these data need to be removed because values as less as 100 cannot be used as landsize or buildingarea for a house. So, all the records having landsize and buildingarea less than 100 was removed. 
More than 50% of the data have missing values. All the missing values were replaced with the average of the data.
After performing the cleaning and pre-processing of the data, 5301 records were left. Further analysis was performed on these records.
