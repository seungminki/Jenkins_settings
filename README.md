# Jenkins_settings

### Docker image 생성
$ docker build --tag jenkins:latest .

### docker container 
docker run --name jenkins-docker -p 8080:8080 -p 50000:50000 -d -v /var/run/docker.sock:/var/run/docker.sock -v jenkins_home:/var/jenkins_home jenkins:latest
