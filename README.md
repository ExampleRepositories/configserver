# Config Server Sample

Run this project as a Spring Boot app, e.g. import into IDE and run
main method, or use Maven: 

```
$ mvn spring-boot:run
```


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