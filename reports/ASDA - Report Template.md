# Basic EDA of Two Datasets – Report Structure for Week 2

---
# Dataset 1
## 1. Dataset Overview

| Item Description |   |
|-------------------|---|
| Dataset name |California Housing Prices   |
| Number of rows |20640   |
| Number of columns |10   |
| Format file (.csv, .txt, etc) |.csv   |
| Authors of the dataset |Cam Nugent   |
| Source (name) |Kaggle   |
| Source (link) |https://www.kaggle.com/datasets/camnugent/california-housing-prices?select=housing.csv   |

**Short description (what is it about?)**
The data pertains to the houses found in a given California district and some summary stats about them based on the 1990 census data.

---

## 2. Structure of the Dataset

| Column name        | Data type   |   Non-null count |   Unique values | Examples                                         |
|:-------------------|:------------|-----------------:|----------------:|:-------------------------------------------------|
| longitude          | float64     |            20640 |             844 | -121.88, -121.32, -119.33, -117.98, -117.65      |
| latitude           | float64     |            20640 |             862 | 37.46, 38.59, 36.3, 33.76, 34.12                 |
| housing_median_age | float64     |            20640 |              52 | 5.0, 24.0, 11.0, 29.0, 17.0                      |
| total_rooms        | float64     |            20640 |            5926 | 1819.0, 4378.0, 3045.0, 1518.0, 3006.0           |
| total_bedrooms     | float64     |            20433 |            1923 | 245.0, 910.0, nan, 312.0, 427.0                  |
| population         | float64     |            20640 |            3888 | 802.0, 2149.0, 1563.0, 1086.0, 1291.0            |
| households         | float64     |            20640 |            1815 | 228.0, 812.0, 516.0, 317.0, 406.0                |
| median_income      | float64     |            20640 |           12928 | 10.9722, 2.5035, 5.4337, 4.32, 6.2083            |
| median_house_value | float64     |            20640 |            3842 | 500001.0, 123700.0, 133800.0, 196900.0, 242700.0 |
| ocean_proximity    | object      |            20640 |               5 | <1H OCEAN, INLAND, INLAND, <1H OCEAN, INLAND     |

---

## 3. Descriptive Statistics

### Numeric Columns

|       |   longitude |    latitude |   housing_median_age |   total_rooms |   total_bedrooms |   population |   households |   median_income |   median_house_value |
|:------|------------:|------------:|---------------------:|--------------:|-----------------:|-------------:|-------------:|----------------:|---------------------:|
| count | 20640       | 20640       |           20640      |      20640    |        20433     |     20640    |     20640    |     20640       |                20640 |
| mean  |  -119.57    |    35.6319  |              28.6395 |       2635.76 |          537.871 |      1425.48 |       499.54 |         3.87067 |               206856 |
| std   |     2.00353 |     2.13595 |              12.5856 |       2181.62 |          421.385 |      1132.46 |       382.33 |         1.89982 |               115396 |
| min   |  -124.35    |    32.54    |               1      |          2    |            1     |         3    |         1    |         0.4999  |                14999 |
| 25%   |  -121.8     |    33.93    |              18      |       1447.75 |          296     |       787    |       280    |         2.5634  |               119600 |
| 50%   |  -118.49    |    34.26    |              29      |       2127    |          435     |      1166    |       409    |         3.5348  |               179700 |
| 75%   |  -118.01    |    37.71    |              37      |       3148    |          647     |      1725    |       605    |         4.74325 |               264725 |
| max   |  -114.31    |    41.95    |              52      |      39320    |         6445     |     35682    |      6082    |        15.0001  |               500001 |

### Categorical / Object Columns

|                                  | ocean_proximity   |
|:---------------------------------|:------------------|
| Count                            | 20640             |
| Number of unique values          | 5                 |
| Most frequent value              | <1H OCEAN         |
| Most frequent value (frequency)  | 9136              |
| Least frequent value             | ISLAND            |
| Least frequent value (frequency) | 5                 |
---

## 3. Missing Values and Duplicates

| Column name        |   Missing count |   % Missing |
|:-------------------|----------------:|------------:|
| longitude          |               0 |     0       |
| latitude           |               0 |     0       |
| housing_median_age |               0 |     0       |
| total_rooms        |               0 |     0       |
| total_bedrooms     |             207 |     1.00291 |
| population         |               0 |     0       |
| households         |               0 |     0       |
| median_income      |               0 |     0       |
| median_house_value |               0 |     0       |
| ocean_proximity    |               0 |     0       |

**Total missing values:** 207

**Percentage of dataset affected:** 0.10%

**Duplicated rows found:** 0

**Percentage of rows in dataset affected:** 0.00%

---

## 4. Data Consistency

| Item | Description |
|------|--------------|
| Does the dataset contain unnecessary columns? Which? | Yes, the Dataset contains Unnecessary columns such as longitude and Latitude    |
| Do the data types correspond to the columns? |   |
| Is the labeling of the columns appropriate? | somehow because the first letters of the labels can be capitalize for example latitude to Latitude.  |
| Are there mixed values in a column (e.g., numbers and characters)? | Yes, in the column Ocean_promity(<1H OCEAN).  |
| Are string columns clean? | Yes  |
| Does the dataset look machine generated? | Yes because no spelling inconsistency, no extra spaces found. Data is well formatted.  |
| Other |   |

---

## 5. Overall Assessment

**Is it worth it to further analyze the dataset?**
Yes, definitely. What we've done so far is a good foundation on analyzing the data set but we can surely analyze it further to explore and visualize it.

**What possible analyses can be performed?**
We can perform analyses on the outliers, check for trends (if any), populating the missing values. Also can see if data needs correction aginst its data type. 

---

## 6. Next Steps

**Handling missing values? How?**
The dataset has missing values only in the total_bedrooms column (about 1%).
Since this is a small portion of the data, we can handle it in several ways:
Replace missing values with the median of the column;
Replace with the mean;
Remove the rows with missing values.

**Removing duplicates?** 
When checking for duplicates, we found 0 duplicated rows in the dataset.
This means every record (district) is unique, and no two rows contain the same information.
Therefore, no action is needed — the dataset already has clean, non-duplicate data.
- Cleaning the columns? Which?  
- Creating a subset of the dataframe? 

END OF DATASET 1
____________________________________________________________________________________________________

# Dataset 2

## 1. Dataset Overview

| Item Description |   |
|-------------------|---|
| Dataset name |Amazon_Delivery_Dataset   |
| Number of rows |43739   |
| Number of columns |16   |
| Format file (.csv, .txt, etc) |.csv   |
| Authors of the dataset | Sujal Suthar   |
| Source (name) |Kaggle   |
| Source (link) |https://www.kaggle.com/datasets/sujalsuthar/amazon-delivery-dataset   |

**Short description (what is it about?)**
This Amazon Delivery Dataset provides a comprehensive view of the company's last-mile logistics operations. The dataset enables researchers and analysts to uncover insights into factors influencing delivery efficiency, identify areas for optimization, and explore the impact of various variables on the overall customer experience.

---

## 2. Structure of the Dataset

| Column name     | Data type   |   Non-null count |   Unique values | Examples                                                                  |
|:----------------|:------------|-----------------:|----------------:|:--------------------------------------------------------------------------|
| Order_ID        | object      |            43739 |           43739 | ysql652484304, omei605786978, xxor408538921, digx266253552, nlsl993697678 |
| Agent_Age       | int64       |            43739 |              22 | 35, 29, 27, 23, 30                                                        |
| Agent_Rating    | float64     |            43685 |              28 | 4.6, 4.6, 4.7, 4.0, 4.3                                                   |
| Store_Latitude  | float64     |            43739 |             521 | 12.310972, 12.304569, 23.374878, 18.592718, 22.311358                     |
| Store_Longitude | float64     |            43739 |             415 | 76.659264, 76.643622, 85.335739, 73.773572, 73.164798                     |
| Drop_Latitude   | float64     |            43739 |            4367 | 12.380972, 12.314569, 23.394878, 18.612718, 22.361358                     |
| Drop_Longitude  | float64     |            43739 |            4367 | 76.729264, 76.653622, 85.355739, 73.793572, 73.214798                     |
| Order_Date      | object      |            43739 |              44 | 2022-04-02, 2022-03-11, 2022-03-03, 2022-03-13, 2022-03-24                |
| Order_Time      | object      |            43739 |             177 | 20:40:00, 08:10:00, 08:20:00, 11:55:00, 20:30:00                          |
| Pickup_Time     | object      |            43739 |             193 | 20:45:00, 08:25:00, 08:30:00, 12:10:00, 20:45:00                          |
| Weather         | object      |            43648 |               6 | Sandstorms, Fog, Sandstorms, Fog, Windy                                   |
| Traffic         | object      |            43739 |               5 | Jam , Low , Low , High , Jam                                              |
| Vehicle         | object      |            43739 |               4 | motorcycle , scooter , scooter , scooter , motorcycle                     |
| Area            | object      |            43739 |               4 | Metropolitian , Urban , Metropolitian , Metropolitian , Metropolitian     |
| Delivery_Time   | int64       |            43739 |              89 | 53, 85, 55, 160, 180                                                      |
| Category        | object      |            43739 |              16 | Grocery, Skincare, Sports, Shoes, Books                                   |


---

## 3. Descriptive Statistics

### Numeric Columns

|       |   Agent_Age |   Agent_Rating |   Store_Latitude |   Store_Longitude |   Drop_Latitude |   Drop_Longitude |   Delivery_Time |
|:------|------------:|---------------:|-----------------:|------------------:|----------------:|-----------------:|----------------:|
| count | 43739       |   43685        |      43739       |        43739      |     43739       |       43739      |      43739      |
| mean  |    29.5671  |       4.63378  |         17.211   |           70.6612 |        17.459   |          70.8218 |        124.906  |
| std   |     5.81516 |       0.334716 |          7.76423 |           21.475  |         7.34295 |          21.1531 |         51.9155 |
| min   |    15       |       1        |        -30.9029  |          -88.3662 |         0.01    |           0.01   |         10      |
| 25%   |    25       |       4.5      |         12.9333  |           73.1703 |        12.986   |          73.28   |         90      |
| 50%   |    30       |       4.7      |         18.5514  |           75.8985 |        18.6336  |          76.0026 |        125      |
| 75%   |    35       |       4.9      |         22.7322  |           78.0454 |        22.785   |          78.1041 |        160      |
| max   |    50       |       6        |         30.9141  |           88.4335 |        31.0541  |          88.5635 |        270      |

### Categorical / Object Columns

|                                  | Order_ID      | Order_Date   | Order_Time   | Pickup_Time   | Weather   | Traffic   | Vehicle    | Area          | Category    |
|:---------------------------------|:--------------|:-------------|:-------------|:--------------|:----------|:----------|:-----------|:--------------|:------------|
| Count                            | 43739         | 43739        | 43739        | 43739         | 43648     | 43739     | 43739      | 43739         | 43739       |
| Number of unique values          | 43739         | 44           | 177          | 193           | 6         | 5         | 4          | 4             | 16          |
| Most frequent value              | ialx566343618 | 2022-03-15   | 21:55:00     | 21:30:00      | Fog       | Low       | motorcycle | Metropolitian | Electronics |
| Most frequent value (frequency)  | 1             | 1141         | 460          | 481           | 7440      | 14999     | 25527      | 32698         | 2849        |
| Least frequent value             | ialx566343618 | 2022-02-18   | 16:30:00     | 16:20:00      | Sunny     | NaN       | bicycle    | Semi-Urban    | Shoes       |
| Least frequent value (frequency) | 1             | 819          | 51           | 36            | 7078      | 91        | 15         | 152           | 2666        |

---

## 3. Missing Values and Duplicates


| Column name     |   Missing count |   % Missing |
|:----------------|----------------:|------------:|
| Order_ID        |               0 |    0        |
| Agent_Age       |               0 |    0        |
| Agent_Rating    |              54 |    0.12346  |
| Store_Latitude  |               0 |    0        |
| Store_Longitude |               0 |    0        |
| Drop_Latitude   |               0 |    0        |
| Drop_Longitude  |               0 |    0        |
| Order_Date      |               0 |    0        |
| Order_Time      |               0 |    0        |
| Pickup_Time     |               0 |    0        |
| Weather         |              91 |    0.208052 |
| Traffic         |               0 |    0        |
| Vehicle         |               0 |    0        |
| Area            |               0 |    0        |
| Delivery_Time   |               0 |    0        |
| Category        |               0 |    0        |

**Total missing values:** 145

**Percentage of dataset affected:** 0.02%

**Duplicated rows found:** 0

**Percentage of rows in dataset affected:** 0.00%

---

## 4. Data Consistency

| Item | Description |
|------|--------------|
| Does the dataset contain unnecessary columns? Which? | Yes , Columns such as Store_Latitude,Store_Longitude, Drop_Latitude and Drop_Longitude. |
| Do the data types correspond to the columns? | Yes the data types correspond correctly to the nature of the data in each column  |
| Is the labeling of the columns appropriate? |  Yes |
| Are there mixed values in a column (e.g., numbers and characters)? | Yes in the first column (Order ID) have generated values from Number and Characters.  |
| Are string columns clean? | Yes  |
| Does the dataset look machine generated? | No  |
| Other |   |

---

## 5. Overall Assessment

- Is it worth it to further analyze the dataset?  
- What possible analyses can be performed?

---

## 6. Next Steps

- Handling missing values? How?  
- Removing duplicates?  
- Cleaning the columns? Which?  
- Creating a subset of the dataframe?  

