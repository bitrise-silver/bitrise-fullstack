This project demonstrates a real-world fullstack project which can be built and deployed in bitrise.io.

## Setup local development

1. Install Podman Desktop and Kind, on macOS you may want to keep a copy of .ssh/known_hosts and empty it to make Kind work. Note: Do NOT create Kind cluster yet
2. Run `make -f Makefile.dev setup`
3. Backend development in `src/backend/helloworld`
4. Frontend development in `src/frontend`

## Deployment to local Kind cluster

1. Run `make image-build` in `src/backend/helloworld`
2. Run `make image-build` in `src/frontend`
3. Run `make -f Makefile.dev deploy` in root folder