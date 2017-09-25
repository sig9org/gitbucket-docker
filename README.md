gitbucket-docker
========
Docker image of GitBucket which is an open-source GitHub clone powered by Scala.

[![Docker build](http://dockeri.co/image/sig9/gitbucket)](https://registry.hub.docker.com/u/sig9/gitbucket/)

How to use this image
--------

```
docker run -d -p 8080:8080 sig9/gitbucket
```

Add `-p 29418:29418` option if you would like to enable SSH for repository access:

```
docker run -d -p 8080:8080 -p 29418:29418 sig9/gitbucket
```

You can also specify the data directory by `-v` option:

```
docker run -d -p 8080:8080 -v `pwd`/gitbucket:/gitbucket sig9/gitbucket
```
