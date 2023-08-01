IMAGE_NAME := my_kittygram_app

build:
	docker build -t $(IMAGE_NAME) .

run:
	docker run -p 9000:9000 $(IMAGE_NAME)

run-mount:
	docker run -p 9000:9000 -v $(PWD):/app $(IMAGE_NAME)
