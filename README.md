**
This can be used as a distribution cache for the Oracle database same as MSSQL.
**
`
builder.Services.AddDistributedOracleCache(options =>
{
options.ConnectionString = builder.Configuration.GetConnectionString("DB Connection name");
options.SchemaName = "Schema Name";
options.TableName = "TABLE ANME";
});

`
