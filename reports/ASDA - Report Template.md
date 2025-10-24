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
| Authors of the dataset |not provided on Kaggle   |
| Source (name) |Kaggle   |
| Source (link) |https://www.kaggle.com/datasets/camnugent/california-housing-prices?select=housing.csv   |

**Short description (what is it about?)**

---

## 2. Structure of the Dataset

| Column name | Data type | Non-null count | Unique values | Example values |
|--------------|------------|----------------|----------------|----------------|
|   |   |   |   |   |
|   |   |   |   |   |
|   |   |   |   |   |

---

## 3. Descriptive Statistics

### Numeric Columns

|   | Column 1 | Column 2 | Column 3 |
|---|-----------|-----------|-----------|
| Count |   |   |   |
| Mean |   |   |   |
| Standard deviation |   |   |   |
| Min |   |   |   |
| 25% |   |   |   |
| 50% |   |   |   |
| 75% |   |   |   |
| Max |   |   |   |

### Categorical / Object Columns

|   | Column 1 | Column 2 | Column 3 |
|---|-----------|-----------|-----------|
| Count |   |   |   |
| Number of unique values |   |   |   |
| Most frequent value |   |   |   |
| Most frequent value (frequency) |   |   |   |
| Least frequent value |   |   |   |
| Least frequent value (frequency) |   |   |   |

---

## 3. Missing Values and Duplicates

| Column name | Missing count | % Missing |
|--------------|----------------|------------|
|   |   |   |
|   |   |   |
|   |   |   |

**Total missing values:**  
**Percentage of dataset affected:**  

**Duplicated rows found:**  
**Percentage of rows in dataset affected:**

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

- Is it worth it to further analyze the dataset?  
- What possible analyses can be performed?

---

## 6. Next Steps

- Handling missing values? How?  
- Removing duplicates?  
- Cleaning the columns? Which?  
- Creating a subset of the dataframe? 


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

|   | Column 1 | Column 2 | Column 3 |
|---|-----------|-----------|-----------|
| Count |   |   |   |
| Mean |   |   |   |
| Standard deviation |   |   |   |
| Min |   |   |   |
| 25% |   |   |   |
| 50% |   |   |   |
| 75% |   |   |   |
| Max |   |   |   |

### Categorical / Object Columns

|   | Column 1 | Column 2 | Column 3 |
|---|-----------|-----------|-----------|
| Count |   |   |   |
| Number of unique values |   |   |   |
| Most frequent value |   |   |   |
| Most frequent value (frequency) |   |   |   |
| Least frequent value |   |   |   |
| Least frequent value (frequency) |   |   |   |

---

## 3. Missing Values and Duplicates

| Column name | Missing count | % Missing |
|--------------|----------------|------------|
|   |   |   |
|   |   |   |
|   |   |   |

**Total missing values:**  
**Percentage of dataset affected:**  

**Duplicated rows found:**  
**Percentage of rows in dataset affected:**

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

