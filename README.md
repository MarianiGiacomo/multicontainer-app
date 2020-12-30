# multicontainer-app
A setup for a Vue application and backend services running in separate Docker containers

## Install submodules
`git submodules init`

## Add environment variables
Create a `.env` file in the root folder to pass the environment variable to `docker-compose`. Here is an example:

```
FE_PORT=8081
BE_HOST=http://localhost
BE_PORT=8001
SERVICE_API_PATH=service
SERVICE_URL=http://service
SERVICE_PORT=3001
```
`SERVICE_URL` should point to the service name if run locally.

## Run the application with backend and services
Run `docker-compose up`

Access the application from `http://localhost:${FE_PORT}`
