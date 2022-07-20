# Databases

## MySQL

```shell
mysql -u <USERNAME> -p<PASSWORD> -h <HOST> -P <PORT> -D <DATABASE>
```

```mysql
# show all tables
SHOW TABLES;

# show schema of table;
SHOW COLUMNS FROM <table_name>;
DESCRIBE <table_name>;

# delete all rows from table
DELETE FROM <table_name>;

# delete select rows from table
DELETE FROM <table_name> WHERE <condition>;
```

