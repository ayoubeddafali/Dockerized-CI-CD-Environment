# Dockerized CI/CD Environment

### This is a simple dockerized environment for CI/CD pipelines.



## Main Tools :

There are 4 containers running :

  - Jenkins Container (for pipelines).
  - Nexus Container (artifats manager).
  - SonarQube Container (code quality).
  - Postgres Container (database used by sonar).

You can find/change the port mapping in the `docker-compose.yml` file.
  - **8000** -> Jenkins
  - **8081** -> Nexus
  - **9000** -> Sonar

## How To install :

Start first with building the images, by running the script `build` inside the docker folder:

```bash
$ ./build
```

It will build three images : *Jenkins*, *Nexus* and  *Sonar*.

After that, you can start the environment (It will take some time) :

```bash
$ docker-compose up
```

To see the logs :

```bash
$ docker logs -f
```

## Maintainer

> [ayoubensalem](https://www.github.com/ayoubensalem)
