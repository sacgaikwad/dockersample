List containers: 
	docker ps -a

Remove Container:
	docker rm "container"

Stop container:
	docker stop "container"

Docker Build:
	docker build -f Dockerfile -t docker.sample.service .

Create and Run container:
	docker run -d -p 8080:80 --name docker.sample.service docker.sample.service

Remove all Images:
	for /F %i in ('docker images -a -q') do docker rmi -f %i