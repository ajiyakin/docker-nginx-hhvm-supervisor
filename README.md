# docker-nginx-hhvm-supervisor

Docker images for PHP development using NGINX, HHVM and Supervisor as services manager.

To run this images, just use this command:


    docker run -d [--name=<container_name>] --volume=<project_path>:/usr/share/nginx/html ajiyakin/nginx-hhvm-supervisor:latest


`<container_name>` is the name that you want for container. If you not specified
the name for container, you will get random name from docker automatically.


`--volume` command will mount your project folder to the container.
`<project_path>` is ABSOLUTE PATH to your project directory. And
`/usr/share/nginx/html` is default location for nginx on the container.


`-p` command used to port mapping from host's port 8000 to container's
port 80 which is default http port.
