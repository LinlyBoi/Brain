#DataBase 
- Standard database query language
- Declarative 4th gen language  --> what needs to be done not how
- Built on [[Relational Algebra]]
- Comparison symbols: = , <> , <  > , >= , <=
- Renaming  --> Aliases
```SQL
  Select S1.name, S2.name from S1,S2
  SELECT S.name AS name FROM Students AS S;
```
# Set operations
-  UNION and INTERSECT and EXCEPT
	- Operates on tuples (output of [[#SELECT]])
	- DISTINCT removes duplicates (useful when querying single columns)
 ```SQL
  SELECT * FROM S1 UNION SELECT * FROM S2;
  SELECT * FROM S1 INTERSECT SELECT * FROM S2;
  SELECT * FROM S1 EXCEPT SELECT * FROM S2;
  SELECT DISTINCT * S1; 
  ```
- Cartesian product
	-  Dumb needs a WHERE clause to get something meaningful
```SQL
SELECT * FROM S1,S2;
```
# Join operations
- [[Relational Algebra#^0c1057|Theta-join]] θ
  ```SQL
  SELECT * FROM S1,S2 WHERE C;
  FROM S1 NATURAL JOIN S2;
```



# SQL
```ad-tip
SQL deals with Sets with duplicates [[Sets#Multi-Sets|Multi-Sets]] and calls them bags
```

```ad-important
title: Conditions Involving Relations
- IN   -> '=' 
- ALL -> 'AND' 
- ANY -> 'OR'
- EXISTS -> NOT NULL
- NOT -> Negates any of above
- LIKE
```

# Aggregation
- Does things that we do in Data Science and [[R]]
- Counting columns can be useful as it will skip nulls
- COUNT is the only one that handles multiple columns
- Written **after** SELECT clause 
```SQL
SELECT COUNT (DISTINCT,col_NAME) FROM Sailors;
```

```ad-hint
title: Aggregation Operators
- COUNT [Distinct] COLUMN
- SUM [Distinct] COLUMN
- AVG [Distinct] COLUMN
- MAX COLUMN
- MIN COLUMN

```

```ad-seealso
title: See also 
[[Correlational SubQueries]]
```

# Conceptual Query Evaluation
```ad-tip
title: Steps
1. Compute cross product of relation-list
2. Discrad resulting tuples if they fail qualifications
3. Delete attributes that are not in the target-list (column-list)
4. if DISTINCT specified, eliminate duplicate rows.
```
- Evaluates qualifications row by row

# Sub Queries 
- DBMS has query optimisation but sometimes that isn't enough
- Joins are expensive
- Dividing joins into smaller queries first before joining
- Utilises nested queries (SELECT in SELECT etc.)
- Usually present in the WHERE clause 


