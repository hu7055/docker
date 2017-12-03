# Create docker image
	1. Copy war and "Dockerfile" to linux
	2. Build docker image Docker build -f Dockerfile -t dlaservice
	3. Run docker container Docker run -p 8080:8080 -t dlaservice
	4. Check docker images Docker images
	5. See runing container Docker ps
