docker-hints
============

Useful tips for Docker.

List containers with IP addresses

```
docker ps -a -q | xargs docker inspect --format '{{.Name}}: {{.NetworkSettings.IPAddress}}'
```
