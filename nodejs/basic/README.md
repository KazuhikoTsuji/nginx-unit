docker build -t nginxunit-nodejs:basic .  
docker run -d --name nginxunit-nodejs -p 8080:8080 nginxunit-nodejs:basic  