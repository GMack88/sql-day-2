#SQL day 2 (aka sqewl, aka skl, .)

- Student can add foreign key to new table
- Student can add foreign key to existing table
- Student can use join
- Student can use sub-selects/nested queries
- Student can set null values
- Student can Group by
- Student can update rows
- Student can delete rows
- Student can use distinct
- Student can describe one-to-one relationships
- Student can describe one-to-many relationships
- Student can describe many-to-many relationships

## **First normal form**

- A relation is in first normal form if and only if the data in each column is indivisible.

good data:

- String
- Integer
- Null
- Boolean
- Float

avoid:

- Objects
- Arrays

## **Second Normal Form**

- A relation is in second normal form if it is in first normal form and all columns must have a primary key and all non-primary key columns are dependents of the primary key.

## **Third Normal Form**

- Must be in second normal form
- Contains ony columns that are non-transitively dependent on a primary key.
- Transitive Property: If A is greater than B, and B is gretaer than C, then A is greater than C.

- A, B, primaryKey; if the value of A relies on th eprimarykey, and B relies on the primarykey and A also relies on B then you can say A relies on the PrimaryKey through B.

```sql
personId, firstName, lastName => non transitively dependent

personId, bodyMassIndex, isObese => transitively dependent
```

**One to one relationship**

- One column in a table is associated with one and only one column from another table.
- example <img width='500px' src='https://upload.wikimedia.org/wikipedia/commons/thumb/f/f7/CPT-Databases-OnetoOne.svg/500px-CPT-Databases-OnetoOne.svg.png'>

**One-Many Relationship **

- The One-to-Many relationship is defined as a relationship between two tables where a row from one table can have multiple matching rows in another table. This relationship can be created using Primary key-Foreign key relationship.
- For example, a book can have multiple authors.

**Many-to-Many relationship**

- Multiple columns in a table can be associated with multiple columns from another table.
- example: <img width='500px' src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c4/CPT-Databases-ManytoMany.svg/500px-CPT-Databases-ManytoMany.svg.png">
- <img width='500px' src="https://upload.wikimedia.org/wikipedia/commons/0/02/Databases-ManyToManyWJunction.jpg">
