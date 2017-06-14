# docker run

> Creates and starts a container in one operation.

- The default `docker run` command will start a new container, run a command in the foreground, and then stop the container when finished:

`docker run {{image_name}} [optional_command_to_run]`

- Start a named container and then run detached in the background:

`docker run --name {{container_name}} -d {{image_name}}`

- Start a container and run a shell interactively:

`docker run -it {{image_name}} /bin/sh`

- Start a container, run a command, and delete the container when finished:

`docker run --rm {{image_name}} {{command}}`

- Web server example that starts a named container, maps a local port to a container port, mounts a local directory into the container, and then runs in the background:

`docker run --name {{foo_server}} -p {{80:80}} -v {{/path/to/local/html_files:/var/html}} {{webserver_image_name}}`
