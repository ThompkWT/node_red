# node_red
## Docker
[Docker Setup](https://nodered.org/docs/getting-started/docker)

```bash
docker run -it -p 1880:1880 --name mynodered nodered/node-red


# percistent data volume
$ docker volume create --name node_red_user_data
$ docker volume ls
DRIVER              VOLUME NAME
local               node_red_user_data
$ docker run -it -p 1880:1880 -v node_red_user_data:/data --name mynodered nodered/node-red

```

