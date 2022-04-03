# Docker Crash Course - YT
A Cheat Sheet to help you get through the video series.

## Microsoft SQL Server
https://hub.docker.com/_/microsoft-mssql-server

Windows PC:
```sh
docker run --name sqlserver -e "ACCEPT_EULA=Y" -e "SA_PASSWORD=Benjica1!" -p 1401:1433 -d mcr.microsoft.com/mssql/server:2019-latest
```
MacOS & Linux:
```sh
docker run --name sqlserver2019 -e 'ACCEPT_EULA=Y' -e 'SA_PASSWORD=Benjica1!' -p 1401:1433 -d mcr.microsoft.com/mssql/server:2019-latest
```

## PostgreSQL
https://hub.docker.com/_/postgres/
```sh
docker run --name postgresql -p 5401:5432 -e POSTGRES_PASSWORD=Benjica1! -d postgres:latest
```
## Docker Commands
view all running containers
```sh
docker ps
```
view all containers regardless of status
```sh
docker ps -a
```
stop a container
```sh
docker stop sqlserver
```
start a container
```sh
docker start sqlserver
```
remove a container
```sh
docker rm sqlserver
```
