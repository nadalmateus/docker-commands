# Docker Commands
Some useful docker commands

## Databases
#### Postgree
```
docker run -d --name postgres -p 5432:5432 -e "POSTGRES_PASSWORD=1q2w3e4r@#$" postgres
```
#### MS SQL Server
```
docker run -d --name sqlserver -p 1433:1433 -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=1q2w3e4r@#$" mcr.microsoft.com/mssql/server
```
