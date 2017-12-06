```
docker build . -t voltest    

docker run --rm -it -v $(pwd)/data:/data voltest
/ # touch /data/foo
/ # exit

# back on host
ls ./data 
foo

```
