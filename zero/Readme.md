## A Docker Image of 0 bytes

```
docker build -t zero .
Sending build context to Docker daemon  3.584kB
Step 1/2 : FROM scratch
 ---> 
Step 2/2 : COPY zerobytesfile /
 ---> Using cache
 ---> 929db9e57532
Successfully built 929db9e57532
Successfully tagged zero:latest

docker images zero
REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE
zero                latest              929db9e57532        5 minutes ago       0
```
