# Wordpress Plugin Development Environment

## Environment
- PHP 7.4.9
  - Composer 2.1.9
- wp-cli 2.5.0
- Docker 20.10.8
  - Docker Compose 2.0.0

## Usage
- Setup Environment
  - install php dependency
  ```
  composer install
  ```
  - install wp-cli
  ```
  brew install wp-cli
  ```
- initialize your wordpress plugin

- Write your test code in `src/test`
- Write your code in `src`
- run test in wordpress container
  ```
  ./runtest
  ```
  - if you want to specify test suite
  ```
  ./runtest TEST_SUITE
  ```
**NOTE:** This script does not stop `database` container. If you want to shutdown this environment, run following command.
```
docker-compose down
```

## ToDo 