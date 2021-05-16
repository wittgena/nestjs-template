# NestJS Template
## 디스크립션

[NestJS](https://github.com/nestjs/nest) boilerplate 

- mysql
- jwt


## 가이드
- .env 파일생성 필요

```bash
$ cp env.sample .env
```

- node 모듈 인스톨

```bash
$ yarn 
```

- start

```bash
$ yarn run:dev
```

## TypeORM

- 기본설정 (env.sample)

```
DB_TYPE=mysql
DB_USERNAME=root
DB_PASSWORD=password
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=database
DB_SYNC=false
```

### 마이그레이션
- migration

```bash
$ docker exec -it nest migration:run
```

- revert migration

```bash
$ docker exec -it nest migration:revert
```


### docker-compose 실행
- run 

```bash
# 첫실행시 --build 옵션추가 
$ docker-compose up --build
```

## Test

### local
```bash
# unit tests
$ yarn test

# e2e tests
$ yarn test:e2e

# test coverage
$ yarn test:cov
```

### docker
```bash
# unit tests
$ docker exec -it nest yarn test

# e2e tests
$ docker exec -it nest yarn test:e2e

# test coverage
$ docker exec -it nest yarn test:cov
```

## Swagger
http://localhost/api/docs