# Break the network
Run 'getting started' container with no network:
```bash
docker run -d --network none docker/getting-started
``` 

Go inside of the containe rand do ping google
docker exec CONTAINER_ID ping google.com -W 2

which should fail and return:
ping: bad address 'google.com'