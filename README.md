# Car-Sales-Analysis
This is a US dataset of over 23,000 records on the sales of cars.

---
## Contents
Project Overview | Data Source | Tools Used | Table Outlay | Query Languages (SQL) | Visualization

---
## Project Overview:
>> This project analyzes a car sales dataset from a U.S.-based company to uncover valuable insights into sales performance and market behavior. The work involves cleaning and preparing the data, performing exploratory data analysis (EDA), and creating visualizations to highlight key factors such as pricing trends, brand competitiveness, and customer purchasing patterns. Using pivot tables, the analysis further explores metrics like total sales by transmission type and gender, regional and gender distributions, as well as sales by color and gender revenue, providing a deeper understanding of the main factors driving car sales.

## Data Sources:
www.kaggle.com/dataset

## Tools Used:
+ Pivot Table / Charts
+ PowerBI
+ SQL


## Table Outlay:
First Three Records

| Car_id | Date | Customer | Gender | Annual_Income | Dealer_Name | Company | Model | Engine | Transmission | Color | Price | Dealer_No | Body_Style | Phone | Dealer_Region |
|-----|-----|-----|------|-----|-----|-----|------|-----|-----|------|-----|-----|-----|------|-----|
| C_CND_000001 | 01/02/2022 |	Geraldine |	Male |	13500	| Buddy Storbeck's Diesel Service Inc	| Ford	| Expedition	| DoubleÃ‚Â Overhead Camshaft	| Auto |	Black | 26000	| 06457-3834 | SUV |  8264678 | Middletown |
| C_CND_000002 | 01/02/2022 |	Gia |	Male |	1480000 |	C & M Motors Inc |	Dodge |	Durango |	DoubleÃ‚Â Overhead Camshaft |	Auto |	Black | 19000 | 60504-7114 | SUV | 6848189 | Aurora |
| C_CND_000003 | 01/02/2022 |	Gianna |	Male | 1035000 |	Capitol KIA |	Cadillac |	Eldorado |	Overhead Camshaft |	Manual |	Red | 31500 | 38701-8047 | Passenger | 7298798 | Greenville |

## Query Language: (SQL)
Some of the query language to retrieve records are displayed here
```SQL
--- Retrieve the types of Body_Style, arranging from largest to smallest sold amount.

SELECT Body_Style, COUNT( Body_Style) AS 'Total' FROM new_car_dataset
GROUP BY Body_Style
ORDER BY Total Desc
;

```
```SQL
--- Leading Dealer Region by sales
SELECT Dealer_Region, SUM(Price) AS 'Total_Sales' FROM new_car_dataset
GROUP BY Dealer_Region
ORDER BY Total_Sales DESC
;
```
```SQL
--- Retrieve Sale by Gender distribution, from highest to least
SELECT Gender, COUNT(Gender) AS 'Total_Gender', SUM(Price) AS 'Total_Price' FROM new_car_dataset
GROUP BY Gender
ORDER BY Total_Price DESC
;
```

## Visualization
### Pivot Tables
<img width="1081" height="528" alt="new car dataset_ pivot tables 2" src="https://github.com/user-attachments/assets/26817a8c-f7fc-4059-a77d-832df2153f84" />

## Charts
![Car Chart II](https://github.com/user-attachments/assets/cf536f7d-d4ab-40a3-8f76-83985306cc9d)

### PowerBI Dashboard
<img width="882" height="503" alt="CAR DATA SET PowerBI" src="https://github.com/user-attachments/assets/27cf96e4-af62-4658-8dde-a7bb3532e195" />

#### Here is the link to my LinkedIn profile:
https://www.linkedin.com/in/ogo-oluwa-adeyemo/


