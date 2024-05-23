### <a name="kropka1"><p align="justify">1. Display Dim Currency Table.</p></a>

```sql
SELECT * FROM [dbo].[DimCurrency]
```

![1](https://github.com/denispatric/denispatric/assets/83760732/7bd75ba1-a940-45bd-92d1-6c6fb80ab3b4)



### <a name="kropka2"><p align="justify">2. .</p></a>

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




