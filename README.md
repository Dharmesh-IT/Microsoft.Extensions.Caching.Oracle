**
This can be used as a distribution cache for the Oracle database same as MSSQL.
**

`
builder.Services.AddDistributedOracleCache(options =>
{
options.ConnectionString = "DB Connection name";
options.SchemaName = "Schema Name";
options.TableName = "TABLE ANME";
});

`
