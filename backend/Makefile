# Имя образа, которое мы будем использовать
IMAGE_NAME := deonisg/kittygram_backend

# Цель для сборки Docker образа
build:
    docker build -t $(IMAGE_NAME) .

# Цель для запуска контейнера
run:
    docker run -p $(GATEWAY_PORT):9000 $(IMAGE_NAME)

# Цель для запуска контейнера с монтированием текущего каталога в /app
run-mount:
    docker run -p $(GATEWAY_PORT):9000 -v $(PWD):/app $(IMAGE_NAME)

# Цель для запуска приложения через make в контейнере
run-make:
    docker run $(IMAGE_NAME) make run

.PHONY: build run run-mount run-make