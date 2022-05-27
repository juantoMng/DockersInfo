# DockersInfo
## Cmds - Dockers

### Docker object type
*	Containers
*	Images
*	Plugins
*	Volumes
*	Networks
*	Daemons
*	Services
*	Nodes
*	Secrets
*	Configs

**docker -help**	Muestra la ayuda de Dockers


### Management Commands:
| Command | Comment |
| - | - |
|builder	|Manage builds|
|config	|Manage Docker configs|
|container	|Manage containers|
|context	|Manage contexts|
|image	|Manage images|
|manifest	|Manage Docker image manifests and manifest lists|
|network	|Manage networks|
|node	|Manage Swarm nodes|
|plugin	|Manage plugins|
|secret	|Manage Docker secrets|
|service	|Manage services|
|stack	|Manage Docker stacks|
|swarm	|Manage Swarm|
|system	|Manage Docker|
|trust	|Manage trust on Docker images|
|volume	|Manage volumes|



### Commands
| Command | Comment |
| - | - |
|attach	|Attach local standard input, output, and error streams to a running container|
|build	|Build an image from a Dockerfile|
|commit	|Create a new image from a container's changes|
|cp	|Copy files/folders between a container and the local filesystem|
|create	|Create a new container|
|diff	|Inspect changes to files or directories on a container's filesystem|
|events	|Get real time events from the server|
|exec	|Run a command in a running container|
|export	|Export a container's filesystem as a tar archive|
|history	|Show the history of an image|
|images	|List images|
|import	|Import the contents from a tarball to create a filesystem image|
|info	|Display system-wide information|
|inspect	|Return low-level information on Docker objects|
|kill	|Kill one or more running containers|
|load	|Load an image from a tar archive or STDIN|
|login	|Log in to a Docker registry|
|logout	|Log out from a Docker registry|
|logs	|Fetch the logs of a container|
|pause	|Pause all processes within one or more containers|
|port	|List port mappings or a specific mapping for the container|
|ps	|List containers|
|pull	|Pull an image or a repository from a registry|
|push	|Push an image or a repository to a registry|
|rename	|Rename a container|
|restart	|Restart one or more containers|
|rm	|Remove one or more containers|
|rmi	|Remove one or more images|
|run	|Run a command in a new container|
|save	|Save one or more images to a tar archive (streamed to STDOUT by default)|
|search	|Search the Docker Hub for images|
|start	|Start one or more stopped containers|
|stats	|Display a live stream of container(s) resource usage statistics|
|stop	|Stop one or more running containers|
|tag	|Create a tag TARGET_IMAGE that refers to SOURCE_IMAGE|
|top	|Display the running processes of a container|
|unpause	|Unpause all processes within one or more containers|
|update	|Update configuration of one or more containers|
|version	|Show the Docker version information|
|wait	|Block until one or more containers stop, then print their exit codes|


## Management Commands:

### builder
Manage builds

__Sintaxis__
```bash
Usage:  docker builder COMMAND

Commands:
  build       Build an image from a Dockerfile
  prune       Remove build cache
```

### build
Build an image from a Dockerfile
```bash
docker builder build [OPTIONS] PATH | URL | -
```
### prune
Remove build cache
```bash
docker builder prune
```
### config
Manage Docker configs
```bash
docker config COMMAND
```
### create
Create a config from a file or STDIN
```bash
docker config create [OPTIONS] CONFIG file|-
```
### inspect
Display detailed information on one or more configs
```bash
docker config inspect [OPTIONS] CONFIG [CONFIG...]
```
### ls
List configs
```bash
docker config ls [OPTIONS]
```
### rm
Remove one or more configs
docker config rm CONFIG [CONFIG...]

Example
```bash
docker config rm my_config
```

## container
Manage containers
Sintaxis
```bash
docker container COMMAND
```
### attach
Attach local standard input, output, and error streams to a running container
```bash
docker container attach [OPTIONS] CONTAINER
```

### commit
Create a new image from a container’s changes
```bash
docker container commit [OPTIONS] CONTAINER [REPOSITORY[:TAG]]
```

### cp
Copy files/folders between a container and the local filesystem
```bash
docker container cp [OPTIONS] CONTAINER:SRC_PATH DEST_PATH|-
```

### create
Create a new container
```bash
docker container create [OPTIONS] IMAGE [COMMAND] [ARG...]
```

### diff
Inspect changes to files or directories on a container’s filesystem
```bash
docker container diff CONTAINER
```

### exec
Run a command in a running container
```bash
docker container exec [OPTIONS] CONTAINER COMMAND [ARG...]
```

### export
Export a container’s filesystem as a tar archive
```bash
docker container export [OPTIONS] CONTAINER
```

### inspect
Display detailed information on one or more containers
```bash
docker container inspect [OPTIONS] CONTAINER [CONTAINER...]
```

### kill
Kill one or more running containers
```bash
docker container kill [OPTIONS] CONTAINER [CONTAINER...]
```

### logs
Fetch the logs of a container
```bash
docker container logs [OPTIONS] CONTAINER
```

### ls
List containers
```bash
docker container ls [OPTIONS]
```

### pause
Pause all processes within one or more containers
```bash
docker container pause CONTAINER [CONTAINER...]
```

### port
List port mappings or a specific mapping for the container
```bash
docker container port CONTAINER [PRIVATE_PORT[/PROTO]]
```

### prune
Remove all stopped containers
```bash
docker container prune [OPTIONS]
```
### rename
Rename a container
```bash
docker container rename CONTAINER NEW_NAME
```

### restart
Restart one or more containers
```bash
docker container restart [OPTIONS] CONTAINER [CONTAINER...]
```

### rm
Remove one or more containers
```bash
docker container rm [OPTIONS] CONTAINER [CONTAINER...]
```

### run
Run a command in a new container
```bash
docker container run [OPTIONS] IMAGE [COMMAND] [ARG...]
```

### start
Start one or more stopped containers
```bash
docker container start [OPTIONS] CONTAINER [CONTAINER...]
```

### stats
Display a live stream of container(s) resource usage statistics
```bash
docker container stats [OPTIONS] [CONTAINER...]
```

### stop
Stop one or more running containers
```bash
docker container stop [OPTIONS] CONTAINER [CONTAINER...]
```

### top
Display the running processes of a container
```bash
docker container top CONTAINER [ps OPTIONS]
```

### unpause
Unpause all processes within one or more containers
```bash
docker container unpause CONTAINER [CONTAINER...]
```

### update
Update configuration of one or more containers
```bash
docker container update [OPTIONS] CONTAINER [CONTAINER...]
```

### wait
Block until one or more containers stop, then print their exit codes
```bash
docker container wait CONTAINER [CONTAINER...]
```

## context
Manage contexts
Sintaxis
```bash
docker context COMMAND
```
### create
Create a context
```bash
docker context create [OPTIONS] CONTEXT
```

### export
Export a context to a tar or kubeconfig file
```bash
docker context export [OPTIONS] CONTEXT [FILE|-]
```
### import
Import a context from a tar or zip file
```bash
docker context import CONTEXT FILE|-
```
### inspect
Display detailed information on one or more contexts
```bash
docker context inspect [OPTIONS] [CONTEXT] [CONTEXT...]
```
### ls
List contexts
```bash
docker context ls [OPTIONS]
```

### rm
Remove one or more contexts
```bash
docker context rm CONTEXT [CONTEXT...]
```
### update
Update a context
```bash
docker context update [OPTIONS] CONTEXT
```
### use
Set the current docker context
```bash
docker context use CONTEXT
```

### cp
Copy files/folders between a container and the local filesystem
```bash
docker cp [OPTIONS] CONTAINER:SRC_PATH DEST_PATH|-
```

### create

Create a new container
```bash
docker create [OPTIONS] IMAGE [COMMAND] [ARG...]
```

### diff
Inspect changes to files or directories on a container’s filesystem
```bash
docker diff CONTAINER
```

### events
Get real time events from the server
```bash
docker events [OPTIONS]
```

### exec
Run a command in a running container
```bash
docker exec [OPTIONS] CONTAINER COMMAND [ARG...]
```
Example
```bash
docker run --name ubuntu_bash --rm -i -t ubuntu bash

docker exec -d ubuntu_bash touch /tmp/execWorks
```

export
Export a container’s filesystem as a tar archive
```bash
docker export [OPTIONS] CONTAINER
```
Example
```bash
docker export red_panda > latest.tar
docker export --output="latest.tar" red_panda
```
### history
Show the history of an image
```bash
docker history [OPTIONS] IMAGE
```
Example
```bash
docker history docker
```

