# docker-graphite-statsd-v1
## Description
Ready to go solution to up Grafana stack systemm which include Grafana, Graphite, Statsd servers.
**NOTE** Grafana contains from splitted on 2 parts: server and db that allow to save grafana data in case of any upgrading issue with server part.

## Requirements

The following software is required to stand up a Grafana, Graphite, Statsd
environment:

|               Prerequisite                       |                 Description              |
|--------------------------------------------------|------------------------------------------|
|[Docker](https://www.docker.com/)                 | Container management tool                |
|[Docker compose](https://docs.docker.com/compose/)| A tool for defining multi-container apps |

**NOTE for Windows/OSX users:** The easiest way of getting Docker is by installing the
[docker toolbox](https://www.docker.com/products/docker-toolbox).

## Quick Start

Getting started with Grafana stack should be fast and easy once you
have Docker up and running. Here are the steps:

**NOTE for Windows/OSX users:** Make sure `docker` is up and running by following the [windows guide](https://docs.docker.com/engine/installation/windows/#using-docker-from-windows-command-prompt-cmd-exe) / [osx guide](https://docs.docker.com/engine/installation/mac/#from-your-shell).

* clone the repo
* cd to the project directory
* run the following:

``` sh
docker-compose up -d
```
* If all is fine you should check created containers by executing following command:

``` sh
docker-compose ps
```
* and you should see following containers:

``` sh
docker-graphite-statsd_grafana_1
docker-graphite-statsd_grafana_db_1
docker-graphite-statsd_graphite_1
```