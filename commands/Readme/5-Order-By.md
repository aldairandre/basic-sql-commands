# The SQL ORDER BY Keyword

The `ORDER BY`  keyword is used to sort the result-set in ascending or descending order.

The `ORDER BY`  keyword sorts the records in ascending order by default. To sort the records in descending order, use the DESC keyword.

`ORDER BY`  Syntax

```
  SELECT column1, column2, ...
  FROM table_name
  ORDER BY column1, column2, ... ASC|DESC;
```

`ORDER BY` **Example**

The following SQL statement selects all customers from the "Customers" table, sorted by the "Country" column:

*Example*
```
  SELECT * FROM Customers
  ORDER BY Country;
```