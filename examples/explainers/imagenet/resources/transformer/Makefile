IMAGE_VERSION=0.2
IMAGE_NAME=docker.io/seldonio/imagenet-transformer

build:
	s2i build -E environment . seldonio/seldon-core-s2i-python36:1.5.0-dev $(IMAGE_NAME):$(IMAGE_VERSION)

push_to_dockerhub:
	docker push $(IMAGE_NAME):$(IMAGE_VERSION)
