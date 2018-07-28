# IDatabaseApi.GetConnection method

返回给定连接字符串的IDbConnection对象。

```csharp
public IDbConnection GetConnection(string connectionString)
```

| parameter | description |
| --- | --- |
| connectionString | 用于创建连接的连接字符串。 |

## Return Value

IDbConnection 对象。

## Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | 如果connectionString是null就抛出。 |

## See Also

* interface [IDatabaseApi](sdk/IDatabaseApi.md)
* namespace [SiteServer.Plugin](sdk/README.md)

<!-- DO NOT EDIT: generated by xmldocmd for SiteServer.Plugin.dll -->