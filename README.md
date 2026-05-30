Database Setup and Schema Design
Overview

This project demonstrates the design and implementation of a relational database schema for a Library Management System. The objective is to create a well-structured database by identifying entities, defining relationships, applying normalization principles, and implementing the schema using SQL.

Objective
Learn database creation and schema design.
Create tables using SQL DDL commands.
Define Primary Keys and Foreign Keys.
Establish relationships between entities.
Apply normalization techniques to reduce redundancy.
Generate an Entity Relationship (ER) Diagram.
Tools Used
MySQL Workbench
SQL
ER Diagram Designer
Database Domain

Library Management System

Main Entities
Books
Authors
Members
Borrow Records
Categories
Database Schema
Tables Created
Authors
author_id (Primary Key)
author_name
Categories
category_id (Primary Key)
category_name
Books
book_id (Primary Key)
title
author_id (Foreign Key)
category_id (Foreign Key)
publication_year
Members
member_id (Primary Key)
member_name
email
phone
Borrow_Records
borrow_id (Primary Key)
member_id (Foreign Key)
book_id (Foreign Key)
issue_date
return_date
Relationships
One Author can write many Books.
One Category can contain many Books.
One Member can borrow many Books.
One Book can be borrowed multiple times.
Normalization Applied
First Normal Form (1NF)
Eliminated repeating groups.
Ensured atomic values in each column.
Second Normal Form (2NF)
Removed partial dependencies.
Non-key attributes depend on the entire primary key.
Third Normal Form (3NF)
Removed transitive dependencies.
Ensured data integrity and minimized redundancy.
