```
docker network create foonet
docker run --name db -d postgres
docker network connect foonet db
docker run -it --rm --net foonet busybox

/ # ping db
PING db (172.19.0.2): 56 data bytes
64 bytes from 172.19.0.2: seq=0 ttl=64 time=0.219 ms
64 bytes from 172.19.0.2: seq=1 ttl=64 time=0.096 ms

docker network inspect foonet
