FROM microsoft/dotnet 
MAINTAINER MaxG mrozado@lagash.com

COPY . /app 
WORKDIR /app 
RUN ["dotnet", "restore"] 
RUN ["dotnet", "build"]
EXPOSE 5000
ENV ASPNETCORE_URLS http://*:5000
ENTRYPOINT ["dotnet", "run"]
ENV ASPNETCORE_ENVIRONMENT=Development
