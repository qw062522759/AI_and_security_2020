#  Pandas讀寫MySQL資料庫
```
win10.ova

安裝anaconda

安裝額外套件
安裝資料庫MYSQL
```
```
pandas
sqlalchemy
pymysql

pandas模組提供了read_sql_query（）函式實現了對資料庫的查詢，
to_sql（）函式實現了對資料庫的寫入，並不需要實現新建MySQL資料表。

sqlalchemy模組實現了與不同資料庫的連線
pymysql模組則使得Python能夠操作MySQL資料庫。
```

# MYSQL 
```
https://tech.digitgeek.net/t/51.html
```
```
mysql->CREATE DATABASE dbname;//建立資料庫 

mysql->CREATE TABLE tablename;//建立表 

               CREATE TABLE tablename (colname1 varchar(15), colname2 int(8), colname3 date);

mysql->SHOW DATABASES;//顯示資料庫資訊，有那些可用的資料庫。 

mysql->USE dbname;//選擇資料庫 

mysql->SHOW TABLES;//顯示表資訊，有那些可用的表

mysql->DESCRIBE tablename;//顯示建立的表的資訊
```
## Redis
```
Redis ( REmote DIctionary Server )
Redis 是一個開源的NoSQL資料庫。
高效能 ( in-memory )的 Key-Value 的儲存系統。
支援多種數據結構如：string、hash、list、set、sorted set、bitmap、hyperloglog。
版本 3.0 後支援數據備份，為 Master-Slave 模式的備份
```
```
https://dotblogs.com.tw/zackmyself/2017/04/27/005621

https://github.com/microsoftarchive/redis/releases

https://marcus116.blogspot.com/2019/02/how-to-install-redis-in-windows-os.html

http://dog0416.blogspot.com/2017/03/redis-redis-window-mac.html

redis-cli info 看 command 工具版本號
```

```
How to set/get pandas.DataFrame to/from Redis?
https://stackoverflow.com/questions/37943778/how-to-set-get-pandas-dataframe-to-from-redis
```
## MongoDB
```

``

