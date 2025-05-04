all: build image-build

build:
	go build .

image-build:
	podman build -t helloworld-backend:latest .

image-run:
	podman run --rm --name helloworld-backend -p 8080:8080 helloworld-backend:latest