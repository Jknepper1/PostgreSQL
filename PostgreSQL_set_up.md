# **PostgreSQL Setup Steps**
## _This is a guide for setting up PostgreSQL in Ubuntu_

---
#### Logging in to default user

```C
$ sudo -u postgres psql
```
Check out the link below for help changing the _Postgres authentication config file_

https://www.atlassian.com/data/admin/how-to-set-the-default-user-password-in-postgresql

## Common Commands

\l - List all databases

\c - switch to another database

\dt list database tables

\d <table-name> - describe a table

\dn - List all schemas

\du - List users and their roles

\du <username> - Retrive a specific user

\df - list all functions 

\dv - List all views

\i - Run commands from a file

\o - Save query results to a file

\q - Quit Psql


## Users

CREATE USER [name];

sudo -u postgres createuser [name] -P <-- From prompt 

CREATE USER [name] WITH PASSWORD '[password]';

ALTER USER [name] WITH PASSWORD '[password]';

createuser [option] [name]

CREATE USER [name] WITH [option];

^^ All of these commands are from https://phoenixnap.com/kb/postgres-create-user

## Tables

https://www.postgresql.org/docs/current/tutorial-table.html

https://www.postgresql.org/docs/current/sql-createtable.html

## Version

postgres --version or -V

https://phoenixnap.com/kb/check-postgresql-version

Ubuntu version:

cat /etc/os-release

lsb_release -a

hostnamectl

uname -r

