1. Create a custom bridge network.
docker network create caddytest

2. List networks
   
3. Stop and restart caddy app servers, but this time attach them to caddytest network.

4. Create getting started container and run it in the shell
docker run -it --network caddytest docker/getting-started /bin/sh

5. curl both app site/containers from the inside, I have to see html content of both sites.
curl caddy1
curl caddy2


Curious question:
what are the ip addresses of both caddy app servers from inside the getting started container?
their ip addresses are visible via ping command
172.20.0.2 and 172.20.0.3

This is awesome, because these ip addresses are internal to the custom bridge network only!