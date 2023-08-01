# Makefile для упрощения сборки и запуска контейнера

# Имя образа, которое мы будем использовать
IMAGE_NAME := my_kittygram_app

# Цель для сборки Docker образа
build:
	docker build -t $(IMAGE_NAME) .

# Цель для запуска контейнера
run:
	docker run -p 9000:9000 $(IMAGE_NAME)

# Цель для запуска контейнера с монтированием текущего каталога в /app
run-mount:
	docker run -p 9000:9000 -v $(PWD):/app $(IMAGE_NAME)

.PHONY: build run run-mount
