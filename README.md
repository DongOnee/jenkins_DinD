# Jenkins Docker (Docker in Docker, docker-compose)

## how to use
### Preparations
docker-compose 를 이용하기 위해서 다운 받아야 된다. 
```
curl -L "https://github.com/docker/compose/releases/download/1.25.5/docker-compose-$(uname -s)-$(uname -m)"
```
컨테이너 안에서 다운 받으면 너무 느리기 때문에 미리 다운받은 후 mount, link 시키도록 하자.
### Build & Run
```
docker network create devops
docker-compose up -d --build
```
~~docker network 는 안해도 될듯..~~
### Shutdown
```
docker-compose down
```