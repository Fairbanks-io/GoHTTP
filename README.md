# GoHTTP

 A simple Golang HTTP file server with some extras
 - Request Logging
 - Tracing IDs
 - Error Handling
 - Health Check

### Getting Started
To run, add your files to **src/public**, then launch:
```
./make
```

To run from source, launch with:
```
go run src/main.go
```

### Docker
To launch GoHTTP with Docker, you can create an image by running:
```
docker build -t fairbanks-io/gohttp:latest .
```

### Extras
A health check endpoint is available on `/healthz`

### Coming Soon
- [x] Docker Support