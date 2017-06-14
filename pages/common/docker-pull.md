# docker pull

> Pull an image or a repository from a registry.

- Download the latest image from a Docker Hub repository:

`docker pull {{image_name}}`

- Download a tagged image from a Docker Hub repository:

`docker pull {{image_name}}:{{tag_name}}`

- Download all tagged images from a Docker Hub repository:

`docker pull -a {{repository_name}}`

- Pull from a non Docker Hub repository:

`docker pull {{registry_url}}:{{registry_port}}/{{repository_name}}/{{image_name}}`
