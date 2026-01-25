1. Pull Caddy
docker pull caddy

2. Create two index files: index1.html and index2.html
   
3. Run a container 1 and container 2 with different index files
docker run -d -p 8881:80 -v $PWD/index1.html:/usr/share/caddy/index.html caddy
docker run -d -p 8882:80 -v $PWD/index2.html:/usr/share/caddy/index.html caddy