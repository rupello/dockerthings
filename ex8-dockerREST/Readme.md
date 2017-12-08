### Talking REST to the Docker Daemon

`echo -e "GET /images/json HTTP/1.0\r\n" | nc -U /var/run/docker.sock`

or

`curl --unix-socket /var/run/docker.sock http://localhost/images/json`

(see docker from a distance)
