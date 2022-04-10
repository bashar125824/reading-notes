# What is Database ?

***Database is a collection of related data and data is a collection of facts and figures that can be processed to produce information.***

***Mostly data represents recordable facts. Data aids in producing information, which is based on facts. For example, if we have data about marks obtained by all students, we can then conclude about toppers and average marks.***

***A database management system stores data in such a way that it becomes easier to retrieve, manipulate, and produce information.***

---

## Databases Users :

- **Database Administrator (DBA)**

***Database Administrator (DBA) is a person/team who defines the schema and also controls the 3 levels of database.***

***The DBA will then create a new account id and password for the user if he/she need to access the database.***

***DBA is also responsible for providing security to the data base and he allows only the authorized users to access/modify the data base.***

***DBA also monitors the recovery and back up and provide technical support.***

***The DBA has a DBA account in the DBMS which called a system or superuser account.***

***DBA repairs damage caused due to hardware and/or software failures.***

- **End Users**

***Parametric End Users are the unsophisticated who don’t have any DBMS knowledge but they frequently use the data base applications in their daily life to get the desired results.***

***For examples, Railway’s ticket booking users are naive users. Clerks in any bank is a naive user because they don’t have any DBMS knowledge but they still use the database and perform their given task.***

- **Data Base Designers**

***Data Base Designers are the users who design the structure of data base which includes tables, indexes, views, constraints, triggers, stored procedures. He/she controls what data must be stored and how the data items to be related.***

---


# What is Schema ?

***A database schema is an abstract design that represents the storage of your data in a database. It describes both the organization of data and the relationships between tables in a given database. Developers plan a database schema in advance so they know what components are necessary and how they will connect to each other.***

---

# Why we use schemas ?


***help us visualize how a database should be structured. A project may only use a few tables and fields. Still, having a schema gives us a clear point of reference about what tables and fields a project contains.***

---

# What they do look a like ?

**It will include :**

- *All important or relevant data*
- *Consistent formatting for all data entries*
- *Unique keys for all entries and database objects*
- *Each column in a table has a name and data type*


*Example on a schema*

![IMG](https://www.researchgate.net/profile/David-Ryan-25/publication/313630249/figure/fig1/AS:848570576035842@1579326399414/Database-Schema-The-schema-contains-a-coarse-environment-definition-as-well-as-available.ppm)

---

# What is a primary key ?

***A primary key is a special relational database table column (or combination of columns) designated to uniquely identify each table record .***

***It is used as a unique identifier to quickly parse data within the table. A table cannot have more than one primary key.***

**A primary key’s main features are:**

- ***It must contain a unique value for each row of data.***
- ***It cannot contain null values , every row must have a primary key value.***

---

# What is a foreign key ?

***A foreign key is a column or group of columns in a relational database table that provides a link between data in two tables. It acts as a cross-reference between tables because it references the primary key of another table, thereby establishing a link between them.***

---

# What is a Composite Key?

***A composite key, in the context of relational databases, is a combination of two or more columns in a table that can be used to uniquely identify each row in the table. Uniqueness is only guaranteed when the columns are combined; when taken individually the columns do not guarantee uniqueness.***

---

# How are they different ?

**Primary key** *is a Candidate key chosen to uniquely identify tuples in the table.*

**Foreign key** *is an attribute which is a Primary key in its parent table but is included as an attribute in the host table.*

**Composite key** *is a Candidate key that consists of more than one attribute.*

---

# What is a 1:1 relationship ?

***It’s a relationship where a record in one entity (table) is associated with exactly one record in another entity (table).***

***Examples from real life on it :***

- **Country - capital city** *: Each country has exactly one capital city. Each capital city is the capital of exactly one country.*

- **Person - their fingerprints** *: Each person has a unique set of fingerprints. Each set of fingerprints identifies exactly one person.*

- **Email - user account** *: For many websites, one email address is associated with exactly one user account and each user account is identified by its email address.*

---

# What is a Many:Many relationship ?

***many-to-many relationship is where more than one record in a table is related to more than one record in another table.***

***Examples from real life on it :***

- **Professors - University courses** *: Each course has many professors that teach it. Each professor teach many courses .*

---

# How about a 1: Many or a Many: 1?

***one-to-many relationship occurs when a parent record in one table can potentially reference several child records in another table. In a one-to-many relationship, the parent is not required to have child records; therefore, the one-to-many relationship allows zero child records, a single child record or multiple child records. The important thing is that the child cannot have more than one parent record.***

***1:many relationship is the opposite for many:many relationship***

***Examples from real life on it :***

- **People-Addresses** *(Each person can live at one address, but each address can house one or more people.)* 

- **Owners-Pets** *(Each pet has one owner, but each owner can have one or more pets.)*

---

## Things I want to know more about :

1. ***I want to know more about how to connect databases to applications.***

2. ***Know more about database servers and how to deal with it.***

