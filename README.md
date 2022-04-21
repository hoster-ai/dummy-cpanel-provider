  <div style="font-size:25px;text-align:center">cPanel provider dummy service provider</div>
  <hr>
  
## Installation

```bash
$ npm install
```

## Running the app

Start dev the docker images

```bash
# Start the dev docker images
docker-compose up -d

# development
$ npm run start

# watch mode
$ npm run start:dev

# production mode
$ npm run start:prod
```

# Supported HTTP calls
| Method | Endpoint |
| ------- | ------- |
| GET | /info |
| POST | /create |
| POST | /renew |
| POST | /upgrade |
| POST | /downgrade |
| POST | /suspend |
| POST | /unsuspend |
| POST | /delete |
| POST | /upgradeable |
| POST | /downgradeable |
| POST | /validate/action-fiels |
| POST | /validate/addons |

## .env required
 ```bash
 # General
 SERVICE_PROVIDER_TOKEN=test
 SERVICE_PROVIDER_API_URL='http://localhost:3000/service-providers/'

 ```

## Authentication
 Provider's token as bearer in headers

 *example*
 ```
 Authorization: Bearer test
 ```

 

## Test

```bash
# unit tests
$ npm run test

# e2e tests
$ npm run test:e2e

# test coverage
$ npm run test:cov
```

