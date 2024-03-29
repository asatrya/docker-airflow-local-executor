# docker-airflow-local-executor

This repository contains a Dockerized version of Apache Airflow running on Local Executor.

## Informations

* Based on Python (3.7-slim-stretch) official Image [python:3.7-slim-stretch](https://hub.docker.com/_/python/) and uses the official [Postgres](https://hub.docker.com/_/postgres/) as backend
* This is a simplified version of https://github.com/puckel/docker-airflow

## How to Run

1) Configure `.env`

   ```sh
   nano .env
   ```
2) Locate your DAG files on `./dags` folder

3) Build and run Docker container

   ```sh
   docker-compose -f docker-compose-LocalExecutor.yml up -d
   ```

4) Access Airflow UI on http://localhost:8080
