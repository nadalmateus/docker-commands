# Docker Commands
Some useful docker commands

### PostgreSQL
```
docker run -d --name postgres -p 5432:5432 -e "POSTGRES_PASSWORD=Pass@123" postgres
```

### SQL Server - Windows
```
docker run -d --name sqlserver -p 1433:1433 -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=Pass@123" mcr.microsoft.com/mssql/server
``` 

###### Connection String
```
Server=localhost,1433;Database=master;User ID=sa;Password=1q2w3e4r@#$
```

or if you get some error, first run the dev certs and then try the connect string with these params
```
dotnet dev-certs https --clean
dotnet dev-certs https --trust
```
```
Server=localhost,1433;Database=master;User ID=sa;Password=1q2w3e4r@#$;Trusted_Connection=False; TrustServerCertificate=True;
```
