prometheus-stack
================

_*prometheus-stack*_ lets you run grafana and prometheus in docker container.

## Running

Clone the project and run the following:
* `cd prometheus-stack` 
* `docker-compose pull`
* `docker-compose up -d`

## Stopping

Go to the directory where `docker-compose.yml` is present and run the following:
* `docker-compose down`

## Configuration

* `docker-compose.yml` file contains the volumes and port related information. By default, prometheus runs on `9090` and grafana runs on `3000`.
* `prometheus/prometheus.yml` file contains scrape and target related information. By default, it scrapes itself in every 10s.

## Data Directory

By default, `grafana_data` and `prometheus_data` are data stores for grafana and prometheus respectively. You can replace these directories in `docker-compose.yml` file.

## Contributing

Feel free to raise the PR, if you find any issue or want to improve the project.