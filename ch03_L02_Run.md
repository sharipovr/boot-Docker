1. Now pull the Ghost image from Docker Hub:

``` bash
docker pull ghost
```

2. Run the Ghost
``` bash
docker run -d -e NODE_ENV=development -e url=http://localhost:3001 -p 3001:2368 -v ghost-vol:/var/lib/ghost ghost
```


=================================================

Check if volume works.
1. WE need to stop running container and remove it with:
``` bash
docker stop CONTAINER_ID
docker rm CONTAINER_ID
``` 

2. Start a new container with the same command as before, therefore using the same volume.
``` bash
docker run -d -e NODE_ENV=development -e url=http://localhost:3001 -p 3001:2368 -v ghost-vol:/var/lib/ghost ghost
```