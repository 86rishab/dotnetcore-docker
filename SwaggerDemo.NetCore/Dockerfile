FROM mcr.microsoft.com/dotnet/core/aspnet:2.2 AS runtime

COPY /bin/Release/netcoreapp2.2/publish/ /var/aspnetcore
#Since I have used "always copy to output folder" I dont need to copy xml file specifically
#COPY SwaggerDemo.NetCore.XML /var/aspnetcore

WORKDIR /var/aspnetcore

ENV ASPNETCORE_ENVIRONMENT Staging

ENV ASPNETCORE_URLS http://+:56884

ENTRYPOINT ["dotnet", "/var/aspnetcore/SwaggerDemo.NetCore.dll"]
