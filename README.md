# docker-setup



### To build an image

```
docker build -t <username>/<image-name> .
```

### To run  (this commands also works if image uploaded to Dockerhub, can be run on remote computer)

```
docker run -p 80:80 <username>/<image-name>

### To tag image  (must be done prior to uploading to DockerHub)

Run `docker image` to find the Image ID of your image.
```
docker tag <Image ID> <username>/<image-name>:<version>
```

### To push up to DockerHub

```
docker push <username>/<image-name>






