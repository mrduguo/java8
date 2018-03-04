# spring boot application java8 base image  [![Build Status](https://travis-ci.org/mrduguo/java8.svg?branch=master)](https://travis-ci.org/mrduguo/java8)

## What's included


* Run the jar file in / folder
* Expose port 8080
* Added https://letsencrypt.org certs

## Use in Dockerfile


```bash

FROM mrduguo/java8

```

### Docker hub published tags

https://hub.docker.com/r/mrduguo/java8/tags/



## Build


```bash

./gradlew

```

It will build the docker image with latest and versioned tags.


## Run locally to inpsect the image


```bash

# ./gradlew
docker run -it --rm --entrypoint sh mrduguo/java8 


```
