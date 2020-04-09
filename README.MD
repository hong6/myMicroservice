# Build Microservice with ASP.NET Core

## About
Experiment creating microservices with .NET

## Framework and tools
.NET SDK 3.1.201, VSCode, Docker image

## create and run the service
`dotnet new webapi -o myMicroservice --no-https` 

`dotnet run` 

`http://localhost:5000/WeatherForecast` 

## Download and Install Docker
`docker --version` 

## Add Docker metadata
`Dockerfile`

`.dockerignore`

## Create and Run Docker image
`docker build -t mymicroservice .`

`docker run -it --rm -p 3000:80 --name mymicroservicecontainer mymicroservice`

## Browser URL or view the container running
- `http://localhost:3000/WeatherForecast`

- `docker ps`

## Credited by Microsoft documentation