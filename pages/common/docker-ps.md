# docker ps

> List docker containers.

- Display running containers (does not show stopped containers):

`docker ps`

- Show all containers (running and stopped):

`docker ps -a`

- Show the most recently created container:

`docker ps -l`

- Use the -q flag with any `docker ps` command to only return the container id. This is useful when combined with other docker commands. E.g.,:

`docker logs $(docker ps -l -q)`
