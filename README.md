# About this repository

This repository uses Redis core data structures, Streams, RediSearch and TimeSeries to build a
Java/Spring Boot/Spring Data Redis Reactive application that shows a searchable transaction overview with realtime updates
as well as a personal finance management overview with realtime balance and biggest spenders updates. UI in Bootstrap/CSS/Vue.

Features in this demo:

- Redis Streams for the realtime transactions
- Redis TimeSeries for the balance over time
- RediSearch for searching transactions
- Sorted Sets for the 'biggest spenders'
- Redis hashes for session storage (via Spring Session)

## Architecture

![Architecture](architecture.png)

## Prerequisites

1. JDK 21 or higher (<https://openjdk.java.net/install/index.html>). Not needed if you're using Docker.
1. Maven. Not needed if you're using Docker.
1. Docker Desktop (<https://www.docker.com/products/docker-desktop>), or Colima with a docker/k8s/containerd runtime

## Running locally

1. Checkout the project
1. `docker-compose.sh up`
1. Navigate to <http://localhost:8080>
1. Login with user `lars` and password `larsje`
1. Stop and clean with `docker-compose down -v --rmi local --remove-orphans`