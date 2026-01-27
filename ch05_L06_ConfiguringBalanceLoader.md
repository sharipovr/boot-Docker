1. Stop any container that are,'t caddy app server
2. Create Caddyfile
3. Start the load balancer on 8880 and give him a caddyfile
docker run -d --network caddytest -p 8880:80 -v $PWD/Caddyfile:/etc/caddy/Caddyfile caddy