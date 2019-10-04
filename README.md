[![pipeline status](https://gitlab.forge.orange-labs.fr/lucy/ihl/monitoring-dockers-with-prometheus/badges/master/pipeline.svg)](https://gitlab.forge.orange-labs.fr/lucy/ihl/monitoring-dockers-with-prometheus/commits/master)
[![Try in PWD](https://dabuttonfactory.com/button.png?t=Test+with+PlayGround&f=Calibri-Bold&ts=24&tc=fff&tshs=1&tshc=000&hp=20&vp=8&c=5&bgt=gradient&bgc=e54405&ebgc=000)](http://lucy1.rd.francetelecom.fr/?stack=https://gitlab.forge.orange-labs.fr/jtkp3624/monitoring-dockers-with-prometheus/blob/master/docker-compose.yml&stack_name=prometheus)


# 1. Monitoring dockers with Prometheus

In this project, we provide both Prometheus and Grafana monitoring for Docker's metrics. In particular, we monitor clearwater vIMS docker.
## What's inside

* Docker compose file with a [Prometheus](https://hub.docker.com/r/prom/prometheus/), [Grafana](https://hub.docker.com/r/grafana/grafana) and [container exporter](https://hub.docker.com/r/prom/container-exporter/) configurations
* Description file Prometheus.yml including Prometheus configuration. 

## Prerequisites 
* To start you need to install docker and [docker-compose](https://docs.docker.com/compose/install/) if not already installed. 

## Launch Prometheus and Grafana dockers 
```
$ git clone https://gitlab.forge.orange-labs.fr/lucy/ihl/monitoring-dockers-with-prometheus.git
```
```
$ docker-compose up
```
## Prometheus and Grafana
In a browser 
* localhost@:9090 for Prometheus Dashbord
* localhost@:3000 for Grafana Dashbord


# 2. Monitoring Clearwater vIMS docker

 * Clone the project [clearwater vIMS docker](https://github.com/cherrared/clearwater-docker.git)
```
$ git clone https://github.com/sofianinho/clearwater-docker.git
```
* Launch clearwater vIMS docker 
```
$ docker-compose up
```

* You can monitor and visualize Clearwater's metrics on Prometheus and Grafana Dashbords.
* If you want to monitor your Docker deployment via a web UI you can install and run [Weave Scope](https://www.weave.works/docs/scope/latest/installing/). It provides real time visualizations showing all of your containers, their resource usage and the connectivity between them.

