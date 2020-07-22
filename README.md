# Using docker to build a new redis environment
```sh
docker pull redis
# pull docker image

docker run --name redis-lab -dp 6379:6379 redis
# run the container

# Go to docker cli mode by IDE or using exec
docker exec -it redis-lab bash

```

In docker cli
```sh
redis-cli

# Entering redis-cli mode
127.0.0.1:6379> ping
PONG
127.0.0.1:6379> set hello "hello world"
OK
127.0.0.1:6379> get hello
"hello world"
```

