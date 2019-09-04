# Local Docker DB

## What?
A collection of Docker Compose files I've used to quickly spin local databases of various sorts.

## Why?
Because I've oft needed them, particularly when I just don't wanna deal with the hassle of spinning up a DB on my own system.

## How? 
Clone the repo or copy a `docker-compose.yml` file to your system, `cd` into that directory, and turn it on with `docker-compose up`. For a full reference on how to use Docker Compose, [go here](https://docs.docker.com/compose/reference/).

## Local Persistence
In each setup a docker managed volume is created to persist the database. This can be deleted by Docker compose by passing the "-v" option when deleting the container(s).

```
docker-compose down -v
```

## Authentication
For authenticating as super user with each of these examples, `root` should be the username and `password` should be the password.
