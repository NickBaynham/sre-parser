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
```
