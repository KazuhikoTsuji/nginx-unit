docker build -t nginxunit-java:basic .  
docker run -d --name nginxunit-java -p 8080:8080 nginxunit-java:basic  