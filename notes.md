# _To know about your CODENAME version enter the follow command in the terminal_

```
grep CODENAME /etc/os-release

lsb_release -c
To check if you are running a 64bit OS, use this command: uname -m
```

# Docker part

`docker build <filePathOfDockerfil>` - build the initial image<br>
`docker run <containerID>` - run you project image<br>
`docker ps`- list all containers that are currently running<br>
`docker stop <containerID>` - stops container with given ID<br>
`docker rmi <imageID>` - remove images<br>
`docker start <nameTag>` - restart the container stoped<br>

## The flags meaning:

`-d`: runs the process in background and print the Container ID
`-p`: publishes port(s) from the container to host. Format is hostPort:containerPort. Example -p 80<br>
`-a`: list all process the docker created<br>
`-i`: keep STDIN open even if not attached (for interactive commands like bash or zsh)<br>
`-t`: Allocates a pseudo-TTY to the container<br>
`-v`: Bind mount a volume<br>
`--name`: Name you image<br>
Example of using these flags together:

```
bash
$ docker run -it ubuntu bash
```

# Docker Compose

`docker compose up` - start services defined in docker-compose file<br>
`docker compose down` - remove services and networks<br>
`docker compose logs` - show log of service<br>
`docker compose restart` - restarts one or more services<br>
`docker compose kill` - force stop service<br>
`docker compose pause` - suspend all processes within an existing container<br>
`docker compose unpause` - resume a paused container<br>
`docker compose rm` - removes stopped containers<br>
`docker compose rmi` - removes images used by stopped containers<br>
`docker compose build` - builds services<br>
`docker compose push` - pushes service images to registry<br>
`docker compose pull` - pulls and reuses locally available images for services<br>
`docker compose config` - validate and view the configuration<br>
`docker compose create` - creates containers without starting them<br>
`docker compose scale` - scales the number of containers for a service<br>
`docker compose events` - Monitor Docker's events API<br>
`docker compose exec` - Run a new command in a running container<br>
`docker compose top` - display the running processes inside a container<br>
`docker compose inspect` - return low-level information on objects in Docker<br>
`docker compose login` - Log in to Docker Registry<br>

### Extra notes

> _*Every code changes, we will need to down the image and rebuild up*_
