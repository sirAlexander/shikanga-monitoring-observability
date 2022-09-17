# Sample application for tutorials

This repository contains the environment for completing the tutorials at [grafana.com/tutorials](https://grafana.com/tutorials).

## Prequisites

You will need to have the following installed locally to complete this workshop:

- [Docker](https://docs.docker.com/install/)
- [Docker Compose](https://docs.docker.com/compose/install/)

If you're running Docker for Desktop for macOS or Windows, Docker Compose is already included in your installation.

## Building the application
 
1. Navigate into the `app` directory and run the docker build command
2. The build should create a local app docker image `local/grafana-101_app`
3. Navigate out into the `grafana-101` folder
```shell
cd app/

docker build -t local/grafana-101_app .

cd ..
```

## Running

To start the sample application and the supporting services:

```shell
docker-compose up -d
```

## Cleaning Up

```shell
docker-compose down -v
```
**Note:** only use -v if you also want to get rid of all the associated volumes created.