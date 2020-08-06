docker build -t nginxunit-python:basic .  
docker run -d --name nginxunit-python -p 8080:8080 nginxunit-python:basic  