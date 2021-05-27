FROM microsoft/dotnet:latest

COPY . /app
COPY *.sln .
COPY webhook.txt .
COPY pair.txt .
COPY interval.txt .

WORKDIR /app

RUN ["dotnet", "restore"]

RUN ["dotnet", "build"]

EXPOSE 5000/tcp

ENTRYPOINT ["/entrypoint.sh"]