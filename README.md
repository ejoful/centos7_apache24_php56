# dockerfiles-centos-httpd

CentOS Dockerfile for Centos7, Apache httpd 2.4, php56


## Build

Copy the sources down and do the build

```
# docker build --rm -t <username>/lnmp .
```

## Usage

To run (if port 8080 is available and open on your host):

```
# docker run -d -p 8080:8080 <username>/lnmp
```

or to assign a random port that maps to port 80 on the container:

```
# docker run -d -p 8080 <username>/lnmp
```

To the port that the container is listening on:

```
# docker ps
```

## Test

```
# curl http://localhost:8080
```

