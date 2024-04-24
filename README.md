<p align="center"><img src="https://media.licdn.com/dms/image/D5612AQHBvAU4QyKoAw/article-cover_image-shrink_720_1280/0/1695141734518?e=2147483647&v=beta&t=Pj_0UCFFdJR9t1r-J145TmD_YfPbHtA6aoXeQQAWjD4" alt="java 21" width="256px"/></p>

# A Containerized Hello World Java 21 deployment with Docker

a very simple rest-api-hello-world java application with Spring Boot and Maven, containerized with dockerfile, ready to build and deployed with a very simple way.

There are componenets of Dockerfiles provided

1. [Simple Java Project](https://github.com/joel2064/java_p1) 
2. [Git](https://hub.docker.com/r/alpine/git) Alpine
3. [jdk 21](https://hub.docker.com/layers/library/maven/3-eclipse-temurin-21-alpine/images/sha256-0f8cdcd68a68c621f6676d8c09a5e6779640005fba7ea873fc978dc2cd8d508f/) Alpine
4. [jre 21](https://hub.docker.com/layers/library/eclipse-temurin/21-jre-alpine/images/sha256-efdec7ae2b3e60bb253cdbe046249ddc07f3f0056837658616a94097f22a7449?context=explore) Alpine

It's important that you understand [Go build flags](https://pkg.go.dev/cmd/go#hdr-Compile_packages_and_dependencies) to build a functioning binary for your application. Not all apps will work with build configuration provided in the Dockerfiles.

## How to build the example

```bash
$ docker build -t <username_docker_hub>/<project_name>:<version> .
```

## How to run?

```bash
$ docker run -p 8080:8080 -d <login_hub>/<project_name>:<version>
```
