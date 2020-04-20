# Build Microservice with ASP.NET Core and Distribute with Docker image

## About
Experiment creating microservices with .NET

## Framework and tools
.NET SDK 3.1.201, VSCode, Docker image

## Create and run the service
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

`docker run -it --rm -p 5566:80 --name mymicroservicecontainer mymicroservice`

## Browser URL or view the container running
- `http://localhost:5566/WeatherForecast`

- `docker ps`

## Credited by Microsoft documentation
Docker Cli
List all containers (only IDs) 
`docker ps -aq.`

Stop all running containers. 
`docker stop $(docker ps -aq)`

Remove all containers. 
`docker rm $(docker ps -aq)`

Remove all images. 
`docker rmi $(docker images -q)`