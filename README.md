# Config Server Sample

Run this project as a Spring Boot app, e.g. import into IDE and run
main method, or use Maven: 

```
$ mvn spring-boot:run
```

## Pre-requisites

You need to be running redis locally (there is a `docker-compose.yml` if you would
like to use that). This is to support broadcast of config changes to client apps
via Spring Cloud Stream. If you want to play and don't need that feature just
comment out the monitor and redis dependencies.

## Resources

| Path             | Description  |
|------------------|--------------|
| /{app}/{profile} | Configuration data for app in Spring profile (comma-separated).|
| /{app}/{profile}/{label} | Add a git label |
| /{app}/{profiels}{label}/{path} | An environment-specific plain text config file (at "path") |

## Local urls

http://localhost:8888/camel/default

## Documentations

http://cloud.spring.io/spring-cloud-config/spring-cloud-config.html#_spring_cloud_config_server