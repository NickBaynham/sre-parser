# sre-parser
Watchlist - parser microservice
Linux updated to: https://github.com/sonatype-nexus-community/nancy/releases/download/v1.0.33/nancy_1.0.33_linux_amd64.rpm

## To build the project manually:
```
cd /root/agent/workspace/movies-parser_develop
docker build -f Dockerfile.test -t parser .
docker run parser:latest
```

## Troubleshoot
```
docker container run -it parser /bin/bash
cd /go/src/github/mlabouardy/movies-parser
LINK=" /usr/local/bin/nancy https://github.com/sonatype-nexus-community/nancy/releases/download/v0.1.17/nancy-linux.amd64-v0.1.17"
wget $LINK -O nancy
chmod +x nancy
go get -u golang.org/x/lint/golint
go get -v
nancy /go/src/github/mlabouardy/movies-parser/Gopkg.lock
exit
```
