# go-docker-compose

Example application demonstrating how to use Docker compose with Go applications. The repository contains a simple application written in Golang that contains a single API to display the "Quote of the day".

The app fetches the quote of the day from a public API hosted at `http://quotes.rest/`, then it caches the result in Redis. For subsequent API calls, the app will return the result from Redis cache instead of fetching it from the public API.

Clone the repository and type the following command to start the app -

```bash
$ docker-compose up
```

```bash
$ curl http://localhost:8080/qod
If I work as hard as I can, I wonder how much I can do in a day?
```

Read the Tutorial: [Docker Compose: Defining and running multi-container docker applications](http://localhost:1313/docker-compose-multi-container-orchestration-golang/)