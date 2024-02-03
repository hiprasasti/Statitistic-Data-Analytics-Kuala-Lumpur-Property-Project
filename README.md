# Statitistic-for-Kuala-Lumpur-Property-Project

## Project
The data set is in raw version, therefore need several actions of cleaning and restructurize to be able for statistic analysis and discover the right property price.
Link: https://docs.google.com/spreadsheets/d/1rVKZonBbf19T8rlHl9Bkir35IfG_SNhN/edit?usp=drive_link&ouid=114753462952958042582&rtpof=true&sd=true

## Data Used
**Data** - Kuala Lumpur property with 5001 rows and 8 columns.

**Data Cleaning** - Google Spreadsheet.

**Analysis** -  XLMiner Toolpak, extensions in Google Spreadsheets.


## Business Questions
1. How many unit properties in the database that ready in the market?
2. What is the minimum, maximum, mean, and median price in the market?
3. How many minimum, maximum, and mean of total rooms?
4. How many mean number of bathrooms?
5. Top 3 locations in Kuala Lumpur based on number of properties?
6.  What kind of properties characteristics of those properties?
7.  Top 3 locations in Kuala Lumpur based on average price?
8.  What factor that related to pricing in Mont. Kiara? 
9.  How much price of the house in Mont.Kiara with 3 rooms, 2 bathrooms, 2 carparks and 100sqft that you recommended?

## Cleaning and Structurize Steps
1. Remove duplicates and trim white spaces.
2. On Location column:
+ remove Kuala Lumpur from Location column.
+ check typo with pivot table.
+ check real location, in case any location located within other area.
3. On Price column:
+ remove row(s) with blank price.
+ remove the RM in price with split function.
4. On Rooms column:
+ remove row(s) with blank rooms.
+ replace studio with 0, and sum up all the total rooms.
5. On Bathrooms column, remove all blank bathrooms, and check the data.
6. On Car Parks column, keep blank as 0 number, assuming the property doesn't have any parking space.
7. On Furnishing column: keep blank rows and unknown unfurnished and transform it into code.
8. On Land Type and Size column, split the type of the land and convert all to sq.ft. Please recalcultae if the re is data with different measurement.
9. Checking outliers:
+ by using Upper Inner fence and Lower Inner fence, and IQR remove outliers with farther relations price and numbers.


## Summary of Findings
+ After cleaning process, there are 4270 units that available in the property market.
+ Descriptive analysis on price available in the deck.
+ Average unit price in KL is RM 1.595.457
+ Average room per unit are 3 to 4 rooms.
+ Average bathroom per unit are 3 bathrooms.
+ Average car parks is 1.
+ Averaga unit size is 1933 sq.ft.
+ Top three location in Kuala Lumpur based on number of properties are Mont. Kiara with 633 properties, KLCC with 511 properties, and Desa ParkCity with 314 properties. Each charactheristics available at presentation deck.
+ Top three location in Kuala Lumpur based on wisely-average-price are Bukit Kiara, federal Hill, and Semarak.
+ From statistic correlation analysis, size is the biggest factor in controlling property price, following by number of rooms and bathrooms.
+ Price recommendation in Mont. Kiara with 3 rooms, 2 bathrooms, 2 car parks and size only 100 sq.ft is RM 272.925 (note to remind, the size is the minimum, therefore the house is 3 or 2 and half story).

## Limitations
- Some records had not country information, and these were exclude during querying.
- Some records had 0 adr

## Result
+ Property in Kuala Lumpur dexk can be access here: https://drive.google.com/file/d/1JczK3eu6zPMJrdI8h81mqvw1MAA45nrB/view?usp=drive_link
