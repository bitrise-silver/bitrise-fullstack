all: build image-build

build:
	yarn install

image-build:
	podman build -t helloworld-frontend:latest .

image-run:
	podman run --rm --name helloworld-frontend -p 3000:3000 helloworld-frontend:latest