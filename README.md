# MySQLi-PHP
Library for MySQLi intigration in PHP
##How to use
Change the MySQLi credentials in `database.php` file.
```php
private $db_host = DB_HOST;
private $db_user = DB_USER;
private $db_pass = DB_PASSWORD;
private $db_name = DB_NAME;
```
Create Databse object
```php
$db = new Database();
```
Call this method first to establish MySQLi connection to server
```php
$db->connect();
```

###Executing SQL query
```php
$q = $db->sql(YOUR_SQL_STATEMENT);
```
###Executing SQL SELECT query
```php
$q = $db->sql(TABLE_NAME, [$rows="*", JOIN_STATEMENT = null, WHERE_STATEMENT = null, ORDER = "ASC", LIMIT]);
```
