FROM mcr.microsoft.com/dotnet/sdk:latest AS build
WORKDIR /src
COPY . .

FROM mcr.microsoft.com/dotnet/runtime:latest
WORKDIR /app
ENTRYPOINT ["dotnet", "Worker.dll"]
