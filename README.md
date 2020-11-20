# Monitoring Spring Boot with Prometheus + Grafana (Preconfigured Dashboard)

![Grafana Dashboard](https://github.com/BatuhanKucukali/spring-boot-prometeus-grafana-example/blob/master/grafana-dashboard.png?raw=true "Grafana Dashboard")

## Technologies
* [Spring Boot](https://spring.io/)

## Prerequisites
* [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
* [JDK](https://openjdk.java.net/)
* [Maven](https://maven.apache.org/)
* [Docker](https://www.docker.com/)

## Run this project
1 . Clone project on your machine
```
git clone https://github.com/BatuhanKucukali/spring-boot-prometeus-grafana-example
```
2 . Change directory
```
cd spring-boot-prometeus-grafana-example
```
3 . Run Project
```
./mwnw spring-boot:run
```
4 . Run Dependencies
```
docker-compose up
```

:warning: **Note:** Since we are using Docker to run Prometheus, it will be running in a Docker network that won't 
understand localhost/120.0.01, as you might expect. Since our app is running on localhost, and for the Docker container, 
localhost means its own network, we have to specify our system IP in place of it.

**Change ip address in prometheus.yml**

To check your system IP you can run ipconfig or ifconfig in your terminal, depending upon your OS.

## Sources

* https://tanzu.vmware.com/developer/guides/spring/spring-prometheus/?utm_source=twitter&utm_medium=social
* https://stackabuse.com/monitoring-spring-boot-apps-with-micrometer-prometheus-and-grafana/
* https://royportas.com/posts/2020-02-25-prometheus-and-grafana-configuration-for-docker-compose/
* https://grafana.com/grafana/dashboards/10280

## Getting help

If you're having trouble getting this project running, feel free to [open an issue](https://github.com/BatuhanKucukali/spring-boot-prometeus-grafana-example/issues/new) or [email me](mailto:mail@batuhankucukali.com)!