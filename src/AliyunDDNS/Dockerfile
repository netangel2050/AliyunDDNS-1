FROM mcr.microsoft.com/dotnet/core/runtime
FROM mcr.microsoft.com/dotnet/core/aspnet
MAINTAINER symbolspace<symbolspace@outlook.com>

LABEL description="AliyunDDNS"
LABEL version="1.0"

RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

WORKDIR /app
COPY . .
ENTRYPOINT ["dotnet", "AliyunDDNS.dll"]