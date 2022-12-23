# JWT Demo

## Start server

1. Copy `env.sample` to `.env`
1. Change the value of `SECRET_KEY` to any random string which 256 bit size (32 characters at least)
1. Run `$ docker compose up` at your terminal
1. Access this API by make a request to `localhost:9000/<endpoint>`
1. Pull requests always open :)

## Endpoints
| Endpoint | Method | Description |
| :--      | :---:  | :---        |
| `/`      | `ANY`  | healthcheck endpoint |
| `/api/v0/secret-key` | `GET` | Server will return keys that used to validate JWT with `{ "key": "<secret-key>" }` <br />(**FOR DEMO PURPOSE!!!**) |
| `/api/v0/goods/return` | `POST` | Simulate the communication between client and server |
