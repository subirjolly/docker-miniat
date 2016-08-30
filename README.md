# docker-miniat
miniat dockerfiles

## Ubuntu Image
docker pull subirjolly/miniat-ubuntu

## Docker Compose
Documentation: https://docs.docker.com/compose/

### Ubuntu Docker Compose
**Starting Image**
```
cd ubuntu
docker-compose up
# or for daemon mode
docker-compose up -d
```
**Stopping Image**
```
docker-compose stop
```
**To remove stopped volumes for your containers**
```
docker-compose rm -fv
```
