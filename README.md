# Customer_Behaviour_Analysis

## Project Overview:
The customer shopping behaviour using transactional data from 3900 purchases across various product categories. The goal is uncover insights into spending pattern, customer segments, product preferences, and subscription behaviour to guide the business insights

## Data Summary:
Rows: 3900, columns: 18
Key Features: 
- Customer Demographics(Age, Location, Gender, Subscription Status)
- Purchase details('item_purchased', 'category', 'purchase_amount', 'size', 'color', 'season')
- Shopping Behaviour(review_rating', 'shipping_type', 'discount_applied', 'promo_code_used','previous_purchases',
  'payment_method', 'frequency_of_purchases')
- Missing Data : 37 values in Review rating Column.

## EDA using Python:
We began exploring data for preparing and cleaning using python(pandas).
- Data Loading : Imported the dataset using Pandas as a copy.
- Initial exploration is done using pandas methods using info() to check the data structure and describe() method to
  understand the statistical measures of the data.
  
  <img width="350" height="349" alt="image" src="https://github.com/user-attachments/assets/1e733357-45ac-4ea2-a7b7-06e8f69b8fb7" /><img width="450" height="250" alt="image" src="https://github.com/user-attachments/assets/4d95bac8-d539-4cc7-bd97-58f0088359a3" />

### Handling Null Values:
check for null values and imputed missing values in the Review rating column using median rating of each product category. 
### Column Standardisation:
Renaming columns to snake case for better readability.
### Feature Engineering:
created new columns 
- which categorises the ages of the customers like young, adult, senior.
- Purchase frequency days of customer like weekly, monthly, biweekly etc.
- Removed redundant columns like Promo_code applied and discount applied and merged as a single column.

### DataBase Integration:
- Established connecction with mysql DB.
- Exported the data to mysql DB using sqlalchemy library and create_engine module to analyse the data unsing mysql.

## Data Analysis using SQL: 
We performed structured analysis in mysql to naswer key business questions.

### 1. Revenue by Gender: 
<img width="151" height="64" alt="image" src="https://github.com/user-attachments/assets/b5398559-e956-437c-93ff-af09a669b497" />

### 2. High spending discount users:
<img width="226" height="233" alt="image" src="https://github.com/user-attachments/assets/51674701-1b72-4e02-9bbe-6a0d2c9ac892" />

### 3. Top 5 products by rating:
<img width="197" height="111" alt="image" src="https://github.com/user-attachments/assets/c94f2eed-d750-44fd-b68a-16e54cc94908" />

### 4. Revenue by Subscriptions and non-subscription customers:
<img width="337" height="77" alt="image" src="https://github.com/user-attachments/assets/45e12683-9334-4cf4-b490-5cd048001d86" />

### 5. Products with highest percentage of purchase when discount applied:
<img width="164" height="116" alt="image" src="https://github.com/user-attachments/assets/2662cf99-5f17-4c52-b23b-ce1abe150276" />

## Dashboard in Power BI:
<img width="662" height="372" alt="CustomerDashboard-SC" src="https://github.com/user-attachments/assets/8dd32db6-45ac-43e8-a373-6e2dc9dfe3a9" />

finally we built a dashboard which visualizes all revenues, sales by category and gender also based on subscription status. 

## Business recommendations:

- #### Boosts the Subscriptions: Promotes exclusive benefits for subscribers.
- #### Customer Loyality Programms : Reward repeat buyers to move them to loyal customers.
- #### Review Discount policy: Balance the sales wit margin control.
- #### Product positioning: Highlight top rated product in campaigns. 


  


