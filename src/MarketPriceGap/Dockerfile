FROM microsoft/dotnet:latest

COPY . /app
COPY *.sln .
COPY webhook.txt .
COPY pair.txt .
COPY interval.txt .

WORKDIR /app

EXPOSE 5000/tcp

ENTRYPOINT ["/entrypoint.sh"]