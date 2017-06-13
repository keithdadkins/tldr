# docker ps

> List docker containers.

- Display running containers (does not show stopped containers):

`docker ps`

- Show all containers (running and stopped):

`docker ps -a`

- Show the most recently created container:

`docker ps -l`

- Tip: Use the -q flag with any `docker ps` command to only display the container id. This is useful for scripts and piping to other docker commands. For example, the following command will show the logs for the most recently created container:

`docker logs $(docker ps -l -q)`
