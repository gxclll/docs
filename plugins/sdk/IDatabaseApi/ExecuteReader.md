# IDatabaseApi.ExecuteReader method (1 of 6)

对连接字符串中指定的数据库执行SQL 命令并返回IDataReader。

```csharp
public IDataReader ExecuteReader(IDbConnection connection, string sqlString)
```

| parameter | description |
| --- | --- |
| connection | 有效的IDbConnection。 |
| sqlString | SQL语句。 |

## Return Value

命令执行后获取的DataReader。

## Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | 如果sqlString为空，则抛出。 |

## Examples

```csharp
IDataReader dr = databaseApi.ExecuteReader(conn, "SELECT * FROM table");
```

## See Also

* interface [IDatabaseApi](../IDatabaseApi.md)
* namespace [SiteServer.Plugin](../../SiteServer.Plugin.md)

---

# IDatabaseApi.ExecuteReader method (2 of 6)

对连接字符串中指定的数据库执行SQL 命令并返回IDataReader。

```csharp
public IDataReader ExecuteReader(IDbTransaction transaction, string sqlString)
```

| parameter | description |
| --- | --- |
| transaction | 有效的IDbTransaction。 |
| sqlString | SQL语句。 |

## Return Value

命令执行后获取的DataReader。

## Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | 如果sqlString为空，则抛出。 |

## See Also

* interface [IDatabaseApi](../IDatabaseApi.md)
* namespace [SiteServer.Plugin](../../SiteServer.Plugin.md)

---

# IDatabaseApi.ExecuteReader method (3 of 6)

对连接字符串中指定的数据库执行SQL 命令并返回IDataReader。

```csharp
public IDataReader ExecuteReader(string connectionString, string sqlString)
```

| parameter | description |
| --- | --- |
| connectionString | 数据库连接字符串。 |
| sqlString | SQL语句。 |

## Return Value

命令执行后获取的DataReader。

## Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | 如果connectionString为空，则抛出。 |
| ArgumentNullException | 如果sqlString为空，则抛出。 |

## See Also

* interface [IDatabaseApi](../IDatabaseApi.md)
* namespace [SiteServer.Plugin](../../SiteServer.Plugin.md)

---

# IDatabaseApi.ExecuteReader method (4 of 6)

对连接字符串中指定的数据库执行SQL 命令并返回IDataReader。

```csharp
public IDataReader ExecuteReader(IDbConnection connection, string sqlString, 
    IDataParameter[] commandParameters)
```

| parameter | description |
| --- | --- |
| connection | 有效的IDbConnection。 |
| sqlString | SQL语句。 |
| commandParameters | 用于执行命令的IDataParameter数组。 |

## Return Value

命令执行后获取的DataReader。

## Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | 如果有任何IDataParameters参数名为空，或者如果参数计数不匹配所提供的值的数量，则抛出。 |
| ArgumentNullException | 如果sqlString为空，则抛出。 |
| ArgumentException | 如果参数计数与提供的值数量不匹配，则抛出。 |
| ArgumentNullException | 如果connection为空，则抛出。 |

## See Also

* interface [IDatabaseApi](../IDatabaseApi.md)
* namespace [SiteServer.Plugin](../../SiteServer.Plugin.md)

---

# IDatabaseApi.ExecuteReader method (5 of 6)

对连接字符串中指定的数据库执行SQL 命令并返回IDataReader。

```csharp
public IDataReader ExecuteReader(IDbTransaction transaction, string sqlString, 
    IDataParameter[] commandParameters)
```

| parameter | description |
| --- | --- |
| transaction | 有效的IDbTransaction。 |
| sqlString | SQL语句。 |
| commandParameters | 用于执行命令的IDataParameter数组。 |

## Return Value

命令执行后获取的DataReader。

## See Also

* interface [IDatabaseApi](../IDatabaseApi.md)
* namespace [SiteServer.Plugin](../../SiteServer.Plugin.md)

---

# IDatabaseApi.ExecuteReader method (6 of 6)

对连接字符串中指定的数据库执行SQL 命令并返回IDataReader。

```csharp
public IDataReader ExecuteReader(string connectionString, string sqlString, 
    IDataParameter[] commandParameters)
```

| parameter | description |
| --- | --- |
| connectionString | 数据库连接字符串。 |
| sqlString | SQL语句。 |
| commandParameters | 用于执行命令的IDataParameter数组。 |

## Return Value

命令执行后获取的DataReader。

## Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | 如果connectionString为空，则抛出。 |
| InvalidOperationException | 如果有任何IDataParameters参数名为空，或者如果参数计数不匹配所提供的值的数量，则抛出。 |
| ArgumentNullException | 如果sqlString为空，则抛出。 |
| ArgumentException | 如果参数计数与提供的值数量不匹配，则抛出。 |

## See Also

* interface [IDatabaseApi](../IDatabaseApi.md)
* namespace [SiteServer.Plugin](../../SiteServer.Plugin.md)

<!-- DO NOT EDIT: generated by xmldocmd for SiteServer.Plugin.dll -->
