```
docker run --name db -d postgres
docker run -it --rm --link db:db busybox  

/ # ping db
PING db (172.17.0.2): 56 data bytes
64 bytes from 172.17.0.2: seq=0 ttl=64 time=0.198 ms
64 bytes from 172.17.0.2: seq=1 ttl=64 time=0.105 ms
64 bytes from 172.17.0.2: seq=2 ttl=64 time=0.106 ms

/ # telnet db 5432
```
