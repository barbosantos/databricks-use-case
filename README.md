# Data Enginer case 3

You have been provided with an excel file with three sheets, each one represents one of the tables described below. Use this data to answer the questions, either by loading them into a SQL engine/Blob/S3/Local machine of your choice, or by examining the data and constructing queries that would work if the data were available in SQL tables.

Table 1: Customers
```
customer_name (VARCHAR)
customer_id (INT)
customer_dob (DATE)
gender (VARCHAR)
```

Table 2: Transactions
```
transaction_id (INT) customer_id (INT)
product_id (INT)
store_id (INT)
offer_id (INT)
sales_amount (DOUBLE)
transaction_date (DATE)
```

Table 3: offers
```
customer_id (INT)
offer_id (INT)
start_date (DATE)
end_date (DATE)
```

1. Write a query that gives us an aggregated table that provides:
```
o Customer name,
o Customer id,
o Customer’s age (in years),
o Total sales per customer,
o Number of offers received,
o Number of offers redeemed,
o Number of visits for each day of week (Mon-Sun), e.g. one column per weekday.
```

2. Additionally, write a query that tells us on which day of week that customers of the same age group (0-9 years, 10-19 years, etc.) visits the stores most often.
