docker build -t nginxunit-go:basic .  
docker run -d --name nginxunit-go -p 8080:8080 nginxunit-go:basic  