```
docker build -t gohello .
Sending build context to Docker daemon  3.072kB
Step 1/6 : FROM golang:1.8
 ...
Successfully tagged gohello:latest
docker run --rm gohello
+ exec app
hello world
```

## Interactive
```
docker run -it gohello bash
root@0db03adf7c03:/go/src# which app
/go/bin/app
root@0db03adf7c03:/go/src# app
hello world
```
