# SQL Server – IDENTITY, UNIQUE and CHECK Constraints

## Project Overview
This project demonstrates SQL Server concepts using a user table. It covers IDENTITY properties, UNIQUE constraints, CHECK constraints, manual identity insertion, and identity functions.

## Database Name
`BIKSERVICE`

## Table Name
`TBL_USER`

## Concepts Covered
- CREATE DATABASE and USE
- CREATE TABLE
- IDENTITY(1,1)
- UNIQUE Constraint
- NOT NULL Constraint
- CHECK Constraint
- INSERT INTO
- SELECT Statement
- SET IDENTITY_INSERT ON / OFF
- @@IDENTITY
- IDENT_CURRENT()
- SCOPE_IDENTITY()

## Column Details

| Column Name | Data Type | Constraint |
|---|---|---|
| UID | NUMERIC(10) | IDENTITY, UNIQUE, NOT NULL |
| UNAME | NVARCHAR(10) | NOT NULL |
| PASSWORD | NVARCHAR(20) | NOT NULL |
| AGE | NUMERIC(10) | CHECK (AGE > 18) |
| EMAIL | NVARCHAR(50) | UNIQUE |

## Identity Functions

**1. @@IDENTITY**

Returns the last identity value generated in the current session.

**2. IDENT_CURRENT()**

Returns the last identity value generated for a specific table.

**3. SCOPE_IDENTITY()**

Returns the last identity value generated in the current scope.

## Constraints Explanation

- **IDENTITY:** Automatically generates numeric values.
- **UNIQUE:** Prevents duplicate values.
- **NOT NULL:** Does not allow NULL values.
- **CHECK:** Ensures that values satisfy a specified condition.

## Technologies Used
- Microsoft SQL Server
- SQL Server Management Studio (SSMS)
- SQL

## Learning
