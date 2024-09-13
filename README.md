# Sample Node.js application

This repository is a sample Node.js application for Docker's documentation.

## Nefi's Notes
Dockerfile came from here: https://docs.docker.com/guides/language/nodejs/containerize/

App git repo: https://github.com/docker/docker-nodejs-sample

### Useful commands
```
docker build --platform linux/amd64 -t nflondo/nodejs-sample-x86:0.1 .
docker tag local-image:tagname new-repo:tagname
docker push new-repo:tagname
docker push nflondo/nodejs-sample:tagname
docker push nflondo/nodejs-sample-x86:0.1
docker service create --name=nodejs-sample -p 3000:3000 nflondo/nodejs-sample-x86:0.1
```