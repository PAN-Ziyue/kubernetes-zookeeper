VERSION=1.0-3.6.2
PROJECT_ID=pan-ziyue
PROJECT=ghcr.io/${PROJECT_ID}

all: build

build:
	docker build --pull -t ${PROJECT}/kubernetes-zookeeper:${VERSION} .

push: build
	gcloud docker -- push ${PROJECT}/kubernetes-zookeeper:${VERSION}

.PHONY: all build push
