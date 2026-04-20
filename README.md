# ARCHIVED

This repository is archived. We have stopped using this in favor of Docker Compose [healthcheck](https://docs.docker.com/reference/compose-file/services/#healthcheck).

# whenavail # 
A script for monitoring a port on another host and then executing a command when ready.

When using docker compose, all defined services are started simultaneously. However we 
often have situations where we need a database container started and online before we 
can run database migrations or other scripts. Using ```whenavail``` we can watch host 
and port and then run a command when it is ready.

## Usage ##
```
whenavail <remote_host> <remote_port> <timeout> command [arguments] ...
```
