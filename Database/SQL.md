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
	 ```SQL
	  SELECT * FROM S1 UNION SELECT * FROM S2;
	  SELECT * FROM S1 INTERSECT SELECT * FROM S2;
	  SELECT * FROM S1 EXCEPT SELECT * FROM S2;
	  ```
- Cartesian product
	-  Dumb needs a WHERE cause to get something meaningful
	```SQL
	SELECT * FROM S1,S2;
	```
# Join operations
- [[Relational Algebra#^0c1057|Theta-join]] θ
  ```SQL
  SELECT * FROM S1,S2 WHERE C;
  FROM S1 NATURAL JOIN S2;
```

# Sub queries