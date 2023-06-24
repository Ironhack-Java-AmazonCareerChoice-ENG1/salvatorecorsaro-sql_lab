# JAVA SPECIAL COFFEE ROASTERS

## SALES RAW DATA
```
id,transaction_time,customer_name,coffee_type,coffee_size,coffee_price,coffee_origin,roasting_level,total_amount,payment_method
1,2023-01-01 08:30:00,John Doe,Espresso,Small,3,Brazil,Medium,3,Cash
2,2023-01-01 09:00:00,Jane Doe,Latte,Large,5,Colombia,Dark,5,Debit Card
3,2023-01-01 09:30:00,John Doe,Americano,Medium,4,Ethiopia,Light,4,Credit Card
4,2023-01-01 10:00:00,Alice Smith,Cappuccino,Small,4,Guatemala,Medium,8,Credit Card
5,2023-01-01 10:30:00,Bob Smith,Espresso,Large,5,Brazil,Dark,5,Cash
6,2023-01-01 11:00:00,John Doe,Cappuccino,Small,4,Ethiopia,Light,4,Credit Card
7,2023-01-02 08:00:00,Alice Smith,Latte,Small,3,Colombia,Medium,3,Debit Card
8,2023-01-02 08:30:00,Bob Smith,Americano,Medium,4,Brazil,Dark,4,Cash
9,2023-01-02 09:00:00,Jane Doe,Cappuccino,Large,5,Guatemala,Light,5,Debit Card
10,2023-01-02 09:30:00,John Doe,Espresso,Small,3,Ethiopia,Medium,3,Cash

```


## Normalization Exercise:

Normalize the data to follow the rules of the 3rd Normal Form (3NF). You should end up with multiple tables such as transactions, customers, coffees, payment_methods. Note that your normalization process might result in a different schema based on how you interpret the data and requirements.

## Exercises:

- Insert unique customer names from sales_raw_data into a new table customers.
- Update any customer name in customers to have consistent casing if it's repeated with different cases.
- Delete any rows in customers where the customer_name is NULL or an empty string.
- Count the number of unique coffee types sold by the shop.
- Calculate the average, total, minimum, and maximum coffee_price.
- Group the sales_raw_data table by coffee_type and calculate the total total_amount for each coffee_type.
- From the previous query, include only those coffee_type where the total total_amount is greater than 1000.
- Find all sales made to customers whose names start with 'A'.
- Find all sales transactions that took place between '2023-01-01' and '2023-03-31'.
- Find all sales of 'Espresso' or 'Latte' that were above the average coffee_price.
- Display the coffee_type and total sales amount for each type, sorted by total sales amount in descending order.
- List the distinct coffee origins in sales_raw_data.
- Count the number of transactions for each payment_method.
- Find the customer_name who has made the most purchases.
- Identify the coffee_origin that's most popular among customers.
- Find the day of the week with the highest total sales.