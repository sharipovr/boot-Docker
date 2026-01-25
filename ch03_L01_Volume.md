1. Create a new empty volume:

``` bash
docker volume create ghost-vol
```

2. Check if it works:
``` bash
docker volume ls
```

3. Inspect the volume to see where is it stored on my machine:
   
``` bash
docker volume inspect ghost-vol
```
