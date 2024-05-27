| Query | Description |
|-------|-------------|
| `SELECT NumberEmployees, OrderFrequency FROM [dbo].[DimReseller] WHERE NumberEmployees < 5 ORDER BY NumberEmployees;` | Retrieves the number of employees and order frequency from the `DimReseller` table where the number of employees is less than 5, sorted by number of employees. |
| `SELECT * FROM [dbo].[DimCurrency];` | Retrieves all columns from the `DimCurrency` table. |
| `SELECT CurrencyKey, CurrencyName FROM [dbo].[DimCurrency];` | Retrieves the currency key and currency name from the `DimCurrency` table. |
| `SELECT * FROM [dbo].[DimReseller] ORDER BY NumberEmployees;` | Retrieves all columns from the `DimReseller` table, sorted by number of employees. |
| `SELECT * FROM [dbo].[DimReseller] WHERE FirstOrderYear = '2011';` | Retrieves all columns from the `DimReseller` table where the first order year is 2011. |
| `SELECT * FROM [dbo].[DimReseller] WHERE OrderMonth >= 4 AND OrderMonth <= 7;` | Retrieves all columns from the `DimReseller` table where the order month is between April and July. |
| `SELECT * FROM [dbo].[DimReseller] WHERE OrderMonth = 2 OR OrderMonth = 4 OR OrderMonth = 6;` | Retrieves all columns from the `DimReseller` table where the order month is February, April, or June. |
| `SELECT * FROM [dbo].[DimReseller] WHERE OrderMonth IN (1, 3, 5);` | Retrieves all columns from the `DimReseller` table where the order month is January, March, or May. |
| `SELECT * FROM [dbo].[DimReseller] WHERE ResellerName LIKE 'De%';` | Retrieves all columns from the `DimReseller` table where the reseller name starts with "De". |
| `SELECT * FROM [dbo].[DimReseller] WHERE AddressLine2 IS NULL;` | Retrieves all columns from the `DimReseller` table where the address line 2 is NULL. |
| `SELECT * FROM [dbo].[DimReseller] WHERE NumberEmployees > 9 AND OrderMonth BETWEEN 2 AND 8;` | Retrieves all columns from the `DimReseller` table where the number of employees is greater than 9 and the order month is between February and August. |
| `SELECT Customers.CustomerName, Orders.OrderID FROM Customers INNER JOIN Orders ON Customers.CustomerID = Orders.CustomerID ORDER BY CustomerName;` | Retrieves customer names and their corresponding order IDs, sorted by customer name. |




### <a name="1"><p align="justify">1. This query will return all rows and all columns from the DimCurrency table. Since there are no filtering (WHERE) or sorting (ORDER BY) clauses, it will retrieve the complete dataset as it is stored in the table.</p></a>

```sql
SELECT * FROM [dbo].[DimCurrency]
```

![1](https://github.com/denispatric/denispatric/assets/83760732/7bd75ba1-a940-45bd-92d1-6c6fb80ab3b4)



### <a name="2"><p align="justify">2. This query will return the CurrencyKey and CurrencyName columns from all rows in the DimCurrency table.</p></a>

```sql
SELECT CurrencyKey,CurrencyName FROM [dbo].[DimCurrency]
```

![2](https://github.com/denispatric/denispatric/assets/83760732/9a45a9ae-671a-479f-b83e-52a43a931507)



### <a name="3"><p align="justify">3. This query will return all columns from the DimReseller table, with the rows sorted in ascending order based on the NumberEmployees column.</p></a>

```sql
SELECT * FROM [dbo].[DimReseller]
ORDER BY NumberEmployees
```

![3](https://github.com/denispatric/denispatric/assets/83760732/1ed8ceca-5155-4fcb-b537-157e6735da44)



### <a name="4"><p align="justify">4. This query will return all rows from the DimReseller table where the NumberEmployees value is less than 5. The resulting rows will include only the NumberEmployees and OrderFrequency columns and will be sorted by the NumberEmployees column in ascending order. </p></a>

```sql
SELECT NumberEmployees, OrderFrequency FROM [dbo].[DimReseller]
WHERE NumberEmployees <5
ORDER BY NumberEmployees
```

![4](https://github.com/denispatric/denispatric/assets/83760732/74ec685a-eb70-453f-9456-505ed4d6ec46)



### <a name="5"><p align="justify">5. This query will return all columns from the DimReseller table where the FirstOrderYear column has the value '2011'. </p></a>

```sql
SELECT * FROM [dbo].[DimReseller]
WHERE FirstOrderYear = '2011'
```

![5](https://github.com/denispatric/denispatric/assets/83760732/35334868-c505-4c12-a38c-10d9c1071899)



### <a name="6"><p align="justify">6. This query will return all columns from the DimReseller table where the OrderMonth falls within the range of April (4) to July (7), inclusive.</p></a>

```sql
SELECT * FROM [dbo].[DimReseller]
WHERE OrderMonth >=4 AND OrderMonth <=7
```

![6](https://github.com/denispatric/denispatric/assets/83760732/686087e3-7a5c-4998-a2bc-5ce021a9cc68)


### <a name="7"><p align="justify">7. This query will return all columns from the DimReseller table where the OrderMonth is equal to 2, 4, or 6.</p></a>

```sql
SELECT * FROM [dbo].[DimReseller]
WHERE OrderMonth = 2 OR OrderMonth = 4 OR OrderMonth = 6
```

![7](https://github.com/denispatric/denispatric/assets/83760732/762e7371-fdfc-4580-81c8-980104f024db)



### <a name="8"><p align="justify">8. This query will return all columns from the DimReseller table where the OrderMonth is equal to 1, 3, or 5.

</p></a>

```sql
SELECT * FROM [dbo].[DimReseller]
WHERE OrderMonth IN (1, 3, 5)
```

![8](https://github.com/denispatric/denispatric/assets/83760732/1b0cb0aa-4efd-4229-8363-60743b7088ff)


### <a name="9"><p align="justify">9. This query will return all columns from the DimReseller table where the ResellerName starts with the letters "De".</p></a>

```sql
SELECT * FROM [dbo].[DimReseller]
WHERE ResellerName LIKE 'De%'
```

![9](https://github.com/denispatric/denispatric/assets/83760732/891dd80d-29db-45b9-acc8-8ac1c4bc1ba3)


### <a name="10"><p align="justify">10. This query will return all columns from the DimReseller table where the AddressLine2 column is NULL.

</p></a>

```sql
SELECT * FROM [dbo].[DimReseller]
WHERE AddressLine2 IS NULL
```

![10](https://github.com/denispatric/denispatric/assets/83760732/737ec940-4223-455d-8f81-aa313a06e9a3)


### <a name="11"><p align="justify">11. This query will return all columns from the DimReseller table where the NumberEmployees column is greater than 9 and the OrderMonth falls within the range of February (2) to August (8), inclusive.</p></a>

```sql
SELECT * FROM [dbo].[DimReseller]
WHERE NumberEmployees >9 AND OrderMonth BETWEEN 2 AND 8
```

![11](https://github.com/denispatric/denispatric/assets/83760732/dc5ac411-0b2d-46d4-9047-6919333cbabc)

### <a name="12"><p align="justify">12. This query updates the FirstName column of the DimEmployee table. It sets the value of FirstName to 'Denis' for the row where the EmployeeKey is 1.</p></a>

```sql
UPDATE [dbo].[DimEmployee]
SET FirstName = 'Denis'
WHERE EmployeeKey = 1
```

![12](https://github.com/denispatric/denispatric/assets/83760732/0e462028-5eda-47e2-a18c-a0cc8bffa22c)

![image](https://github.com/denispatric/denispatric/assets/83760732/93fcd334-ece5-43ff-a540-414a22633d37)


### <a name="13"><p align="justify">13. This query selects the CustomerName column from the Customers table and the OrderID column from the Orders table. It then performs an inner join between the Customers and Orders tables based on the CustomerID column. Finally, it orders the result set by the CustomerName column in ascending order.</p></a>

```sql
SELECT Customers.CustomerName, Orders.OrderID
FROM Customers INNER JOIN Orders
ON Customers.CustomerID = Orders.CustomerID
ORDER BY CustomerName
```
![image](https://github.com/denispatric/denispatric/assets/83760732/e8ecf0e2-c651-452c-91b6-d4d3051838bd)



### <a name="14"><p align="justify">14. This set of queries will create a table, ALTER and then DROP table</p></a>


Step 1: Create a table
```sql
CREATE TABLE RandomTable (
    ID INT PRIMARY KEY,
    Name VARCHAR(50),
    Age INT
);
```
![image](https://github.com/denispatric/denispatric/assets/83760732/fe0682c1-d668-4d6f-aab6-b9358bf50bc8)


Step 2: Alter the table to add a new column
```sql
ALTER TABLE RandomTable
ADD Email VARCHAR(100);
```
![image](https://github.com/denispatric/denispatric/assets/83760732/cc5516e4-eb71-4d1b-9da9-8a72a5f8e3e1)


Step 3: Drop the table
```sql
DROP TABLE RandomTable;
```
![image](https://github.com/denispatric/denispatric/assets/83760732/986e3dfc-6c11-4350-9af1-9442500859a6)

### <a name="kropka10"><p align="justify"> This query will display a common list of cities of all customers and suppliers </p></a>

```sql
SELECT City FROM Customers
UNION
SELECT City FROM Suppliers
```
![image](https://github.com/denispatric/denispatric/assets/83760732/bd7f5cc8-efc4-4692-b0dc-bc26e2f527cb)

