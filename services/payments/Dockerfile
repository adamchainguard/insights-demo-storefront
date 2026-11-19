FROM mcr.microsoft.com/dotnet/sdk:latest AS build
WORKDIR /src
COPY . .

FROM mcr.microsoft.com/dotnet/aspnet:latest
WORKDIR /app
ENTRYPOINT ["dotnet", "Payments.dll"]
