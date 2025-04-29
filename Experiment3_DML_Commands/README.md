# Experiment 3: DML Commands

## AIM
To study and implement DML (Data Manipulation Language) commands.

## THEORY

### 1. INSERT INTO
Used to add records into a relation.
These are three type of INSERT INTO queries which are as
A)Inserting a single record
**Syntax (Single Row):**
```sql
INSERT INTO table_name (field_1, field_2, ...) VALUES (value_1, value_2, ...);
```
**Syntax (Multiple Rows):**
```sql
INSERT INTO table_name (field_1, field_2, ...) VALUES
(value_1, value_2, ...),
(value_3, value_4, ...);
```
**Syntax (Insert from another table):**
```sql
INSERT INTO table_name SELECT * FROM other_table WHERE condition;
```
### 2. UPDATE
Used to modify records in a relation.
Syntax:
```sql
UPDATE table_name SET column1 = value1, column2 = value2 WHERE condition;
```
### 3. DELETE
Used to delete records from a relation.
**Syntax (All rows):**
```sql
DELETE FROM table_name;
```
**Syntax (Specific condition):**
```sql
DELETE FROM table_name WHERE condition;
```
### 4. SELECT
Used to retrieve records from a table.
**Syntax:**
```sql
SELECT column1, column2 FROM table_name WHERE condition;
```
**Question 1**
--
-- ![Screenshot 2025-04-29 121653](https://github.com/user-attachments/assets/53b5f3b9-c9b6-4e2b-a010-2876d7e71d58)
-- ![Screenshot 2025-04-29 121523](https://github.com/user-attachments/assets/6218b66c-b292-4f15-9f78-d07da1e45385)



```sql
-- INSERT INTO Customers(CustomerID  ,Name,             Address,         Email)
SELECT CustomerID  ,Name             ,Address         ,Email FROM Old_customers;
```
```sql
-- INSERT INTO Customers(CustomerID ,Name,Address, City     ,   ZipCode)VALUES (301, "Michael Jordan",  "123 Maple St",  "Chicago",  60616);
```
**Output:**

![Screenshot 2025-04-29 121659](https://github.com/user-attachments/assets/8cb31551-6831-454d-b418-edd48d7eb67f)
![Screenshot 2025-04-29 121536](https://github.com/user-attachments/assets/c63a44bb-a3d1-41fb-bac6-878256b773b3)


**Question 2**
---
-- ![Screenshot 2025-04-29 123037](https://github.com/user-attachments/assets/1f0eb809-77c1-44ef-afa2-8421dcb11740)


```sql
-- UPDATE products
SET product_name = 'Grapefruit'
WHERE product_id =4;
```

**Output:**

![Screenshot 2025-04-29 123046](https://github.com/user-attachments/assets/fac16b56-8a39-4f79-85ce-bbb4c7e859c6)


**Question 3**
---
--![Screenshot 2025-04-29 123317](https://github.com/user-attachments/assets/777ae485-23f4-4483-8715-29b910b9a718)


```sql
-- DELETE FROM surgeries
WHERE  surgery_id =3;
```

**Output:**
![Screenshot 2025-04-29 123327](https://github.com/user-attachments/assets/ed8e9b00-3bf7-4fff-8b31-4e8298e55694)


**Question 4**
---
-- ![Screenshot 2025-04-29 123951](https://github.com/user-attachments/assets/fbbc9c48-b733-4c6e-881c-da2102440159)


```sql
-- SELECT customer_id, cust_name, city, grade, salesman_id
FROM  customer
WHERE  grade >100;
```

**Output:**

![Screenshot 2025-04-29 124001](https://github.com/user-attachments/assets/57d14ec4-855c-4b61-8374-1114b9dec239)





## RESULT
Thus, the SQL queries to implement DML commands have been executed successfully.
