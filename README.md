# jenkins-docker-image
This is a custom image for creating jenkins environment that is capable of running Docker commands and managing docker containers.

docker image build -t jenkins-docker .

docker run -d -p 8080:8080 -p 50000:50000 -v jenkins_home:/var/jenkins_home -v /var/run/docker.sock:/var/run/docker.sock --restart unless-stopped jenkins-docker
