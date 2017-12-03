# Create docker image
	1. Copy war and "Dockerfile" to linux
	2. Build docker image Docker build -f Dockerfile -t dlaservice
	3. Run docker container Docker run -p 8080:8080 -t dlaservice
	4. Check docker images Docker images
	5. See runing container Docker ps

# Moving docker image
	1. Docker run ubuntu /bin/bash -c "echo 'creating new file' > /tmp/sample"
	2. Check container id
		a. Docker ps -a
	3. Docker commit 0acb….(container Id) productionready
	4. Docker save -o /tmp/prod.tar productionready
	5. Get the prod.tar and move to another environment
	6. Docker load -i prod.tar
	7. You can see the new docker image which is productionready

# Docker-compose
	1.Run this command to download the latest version of Docker Compose:
curl -L https://github.com/docker/compose/releases/download/1.17.0/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose
