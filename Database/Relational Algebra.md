#DataBase 
# Operations
- Remove parts of a relation –> Selection, Projection
- Combining operations
  1. Cartesian product
  2. Join operations –> Selectively pair tuples from 2 relations
- Renaming –> Change schema name only ρ$_S$(Table)
## [[Sets]] operations
1. Union
2. Intersection --> R  
3. Difference
- Requires two identical schemas

## Projection 
- SELECT statement in [[SQL]]
- Used to form a new Relation from an existing relation’s columns
- Create a “subset” of a relation
- No duplicates in **tuples**
- Returns columns
- Π$_{A_1,A_2,A_3,A_4...A_n}$(R) –> Relation that only has the columns 1 to n of R
  Example R –> Movies(title,year,length,genre,studio,producer)
  Π$_{genre}$(Movies) –> just the genre column

## Selection
- σ operator --> σ$_{gpa≤3}$(Students)
- Gets executed before [[#Projection]]
- Returns  whole tuple/rows
- WHERE statement

## Join
- Theta-join ^0c1057
	- S1 $∞_C$ S2 = σ$_C$(S1xS2) (as if not actually what happens)
- Natural join --> the condition is known and it is the tables have the same attributes
