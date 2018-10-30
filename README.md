# How to use

## Docker Compose

```shell
$ source ./env_set.sh
$ docker-compose build
$ docker-compose up
```

## Docker

```
$ docker build . -t $IMAGE_NAME
$ source ./env_set.sh
$ docker run -itd --name $CONTAINER_NAME -v $HOST_DIRECTORY:$CONTAINER_DIRECTORY -p $HOST_PORT:8888 $IMAGE_NAME jupyter notebook --ip=0.0.0.0 --port=8888 --allow-root --notebook-dir=$CONTAINER_DIRECTORY
```

**Password**

```
$ docker logs $CONTAINER_NAME
```
