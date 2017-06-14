# docker run

> Run a command in a new container.

- Start and run a command in a new container:

`docker run {{image_name}} [optional_command_to_run]`

- Start a named container and then run detached in the background:

`docker run --name {{container_name}} -d {{image_name}}`

- Start a container, run a shell interactively, and then delete the container when finished:

`docker run --rm -it {{image_name}} /bin/sh`

- Example command that maps a local port to a container port, mounts a local directory into the container, and then runs the container detached as a daemon in the background:

`docker run --name my_web_server -d -p 80:80 -v /path/to/local/html_files:/var/www/html my_httpd_image_name`
