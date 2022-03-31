# docker-commands-draft
Some useful docker commands

## Databases
docker run -d --name postgres -p 5432:5432 -e "POSTGRES_PASSWORD=1q2w3e4r@#$" postgres
docker run -d --name sqlserver -p 1433:1433 -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=1q2w3e4r@#$" mcr.microsoft.com/mssql/server
