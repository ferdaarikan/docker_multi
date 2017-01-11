FROM microsoft/dotnet:1.0.1-runtime
EXPOSE 80
RUN mkdir /app
WORKDIR /app

COPY . /app

RUN ["dotnet", "restore"]
RUN ["dotnet", "build"]

COPY ./bin .

CMD ["dotnet", "service-b.dll"]
