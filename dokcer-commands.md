
## Build image

`docker build -t demo-images/angular-k8-app .`

## tag image

`docker tag demo-images/angular-k8-app:latest hyc-urx-docker-local.artifactory.swg-devops.com/urx-cloud/poc/angular-k8-app:latest`

## stop running docker

`docker stop $(docker ps -a -q)`

## run image
`docker run -p 80:80 -it demo-images/angular-k8-app:latest`
