# GoHTTP

 A simple Golang HTTP file server with some extras
 - Request Logging
 - Tracing IDs
 - Error Handling
 - Health Check

### Getting Started
To run, add your files to **src/public**, then launch:
```
go run src/main.go
```

You can also build the application with:
```
go build src/main.go
```

### Docker
To launch GoHTTP with Docker, you can create an image by running:
```
docker build -t fairbanks-io/gohttp:latest .
```

Or, pull the latest image from DockerHub:
```
docker run -d -p 80:8080 --name gohttp fairbanksio/gohttp
```

If you want to pass in your own content, use a volume mount:
```
docker run -d -p 80:8080 --name gohttp -v /my/public/dir:/app/public:Z fairbanksio/go-http
```

### Extras
A health check endpoint is available on `/healthz`

### Coming Soon
- [x] Docker Support
- [ ] Scratch Support