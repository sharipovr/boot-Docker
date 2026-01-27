1. For the Linux binary builds command should be:

GOOS=linux GOARCH=amd64 go build

2. Build the image
docker build . -t goserver:latest

3. Run the container
docker run -p 8991:8991 goserver