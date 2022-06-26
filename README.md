# docker-laravel


## Introduction

Build a simple laravel development environment with docker-compose.

## Usage

```bash
$ git clone https://github.com/reitouhozonn/my-lara-docker.git
$ cd my-lara-docker
$ make create-project # Install the latest Laravel project
```

http://localhost

## Container structures

```bash
├── app
├── web
└── db
```

### app container

- Base image
  - [php](https://hub.docker.com/_/php):8.1-fpm-buster
  - [composer](https://hub.docker.com/_/composer):2.1

### web container

- Base image
  - [nginx](https://hub.docker.com/_/nginx):1.20-alpine
  - [node](https://hub.docker.com/_/node):16-alpine

### db container

- Base image
  - [mysql/mysql-server](https://hub.docker.com/r/mysql/mysql-server):8.0
