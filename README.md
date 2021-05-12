# NestJS Boilerplate
## Description

origin from [NestJS](https://github.com/nestjs/nest) Boilerplate 


## Start Guide
- must update .env file
- Install dependencies `yarn`
- Start the app `yarn start` (app will be exposed through the port 3000)

### migration
- run `docker exec -it nest migration:run`

- for revert, run `docker exec -it nest migration:revert`


### docker-compose first run
- run `docker-compose up --build`


## Test

```bash
# unit tests
$ yarn test

# e2e tests
$ yarn test:e2e

# test coverage
$ yarn test:cov
```

## Swagger
http://localhost/api/docs