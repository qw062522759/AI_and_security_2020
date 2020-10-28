#
```
https://docs.python.org/3/library/sqlite3.html
```

```
port sqlite3

conn = sqlite3.connect('example.db')
```

```
# 
c = conn.cursor()

# Create table建立資料表
c.execute('''CREATE TABLE stocks
             (date text, trans text, symbol text, qty real, price real)''')

# Insert a row of data新增一筆資料
c.execute("INSERT INTO stocks VALUES ('2006-01-05','BUY','RHAT',100,35.14)")

# Save (commit) the changes執行上述動作
conn.commit()

# We can also close the connection if we are done with it.關掉連線
# Just be sure any changes have been committed or they will be lost.
conn.close()
```
# 查詢query()
```
import sqlite3
conn = sqlite3.connect('example.db')
c = conn.cursor()


symbol = 'RHAT'
c.execute("SELECT * FROM stocks WHERE symbol = '%s'" % symbol)

# Do this instead
t = ('RHAT',)
c.execute('SELECT * FROM stocks WHERE symbol=?', t)
print(c.fetchone())
```
### SQL ==structured query Language
```
SELECT * 
FROM stocks 
WHERE symbol = '%s'" % symbol
```
