# docker-hadoop
key word: docker hadoop alpine openjdk openssh single node cluster

# run
```
docker run -d \
--name=hadoop-standalone \
-p 8088:8088 \
-p 50070:50070 \
-p 14000:14000 \
-p 9001:9001 \
test/hadoop:2.7 && \
docker logs -f hadoop-standalone

docker run --rm  \
-p 8088:8088 \
-p 50070:50070 \
-p 14000:14000 \
test/hadoop:2.7 && \
docker logs -f hadoop-standalone
```
