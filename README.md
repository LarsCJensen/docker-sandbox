# docker-sandbox
`docker container create hello-world:linux`

`docker ps --all` - show all containers, not only running
`docker container start <container id>`
`docker container start --attach <container id>` start and attach to it
`docker logs 95833a919e98` - check std-out?? logs for container
`docker run <image>` == docker container create + docker container start + docker container attach

`docker build -t <tag> <ctx>` - looks for a file called `Dockerfile` in the context folder. If a different file, use `-f` to point to file

`docker kill <tag>` - kills running container.

`docker run -d <image>` - run container in detached mode.

`docker exec --interactive --tty 2eea bash` - execute an interactive shell (bash) in container.