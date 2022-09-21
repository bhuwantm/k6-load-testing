# Load Testing and Visualization using k6, prometheus and Grafana

Tools used:

- Prometheus
- Prometheus/node_exporter
- Grafana
- InfluxDB
- k6

&nbsp;

## Setup and Running the test

Create .env file by copying .env-example. Change the variable value as you wish.

`cp .env-example .env`

Run the docker compose file. Add `-d` at the end if you want to run it in detached mode.

`docker-compose up -d`

Run the demo test script using following command:

`docker-compose run k6 run /tests/script.js`

&nbsp;

## Prometheus

Open source systems monitoring and alerting toolkit. It collects and stores its metrics as time series data, i.e. metrics information is stored with the timestamp at which it was recorded, alongside optional key-value pairs called labels.

Docker Network URL: http://prometheus:9090

Local URL: http://localhost:9090

&nbsp;

## Prometheus/node_exporter

Prometheus exporter for hardware and OS metrics. Collects metrics and exposes them to an endpoint, which Prometheus can consume.

&nbsp;

## Grafana

It is an open source data visualization tool developed by Grafana Labs (which also developed K6). It allows us to query, visualize, alert on and understand metrics from multiple sources into a single centralized location.

Docker Network URL: http://grafana:9091

Local URL: http://localhost:9091

&nbsp;

## InfluxDB v1.x.x

The Time Series Database for storage and retrival of time series data like application metrics, system metrics, IoT sensor data etc.

Docker Network URL: http://influxdb:8086

Local URL: http://localhost:8086

&nbsp;

## k6

Open source load testing tool for testing the performance of your backend infrastructure.

- Written in Go for faster performance
- Test Script is written in javascript

&nbsp;

## Running Test

`docker-compose run k6 run /tests/script.js`
