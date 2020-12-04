# Docker tips tricks
Write about docker tips and tricks that might be useful for others.

## Updating files in the docker container

1. See what containers are running.
### `docker ps`

2. Open the shell in the running container. You can get the container hash from the previous command
### `docker exec -it <CONTAINER HASH> bash`

3. Edit whatever file you want. If nano is not found, then you can install it from the terminal. Depending on the OS it might be different. 
### `nano <FILE NAME>`

4. Exit the shell
### `exit`

5. Now in order to apply your changes you have to restart the container.
### `docker restart <CONTAINER HASH>`

That's all!
