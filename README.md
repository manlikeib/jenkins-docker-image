# jenkins-docker-image
This is a custom image for creating jenkins environment that is capable of running Docker commands and managing docker containers.

docker image build -t jenkins-docker .

docker run -p 8080:8080 -p 50000:50000 -d -v jenkins_home:/var/jenkins_home jenkins-docker:latest
