#DataBase 

- Simple 
- Built around single concept $\rightarrow$ The [[Relations#Relational DataBase Concepts|relation]]
- Each relation is a table
- Supports high level language $\rightarrow$ [[SQL]]
- Mathematical design theory $\rightarrow$ [[Relational Algebra]]
   Leaves a lot room for [[Optimisation|optimisation]]
- Most popular model despite newer models existing
   So popular that $\rightarrow$ Object relational models exist
- Degree $\rightarrow$ number of attributes in schema
- Cardinality $\rightarrow$ is the number of tuples in relation

# Design
- Write all attributes as [[Sets]] $\rightarrow$ Student(PID: *string*, Name: *string*, Address: *string*) etc $\dots$
- All relationships as [[Relations]] $\rightarrow$ Teach(ProfessorID: *string*, Number: *integer*, DeptName: *string*)
- Entity set $\rightarrow$ Relation
- [[Entity-Relationship Model#Relationships|Non-Supporting Relationship]] $\rightarrow$ Attributes are [[Entity-Relationship Model#Constraints|Keys]]  of the connected entity sets (such as Student and prof IDs not the whole table)
### Special cases
  1. Weak entity sets $\rightarrow$ Include attributes of  entity and  [[Entity-Relationship Model#Constraints|keys]] of supporting entity sets
  2. Combining relations (especially for [[Data Modelling#^d2f293|one-many relationships]]) $\rightarrow$ Foreign keys
      - Take the key of the one put in the many table
      - Example: Teach relationship (Have prof as `FK` in course table )
  3. *Is-a* relationships and [[Entity-Relationship Model#Subclasses|subclasses]]
     1. [[Entity-Relationship Model|ER]] approach $\rightarrow$ using foreign key of parent entity
        Creates redundancy in keys
     2. Null approach $\rightarrow$ Have all columns in one table and null when needed
        Redundancy if too many NULLS
     4. [[OOP]] approach $\rightarrow$ Each parent and child entity has its own table
        Bad if you need to be joining the tables too much

# Problem solving
- nouns $\rightarrow$ Indicate tables or attributes
- Verbs $\rightarrow$ Indicate relations

# Normalisation
- Find redundant info and remove it
