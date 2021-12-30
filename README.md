# Swagger.NetCore
Implemented Swagger documentation in .Net Core web APIs


build command
=============
dotnet publish -c Release 

docker build 
============
docker build -t dotnetcore-docker-test .

docker run command
==================
docker run -p 8080:56884 --name dotnetcore-docker-test dotnetcore-docker-test
