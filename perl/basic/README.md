docker build -t nginxunit-perl:basic .  
docker run -d --name nginxunit-perl -p 8080:8080 nginxunit-perl:basic  