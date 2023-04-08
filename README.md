# Docker Getting Started workshop

## Mission 1

A simple Dockfile just to run a linux image and print "Hello world"

Go to `./mission-1` folder.

You can run directly the image from the registry:

```sh
docker run cchampou/hello-world
```

## Mission 2

A example of image based on nginx with a simple html file served.

Go to `./mission-2` folder

You can run directly the image from the registry:

```sh
docker run cchampou/hello-world-live
```

Exposition of the port 80:

```sh
docker run -p "80:80" cchampou/hello-world-live
```

## Mission 3

This is an introduction to volumes.

Go to the `./mission-3` folder.

You can run a Nginx container with a volume using:

```sh
docker run -p "80:80" -v "${PWD}/html:/usr/share/nginx/html:ro" nginx:alpine-latest
```
