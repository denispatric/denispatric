### <a name="kropka1"><p align="justify">1. Display Currency Table</p></a>

```sql
SELECT * FROM [dbo].[DimCurrency]
```

![1](https://github.com/denispatric/denispatric/assets/83760732/7bd75ba1-a940-45bd-92d1-6c6fb80ab3b4)



### <a name="kropka2"><p align="justify">2. Display CurrencyKey and CurrencyName table </p></a>

```sql
SELECT CurrencyKey,CurrencyName FROM [dbo].[DimCurrency]
```

![2](https://github.com/denispatric/denispatric/assets/83760732/9a45a9ae-671a-479f-b83e-52a43a931507)



### <a name="kropka3"><p align="justify">3. .</p></a>

```sql
SELECT * FROM [dbo].[DimReseller]
ORDER BY NumberEmployees
```

![3](https://github.com/denispatric/denispatric/assets/83760732/1ed8ceca-5155-4fcb-b537-157e6735da44)



### <a name="kropka4"><p align="justify">4. </p></a>

```sql
SELECT NumberEmployees, OrderFrequency FROM [dbo].[DimReseller]
WHERE NumberEmployees <5
ORDER BY NumberEmployees
```

![4](https://github.com/denispatric/denispatric/assets/83760732/74ec685a-eb70-453f-9456-505ed4d6ec46)



### <a name="kropka5"><p align="justify">5. </p></a>

```sql
SELECT * FROM [dbo].[DimReseller]
WHERE FirstOrderYear = '2011'
```

![5](https://github.com/denispatric/denispatric/assets/83760732/35334868-c505-4c12-a38c-10d9c1071899)



### <a name="kropka6"><p align="justify">6..</p></a>

```sql
SELECT * FROM [dbo].[DimReseller]
WHERE OrderMonth >=4 AND OrderMonth <=7
```

![6](https://github.com/denispatric/denispatric/assets/83760732/686087e3-7a5c-4998-a2bc-5ce021a9cc68)


### <a name="kropka7"><p align="justify">7. .</p></a>

```sql
SELECT * FROM [dbo].[DimReseller]
WHERE OrderMonth = 2 OR OrderMonth = 4 OR OrderMonth = 6
```

![7](https://github.com/denispatric/denispatric/assets/83760732/762e7371-fdfc-4580-81c8-980104f024db)



### <a name="kropka8"><p align="justify">8..</p></a>

```sql
SELECT * FROM [dbo].[DimReseller]
WHERE OrderMonth IN (1, 3, 5)
```

![8](https://github.com/denispatric/denispatric/assets/83760732/1b0cb0aa-4efd-4229-8363-60743b7088ff)


### <a name="kropka9"><p align="justify">9. .</p></a>

```sql
SELECT * FROM [dbo].[DimReseller]
WHERE ResellerName LIKE 'De%'
```

![9](https://github.com/denispatric/denispatric/assets/83760732/891dd80d-29db-45b9-acc8-8ac1c4bc1ba3)


### <a name="kropka10"><p align="justify">10. .</p></a>

```sql
SELECT * FROM [dbo].[DimReseller]
WHERE AddressLine2 IS NULL
```

![10](https://github.com/denispatric/denispatric/assets/83760732/737ec940-4223-455d-8f81-aa313a06e9a3)


### <a name="kropka10"><p align="justify">10. .</p></a>

```sql
SELECT * FROM [dbo].[DimReseller]
WHERE NumberEmployees >9 AND OrderMonth BETWEEN 2 AND 8
```

![11](https://github.com/denispatric/denispatric/assets/83760732/dc5ac411-0b2d-46d4-9047-6919333cbabc)

### <a name="kropka10"><p align="justify">10. .</p></a>

```sql
UPDATE [dbo].[DimEmployee]
SET FirstName = 'Denis'
WHERE EmployeeKey = 1
```

![12](https://github.com/denispatric/denispatric/assets/83760732/0e462028-5eda-47e2-a18c-a0cc8bffa22c)

![image](https://github.com/denispatric/denispatric/assets/83760732/93fcd334-ece5-43ff-a540-414a22633d37)


### <a name="kropka10"><p align="justify">10. .</p></a>

```sql
SELECT Customers.CustomerName, Orders.OrderID
FROM Customers INNER JOIN Orders
ON Customers.CustomerID = Orders.CustomerID
ORDER BY CustomerName
```
![image](https://github.com/denispatric/denispatric/assets/83760732/e8ecf0e2-c651-452c-91b6-d4d3051838bd)



### <a name="kropka10"><p align="justify">Create a table. Use ALTER and DROP table. .</p></a>

```sql
-- Step 1: Create a random table
CREATE TABLE RandomTable (
    ID INT PRIMARY KEY,
    Name VARCHAR(50),
    Age INT
);
```
![image](https://github.com/denispatric/denispatric/assets/83760732/fe0682c1-d668-4d6f-aab6-b9358bf50bc8)

```sql
-- Step 2: Alter the table to add a new column
ALTER TABLE RandomTable
ADD Email VARCHAR(100);
```
![image](https://github.com/denispatric/denispatric/assets/83760732/cc5516e4-eb71-4d1b-9da9-8a72a5f8e3e1)

```sql
-- Step 3: Drop the table
DROP TABLE RandomTable;
```
![image](https://github.com/denispatric/denispatric/assets/83760732/986e3dfc-6c11-4350-9af1-9442500859a6)

### <a name="kropka10"><p align="justify">Display a common list of cities of all customers and suppliers (use the UNION function for this). .</p></a>

```sql
SELECT City FROM Customers
UNION
SELECT City FROM Suppliers
```
![image](https://github.com/denispatric/denispatric/assets/83760732/bd7f5cc8-efc4-4692-b0dc-bc26e2f527cb)

