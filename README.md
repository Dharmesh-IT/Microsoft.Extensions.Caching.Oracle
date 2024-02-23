# Microsoft.Extensions.Caching.Oracle

## This can be used as a distribution cache for the Oracle database same as MSSQL.

```sh
builder.Services.AddDistributedOracleCache(options =>
{
options.ConnectionString = "DB Connection name";
options.SchemaName = "Schema Name";
options.TableName = "TABLE ANME";
});

```

# Ref 

[Distributed caching in ASP.NET Core](https://learn.microsoft.com/en-us/aspnet/core/performance/caching/distributed?view=aspnetcore-8.0)


# Create same table as below in your oracle schema.

### dotnet sql-cache create "Data Source=(localdb)/MSSQLLocalDB;Initial Catalog=DistCache;Integrated Security=True;" dbo TestCache

![alt](https://learn.microsoft.com/en-us/aspnet/core/performance/caching/distributed/_static/sqlservercachetable.png?view=aspnetcore-8.0)