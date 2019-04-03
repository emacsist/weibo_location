# weibo_location
weibo location code

# sql

```sql
create table wb_location (
	p_code int,
	p_name varchar(32),
	c_code int,
	c_name varchar(32)
);
```

clickhouse

```sql
create table wb_location (p_code Int32, p_name String, c_code Int32, c_name String)Engine=MergeTree ORDER BY p_code SETTINGS index_granularity = 8192;
```
