# mysql基础

---

所有数据库导入导出都在退出数据库时执行

1.mysql命令行导出数据库（数据库备份）

```
msyqldump -u root -p --default-character-set=utf8 databasename>path/databasename.sql
```

```
mysqldump -u root -p --default-character-set=utf8 databasename tablename>path/tablename.sql
```

2.mysql命令行导入数据库

```
mysql -u root -p --default-character-set=utf8 databaesname<path/databasename.sql
```

```
mysql -u root -p --default-character-set=utf8 databaesname<path/tablename.sql
```

3.删除表数据

```
delete from tablename where id=1;
```

4.修改表数据

```
update set 字段名=值 where id=1;
```

5.查询数据

```
select * from tablename where 字段名=值；
```

6.插入数据

```
INSERT INTO 表名 （字段名1，字段名2，...）
        VALUES(值1，值2，...);
```
