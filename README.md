# go-hello-world

## build

```
CGO_ENABLED=0 GOOS=linux go build -a -installsuffix cgo .
docker build -t sosimon/go-hello-world .
docker push sosimon/go-hello-world
```

## test

```
docker run -it -p 8080:8080 sosimon/go-hello-world
curl http://localhost:8080
```
